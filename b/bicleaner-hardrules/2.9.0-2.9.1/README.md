# Comparing `tmp/bicleaner-hardrules-2.9.0.tar.gz` & `tmp/bicleaner-hardrules-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/jzaragoza/hardrules/bicleaner-hardrules/dist/.tmp-jgus9hup/bicleaner-hardrules-2.9.0.tar", last modified: Wed Aug  9 09:31:18 2023, max compression
+gzip compressed data, was "bicleaner-hardrules-2.9.1.tar", last modified: Tue Aug 29 08:48:55 2023, max compression
```

## Comparing `bicleaner-hardrules-2.9.0.tar` & `bicleaner-hardrules-2.9.1.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/.github/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2094 2021-05-24 08:58:36.000000 bicleaner-hardrules-2.9.0/.github/stale.yml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2048 2022-11-16 09:46:37.000000 bicleaner-hardrules-2.9.0/.gitignore
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       74 2023-03-06 13:41:25.000000 bicleaner-hardrules-2.9.0/.gitmodules
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3986 2023-08-07 13:44:02.000000 bicleaner-hardrules-2.9.0/CHANGELOG.md
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    35147 2021-05-24 08:58:36.000000 bicleaner-hardrules-2.9.0/LICENSE
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    14068 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/PKG-INFO
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12770 2023-08-07 13:08:29.000000 bicleaner-hardrules-2.9.0/README.md
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/kenlm/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/kenlm/.github/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/kenlm/.github/workflows/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      542 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/.github/workflows/mac.yml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      619 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/.github/workflows/ubuntu.yml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      471 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/.github/workflows/windows.yml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      249 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/.gitignore
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      696 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/BUILDING
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4298 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    26530 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/COPYING
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    35147 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/COPYING.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7637 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/COPYING.LESSER.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    63537 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/Doxyfile
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1150 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/LICENSE
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      220 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/MANIFEST.in
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5394 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/README.md
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)       81 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/clean_query_only.sh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/kenlm/cmake/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2821 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/cmake/KenLMFunctions.cmake
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      334 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/cmake/kenlmConfig.cmake.in
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/kenlm/cmake/modules/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3185 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/cmake/modules/FindEigen3.cmake
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)     1154 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/compile_query_only.sh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.301063 bicleaner-hardrules-2.9.0/kenlm/lm/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2165 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3710 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/bhiksha.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4348 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/bhiksha.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12931 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/binary_format.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3498 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/binary_format.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1379 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/blank.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     8154 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/build_binary_main.cc
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.305063 bicleaner-hardrules-2.9.0/kenlm/lm/builder/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1897 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      826 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/README.md
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      152 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/TODO
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12607 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2258 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3509 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      899 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/combine_counts.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9550 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1701 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2820 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3992 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/count_ngrams_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2411 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/debug_print.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      439 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/discount.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1869 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/dump_counts_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      293 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/hash_gamma.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      715 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/header_info.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10698 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/initial_probabilities.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1452 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/initial_probabilities.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6044 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/interpolate.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1136 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/interpolate.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    11967 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/lmplz_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1625 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/output.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2529 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/output.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1051 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/payload.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    17887 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/pipeline.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2572 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/builder/pipeline.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.305063 bicleaner-hardrules-2.9.0/kenlm/lm/common/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      889 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6078 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/compare.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2366 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/joint_order.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5186 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2155 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1713 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2112 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/ngram.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1872 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/ngram_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1890 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/print.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1483 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/print.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      398 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/renumber.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      755 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/renumber.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      562 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/size_option.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      302 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/size_option.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      550 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/special.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.305063 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.305063 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       60 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy0.1
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      112 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy0.2
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      140 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy0.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       55 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy0.kenlm_intermediate
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       19 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy0.vocab
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       72 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy1.1
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      112 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy1.2
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      120 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy1.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       55 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy1.kenlm_intermediate
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       21 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/bigendian/toy1.vocab
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)      270 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/generate.sh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.305063 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       60 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy0.1
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      112 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy0.2
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      140 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy0.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       55 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy0.kenlm_intermediate
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       19 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy0.vocab
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       72 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy1.1
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      112 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy1.2
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      120 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy1.3
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       55 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy1.kenlm_intermediate
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       21 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/littleendian/toy1.vocab
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      475 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/toy0.arpa
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      470 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/common/test_data/toy1.arpa
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      675 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/config.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3913 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/config.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      722 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/enumerate_vocab.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2544 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/facade.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.309063 bicleaner-hardrules-2.9.0/kenlm/lm/filter/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1327 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1935 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/arpa_io.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2816 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/arpa_io.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2458 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/count_io.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9352 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/filter_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7379 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/format.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     8212 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5778 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5027 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase_table_vocab_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4205 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/thread.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1209 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/vocab.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4123 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/vocab.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1797 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/filter/wrapper.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1068 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/fragment_main.cc
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.309063 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1774 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      737 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_matrix.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1952 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      913 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4904 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1086 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2530 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3222 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      693 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/interpolate_info.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5296 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/interpolate_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10010 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_probabilities.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3385 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_probabilities.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3586 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      572 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5306 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    13813 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1101 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2758 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7645 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/pipeline.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      552 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/pipeline.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1235 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/split_worker.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1100 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/split_worker.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7430 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/streaming_example_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5950 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      590 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3969 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    19605 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2956 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4571 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      512 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_matrix.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1366 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_weights.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      446 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_weights.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      342 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/universal_vocab.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1347 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/universal_vocab.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9039 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/kenlm_benchmark_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7174 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/left.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12402 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/left_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      637 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/lm_exception.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1057 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/lm_exception.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      644 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/max_order.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    16256 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/model.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7051 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/model.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    14544 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/model_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      798 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/model_type.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3534 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/ngram_query.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6003 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/partial.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6672 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/partial_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3743 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/quantize.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7749 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/quantize.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4675 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/query_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7543 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/read_arpa.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3016 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/read_arpa.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1248 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/return.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12060 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/search_hashed.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5935 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/search_hashed.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    23394 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/search_trie.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4906 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/search_trie.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2594 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/sizes.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      374 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/sizes.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3440 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/state.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2780 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/test.arpa
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2694 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/test_nounk.arpa
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5639 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/trie.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3563 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/trie.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10982 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/trie_sort.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2795 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/trie_sort.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3935 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/value.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2045 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/value_build.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2568 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/value_build.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      380 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/virtual_interface.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5668 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/virtual_interface.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    11083 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/vocab.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     8680 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/vocab.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      358 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/weights.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      293 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/word_index.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.309063 bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      176 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/README
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4261 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/nplm.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1975 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/nplm.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.309063 bicleaner-hardrules-2.9.0/kenlm/python/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      988 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1957 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/_kenlm.pxd
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)     1427 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/example.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)   445847 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/kenlm.cpp
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9323 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/kenlm.pyx
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      906 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/score_sentence.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      325 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/python/score_sentence.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1976 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/setup.py
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.317063 bicleaner-hardrules-2.9.0/kenlm/util/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3873 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1176 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/bit_packing.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5967 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/bit_packing.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1490 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/bit_packing_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1227 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/cat_compressed_main.cc
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.317063 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1042 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1527 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/LICENSE
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    27617 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum-dtoa.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4300 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum-dtoa.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    24726 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5891 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9913 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/cached-powers.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3021 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/cached-powers.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5030 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/diy-fp.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1804 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-conversion.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    15851 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-to-string.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    22349 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-to-string.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    31645 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fast-dtoa.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4064 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fast-dtoa.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    15352 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fixed-dtoa.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2770 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fixed-dtoa.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    15223 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/ieee.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    27857 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/string-to-double.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10848 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/string-to-double.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    23469 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/strtod.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3038 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/strtod.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    15340 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/utils.h
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1367 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/ersatz_progress.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1603 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/ersatz_progress.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2765 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/exception.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4392 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/exception.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3994 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/fake_ostream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    18350 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4746 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10877 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file_piece.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6515 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file_piece.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5364 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file_piece_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2424 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/file_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5545 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/fixed_array.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      729 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/float_to_string.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      609 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/float_to_string.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1441 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/getopt.c
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      472 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/getopt.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      270 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/have.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    22498 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1636 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1959 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4905 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/joint_sort.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1738 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/joint_sort_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    13507 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/mmap.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6780 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/mmap.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3379 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/multi_intersection.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1887 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/multi_intersection_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4074 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/murmur_hash.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      616 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/murmur_hash.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1546 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/parallel_read.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      461 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/parallel_read.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3480 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/pcqueue.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      355 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/pcqueue_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      705 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/pool.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2935 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/pool.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    13233 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    11788 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table_benchmark_main.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2269 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3526 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/proxy_iterator.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    13086 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/read_compressed.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2034 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/read_compressed.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2669 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/read_compressed_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1118 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/scoped.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3660 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/scoped.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6581 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/sized_iterator.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      559 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/sized_iterator_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3257 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/sorted_uniform.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3621 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/sorted_uniform_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      751 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/spaces.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      167 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/spaces.hh
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.317063 bicleaner-hardrules-2.9.0/kenlm/util/stream/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1237 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/CMakeLists.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2420 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/block.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4367 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/chain.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     8996 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/chain.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1606 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/config.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      278 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/count_records.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      300 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/count_records.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2436 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/io.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1843 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/io.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      823 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/io_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1418 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/line_input.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      515 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/line_input.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2363 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_progress.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1848 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_progress.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3362 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3627 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3241 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      899 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    20450 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/sort.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1663 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/sort_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1821 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      759 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/stream_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      732 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/stream/typed_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     5480 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/string_piece.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     9185 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/string_piece.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1478 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/string_piece_hash.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1039 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/string_stream.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1778 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/string_stream_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     3825 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/thread_pool.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4890 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/tokenize_piece.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1135 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/tokenize_piece_test.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    11091 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/usage.cc
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      702 2023-03-06 13:42:00.000000 bicleaner-hardrules-2.9.0/kenlm/util/usage.hh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1694 2023-08-09 09:26:48.000000 bicleaner-hardrules-2.9.0/pyproject.toml
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.317063 bicleaner-hardrules-2.9.0/scripts/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     7429 2023-01-12 14:43:19.000000 bicleaner-hardrules-2.9.0/scripts/convert_to_generic_platform_wheel.py
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)      746 2023-08-09 09:31:07.000000 bicleaner-hardrules-2.9.0/scripts/release.sh
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       38 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/setup.cfg
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      288 2023-03-06 13:49:44.000000 bicleaner-hardrules-2.9.0/setup.py
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.297063 bicleaner-hardrules-2.9.0/src/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    14068 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/PKG-INFO
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10147 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/SOURCES.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)        1 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/dependency_links.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       75 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/entry_points.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      130 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/requires.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       10 2023-08-09 09:31:18.000000 bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/top_level.txt
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/src/hardrules/
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)      107 2023-01-30 13:17:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/__init__.py
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)    15955 2023-08-07 12:58:40.000000 bicleaner-hardrules-2.9.0/src/hardrules/bicleaner_hardrules.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    17887 2023-05-08 08:44:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/hardrules.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    14843 2023-08-07 12:52:21.000000 bicleaner-hardrules-2.9.0/src/hardrules/lm.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     2193 2023-01-30 13:17:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/tokenizer.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     6551 2023-01-30 13:17:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/training.py
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)     3122 2023-01-30 13:17:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/util.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    40402 2023-01-30 13:17:19.000000 bicleaner-hardrules-2.9.0/src/hardrules/writing_scripts.py
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-08-09 09:31:18.321063 bicleaner-hardrules-2.9.0/tests/
--rwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)     2367 2021-07-12 10:20:26.000000 bicleaner-hardrules-2.9.0/tests/hardrules_test.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      739 2021-05-24 08:58:36.000000 bicleaner-hardrules-2.9.0/tests/test-corpus.en-de
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/.github/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2094 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/.github/stale.yml
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2048 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/.gitignore
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       74 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/.gitmodules
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4054 2023-08-29 08:42:34.000000 bicleaner-hardrules-2.9.1/CHANGELOG.md
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    35147 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/LICENSE
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    14068 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/PKG-INFO
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    12770 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/README.md
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/kenlm/
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.923861 bicleaner-hardrules-2.9.1/kenlm/.github/
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/kenlm/.github/workflows/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      542 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/.github/workflows/mac.yml
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      619 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/.github/workflows/ubuntu.yml
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      471 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/.github/workflows/windows.yml
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      249 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/.gitignore
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      696 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/BUILDING
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4298 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    26530 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/COPYING
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    35147 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/COPYING.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7637 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/COPYING.LESSER.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    63537 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/Doxyfile
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1150 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/LICENSE
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      220 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/MANIFEST.in
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5394 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/README.md
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)       81 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/clean_query_only.sh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/kenlm/cmake/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2821 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/cmake/KenLMFunctions.cmake
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      334 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/cmake/kenlmConfig.cmake.in
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/kenlm/cmake/modules/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3185 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/cmake/modules/FindEigen3.cmake
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)     1154 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/compile_query_only.sh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.931861 bicleaner-hardrules-2.9.1/kenlm/lm/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2165 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3710 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/bhiksha.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4348 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/bhiksha.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    12931 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/binary_format.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3498 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/binary_format.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1379 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/blank.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     8154 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/build_binary_main.cc
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.931861 bicleaner-hardrules-2.9.1/kenlm/lm/builder/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1897 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      826 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/README.md
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      152 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/TODO
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    12607 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2258 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3509 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      899 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/combine_counts.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9550 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1701 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2820 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3992 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/count_ngrams_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2411 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/debug_print.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      439 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/discount.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1869 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/dump_counts_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      293 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/hash_gamma.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      715 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/header_info.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10698 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/initial_probabilities.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1452 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/initial_probabilities.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6044 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/interpolate.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1136 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/interpolate.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    11967 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/lmplz_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1625 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/output.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2529 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/output.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1051 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/payload.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    17887 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/pipeline.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2572 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/builder/pipeline.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.935861 bicleaner-hardrules-2.9.1/kenlm/lm/common/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      889 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6078 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/compare.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2366 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/joint_order.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5186 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2155 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1713 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2112 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/ngram.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1872 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/ngram_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1890 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/print.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1483 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/print.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      398 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/renumber.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      755 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/renumber.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      562 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/size_option.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      302 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/size_option.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      550 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/special.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.935861 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.935861 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       60 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy0.1
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      112 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy0.2
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      140 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy0.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       55 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy0.kenlm_intermediate
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       19 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy0.vocab
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       72 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy1.1
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      112 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy1.2
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      120 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy1.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       55 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy1.kenlm_intermediate
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       21 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/bigendian/toy1.vocab
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)      270 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/generate.sh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.935861 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       60 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy0.1
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      112 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy0.2
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      140 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy0.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       55 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy0.kenlm_intermediate
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       19 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy0.vocab
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       72 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy1.1
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      112 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy1.2
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      120 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy1.3
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       55 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy1.kenlm_intermediate
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       21 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/littleendian/toy1.vocab
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      475 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/toy0.arpa
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      470 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/common/test_data/toy1.arpa
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      675 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/config.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3913 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/config.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      722 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/enumerate_vocab.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2544 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/facade.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.935861 bicleaner-hardrules-2.9.1/kenlm/lm/filter/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1327 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1935 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/arpa_io.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2816 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/arpa_io.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2458 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/count_io.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9352 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/filter_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7379 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/format.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     8212 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5778 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5027 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase_table_vocab_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4205 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/thread.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1209 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/vocab.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4123 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/vocab.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1797 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/filter/wrapper.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1068 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/fragment_main.cc
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.939861 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1774 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      737 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_matrix.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1952 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      913 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4904 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1086 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2530 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3222 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      693 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/interpolate_info.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5296 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/interpolate_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10010 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_probabilities.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3385 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_probabilities.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3586 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      572 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5306 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    13813 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1101 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2758 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7645 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/pipeline.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      552 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/pipeline.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1235 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/split_worker.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1100 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/split_worker.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7430 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/streaming_example_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5950 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      590 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3969 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    19605 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2956 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4571 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      512 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_matrix.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1366 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_weights.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      446 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_weights.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      342 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/universal_vocab.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1347 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/universal_vocab.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9039 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/kenlm_benchmark_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7174 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/left.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    12402 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/left_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      637 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/lm_exception.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1057 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/lm_exception.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      644 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/max_order.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    16256 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/model.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7051 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/model.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    14544 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/model_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      798 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/model_type.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3534 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/ngram_query.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6003 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/partial.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6672 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/partial_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3743 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/quantize.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7749 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/quantize.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4675 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/query_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7543 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/read_arpa.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3016 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/read_arpa.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1248 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/return.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    12060 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/search_hashed.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5935 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/search_hashed.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    23394 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/search_trie.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4906 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/search_trie.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2594 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/sizes.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      374 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/sizes.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3440 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/state.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2780 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/test.arpa
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2694 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/test_nounk.arpa
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5639 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/trie.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3563 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/trie.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10982 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/trie_sort.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2795 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/trie_sort.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3935 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/value.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2045 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/value_build.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2568 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/value_build.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      380 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/virtual_interface.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5668 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/virtual_interface.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    11083 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/vocab.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     8680 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/vocab.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      358 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/weights.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      293 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/word_index.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.939861 bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      176 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/README
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4261 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/nplm.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1975 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/nplm.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.939861 bicleaner-hardrules-2.9.1/kenlm/python/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      988 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1957 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/_kenlm.pxd
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)     1427 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/example.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)   445847 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/kenlm.cpp
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9323 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/kenlm.pyx
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      906 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/score_sentence.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      325 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/python/score_sentence.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1976 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/setup.py
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.943861 bicleaner-hardrules-2.9.1/kenlm/util/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3873 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1176 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/bit_packing.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5967 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/bit_packing.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1490 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/bit_packing_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1227 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/cat_compressed_main.cc
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1042 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1527 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/LICENSE
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    27617 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum-dtoa.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4300 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum-dtoa.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    24726 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5891 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9913 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/cached-powers.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3021 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/cached-powers.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5030 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/diy-fp.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1804 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-conversion.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    15851 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-to-string.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    22349 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-to-string.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    31645 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fast-dtoa.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4064 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fast-dtoa.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    15352 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fixed-dtoa.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2770 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fixed-dtoa.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    15223 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/ieee.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    27857 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/string-to-double.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10848 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/string-to-double.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    23469 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/strtod.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3038 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/strtod.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    15340 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/utils.h
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1367 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/ersatz_progress.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1603 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/ersatz_progress.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2765 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/exception.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4392 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/exception.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3994 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/fake_ostream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    18350 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4746 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10877 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file_piece.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6515 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file_piece.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5364 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file_piece_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2424 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/file_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5545 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/fixed_array.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      729 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/float_to_string.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      609 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/float_to_string.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1441 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/getopt.c
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      472 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/getopt.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      270 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/have.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    22498 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1636 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1959 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4905 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/joint_sort.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1738 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/joint_sort_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    13507 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/mmap.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6780 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/mmap.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3379 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/multi_intersection.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1887 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/multi_intersection_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4074 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/murmur_hash.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      616 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/murmur_hash.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1546 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/parallel_read.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      461 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/parallel_read.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3480 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/pcqueue.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      355 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/pcqueue_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      705 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/pool.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2935 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/pool.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    13233 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    11788 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table_benchmark_main.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2269 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3526 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/proxy_iterator.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    13086 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/read_compressed.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2034 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/read_compressed.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2669 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/read_compressed_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1118 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/scoped.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3660 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/scoped.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6581 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/sized_iterator.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      559 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/sized_iterator_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3257 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/sorted_uniform.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3621 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/sorted_uniform_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      751 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/spaces.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      167 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/spaces.hh
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/kenlm/util/stream/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1237 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/CMakeLists.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2420 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/block.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4367 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/chain.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     8996 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/chain.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1606 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/config.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      278 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/count_records.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      300 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/count_records.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2436 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/io.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1843 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/io.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      823 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/io_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1418 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/line_input.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      515 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/line_input.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2363 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_progress.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1848 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_progress.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3362 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3627 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3241 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      899 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    20450 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/sort.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1663 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/sort_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1821 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      759 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/stream_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      732 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/stream/typed_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     5480 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/string_piece.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     9185 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/string_piece.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1478 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/string_piece_hash.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1039 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/string_stream.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1778 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/string_stream_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     3825 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/thread_pool.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     4890 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/tokenize_piece.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1135 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/tokenize_piece_test.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    11091 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/usage.cc
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      702 2023-08-29 08:48:47.000000 bicleaner-hardrules-2.9.1/kenlm/util/usage.hh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     1694 2023-08-29 08:42:50.000000 bicleaner-hardrules-2.9.1/pyproject.toml
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/scripts/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     7429 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/scripts/convert_to_generic_platform_wheel.py
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)      746 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/scripts/release.sh
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       38 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/setup.cfg
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      288 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/setup.py
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.927861 bicleaner-hardrules-2.9.1/src/
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    14068 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/PKG-INFO
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    10147 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/SOURCES.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)        1 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/dependency_links.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       75 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/entry_points.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      130 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/requires.txt
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)       10 2023-08-29 08:48:55.000000 bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/top_level.txt
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/src/hardrules/
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)      107 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/__init__.py
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)    15971 2023-08-29 08:41:35.000000 bicleaner-hardrules-2.9.1/src/hardrules/bicleaner_hardrules.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    17887 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/hardrules.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    14843 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/lm.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     2193 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/tokenizer.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)     6551 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/training.py
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)     3122 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/util.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)    40402 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/src/hardrules/writing_scripts.py
+drwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)        0 2023-08-29 08:48:55.947861 bicleaner-hardrules-2.9.1/tests/
+-rwxrwxr-x   0 jzaragoza  (1000) jzaragoza  (1000)     2367 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/tests/hardrules_test.py
+-rw-rw-r--   0 jzaragoza  (1000) jzaragoza  (1000)      739 2023-08-29 08:40:07.000000 bicleaner-hardrules-2.9.1/tests/test-corpus.en-de
```

### Comparing `bicleaner-hardrules-2.9.0/.github/stale.yml` & `bicleaner-hardrules-2.9.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/.gitignore` & `bicleaner-hardrules-2.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/CHANGELOG.md` & `bicleaner-hardrules-2.9.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Bicleaner Hardrules 2.9.1:
+* Fix hardrules crash without metadata.
+
 Bicleaner Hardrules 2.9.0:
 * Accept HF identifiers in `--metadata` argument.
 
 Bicleaner Hardrules 2.8.1:
 * Fix `no_url` regex
 * Fix builds with pip >= 23 using `fasttext-wheel`.
```

### Comparing `bicleaner-hardrules-2.9.0/LICENSE` & `bicleaner-hardrules-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/PKG-INFO` & `bicleaner-hardrules-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-hardrules
-Version: 2.9.0
+Version: 2.9.1
 Summary: Pre-filtering step for obvious noise based on rules, poor language based on general language modelling and vulgar language based on specific language modelling
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: HomePage, https://github.com/bitextor/bicleaner-hardrules
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
 Project-URL: MaCoCu, https://macocu.eu
```

### Comparing `bicleaner-hardrules-2.9.0/README.md` & `bicleaner-hardrules-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/.github/workflows/mac.yml` & `bicleaner-hardrules-2.9.1/kenlm/.github/workflows/mac.yml`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/.github/workflows/ubuntu.yml` & `bicleaner-hardrules-2.9.1/kenlm/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/BUILDING` & `bicleaner-hardrules-2.9.1/kenlm/BUILDING`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/COPYING` & `bicleaner-hardrules-2.9.1/kenlm/COPYING`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/COPYING.3` & `bicleaner-hardrules-2.9.1/kenlm/COPYING.3`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/COPYING.LESSER.3` & `bicleaner-hardrules-2.9.1/kenlm/COPYING.LESSER.3`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/Doxyfile` & `bicleaner-hardrules-2.9.1/kenlm/Doxyfile`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/LICENSE` & `bicleaner-hardrules-2.9.1/kenlm/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/README.md` & `bicleaner-hardrules-2.9.1/kenlm/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/cmake/KenLMFunctions.cmake` & `bicleaner-hardrules-2.9.1/kenlm/cmake/KenLMFunctions.cmake`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/cmake/modules/FindEigen3.cmake` & `bicleaner-hardrules-2.9.1/kenlm/cmake/modules/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/compile_query_only.sh` & `bicleaner-hardrules-2.9.1/kenlm/compile_query_only.sh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/lm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/bhiksha.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/bhiksha.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/bhiksha.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/bhiksha.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/binary_format.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/binary_format.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/binary_format.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/binary_format.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/blank.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/blank.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/build_binary_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/build_binary_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/README.md` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/adjust_counts_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/adjust_counts_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/combine_counts.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/combine_counts.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/corpus_count_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/corpus_count_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/count_ngrams_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/count_ngrams_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/debug_print.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/debug_print.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/dump_counts_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/dump_counts_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/header_info.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/header_info.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/initial_probabilities.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/initial_probabilities.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/initial_probabilities.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/initial_probabilities.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/interpolate.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/interpolate.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/interpolate.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/interpolate.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/lmplz_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/lmplz_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/output.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/output.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/output.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/output.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/payload.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/payload.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/pipeline.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/pipeline.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/builder/pipeline.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/builder/pipeline.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/compare.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/compare.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/joint_order.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/joint_order.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/model_buffer_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/model_buffer_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/ngram.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/ngram.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/ngram_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/ngram_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/print.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/print.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/print.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/print.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/renumber.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/renumber.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/size_option.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/size_option.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/common/special.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/common/special.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/config.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/config.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/config.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/config.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/enumerate_vocab.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/enumerate_vocab.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/facade.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/facade.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/arpa_io.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/arpa_io.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/arpa_io.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/arpa_io.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/count_io.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/count_io.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/filter_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/filter_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/format.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/format.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/phrase_table_vocab_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/phrase_table_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/thread.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/thread.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/vocab.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/vocab.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/vocab.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/vocab.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/filter/wrapper.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/filter/wrapper.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/fragment_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/fragment_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_matrix.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_matrix.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/backoff_reunification_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/backoff_reunification_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/bounded_sequence_encoding_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/bounded_sequence_encoding_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/interpolate_info.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/interpolate_info.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/interpolate_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/interpolate_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_probabilities.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_probabilities.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_probabilities.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_probabilities.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/merge_vocab_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/merge_vocab_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/normalize_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/normalize_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/pipeline.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/pipeline.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/pipeline.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/pipeline.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/split_worker.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/split_worker.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/split_worker.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/split_worker.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/streaming_example_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/streaming_example_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_derivatives_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_derivatives_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_instances_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_instances_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_matrix.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_matrix.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/tune_weights.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/tune_weights.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/interpolate/universal_vocab.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/interpolate/universal_vocab.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/kenlm_benchmark_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/kenlm_benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/left.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/left.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/left_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/left_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/lm_exception.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/lm_exception.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/lm_exception.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/lm_exception.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/max_order.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/max_order.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/model.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/model.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/model.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/model.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/model_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/model_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/model_type.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/model_type.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/ngram_query.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/ngram_query.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/partial.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/partial.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/partial_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/partial_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/quantize.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/quantize.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/quantize.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/quantize.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/query_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/query_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/read_arpa.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/read_arpa.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/read_arpa.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/read_arpa.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/return.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/return.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/search_hashed.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/search_hashed.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/search_hashed.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/search_hashed.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/search_trie.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/search_trie.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/search_trie.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/search_trie.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/sizes.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/sizes.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/state.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/state.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/test.arpa` & `bicleaner-hardrules-2.9.1/kenlm/lm/test.arpa`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/test_nounk.arpa` & `bicleaner-hardrules-2.9.1/kenlm/lm/test_nounk.arpa`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/trie.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/trie.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/trie.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/trie.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/trie_sort.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/trie_sort.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/trie_sort.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/trie_sort.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/value.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/value.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/value_build.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/value_build.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/value_build.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/value_build.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/virtual_interface.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/virtual_interface.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/vocab.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/vocab.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/vocab.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/vocab.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/nplm.cc` & `bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/nplm.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/lm/wrappers/nplm.hh` & `bicleaner-hardrules-2.9.1/kenlm/lm/wrappers/nplm.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/_kenlm.pxd` & `bicleaner-hardrules-2.9.1/kenlm/python/_kenlm.pxd`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/example.py` & `bicleaner-hardrules-2.9.1/kenlm/python/example.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/kenlm.cpp` & `bicleaner-hardrules-2.9.1/kenlm/python/kenlm.cpp`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/kenlm.pyx` & `bicleaner-hardrules-2.9.1/kenlm/python/kenlm.pyx`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/python/score_sentence.cc` & `bicleaner-hardrules-2.9.1/kenlm/python/score_sentence.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/setup.py` & `bicleaner-hardrules-2.9.1/kenlm/setup.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/bit_packing.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/bit_packing.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/bit_packing.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/bit_packing.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/bit_packing_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/bit_packing_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/cat_compressed_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/cat_compressed_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/LICENSE` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum-dtoa.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum-dtoa.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/bignum.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/bignum.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/cached-powers.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/cached-powers.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/cached-powers.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/diy-fp.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/diy-fp.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-conversion.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-conversion.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-to-string.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-to-string.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/double-to-string.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/double-to-string.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fast-dtoa.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fast-dtoa.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fixed-dtoa.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/fixed-dtoa.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/ieee.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/ieee.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/string-to-double.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/string-to-double.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/string-to-double.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/string-to-double.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/strtod.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/strtod.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/strtod.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/strtod.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/double-conversion/utils.h` & `bicleaner-hardrules-2.9.1/kenlm/util/double-conversion/utils.h`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/ersatz_progress.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/ersatz_progress.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/ersatz_progress.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/ersatz_progress.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/exception.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/exception.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/exception.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/exception.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/fake_ostream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/fake_ostream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/file.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/file.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file_piece.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/file_piece.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file_piece.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/file_piece.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file_piece_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/file_piece_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/file_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/file_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/fixed_array.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/fixed_array.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/float_to_string.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/float_to_string.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/float_to_string.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/float_to_string.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/getopt.c` & `bicleaner-hardrules-2.9.1/kenlm/util/getopt.c`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/integer_to_string_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/integer_to_string_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/joint_sort.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/joint_sort.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/joint_sort_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/joint_sort_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/mmap.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/mmap.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/mmap.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/mmap.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/multi_intersection.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/multi_intersection.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/multi_intersection_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/multi_intersection_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/murmur_hash.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/murmur_hash.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/murmur_hash.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/murmur_hash.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/parallel_read.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/parallel_read.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/pcqueue.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/pcqueue.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/pool.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/pool.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/pool.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/pool.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table_benchmark_main.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table_benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/probing_hash_table_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/probing_hash_table_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/proxy_iterator.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/proxy_iterator.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/read_compressed.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/read_compressed.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/read_compressed.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/read_compressed.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/read_compressed_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/read_compressed_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/scoped.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/scoped.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/scoped.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/scoped.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/sized_iterator.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/sized_iterator.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/sized_iterator_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/sized_iterator_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/sorted_uniform.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/sorted_uniform.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/sorted_uniform_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/sorted_uniform_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/spaces.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/spaces.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/CMakeLists.txt` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/block.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/block.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/chain.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/chain.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/chain.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/chain.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/config.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/config.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/io.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/io.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/io.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/io.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/io_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/io_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/line_input.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/line_input.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/line_input.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/line_input.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_progress.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_progress.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_progress.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_progress.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/multi_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/multi_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/rewindable_stream_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/rewindable_stream_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/sort.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/sort.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/sort_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/sort_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/stream_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/stream_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/stream/typed_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/stream/typed_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/string_piece.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/string_piece.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/string_piece.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/string_piece.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/string_piece_hash.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/string_piece_hash.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/string_stream.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/string_stream.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/string_stream_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/string_stream_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/thread_pool.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/thread_pool.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/tokenize_piece.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/tokenize_piece.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/tokenize_piece_test.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/tokenize_piece_test.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/usage.cc` & `bicleaner-hardrules-2.9.1/kenlm/util/usage.cc`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/kenlm/util/usage.hh` & `bicleaner-hardrules-2.9.1/kenlm/util/usage.hh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/pyproject.toml` & `bicleaner-hardrules-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-hardrules"
-version = "2.9.0"
+version = "2.9.1"
 authors = [
     { name="Prompsit Language Engineering", email="info@prompsit.com" },
 ]
 maintainers = [
     { name="Jaume Zaragoza", email="jzaragoza@prompsit.com" },
 ]
 description = "Pre-filtering step for obvious noise based on rules, poor language based on general language modelling and vulgar language based on specific language modelling"
```

### Comparing `bicleaner-hardrules-2.9.0/scripts/convert_to_generic_platform_wheel.py` & `bicleaner-hardrules-2.9.1/scripts/convert_to_generic_platform_wheel.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/scripts/release.sh` & `bicleaner-hardrules-2.9.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/PKG-INFO` & `bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-hardrules
-Version: 2.9.0
+Version: 2.9.1
 Summary: Pre-filtering step for obvious noise based on rules, poor language based on general language modelling and vulgar language based on specific language modelling
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: HomePage, https://github.com/bitextor/bicleaner-hardrules
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
 Project-URL: MaCoCu, https://macocu.eu
```

### Comparing `bicleaner-hardrules-2.9.0/src/bicleaner_hardrules.egg-info/SOURCES.txt` & `bicleaner-hardrules-2.9.1/src/bicleaner_hardrules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/bicleaner_hardrules.py` & `bicleaner-hardrules-2.9.1/src/hardrules/bicleaner_hardrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     if args.disable_porn_removal:
         logging.info("Porn removal disabled.")
 
     return args
 
 
 def real_metadata_path(path):
-    if os.path.exists(path):
+    if path is None or os.path.exists(path):
         # local path, we just use it, return abs path
         return path
     elif not path.startswith('bitextor/bicleaner-ai'):
         # In case does not exist, check if it follows the pattern of HF bicleaner-ai models
         # If not, just raise the error
         raise FileNotFoundError(f"No such file or directory: {path}'.")
```

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/hardrules.py` & `bicleaner-hardrules-2.9.1/src/hardrules/hardrules.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/lm.py` & `bicleaner-hardrules-2.9.1/src/hardrules/lm.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/tokenizer.py` & `bicleaner-hardrules-2.9.1/src/hardrules/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/training.py` & `bicleaner-hardrules-2.9.1/src/hardrules/training.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/util.py` & `bicleaner-hardrules-2.9.1/src/hardrules/util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/src/hardrules/writing_scripts.py` & `bicleaner-hardrules-2.9.1/src/hardrules/writing_scripts.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/tests/hardrules_test.py` & `bicleaner-hardrules-2.9.1/tests/hardrules_test.py`

 * *Files identical despite different names*

### Comparing `bicleaner-hardrules-2.9.0/tests/test-corpus.en-de` & `bicleaner-hardrules-2.9.1/tests/test-corpus.en-de`

 * *Files identical despite different names*

