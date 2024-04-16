# Comparing `tmp/genvarloader-0.3.0rc9.tar.gz` & `tmp/genvarloader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genvarloader-0.3.0rc9.tar", max compression
+gzip compressed data
```

## Comparing `genvarloader-0.3.0rc9.tar` & `genvarloader-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,209 @@
--rw-r--r--   0        0        0     1066 2024-02-21 06:02:22.615882 genvarloader-0.3.0rc9/LICENSE.txt
--rw-r--r--   0        0        0     2490 2024-02-21 06:02:22.633881 genvarloader-0.3.0rc9/README.md
--rw-r--r--   0        0        0      853 2024-03-30 22:34:02.264463 genvarloader-0.3.0rc9/genvarloader/__init__.py
--rw-r--r--   0        0        0     6930 2024-03-30 02:40:18.688383 genvarloader-0.3.0rc9/genvarloader/bigwig.py
--rw-r--r--   0        0        0      974 2024-03-15 17:35:16.493320 genvarloader-0.3.0rc9/genvarloader/concurrent.py
--rw-r--r--   0        0        0    30424 2024-03-30 18:32:02.258072 genvarloader-0.3.0rc9/genvarloader/dataset/__init__.py
--rw-r--r--   0        0        0    11497 2024-03-27 00:42:02.847243 genvarloader-0.3.0rc9/genvarloader/dataset/genotypes.py
--rw-r--r--   0        0        0     3508 2024-03-29 06:32:50.132301 genvarloader-0.3.0rc9/genvarloader/dataset/intervals.py
--rw-r--r--   0        0        0     1734 2024-03-30 02:40:39.916247 genvarloader-0.3.0rc9/genvarloader/dataset/reference.py
--rw-r--r--   0        0        0     2231 2024-03-27 00:41:27.472445 genvarloader-0.3.0rc9/genvarloader/dataset/utils.py
--rw-r--r--   0        0        0    11265 2024-03-30 02:41:07.147073 genvarloader-0.3.0rc9/genvarloader/dataset/write.py
--rw-r--r--   0        0        0     6498 2024-03-30 02:41:09.481059 genvarloader-0.3.0rc9/genvarloader/fasta.py
--rw-r--r--   0        0        0    25831 2024-03-30 02:41:00.571114 genvarloader-0.3.0rc9/genvarloader/haplotypes.py
--rw-r--r--   0        0        0    10153 2024-02-27 06:15:30.815938 genvarloader-0.3.0rc9/genvarloader/intervals.py
--rw-r--r--   0        0        0    48210 2024-03-30 22:31:32.165320 genvarloader-0.3.0rc9/genvarloader/loader.py
--rw-r--r--   0        0        0        0 2024-02-27 06:15:30.824938 genvarloader-0.3.0rc9/genvarloader/py.typed
--rw-r--r--   0        0        0     4215 2024-03-30 22:32:45.959898 genvarloader-0.3.0rc9/genvarloader/torch.py
--rw-r--r--   0        0        0     2829 2024-03-16 22:26:22.431646 genvarloader-0.3.0rc9/genvarloader/types.py
--rw-r--r--   0        0        0    12751 2024-03-30 22:31:38.520283 genvarloader-0.3.0rc9/genvarloader/utils.py
--rw-r--r--   0        0        0    11614 2024-03-30 02:40:37.456262 genvarloader-0.3.0rc9/genvarloader/variants/__init__.py
--rw-r--r--   0        0        0    24360 2024-03-30 02:40:35.765273 genvarloader-0.3.0rc9/genvarloader/variants/genotypes.py
--rw-r--r--   0        0        0    28450 2024-03-30 02:40:33.378289 genvarloader-0.3.0rc9/genvarloader/variants/records.py
--rw-r--r--   0        0        0    10369 2024-03-30 02:40:41.323238 genvarloader-0.3.0rc9/genvarloader/zarr.py
--rw-r--r--   0        0        0     1653 2024-03-30 22:34:02.260463 genvarloader-0.3.0rc9/pyproject.toml
--rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 genvarloader-0.3.0rc9/PKG-INFO
+-rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 genvarloader-0.3.1/Cargo.toml
+-rw-r--r--   0     1111     7010     2200 2024-04-16 16:39:32.000000 genvarloader-0.3.1/.gitignore
+-rw-r--r--   0     1111     7010      432 2024-03-15 17:35:16.000000 genvarloader-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0     1111     7010     1066 2024-02-21 06:02:22.000000 genvarloader-0.3.1/LICENSE.txt
+-rw-r--r--   0     1111     7010     2490 2024-02-21 06:02:22.000000 genvarloader-0.3.1/README.md
+-rw-r--r--   0     1111     7010     2520 2024-04-16 16:39:32.000000 genvarloader-0.3.1/cli.py
+-rw-r--r--   0     1111     7010      624 2024-02-21 06:02:22.000000 genvarloader-0.3.1/dev-environment.yml
+-rw-r--r--   0     1111     7010      365 2024-02-21 06:02:22.000000 genvarloader-0.3.1/environment.yml
+-rw-r--r--   0     1111     7010   159221 2024-04-16 16:39:32.000000 genvarloader-0.3.1/poetry.lock
+-rw-r--r--   0     1111     7010      912 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/__init__.py
+-rw-r--r--   0     1111     7010     6056 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/bigwig.py
+-rw-r--r--   0     1111     7010      974 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/concurrent.py
+-rw-r--r--   0     1111     7010    35779 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/__init__.py
+-rw-r--r--   0     1111     7010    32628 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/genotypes.py
+-rw-r--r--   0     1111     7010     5335 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/intervals.py
+-rw-r--r--   0     1111     7010     1679 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/reference.py
+-rw-r--r--   0     1111     7010    15054 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/tracks.py
+-rw-r--r--   0     1111     7010     2589 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/utils.py
+-rw-r--r--   0     1111     7010    12527 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/write.py
+-rw-r--r--   0     1111     7010     8341 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/fasta.py
+-rw-r--r--   0     1111     7010      877 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/genvarloader.pyi
+-rw-r--r--   0     1111     7010    25831 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/haplotypes.py
+-rw-r--r--   0     1111     7010    10153 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/intervals.py
+-rw-r--r--   0     1111     7010    48210 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/loader.py
+-rw-r--r--   0     1111     7010        0 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/py.typed
+-rw-r--r--   0     1111     7010     4215 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/torch.py
+-rw-r--r--   0     1111     7010     8437 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/types.py
+-rw-r--r--   0     1111     7010    13407 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/utils.py
+-rw-r--r--   0     1111     7010    11614 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/__init__.py
+-rw-r--r--   0     1111     7010    28477 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/genotypes.py
+-rw-r--r--   0     1111     7010    29659 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/records.py
+-rw-r--r--   0     1111     7010    10433 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/zarr.py
+-rw-r--r--   0     1111     7010     4206 2024-04-16 16:39:32.000000 genvarloader-0.3.1/src/bigwig.rs
+-rw-r--r--   0     1111     7010     1325 2024-04-16 16:39:32.000000 genvarloader-0.3.1/src/lib.rs
+-rw-r--r--   0     1111     7010     1697 2024-02-21 06:05:07.000000 genvarloader-0.3.1/tests/data/pgen/sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     2189 2024-02-21 06:05:07.000000 genvarloader-0.3.1/tests/data/pgen/sample.gvl.arrow
+-rw-r--r--   0     1111     7010       63 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.pgen
+-rw-r--r--   0     1111     7010       42 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.psam
+-rw-r--r--   0     1111     7010     2241 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.pvar
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010     1761 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     1997 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.arrow
+-rw-r--r--   0     1111     7010      223 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zarray
+-rw-r--r--   0     1111     7010      133 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zattrs
+-rw-r--r--   0     1111     7010    81381 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0
+-rw-r--r--   0     1111     7010     2890 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf
+-rw-r--r--   0     1111     7010     1272 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf.gz
+-rw-r--r--   0     1111     7010      189 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf.gz.csi
+-rw-r--r--   0     1111     7010     6218 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/generate_ground_truth.py
+-rw-r--r--   0     1111     7010      212 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/sample.bed
+-rw-r--r--   0     1111     7010     2327 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/sample.vcf
+-rw-r--r--   0     1111     7010     2136 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/dataset/genotypes/test_dense2sparse.py
+-rw-r--r--   0     1111     7010     1626 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_fasta.py
+-rw-r--r--   0     1111     7010     2814 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_fasta_variants.py
+-rw-r--r--   0     1111     7010     1625 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_loader.py
+-rw-r--r--   0     1111     7010     3102 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/test_max_ends.py
+-rw-r--r--   0     1111     7010     5838 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/test_pgen.py
+-rw-r--r--   0     1111     7010      391 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/test_utils.py
+-rw-r--r--   0     1111     7010      633 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_variants.py
+-rw-r--r--   0     1111     7010     3677 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/bench_cpu_gpu.py
+-rw-r--r--   0     1111     7010     3484 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/test_i2t_t2i.py
+-rw-r--r--   0     1111     7010     1000 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/test_random_nonoverlapping.py
+-rw-r--r--   0     1111     7010     2435 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/utils.py
+-rw-r--r--   0     1111     7010    35103 2024-04-16 16:39:32.000000 genvarloader-0.3.1/Cargo.lock
+-rw-r--r--   0     1111     7010     1797 2024-04-16 16:52:32.000000 genvarloader-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 genvarloader-0.3.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `genvarloader-0.3.0rc9/LICENSE.txt` & `genvarloader-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/README.md` & `genvarloader-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/bigwig.py` & `genvarloader-0.3.1/python/genvarloader/bigwig.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union, cast
+from typing import Dict, List, Optional, Union
 
-import joblib
 import numpy as np
 import polars as pl
 import pyBigWig
-from attrs import define
 from numpy.typing import ArrayLike, NDArray
 
-from .types import Reader
+from .genvarloader import intervals as bw_intervals
+from .types import INTERVAL_DTYPE, RaggedIntervals, Reader
 from .utils import get_rel_starts, normalize_contig_name
 
 
 class BigWigs(Reader):
-    dtype: np.float32  # pyBigWig always returns f32
+    dtype = np.float32  # pyBigWig always returns f32
     chunked = False
 
     def __init__(self, name: str, paths: Dict[str, str]) -> None:
         """Read data from bigWig files.
 
         Parameters
         ----------
@@ -58,23 +57,29 @@
             Path to a table or a DataFrame containing sample names and paths to bigWig files for those samples.
         """
         if isinstance(table, (str, Path)):
             table = Path(table)
             if table.suffix == ".csv":
                 table = pl.read_csv(table)
             elif table.suffix == ".tsv" or table.suffix == ".txt":
-                table = pl.read_tsv(table)
+                table = pl.read_csv(table, separator="\t")
             else:
                 raise ValueError("Table should be a csv or tsv file.")
         paths = dict(zip(table["sample"], table["path"]))
         return cls(name, paths)
 
     def rev_strand_fn(self, x):
         return x[..., ::-1]
 
+    def close(self):
+        if self.readers is not None:
+            for reader in self.readers.values():
+                reader.close()
+            self.readers = None
+
     def read(
         self,
         contig: str,
         starts: ArrayLike,
         ends: ArrayLike,
         **kwargs,
     ) -> NDArray[np.float32]:
@@ -118,70 +123,52 @@
         rel_ends = rel_starts + (ends - starts)
 
         out = np.empty((len(samples), (ends - starts).sum()), dtype=np.float32)
         for s, e, r_s, r_e in zip(starts, ends, rel_starts, rel_ends):
             for i, sample in enumerate(samples):
                 out[i, r_s:r_e] = self.readers[sample].values(contig, s, e, numpy=True)
 
-        out[np.isnan(out)] = 0
+        out = np.nan_to_num(out, copy=False)
 
         return out
 
-    def intervals(self, contig: str, starts: ArrayLike, ends: ArrayLike, **kwargs):
+    def intervals(
+        self,
+        contig: str,
+        starts: ArrayLike,
+        ends: ArrayLike,
+        sample: Optional[Union[str, List[str]]] = None,
+        **kwargs,
+    ) -> RaggedIntervals:
         _contig = normalize_contig_name(contig, self.contigs)
         if _contig is None:
             raise ValueError(f"Contig {contig} not found.")
         else:
             contig = _contig
 
-        samples = kwargs.get("sample", self.samples)
-        if isinstance(samples, str):
-            samples = [samples]
+        if sample is None:
+            samples = self.samples
+        elif isinstance(sample, str):
+            samples = [sample]
+        else:
+            samples = sample
+
         if not set(samples).issubset(self.samples):
             raise ValueError(f"Sample {samples} not found in bigWig paths.")
 
-        starts = np.atleast_1d(np.asarray(starts, dtype=int))
-        ends = np.atleast_1d(np.asarray(ends, dtype=int))
-        starts = np.maximum(0, starts)
-        ends = np.minimum(ends, self.contigs[contig])
+        starts = np.atleast_1d(np.asarray(starts, dtype=np.int32))
+        ends = np.atleast_1d(np.asarray(ends, dtype=np.int32))
+        paths = [self.paths[s] for s in samples]
 
-        def task(contig: str, starts: NDArray, ends: NDArray, path: str):
-            intervals_ls: List[Tuple[int, int, float]] = []
-            # (n_queries)
-            n_per_query = np.empty(len(starts), np.uint32)
-            with pyBigWig.open(path, "r") as f:
-                for i, (s, e) in enumerate(zip(starts, ends)):
-                    _intervals = cast(
-                        Optional[Tuple[Tuple[int, int, float], ...]],
-                        f.intervals(contig, s, e),
-                    )
-                    if _intervals is not None:
-                        intervals_ls.extend(_intervals)
-                        n_per_query[i] = len(_intervals)
-                    else:
-                        n_per_query[i] = 0
-            # (n_intervals, 2)
-            intervals = np.array([i[:2] for i in intervals_ls], np.uint32)
-            # (n_intervals)
-            values = np.array([i[2] for i in intervals_ls], np.float32)
-            return Intervals(intervals, values, n_per_query)
-
-        with joblib.Parallel(n_jobs=-1) as parallel:
-            result = cast(
-                List[Intervals],
-                parallel(
-                    joblib.delayed(task)(contig, starts, ends, self.paths[sample])
-                    for sample in samples
-                ),
-            )
-
-        intervals = np.concatenate([i.intervals for i in result])
-        values = np.concatenate([i.values for i in result])
-        n_per_query = np.concatenate([i.n_per_query for i in result])
-        return Intervals(intervals, values, n_per_query)
-
-
-@define
-class Intervals:
-    intervals: NDArray[np.uint32]  # (n_intervals, 2)
-    values: NDArray[np.float32]  # (n_intervals)
-    n_per_query: NDArray[np.uint32]  # (n_queries)
+        # (intervals, 2) (intervals) (regions, samples)
+        coordinates, values, n_per_query = bw_intervals(paths, contig, starts, ends)
+
+        coordinates = coordinates.astype(np.int32)
+
+        intervals = np.empty(len(coordinates), dtype=INTERVAL_DTYPE)
+        intervals["start"] = coordinates[:, 0]
+        intervals["end"] = coordinates[:, 1]
+        intervals["value"] = values
+
+        intervals = RaggedIntervals.from_lengths(intervals, n_per_query)
+
+        return intervals
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/concurrent.py` & `genvarloader-0.3.1/python/genvarloader/concurrent.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/dataset/__init__.py` & `genvarloader-0.3.1/python/genvarloader/dataset/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,104 @@
 import json
 from pathlib import Path
 from textwrap import dedent
 from typing import (
     TYPE_CHECKING,
+    Any,
     Callable,
+    Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
+    Sized,
     Tuple,
     Union,
 )
 
 import numba as nb
 import numpy as np
 import polars as pl
+import seqpro as sp
 from attrs import define, evolve
+from einops import repeat
 from loguru import logger
 from numpy.typing import NDArray
+from tqdm.auto import tqdm
 
 from ..torch import get_dataloader
-from ..utils import read_bedlike, with_length
+from ..types import INTERVAL_DTYPE, Idx, Ragged, RaggedIntervals
+from ..utils import lengths_to_offsets, read_bedlike, with_length
 from ..variants import VLenAlleles
-from .genotypes import Genotypes, get_diffs, padded_slice, reconstruct_haplotypes
-from .intervals import Intervals, intervals_to_hap_values, intervals_to_values
+from .genotypes import (
+    SparseGenotypes,
+    get_diffs_sparse,
+    padded_slice,
+    reconstruct_haplotypes_from_sparse,
+)
+from .intervals import intervals_to_tracks, tracks_to_intervals
 from .reference import Reference
-from .utils import regions_to_bed, subset_to_full_raveled_mapping
+from .tracks import shift_and_realign_tracks_sparse
+from .utils import oidx_to_raveled_idx, regions_to_bed, splits_sum_le_value
 
 try:
     import torch
     import torch.utils.data as td
 
     TORCH_AVAILABLE = True
 except ImportError:
     TORCH_AVAILABLE = False
 
-Idx = Union[int, np.integer, Sequence[int], NDArray[np.integer], slice]
-ListIdx = Union[Sequence[int], NDArray[np.integer]]
-
 
 @define
 class _Variants:
     positions: NDArray[np.int32]
     sizes: NDArray[np.int32]
     alts: VLenAlleles
 
     @classmethod
-    def from_dataframe(cls, variants: Union[str, Path, pl.DataFrame]):
+    def from_table(cls, variants: Union[str, Path, pl.DataFrame]):
         if isinstance(variants, (str, Path)):
             variants = pl.read_ipc(variants)
         return cls(
             variants["POS"].to_numpy(),
             variants["ILEN"].to_numpy(),
             VLenAlleles.from_polars(variants["ALT"]),
         )
 
 
 @define(frozen=True)
 class Dataset:
     """A dataset of genotypes, reference sequences, and intervals. Note: this class is not meant to be instantiated directly.
-    Use the `open` or `open_with_settings` class methods to create a dataset after writing the data with genvarloader.write()
+    Use the `open` or `open_with_settings` class methods to create a dataset after writing the data with `genvarloader.write()`
     or the genvarloader CLI.
     """
 
     path: Path
     max_jitter: int
-    n_variants: int
-    n_intervals: int
+    jitter: int
     region_length: int
     contigs: List[str]
-    _samples: NDArray[np.str_]
-    _regions: NDArray[np.int32]
+    full_samples: List[str]
+    full_regions: NDArray[np.int32]
     rng: np.random.Generator
     sample_idxs: NDArray[np.intp]
     region_idxs: NDArray[np.intp]
-    return_sequences: Literal[False, "reference", "haplotypes"]
+    sequence_type: Optional[Literal["reference", "haplotypes"]]
+    active_tracks: Optional[List[str]]
+    available_tracks: List[str]
     ploidy: Optional[int] = None
-    _reference: Optional[Reference] = None
-    _variants: Optional[_Variants] = None
-    has_intervals: bool = False
-    return_tracks: bool = False
-    _genotypes: Optional["Genotypes"] = None
-    _intervals: Optional["Intervals"] = None
+    reference: Optional[Reference] = None
+    variants: Optional[_Variants] = None
+    genotypes: Optional[SparseGenotypes] = None
+    intervals: Optional[Dict[str, RaggedIntervals]] = None
     transform: Optional[Callable] = None
-    _idx_map: Optional[NDArray[np.intp]] = None
-    _jitter: Optional[int] = None
+    idx_map: Optional[NDArray[np.intp]] = None
     return_indices: bool = False
-    transformed_intervals: Optional[str] = None
 
     @classmethod
     def open(
         cls,
         path: Union[str, Path],
         reference: Optional[Union[str, Path]] = None,
     ):
@@ -103,29 +110,30 @@
             The path to the dataset.
         reference : Optional[Union[str, Path]], optional
             The path to the reference genome, by default None
         """
         path = Path(path)
         if not path.exists():
             raise FileNotFoundError(f"{path} does not exist.")
-        samples: NDArray[np.str_] = np.load(path / "samples.npy")
         regions: NDArray[np.int32] = np.load(path / "regions.npy")
 
+        has_intervals = (path / "intervals").exists()
+        has_genotypes = (path / "genotypes").exists()
+
         with open(path / "metadata.json") as f:
             metadata = json.load(f)
 
-        contigs = metadata["contigs"]
-        region_length = int(metadata["region_length"])
-        ploidy = int(metadata.get("ploidy", 0))
-        n_variants = int(metadata.get("n_variants", 0))
-        n_intervals = int(metadata.get("n_intervals", 0))
-        max_jitter = int(metadata.get("max_jitter", 0))
+        samples: List[str] = metadata["samples"]
+        contigs: List[str] = metadata["contigs"]
+        region_length: int = metadata["region_length"]
+        ploidy: int = metadata.get("ploidy", 0)
+        max_jitter: int = metadata.get("max_jitter", 0)
         rng = np.random.default_rng()
 
-        if reference is None and n_variants > 0:
+        if reference is None and has_genotypes:
             logger.warning(
                 dedent(
                     """
                     Genotypes found but no reference genome provided. This is required to reconstruct haplotypes.
                     No reference or haplotype sequences can be returned by this dataset instance.
                     """
                 )
@@ -138,255 +146,384 @@
             )
             _reference = Reference.from_path_and_contigs(reference, contigs)
             has_reference = True
         else:
             _reference = None
             has_reference = False
 
-        if n_variants > 0:
-            variants = _Variants.from_dataframe(path / "variants.arrow")
-            has_genotypes = True
+        if has_genotypes:
+            variants = _Variants.from_table(path / "genotypes" / "variants.arrow")
         else:
             variants = None
-            has_genotypes = False
 
-        if n_intervals > 0:
-            has_intervals = True
+        if has_intervals:
+            tracks: List[str] = []
+            for p in (path / "intervals").iterdir():
+                if len(list(p.iterdir())) == 0:
+                    p.rmdir()
+                else:
+                    tracks.append(p.name)
+            tracks.sort()
+            active_tracks = tracks
         else:
-            has_intervals = False
+            tracks = []
+            active_tracks = None
 
         if has_reference and has_genotypes:
-            return_sequences = "haplotypes"
+            sequence_type = "haplotypes"
         elif has_reference:
-            return_sequences = "reference"
+            sequence_type = "reference"
         else:
-            return_sequences = False
-
-        if has_intervals:
-            return_tracks = True
-        else:
-            return_tracks = False
+            sequence_type = None
 
         dataset = cls(
             path=path,
             max_jitter=max_jitter,
-            n_variants=n_variants,
-            n_intervals=n_intervals,
+            jitter=max_jitter,
             region_length=region_length,
             contigs=contigs,
-            _samples=samples,
-            _regions=regions,
+            full_samples=samples,
+            full_regions=regions,
             rng=rng,
             sample_idxs=np.arange(len(samples), dtype=np.intp),
             region_idxs=np.arange(len(regions), dtype=np.intp),
             ploidy=ploidy,
-            _reference=_reference,
-            _variants=variants,
-            has_intervals=has_intervals,
-            return_sequences=return_sequences,
-            return_tracks=return_tracks,
+            reference=_reference,
+            variants=variants,
+            available_tracks=tracks,
+            sequence_type=sequence_type,
+            active_tracks=active_tracks,
         )
 
         logger.info(f"\n{str(dataset)}")
 
         return dataset
 
     @classmethod
     def open_with_settings(
         cls,
         path: Union[str, Path],
         reference: Optional[Union[str, Path]] = None,
         samples: Optional[Sequence[str]] = None,
         regions: Optional[Union[str, Path, pl.DataFrame]] = None,
         return_sequences: Optional[Literal[False, "reference", "haplotypes"]] = None,
-        return_tracks: Optional[bool] = None,
+        return_tracks: Optional[Union[Literal[False], str, List[str]]] = None,
         transform: Optional[Callable] = None,
         seed: Optional[int] = None,
         jitter: Optional[int] = None,
         return_indices: Optional[bool] = None,
-        transformed_intervals: Optional[str] = None,
     ):
         if return_sequences is False:
             reference = None
         ds = cls.open(path, reference).with_settings(
             samples=samples,
             regions=regions,
             return_sequences=return_sequences,
             return_tracks=return_tracks,
             transform=transform,
             seed=seed,
             jitter=jitter,
             return_indices=return_indices,
-            transformed_intervals=transformed_intervals,
         )
         return ds
 
-    @property
-    def has_reference(self) -> bool:
-        return self._reference is not None
+    def with_settings(
+        self,
+        samples: Optional[Sequence[str]] = None,
+        regions: Optional[Union[str, Path, pl.DataFrame]] = None,
+        return_sequences: Optional[Literal[False, "reference", "haplotypes"]] = None,
+        return_tracks: Optional[Union[Literal[False], str, List[str]]] = None,
+        transform: Optional[Union[Literal[False], Callable]] = None,
+        seed: Optional[int] = None,
+        jitter: Optional[int] = None,
+        return_indices: Optional[bool] = None,
+    ):
+        """Modify settings of the dataset, returning a new dataset without modifying the old one.
 
-    @property
-    def has_genotypes(self) -> bool:
-        return self._variants is not None
+        Parameters
+        ----------
+        samples : Optional[Sequence[str]], optional
+            The samples to subset to, by default None
+        regions : Optional[Union[str, Path, pl.DataFrame]], optional
+            The regions to subset to, by default None
+        return_sequences : Optional[Literal[False, "reference", "haplotypes"]], optional
+            The sequence type to return. Set this to False to disable returning sequences entirely.
+        return_tracks : Optional[Union[Literal[False], List[str]]], optional
+            The tracks to return, by default None. Set this to False to disable returning tracks entirely.
+        transform : Optional[Callable], optional
+            The transform to set, by default None
+        seed : Optional[int], optional
+            The seed to set, by default None
+        jitter : Optional[int], optional
+            The jitter to set, by default None
+        return_indices : Optional[bool], optional
+            Whether to return indices, by default None
+        transformed_intervals : Optional[str], optional
+            The transformed intervals to set, by default None
+        extra_tracks : Optional[Dict[str, GenomeTrack]], optional
+            The extra tracks to set, by default None
+        """
+        ds = self
+        to_evolve: Dict[str, Any] = {}
 
-    @property
-    def samples(self):
-        if self._idx_map is None:
-            return self._samples
-        else:
-            return self._samples[self.sample_idxs]
+        if samples is not None or regions is not None:
+            ds = ds.subset_to(regions=regions, samples=samples)
 
-    @property
-    def regions(self):
-        if self._idx_map is None:
-            return self._regions
-        else:
-            return self._regions[self.region_idxs]
+        if return_sequences is not None:
+            if return_sequences == "haplotypes" and not self.has_genotypes:
+                raise ValueError(
+                    "No genotypes found. Cannot be set to yield haplotypes since genotypes are required to yield haplotypes."
+                )
+            if return_sequences == "reference" and not self.has_reference:
+                raise ValueError(
+                    "No reference found. Cannot be set to yield reference sequences since reference is required to yield reference sequences."
+                )
+            if return_sequences is False:
+                to_evolve["sequence_type"] = None
+            else:
+                to_evolve["sequence_type"] = return_sequences
+
+        if return_tracks is not None:
+            if return_tracks is False:
+                to_evolve["active_tracks"] = None
+            else:
+                if isinstance(return_tracks, str):
+                    return_tracks = [return_tracks]
+                if missing := set(return_tracks).difference(self.available_tracks):
+                    raise ValueError(
+                        f"Intervals {missing} not found. Available intervals: {self.available_tracks}"
+                    )
+                to_evolve["active_tracks"] = return_tracks
+
+        if transform is not None:
+            if transform is False:
+                transform = None
+            to_evolve["transform"] = transform
+
+        if seed is not None:
+            to_evolve["rng"] = np.random.default_rng(seed)
+
+        if jitter is not None:
+            if jitter < 0:
+                raise ValueError("Jitter must be a non-negative integer.")
+            elif jitter > self.max_jitter:
+                raise ValueError(
+                    f"Jitter must be less than or equal to the maximum jitter of the dataset ({self.max_jitter})."
+                )
+            to_evolve["jitter"] = jitter
+
+        if return_indices is not None:
+            to_evolve["return_indices"] = return_indices
+
+        return evolve(ds, **to_evolve)
 
     @property
-    def n_samples(self):
-        return len(self.sample_idxs)
+    def has_reference(self) -> bool:
+        return self.reference is not None
 
     @property
-    def n_regions(self):
-        return len(self.region_idxs)
+    def has_genotypes(self) -> bool:
+        return self.variants is not None
 
     @property
-    def shape(self):
-        """Return the shape of the dataset. (n_samples, n_regions)"""
-        return self.n_samples, self.n_regions
+    def has_intervals(self) -> bool:
+        return len(self.available_tracks) > 0
 
     @property
-    def jitter(self):
-        if self._jitter is None:
-            return self.max_jitter
+    def samples(self) -> List[str]:
+        if self.idx_map is None:
+            return self.full_samples
         else:
-            return self._jitter
+            return [self.full_samples[i] for i in self.sample_idxs]
 
     @property
-    def output_length(self):
-        return self.region_length - 2 * self.jitter
+    def regions(self) -> NDArray[np.int32]:
+        if self.idx_map is None:
+            return self.full_regions
+        else:
+            return self.full_regions[self.region_idxs]
 
     @property
-    def _full_shape(self):
-        """Return the full shape of the dataset, ignoring any subsetting. (n_samples, n_regions)"""
-        return len(self._samples), len(self._regions)
+    def n_samples(self) -> int:
+        return len(self.sample_idxs)
 
     @property
-    def available_transformed_intervals(self):
-        if not self.has_intervals:
-            avail = None
-        else:
-            avail = [p.stem[:-1] for p in (self.path / "intervals").glob("*_.npy")]
-        return avail
+    def n_regions(self) -> int:
+        return len(self.region_idxs)
 
     @property
-    def haplotypes(self):
-        """Dataset that only returns haplotypes, if available."""
-        return self.with_settings(return_sequences="haplotypes", return_tracks=False)
+    def output_length(self) -> int:
+        return self.region_length - 2 * self.jitter
 
     @property
-    def reference(self):
-        """Dataset that only returns reference sequences, if available."""
-        return self.with_settings(return_sequences="reference", return_tracks=False)
+    def shape(self) -> Tuple[int, int]:
+        """Return the shape of the dataset. (n_samples, n_regions)"""
+        return self.n_regions, self.n_samples
 
     @property
-    def tracks(self):
-        """Dataset that only returns tracks, if available."""
-        return self.with_settings(return_sequences=False, return_tracks=True)
+    def full_shape(self) -> Tuple[int, int]:
+        """Return the full shape of the dataset, ignoring any subsetting. (n_regions, n_samples)"""
+        return len(self.full_regions), len(self.full_samples)
 
     def __len__(self) -> int:
-        return self.n_samples * self.n_regions
+        return int(np.prod(self.shape))
 
-    def add_transformed_intervals(
+    def write_transformed_tracks(
         self,
-        name: str,
+        new_track: str,
+        existing_track: str,
         transform: Callable[
-            [pl.DataFrame, NDArray[np.intp], NDArray[np.uint32], NDArray[np.float32]],
-            NDArray[np.float32],
+            [NDArray[np.intp], NDArray[np.intp], NDArray[np.intp], Ragged[np.float32]],
+            Ragged[np.float32],
         ],
+        max_mem: int = 2**30,
+        overwrite: bool = False,
     ):
-        """Add transformed interval data to the dataset, writing them to disk with the given name.
-
-        Note: only transformations that would modify non-zero values of tracks are applicable. For example, if the intent
-        is to add a constant to a track, this would not be applicable since zero values are not stored in the intervals, and
-        thus would not be transformed.
+        """Write transformed tracks to the dataset.
 
         Parameters
         ----------
-        name : str
-            The name of the transformed intervals.
-        transform : Callable
-            A function that takes a DataFrame of regions, sample indices, interval starts and
-            ends, and values and returns new values.
+        new_track : str
+            The name of the new track.
+        existing_track : str
+            The name of the existing track to transform.
+        transform
+            A function to apply to the existing track to get a new, transformed track.
+            This will be done in chunks such that the tracks provided will not exceed `max_mem`.
+            The arguments given to the transform will be the regions for each track in the chunk as a polars
+            DataFrame, the sample indices for each track in the chunk, and the tracks themselves.
+            Note that the tracks will be a :class:`Ragged` array with shape (regions, samples)
+            since regions may be different lengths to accomodate indels. This function should then
+            return the transformed tracks as a :class:`Ragged` array with the same shape and lengths.
+        max_mem : int, optional
+            The maximum memory to use in bytes, by default `2**30`
+        overwrite : bool, optional
+            Whether to overwrite the existing track, by default False
         """
+        if new_track == existing_track:
+            raise ValueError(
+                "New track name must be different from existing track name."
+            )
 
-        if not self.has_intervals:
+        if existing_track not in self.available_tracks:
             raise ValueError(
-                "No intervals found. Cannot add transformed intervals since intervals are required to add transformed intervals."
+                f"Requested existing track {existing_track} does not exist in this dataset."
             )
 
-        if self._intervals is None:
-            all_intervals = self.init_intervals()
+        if self.intervals is None:
+            intervals = self.init_intervals(existing_track)[existing_track]
         else:
-            all_intervals = self._intervals
+            intervals = self.intervals[existing_track]
 
-        # limit memory usage to 1 GB per partition
-        # 2 uint32 for positions, 1 float32 for value
-        regions = self.get_bed()
-        max_intervals_per_batch = 89478485  # 2**30 / (2*4) positions / (4) values
-        split_indices = (
-            np.diff(
-                (all_intervals.offsets[1:] % max_intervals_per_batch).astype(np.int32)
+        out_dir = self.path / "intervals" / new_track
+
+        if out_dir.exists() and not overwrite:
+            raise FileExistsError(
+                f"{out_dir} already exists. Set overwrite=True to overwrite."
             )
-            < 0
-        ).nonzero()[0] + 1
-        split_indices = np.r_[0, split_indices, len(all_intervals.offsets) - 1]
+        elif out_dir.exists() and overwrite:
+            # according to GVL file format, should only have intervals.npy and offsets.npy in here
+            for p in out_dir.iterdir():
+                p.unlink()
+            out_dir.rmdir()
+
+        out_dir.mkdir(parents=True, exist_ok=True)
+
+        lengths = self.full_regions[:, 2] - self.full_regions[:, 1]
+        # for each region:
+        # bytes = (4 bytes / bp) * (bp / sample) * samples
+        n_samples = len(self.full_samples)
+        mem_per_region = 4 * lengths * n_samples
+        splits = splits_sum_le_value(mem_per_region, max_mem)
+        memmap_intervals_offset = 0
+        memmap_offsets_offset = 0
         last_offset = 0
-        for offset_s, offset_e in zip(split_indices[:-1], split_indices[1:]):
-            s_idxs, r_idxs = np.unravel_index(
-                np.arange(offset_s, offset_e, dtype=np.intp), self._full_shape
-            )
-            interval_s, interval_e = (
-                all_intervals.offsets[offset_s],
-                all_intervals.offsets[offset_e],
-            )
-            intervals = all_intervals.intervals[interval_s:interval_e]
-            values = all_intervals.values[interval_s:interval_e]
-            transformed_intervals = transform(
-                regions[r_idxs], s_idxs, intervals, values
-            )
-            out = np.memmap(
-                self.path / "intervals" / f"{name}_.npy",
-                dtype=np.float32,
-                mode="w+",
-                shape=len(transformed_intervals),
-                offset=last_offset,
-            )
-            out[:] = transformed_intervals
-            out.flush()
-            last_offset += out.nbytes
+        with tqdm(total=len(splits) - 1) as pbar:
+            for offset_s, offset_e in zip(splits[:-1], splits[1:]):
+                r_idx = np.arange(offset_s, offset_e, dtype=np.intp)
+                n_regions = len(r_idx)
+                s_idx = np.arange(n_samples, dtype=np.intp)
+                r_idx = repeat(r_idx, "r -> (r s)", s=n_samples)
+                s_idx = repeat(s_idx, "s -> (r s)", r=n_regions)
+                ds_idx = np.ravel_multi_index((r_idx, s_idx), self.full_shape)
+
+                pbar.set_description("Writing (decompressing)")
+                regions = self.full_regions[r_idx]
+                # layout is (regions, samples) so all samples are local for statistics
+                tracks = intervals_to_tracks(
+                    ds_idx,
+                    regions,
+                    intervals.data,
+                    intervals.offsets,
+                )
+                track_lengths = lengths[r_idx].reshape(n_regions, n_samples)
+                tracks = Ragged.from_lengths(tracks, track_lengths)
+
+                pbar.set_description("Writing (transforming)")
+                transformed_tracks = transform(ds_idx, r_idx, s_idx, tracks)
+                np.testing.assert_equal(tracks.shape, transformed_tracks.shape)
+
+                pbar.set_description("Writing (compressing)")
+                itvs, interval_offsets = tracks_to_intervals(
+                    regions, transformed_tracks.data
+                )
+                np.testing.assert_equal(
+                    len(interval_offsets), n_regions * n_samples + 1
+                )
+
+                out = np.memmap(
+                    out_dir / "intervals.npy",
+                    dtype=itvs.dtype,
+                    mode="w+" if memmap_intervals_offset == 0 else "r+",
+                    shape=itvs.shape,
+                    offset=memmap_intervals_offset,
+                )
+                out[:] = itvs[:]
+                out.flush()
+                memmap_intervals_offset += out.nbytes
+
+                interval_offsets += last_offset
+                last_offset = interval_offsets[-1]
+                out = np.memmap(
+                    out_dir / "offsets.npy",
+                    dtype=interval_offsets.dtype,
+                    mode="w+" if memmap_offsets_offset == 0 else "r+",
+                    shape=len(interval_offsets) - 1,
+                    offset=memmap_offsets_offset,
+                )
+                out[:] = interval_offsets[:-1]
+                out.flush()
+                memmap_offsets_offset += out.nbytes
+                pbar.update()
+
+        out = np.memmap(
+            out_dir / "offsets.npy",
+            dtype=interval_offsets.dtype,  # type: ignore
+            mode="r+",
+            shape=1,
+            offset=memmap_offsets_offset,
+        )
+        out[-1] = interval_offsets[-1]  # type: ignore
+        out.flush()
 
     def subset_to(
         self,
-        samples: Optional[Sequence[str]] = None,
         regions: Optional[Union[str, Path, pl.DataFrame]] = None,
+        samples: Optional[Sequence[str]] = None,
     ):
         if regions is None and samples is None:
             return self
 
         if samples is not None:
             _samples = set(samples)
-            if missing := _samples.difference(self._samples):
+            if missing := _samples.difference(self.full_samples):
                 raise ValueError(f"Samples {missing} not found in the dataset")
             sample_idxs = np.array(
-                [i for i, s in enumerate(self.samples) if s in _samples], np.intp
+                [i for i, s in enumerate(self.full_samples) if s in _samples], np.intp
             )
-            if self._idx_map is not None:
-                sample_idxs = self.sample_idxs[sample_idxs]
         else:
             sample_idxs = self.sample_idxs
 
         if regions is not None:
             if isinstance(regions, (str, Path)):
                 regions = read_bedlike(regions)
             regions = with_length(regions, self.region_length)
@@ -400,129 +537,34 @@
                 .to_numpy()
             )
             n_available_regions = len(region_idxs)
             if n_query_regions != len(region_idxs):
                 raise ValueError(
                     f"Only {n_available_regions}/{n_query_regions} requested regions exist in the dataset."
                 )
-            if self._idx_map is not None:
-                region_idxs = self.region_idxs[region_idxs]
         else:
             region_idxs = self.region_idxs
 
-        idx_map = subset_to_full_raveled_mapping(
-            self._full_shape,
-            sample_idxs,
-            region_idxs,
+        idx_map = oidx_to_raveled_idx(
+            row_idx=region_idxs,
+            col_idx=sample_idxs,
+            full_shape=self.full_shape,
         )
 
         return evolve(
-            self, sample_idxs=sample_idxs, region_idxs=region_idxs, _idx_map=idx_map
+            self, sample_idxs=sample_idxs, region_idxs=region_idxs, idx_map=idx_map
         )
 
     def to_full_dataset(self):
-        sample_idxs = np.arange(len(self._samples), dtype=np.intp)
-        region_idxs = np.arange(len(self._regions), dtype=np.intp)
+        sample_idxs = np.arange(len(self.full_samples), dtype=np.intp)
+        region_idxs = np.arange(len(self.full_regions), dtype=np.intp)
         return evolve(
-            self, sample_idxs=sample_idxs, region_idxs=region_idxs, _idx_map=None
+            self, sample_idxs=sample_idxs, region_idxs=region_idxs, idx_map=None
         )
 
-    def with_settings(
-        self,
-        samples: Optional[Sequence[str]] = None,
-        regions: Optional[Union[str, Path, pl.DataFrame]] = None,
-        return_sequences: Optional[Literal[False, "reference", "haplotypes"]] = None,
-        return_tracks: Optional[bool] = None,
-        transform: Optional[Callable] = None,
-        seed: Optional[int] = None,
-        jitter: Optional[int] = None,
-        return_indices: Optional[bool] = None,
-        transformed_intervals: Optional[str] = None,
-    ):
-        """Modify settings of the dataset, returning a new dataset without modifying the old one.
-
-        Parameters
-        ----------
-        samples : Optional[Sequence[str]], optional
-            The samples to subset to, by default None
-        regions : Optional[Union[str, Path, pl.DataFrame]], optional
-            The regions to subset to, by default None
-        sequence_mode : Optional[Literal["reference", "haplotypes"]], optional
-            The sequence mode to set, by default None. Set this to False to disable returning sequences entirely.
-        track_mode : Optional[bool], optional
-            The track mode to set, by default None
-        transform : Optional[Callable], optional
-            The transform to set, by default None
-        seed : Optional[int], optional
-            The seed to set, by default None
-        jitter : Optional[int], optional
-            The jitter to set, by default None
-        return_indices : Optional[bool], optional
-            Whether to return indices, by default None
-        transformed_intervals : Optional[str], optional
-            The transformed intervals to set, by default None
-        """
-        ds = self
-        to_evolve = {}
-
-        if samples is not None or regions is not None:
-            ds = ds.subset_to(samples, regions)
-
-        if return_sequences is not None:
-            if return_sequences == "haplotypes" and not self.has_genotypes:
-                raise ValueError(
-                    "No genotypes found. Cannot be set to yield haplotypes since genotypes are required to yield haplotypes."
-                )
-            if return_sequences == "reference" and not self.has_reference:
-                raise ValueError(
-                    "No reference found. Cannot be set to yield reference sequences since reference is required to yield reference sequences."
-                )
-            to_evolve["return_sequences"] = return_sequences
-
-        if return_tracks is not None:
-            if return_tracks:
-                if not self.has_intervals:
-                    raise ValueError(
-                        "No intervals found. Cannot be set to yield tracks since intervals are required to yield tracks."
-                    )
-                to_evolve["return_tracks"] = True
-            else:
-                to_evolve["return_tracks"] = False
-
-        if transform is not None:
-            to_evolve["transform"] = transform
-
-        if seed is not None:
-            to_evolve["rng"] = np.random.default_rng(seed)
-
-        if jitter is not None:
-            if jitter < 0:
-                raise ValueError("Jitter must be a non-negative integer.")
-            elif jitter > self.max_jitter:
-                raise ValueError(
-                    f"Jitter must be less than or equal to the maximum jitter of the dataset ({self.max_jitter})."
-                )
-            to_evolve["_jitter"] = jitter
-
-        if return_indices is not None:
-            to_evolve["return_indices"] = return_indices
-
-        if transformed_intervals is not None:
-            if self.available_transformed_intervals is None:
-                raise ValueError(
-                    "No transformed intervals available. Use the add_transformed_intervals method to add transformed intervals."
-                )
-            elif transformed_intervals not in self.available_transformed_intervals:
-                raise ValueError(
-                    f"Transformed intervals {transformed_intervals} not found. Available transformed intervals: {self.available_transformed_intervals}"
-                )
-            to_evolve["transformed_intervals"] = transformed_intervals
-
-        return evolve(ds, **to_evolve)
-
     def to_dataset(self):
         """Convert the dataset to a map-style PyTorch Dataset."""
         return TorchDataset(self)
 
     def to_dataloader(
         self,
         batch_size: int = 1,
@@ -560,99 +602,102 @@
             pin_memory_device=pin_memory_device,
         )
 
     def __str__(self) -> str:
         return dedent(
             f"""
             GVL store {self.path.name}
+            Is subset: {self.idx_map is not None}
+            # of regions: {self.n_regions:,}
+            # of samples: {self.n_samples:,}
             Original region length: {self.region_length - 2*self.max_jitter:,}
             Max jitter: {self.max_jitter:,}
-            # of samples: {self.n_samples:,}
-            # of regions: {self.n_regions:,}
-            Has genotypes: {self.n_variants > 0}
-            Has intervals: {self.n_intervals > 0}
-            Is subset: {self._idx_map is not None}\
+            Has genotypes: {self.has_genotypes}
+            Has tracks: {self.available_tracks}\
             """
         ).strip()
 
     def __repr__(self) -> str:
         return str(self)
 
-    def isel(self, samples: Idx, regions: Idx):
-        """Select a subset of samples and regions from the dataset.
+    def isel(self, regions: Idx, samples: Idx):
+        """Eagerly select a subset of samples and regions from the dataset.
 
         Parameters
         ----------
         samples : ListIdx
             The indices of the samples to select.
         regions : ListIdx
             The indices of the regions to select.
         """
+        if isinstance(regions, slice):
+            if regions.stop is None:
+                regions = slice(regions.start, len(self.full_regions))
+            _regions = np.arange(
+                regions.start, regions.stop, regions.step, dtype=np.intp
+            )
+        else:
+            _regions = regions
+
         if isinstance(samples, slice):
             if samples.stop is None:
-                samples = slice(samples.start, len(self._samples))
+                samples = slice(samples.start, len(self.full_samples))
             _samples = np.arange(
                 samples.start, samples.stop, samples.step, dtype=np.intp
             )
         else:
             _samples = samples
 
-        if isinstance(regions, slice):
-            if regions.stop is None:
-                regions = slice(regions.start, len(self._regions))
-            _regions = np.arange(
-                regions.start, regions.stop, regions.step, dtype=np.intp
-            )
-        else:
-            _regions = regions
+        if (not isinstance(_samples, Sized)) != (not isinstance(_regions, Sized)):
+            _samples, _regions = np.broadcast_arrays(_samples, _regions)
 
-        ds_idxs = np.ravel_multi_index((_samples, _regions), self.shape)
+        ds_idxs = np.ravel_multi_index((_regions, _samples), self.shape)
         return self[ds_idxs]
 
-    def sel(self, samples: List[str], regions: pl.DataFrame):
-        """Select a subset of samples and regions from the dataset.
+    def sel(self, regions: pl.DataFrame, samples: List[str]):
+        """Eagerly select a subset of samples and regions from the dataset.
 
         Parameters
         ----------
         samples : List[str]
             The names of the samples to select.
         regions : pl.DataFrame
             The regions to select.
         """
-        s_to_i = dict(zip(self._samples, range(len(self._samples))))
+        s_to_i = dict(zip(self.full_samples, range(len(self.full_samples))))
         sample_idxs = np.array([s_to_i[s] for s in samples], np.intp)
         region_idxs = (
             with_length(regions, self.region_length)
             .join(
                 self.get_bed().with_row_count(),
                 on=["chrom", "chromStart", "chromEnd"],
                 how="left",
             )
             .get_column("row_nr")
         )
         if (n_missing := region_idxs.is_null().sum()) > 0:
             raise ValueError(f"{n_missing} regions not found in the dataset.")
         region_idxs = region_idxs.to_numpy()
-        ds_idxs = np.ravel_multi_index((sample_idxs, region_idxs), self.shape)
+        ds_idxs = np.ravel_multi_index((region_idxs, sample_idxs), self.shape)
         return self[ds_idxs]
 
-    def __getitem__(self, idx: Idx) -> Union[NDArray, Tuple[NDArray, NDArray]]:
+    def __getitem__(self, idx: Idx) -> Union[NDArray, Tuple[NDArray, ...], Any]:
         """Get a batch of haplotypes and tracks or intervals and tracks.
 
         Parameters
         ----------
         idx: Idx
             The index or indices to get. If a single index is provided, the output will be squeezed.
         """
-        to_evolve = {}
-        if self._genotypes is None and self.return_sequences == "haplotypes":
-            to_evolve["genotypes"] = self.init_genotypes()
-        if self._intervals is None and self.return_tracks:
-            to_evolve["intervals"] = self.init_intervals(self.transformed_intervals)
-        self = evolve(self, **to_evolve)
+        # Since Dataset is a frozen class, we need to use object.__setattr__ to set the attributes
+        # per attrs docs (https://www.attrs.org/en/stable/init.html#post-init)
+        if self.genotypes is None and self.sequence_type == "haplotypes":
+            object.__setattr__(self, "genotypes", self.init_genotypes())
+        if self.intervals is None and self.active_tracks:
+            object.__setattr__(self, "intervals", self.init_intervals())
 
         if isinstance(idx, (int, np.integer)):
             _idx = [idx]
             squeeze = True
         elif isinstance(idx, slice):
             if idx.stop is None:
                 idx = slice(idx.start, len(self))
@@ -660,206 +705,276 @@
             squeeze = False
         else:
             _idx = idx
             squeeze = False
 
         _idx = np.asarray(_idx, dtype=np.intp)
         _idx[_idx < 0] += len(self)
-        if self._idx_map is not None:
-            _idx = self._idx_map[_idx]
-        s_idx, r_idx = np.unravel_index(_idx, self._full_shape)
-
-        regions = self._regions[r_idx]
+        if self.idx_map is not None:
+            _idx = self.idx_map[_idx]
+        r_idx, s_idx = np.unravel_index(_idx, self.full_shape)
+        to_rc = self.full_regions[r_idx, 3] == -1
+        should_rc = to_rc.any()
 
         out: List[NDArray] = []
 
-        if self.return_sequences == "haplotypes":
+        if self.sequence_type == "haplotypes":
             if TYPE_CHECKING:
-                assert self._genotypes is not None
-                assert self._variants is not None
+                assert self.genotypes is not None
+                assert self.variants is not None
 
-            genos = self._genotypes[s_idx, r_idx]
-            shifts = self.get_shifts(genos, self._variants.sizes)
-            out.append(self.get_haplotypes(genos, regions, shifts))
-        elif self.return_sequences == "reference":
+            geno_offset_idx = self.get_geno_offset_idx(r_idx, s_idx)
+            # (b p)
+            shifts = self.get_shifts(geno_offset_idx)
+            # (b p l)
+            haps = self.get_haplotypes(geno_offset_idx, r_idx, shifts)
+            if should_rc:
+                haps[to_rc] = sp.DNA.reverse_complement(haps[to_rc], -1)
+            out.append(haps)
+        elif self.sequence_type == "reference":
             if TYPE_CHECKING:
-                assert self._reference is not None
+                assert self.reference is not None
+            geno_offset_idx = None
             shifts = None
-            out.append(
-                get_reference(
-                    regions,
-                    self._reference.reference,
-                    self._reference.offsets,
-                    self.region_length,
-                    self._reference.pad_char,
-                ).view("S1")
-            )
+            ref = get_reference(
+                r_idx,
+                self.full_regions,
+                self.reference.reference,
+                self.reference.offsets,
+                self.region_length,
+                self.reference.pad_char,
+            ).view("S1")
+            if should_rc:
+                ref[to_rc] = sp.DNA.reverse_complement(ref[to_rc], -1)
+            out.append(ref)
         else:
+            geno_offset_idx = None
             shifts = None
 
-        if self.return_tracks:
-            out.append(self.get_tracks(_idx, r_idx, shifts))
+        if self.active_tracks:
+            # [(b p l) ...]
+            tracks = self.get_tracks(_idx, r_idx, shifts, geno_offset_idx)
+            if should_rc:
+                for t in tracks:
+                    t[to_rc] = t[to_rc, ..., ::-1]
+            out.extend(tracks)
 
         if self.jitter > 0:
             start = self.rng.integers(
                 self.max_jitter - self.jitter, self.max_jitter + 1
             )
+            # [(b p l-2*j) ...]
             out = [o[..., start : start + self.output_length] for o in out]
 
         if squeeze:
+            # (1 p l) -> (p l)
             out = [o.squeeze() for o in out]
 
         if self.return_indices:
             out.extend((_idx, s_idx, r_idx))
 
-        if self.transform is not None:
-            out = self.transform(*out)
+        _out = tuple(out)
 
         if len(out) == 1:
-            _out = out[0]
-        else:
-            _out = out
+            _out = _out[0]
+
+        if self.transform is not None:
+            if isinstance(_out, tuple):
+                _out = self.transform(*_out)
+            else:
+                _out = self.transform(_out)
 
-        return _out  # type: ignore
+        return _out
 
     def init_genotypes(self):
         if TYPE_CHECKING:
             assert self.ploidy is not None
-        n_samples = len(self._samples)
-        genotypes = Genotypes(
+        genotypes = SparseGenotypes(
             np.memmap(
-                self.path / "genotypes" / "genotypes.npy",
-                shape=(self.n_variants * n_samples, self.ploidy),
-                dtype=np.int8,
-                mode="r",
-            ),
-            np.memmap(
-                self.path / "genotypes" / "first_variant_idxs.npy",
-                dtype=np.uint32,
+                self.path / "genotypes" / "variant_idxs.npy",
+                dtype=np.int32,
                 mode="r",
             ),
             np.memmap(
                 self.path / "genotypes" / "offsets.npy", dtype=np.uint32, mode="r"
             ),
-            n_samples,
+            len(self.full_regions),
+            len(self.full_samples),
+            self.ploidy,
         )
         return genotypes
 
-    def init_intervals(self, transform: Optional[str] = None):
-        if transform is None:
-            values_file = "values.npy"
-        else:
-            values_file = f"{transform}_.npy"
+    def init_intervals(self, tracks: Optional[Union[str, List[str]]] = None):
+        if TYPE_CHECKING:
+            assert self.active_tracks is not False
 
-        intervals = Intervals(
-            np.memmap(
-                self.path / "intervals" / "intervals.npy",
-                shape=(self.n_intervals, 2),
-                dtype=np.uint32,
+        if tracks is None:
+            tracks = self.available_tracks
+        elif isinstance(tracks, str):
+            tracks = [tracks]
+
+        intervals: Dict[str, RaggedIntervals] = {}
+        for track in tracks:
+            itvs = np.memmap(
+                self.path / "intervals" / track / "intervals.npy",
+                dtype=INTERVAL_DTYPE,
                 mode="r",
-            ),
-            np.memmap(
-                self.path / "intervals" / values_file,
-                dtype=np.float32,
-                mode="r",
-            ),
-            np.memmap(
-                self.path / "intervals" / "offsets.npy",
-                dtype=np.uint32,
+            )
+            offsets = np.memmap(
+                self.path / "intervals" / track / "offsets.npy",
+                dtype=np.int32,
                 mode="r",
-            ),
-        )
+            )
+            intervals[track] = RaggedIntervals.from_offsets(
+                itvs, self.full_shape, offsets
+            )
 
         return intervals
 
-    def get_shifts(self, genos: "Genotypes", variant_sizes: NDArray[np.int32]):
-        diffs = get_diffs(genos.first_v_idxs, genos.offsets, genos.genos, variant_sizes)
-        shifts = self.rng.integers(0, diffs + 1, dtype=np.uint32)
+    def get_geno_offset_idx(self, region_idx, sample_idx):
+        if TYPE_CHECKING:
+            assert self.genotypes is not None
+            assert self.ploidy is not None
+        ploid_idx = np.arange(self.ploidy, dtype=np.intp)
+        rsp_idx = (region_idx[:, None], sample_idx[:, None], ploid_idx)
+        geno_offset_idx = np.ravel_multi_index(rsp_idx, self.genotypes.effective_shape)
+        return geno_offset_idx
+
+    def get_shifts(self, geno_offset_idx: NDArray[np.intp]):
+        if TYPE_CHECKING:
+            assert self.genotypes is not None
+            assert self.variants is not None
+        # (b p)
+        diffs = get_diffs_sparse(
+            geno_offset_idx,
+            self.genotypes.variant_idxs,
+            self.genotypes.offsets,
+            self.variants.sizes,
+        )
+        # (b p)
+        shifts = self.rng.integers(0, diffs + 1, dtype=np.int32)
         return shifts
 
     def get_haplotypes(
         self,
-        genos: "Genotypes",
-        regions: NDArray[np.int32],
-        shifts: NDArray[np.uint32],
-    ):
+        geno_offset_idx: NDArray[np.intp],
+        region_idx: NDArray[np.intp],
+        shifts: NDArray[np.int32],
+    ) -> NDArray[np.bytes_]:
         if TYPE_CHECKING:
-            assert self._reference is not None
-            assert self._variants is not None
+            assert self.genotypes is not None
+            assert self.reference is not None
+            assert self.variants is not None
             assert self.ploidy is not None
 
-        haps = np.empty((len(regions), self.ploidy, self.region_length), np.uint8)
-        reconstruct_haplotypes(
+        n_queries = len(region_idx)
+        haps = np.empty((n_queries, self.ploidy, self.region_length), np.uint8)
+        reconstruct_haplotypes_from_sparse(
+            geno_offset_idx,
             haps,
-            regions,
+            self.full_regions[region_idx],
             shifts,
-            genos.first_v_idxs,
-            genos.offsets,
-            genos.genos,
-            self._variants.positions,
-            self._variants.sizes,
-            self._variants.alts.alleles.view(np.uint8),
-            self._variants.alts.offsets,
-            self._reference.reference,
-            self._reference.offsets,
-            self._reference.pad_char,
+            self.genotypes.offsets,
+            self.genotypes.variant_idxs,
+            self.variants.positions,
+            self.variants.sizes,
+            self.variants.alts.alleles.view(np.uint8),
+            self.variants.alts.offsets,
+            self.reference.reference,
+            self.reference.offsets,
+            self.reference.pad_char,
         )
         return haps.view("S1")
 
     def get_tracks(
         self,
-        ds_idx: NDArray[np.intp],
-        r_idx: NDArray[np.intp],
-        shifts: Optional[NDArray[np.uint32]] = None,
+        dataset_idx: NDArray[np.intp],
+        region_idx: NDArray[np.intp],
+        shifts: Optional[NDArray[np.int32]] = None,
+        geno_offset_idx: Optional[NDArray[np.intp]] = None,
     ):
         if TYPE_CHECKING:
-            assert self._intervals is not None
+            assert self.active_tracks is not None
+            assert self.intervals is not None
 
-        if shifts is not None:
-            values = intervals_to_hap_values(
-                ds_idx,
-                r_idx,
-                self.regions,
-                shifts,
-                self._intervals.intervals,
-                self._intervals.values,
-                self._intervals.offsets,
-                self.region_length,
-            )
-        else:
-            values = intervals_to_values(
-                ds_idx,
-                r_idx,
-                self.regions,
-                self._intervals.intervals,
-                self._intervals.values,
-                self._intervals.offsets,
-                self.region_length,
-            )
-        return values
+        # fancy indexing makes a copy so safe to mutate
+        regions = self.full_regions[region_idx]
+        if shifts is None:
+            # no shifts -> don't need to consider max ends, can use uniform region length
+            regions[:, 2] = regions[:, 1] + self.region_length
+
+        tracks: List[NDArray[np.float32]] = []
+        for name in self.active_tracks:
+            intervals = self.intervals[name]
+            # (b*l) ragged
+            _tracks = intervals_to_tracks(
+                dataset_idx,
+                regions,
+                intervals.data,
+                intervals.offsets,
+            )
+
+            if shifts is not None and geno_offset_idx is not None:
+                if TYPE_CHECKING:
+                    assert self.ploidy is not None
+                    assert self.variants is not None
+                    assert self.genotypes is not None
+
+                length_per_region = regions[:, 2] - regions[:, 1]
+                track_offsets = lengths_to_offsets(length_per_region)
+
+                out = np.empty(
+                    (len(region_idx), self.ploidy, self.region_length), np.float32
+                )
+                shift_and_realign_tracks_sparse(
+                    offset_idx=geno_offset_idx,
+                    variant_idxs=self.genotypes.variant_idxs,
+                    offsets=self.genotypes.offsets,
+                    regions=regions,
+                    positions=self.variants.positions,
+                    sizes=self.variants.sizes,
+                    shifts=shifts,
+                    tracks=_tracks,
+                    track_offsets=track_offsets,
+                    out=out,
+                )
+                _tracks = out
+            else:
+                # (b*l) ragged -> (b l)
+                _tracks = _tracks.reshape(len(region_idx), self.region_length)
+
+            tracks.append(_tracks)
+
+        return tracks
 
     def get_bed(self):
-        """Get a polars DataFrame of the regions in the dataset, corresponding to the full length
+        """Get a polars DataFrame of the regions in the dataset, corresponding to the coordinates
         used when writing the dataset. In other words, each region will have length
-        output_length + 2 * max_jitter."""
-        bed = regions_to_bed(self.regions, self.contigs)
+        `ds.output_length + 2 * ds.max_jitter`."""
+        bed = regions_to_bed(self.full_regions, self.contigs)
+        bed = bed.with_columns(chromEnd=pl.col("chromStart") + self.region_length)
         return bed
 
+    def __iter__(self):
+        for i in range(len(self)):
+            yield self[i]
+
 
 @nb.njit(parallel=True, nogil=True, cache=True)
 def get_reference(
+    r_idxs: NDArray[np.int32],
     regions: NDArray[np.int32],
     reference: NDArray[np.uint8],
     ref_offsets: NDArray[np.uint64],
     region_length: int,
     pad_char: int,
 ) -> NDArray[np.uint8]:
     out = np.empty((len(regions), region_length), np.uint8)
     for region in nb.prange(len(regions)):
-        q = regions[region]
+        q = regions[r_idxs[region]]
         c_idx = q[0]
         c_s = ref_offsets[c_idx]
         c_e = ref_offsets[c_idx + 1]
         start = q[1]
         end = q[2]
         out[region] = padded_slice(reference[c_s:c_e], start, end, pad_char)
     return out
@@ -874,10 +989,10 @@
             raise ImportError(
                 "Could not import PyTorch. Please install PyTorch to use torch features."
             )
 
     def __len__(self) -> int:
         return len(self.dataset)
 
-    def __getitem__(self, idx: Idx) -> Union[NDArray, Tuple[NDArray, NDArray]]:
+    def __getitem__(self, idx: Idx) -> Union[NDArray, Tuple[NDArray, ...]]:
         batch = self.dataset[idx]
         return batch
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/dataset/reference.py` & `genvarloader-0.3.1/python/genvarloader/dataset/reference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Dict,
     List,
-    Sequence,
     Union,
     cast,
 )
 
 import numpy as np
 from attrs import define
 from numpy.typing import NDArray
 
 from ..fasta import Fasta
 from ..utils import normalize_contig_name
 
-Idx = Union[int, np.integer, Sequence[int], NDArray[np.integer], slice]
-ListIdx = Union[Sequence[int], NDArray[np.integer]]
-
 
 @define
 class Reference:
     reference: NDArray[np.uint8]
     contigs: List[str]
     offsets: NDArray[np.uint64]
     pad_char: int
 
     @classmethod
     def from_path_and_contigs(cls, fasta: Union[str, Path], contigs: List[str]):
         _fasta = Fasta("ref", fasta, "N")
+
+        if not _fasta.cache_path.exists():
+            _fasta._write_to_cache()
+
         contigs = cast(
             List[str],
             [normalize_contig_name(c, _fasta.contigs) for c in contigs],
         )
-        _fasta.sequences = _fasta._get_contigs(contigs)
+        _fasta.sequences = _fasta._get_sequences(contigs)
         if TYPE_CHECKING:
             assert _fasta.sequences is not None
             assert _fasta.pad is not None
         refs: List[NDArray[np.bytes_]] = []
         next_offset = 0
         _ref_offsets: Dict[str, int] = {}
         for contig in contigs:
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/dataset/utils.py` & `genvarloader-0.3.1/python/genvarloader/dataset/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,71 +3,94 @@
 import numba as nb
 import numpy as np
 import polars as pl
 from numpy.typing import ArrayLike, NDArray
 
 
 @nb.njit(nogil=True, cache=True)
-def padded_slice(arr: NDArray, start: int, stop: int, pad_char: int):
+def padded_slice(arr: NDArray, start: int, stop: int, pad_val: int):
     pad_left = -min(0, start)
     pad_right = max(0, stop - len(arr))
 
     if pad_left == 0 and pad_right == 0:
         out = arr[start:stop]
         return out
 
     out = np.empty(stop - start, arr.dtype)
 
     if pad_left > 0 and pad_right > 0:
         out_stop = len(out) - pad_right
-        out[:pad_left] = pad_char
+        out[:pad_left] = pad_val
         out[pad_left:out_stop] = arr[:]
-        out[out_stop:] = pad_char
+        out[out_stop:] = pad_val
     elif pad_left > 0:
-        out[:pad_left] = pad_char
+        out[:pad_left] = pad_val
         out[pad_left:] = arr[:stop]
     elif pad_right > 0:
         out_stop = len(out) - pad_right
         out[:out_stop] = arr[start:]
-        out[out_stop:] = pad_char
+        out[out_stop:] = pad_val
 
     return out
 
 
-def subset_to_full_raveled_mapping(
-    full_shape: Tuple[int, int], ax1_indices: ArrayLike, ax2_indices: ArrayLike
+def oidx_to_raveled_idx(
+    row_idx: ArrayLike, col_idx: ArrayLike, full_shape: Tuple[int, int]
 ):
-    # Generate a grid of indices for the subset array
-    row_indices, col_indices = np.meshgrid(ax1_indices, ax2_indices, indexing="ij")
-
-    # Flatten the grid to get all combinations of row and column indices in the subset
-    row_indices_flat = row_indices.ravel()
-    col_indices_flat = col_indices.ravel()
-
-    # Convert these subset indices to linear indices in the context of the full array
-    # This leverages the fact that the linear index in a 2D array is given by: index = row * num_columns + column
-    full_array_linear_indices = row_indices_flat * full_shape[1] + col_indices_flat
-
+    full_array_linear_indices = np.ravel_multi_index(
+        np.ix_(row_idx, col_idx),  # type: ignore
+        full_shape,
+    ).ravel()
     return full_array_linear_indices
 
 
-def regions_to_bed(regions: NDArray, contigs: Sequence[str]) -> pl.DataFrame:
+def regions_to_bed(regions: NDArray[np.int32], contigs: Sequence[str]) -> pl.DataFrame:
     """Convert regions to a BED3 DataFrame.
 
     Parameters
     ----------
     regions : NDArray
         Shape = (n_regions, 3) Regions.
     contigs : Sequence[str]
         Contigs.
 
     Returns
     -------
     pl.DataFrame
         Bed DataFrame.
     """
-    bed = pl.DataFrame(
-        regions, schema=["chrom", "chromStart", "chromEnd"]
-    ).with_columns(pl.all().cast(pl.Int64))
+    cols = ["chrom", "chromStart", "chromEnd", "strand"]
+    bed = pl.DataFrame(regions, schema=cols)
     cmap = dict(enumerate(contigs))
-    bed = bed.with_columns(pl.col("chrom").replace(cmap, return_dtype=pl.Utf8))
+    bed = bed.with_columns(
+        pl.col("chrom").replace(cmap, return_dtype=pl.Utf8),
+        pl.col("strand").replace({1: "+", -1: "-"}, return_dtype=pl.Utf8),
+        pl.col("chromStart", "chromEnd").cast(pl.Int64),
+    ).select(*cols)
     return bed
+
+
+@nb.njit(nogil=True, cache=True)
+def splits_sum_le_value(arr: NDArray[np.number], max_value: float) -> NDArray[np.intp]:
+    """Split an array into contiguous sections where the sum is less than or equal to a value.
+
+    Parameters
+    ----------
+    arr : NDArray[np.number]
+        Array to split.
+    max_value : float
+        Maximum value.
+
+    Returns
+    -------
+    NDArray[np.int32]
+        Split indices.
+    """
+    indices = [0]
+    current_sum = 0
+    for idx, value in enumerate(arr):
+        current_sum += value
+        if current_sum > max_value:
+            indices.append(idx)
+            current_sum = value
+    indices.append(len(arr))
+    return np.array(indices, np.intp)
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/dataset/write.py` & `genvarloader-0.3.1/python/genvarloader/dataset/write.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,132 @@
+import gc
 import json
 import re
 import shutil
 from pathlib import Path
-from typing import List, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import polars as pl
-from einops import rearrange
 from loguru import logger
+from natsort import natsorted
 from tqdm.auto import tqdm
-from typing_extensions import assert_never
 
 from ..bigwig import BigWigs
 from ..utils import normalize_contig_name, read_bedlike, with_length
 from ..variants import Variants
-from ..variants.records import RecordInfo
+from ..variants.genotypes import VCFGenos
+from .genotypes import SparseGenotypes
 
 
 def write(
     path: Union[str, Path],
     bed: Union[str, Path, pl.DataFrame],
     vcf: Optional[Union[str, Path]] = None,
-    bigwigs: Optional[BigWigs] = None,
+    bigwigs: Optional[Union[BigWigs, List[BigWigs]]] = None,
     samples: Optional[List[str]] = None,
     length: Optional[int] = None,
     max_jitter: Optional[int] = None,
+    overwrite: bool = False,
 ):
     if vcf is None and bigwigs is None:
         raise ValueError("At least one of `vcf` or `bigwigs` must be provided.")
 
+    if isinstance(bigwigs, BigWigs):
+        bigwigs = [bigwigs]
+
     logger.info(f"Writing to {path}")
 
     metadata = {}
     path = Path(path)
-    if path.exists():
+    if path.exists() and overwrite:
         logger.info("Found existing GVL store, overwriting.")
         shutil.rmtree(path)
+    elif path.exists() and not overwrite:
+        raise FileExistsError(f"{path} already exists.")
     path.mkdir(parents=True, exist_ok=True)
 
     bed, contigs, region_length = prep_bed(bed, length, max_jitter)
     metadata["region_length"] = region_length
     metadata["contigs"] = contigs
     if max_jitter is not None:
         metadata["max_jitter"] = max_jitter
 
-    available_samples = None
+    all_samples: List[str] = []
     if vcf is not None:
         vcf = Path(vcf)
         variants = Variants.from_vcf(vcf, use_cache=False)
 
         if unavailable_contigs := set(contigs) - {
             normalize_contig_name(c, contigs) for c in variants.records.contigs
         }:
             logger.warning(
                 f"Contigs in queries {unavailable_contigs} are not found in the VCF."
             )
 
-        if available_samples is None:
-            available_samples = set(variants.samples)
-        else:
-            available_samples &= set(variants.samples)
+        all_samples.extend(variants.samples)
+    else:
+        variants = None
 
     if bigwigs is not None:
-        if unavailable_contigs := set(contigs) - set(
-            normalize_contig_name(c, contigs) for c in bigwigs.contigs
-        ):
+        unavail = []
+        for bw in bigwigs:
+            if unavailable_contigs := set(contigs) - set(
+                normalize_contig_name(c, contigs) for c in bw.contigs
+            ):
+                unavail.append(unavailable_contigs)
+            all_samples.extend(bw.samples)
+        if unavail:
             logger.warning(
-                f"Contigs in queries {unavailable_contigs} are not found in the BigWigs."
+                f"Contigs in queries {set(unavail)} are not found in the BigWigs."
             )
 
-        if available_samples is None:
-            available_samples = set(bigwigs.samples)
-        else:
-            available_samples &= set(bigwigs.samples)
-
-    if available_samples is None:
-        # this should be unreachable since we check that at least one of vcf or bigwigs is provided
-        assert_never(available_samples)  # type: ignore
+    available_samples = set(all_samples)
 
     if samples is not None:
         _samples = set(samples)
         if missing := (_samples - available_samples):
             raise ValueError(f"Samples {missing} not found in VCF or BigWigs.")
         samples = list(_samples)
     else:
         samples = list(available_samples)
 
-    logger.info(f"Using {len(samples)} samples: {samples}")
+    samples.sort()
+
+    logger.info(f"Using {len(samples)} samples.")
+    metadata["samples"] = samples
+    metadata["n_samples"] = len(samples)
+    metadata["n_regions"] = bed.height
 
     if vcf is not None:
+        if TYPE_CHECKING:
+            assert variants is not None
+
         logger.info("Writing genotypes.")
-        bed, ploidy, n_variants, samples = write_variants(
+        bed = write_variants(
             path,
             bed,
             vcf,
-            variants,  # type: ignore
+            variants,
+            region_length,
             samples,
         )
-        metadata["ploidy"] = ploidy
-        metadata["n_variants"] = n_variants
+        if isinstance(variants.genotypes, VCFGenos):
+            variants.genotypes.close()
+        metadata["ploidy"] = variants.ploidy
+        # free memory
+        del variants
+        gc.collect()
 
     write_regions(path, bed, contigs)
 
     if bigwigs is not None:
         logger.info("Writing BigWig intervals.")
-        n_intervals = write_bigwigs(path, bed, bigwigs, samples)
-        metadata["n_intervals"] = n_intervals
+        for bw in bigwigs:
+            write_bigwigs(path, bed, bw, samples)
 
     with open(path / "metadata.json", "w") as f:
         json.dump(metadata, f)
 
     logger.info("Finished writing.")
 
 
@@ -117,28 +134,38 @@
     bed: Union[str, Path, pl.DataFrame],
     length: Optional[int] = None,
     max_jitter: Optional[int] = None,
 ) -> Tuple[pl.DataFrame, List[str], int]:
     if isinstance(bed, (str, Path)):
         bed = read_bedlike(bed)
 
-    bed = bed.select("chrom", "chromStart", "chromEnd").sort(
-        "chrom", "chromStart", "chromEnd"
-    )
+    if bed.height == 0:
+        raise ValueError("No regions found in the BED file.")
+
+    contigs = natsorted(bed["chrom"].unique().to_list())
+    if "strand" not in bed:
+        bed = bed.with_columns(strand=pl.lit(1, pl.Int32))
+    else:
+        bed = bed.with_columns(
+            pl.col("strand").replace({"+": 1, "-": -1}, return_dtype=pl.Int32)
+        )
+    bed = bed.select("chrom", "chromStart", "chromEnd", "strand")
+    with pl.StringCache():
+        pl.Series(contigs, dtype=pl.Categorical)
+        bed = bed.sort(pl.col("chrom").cast(pl.Categorical), pl.col("chromStart"))
 
     if length is None:
         length = cast(
             int, bed.select((pl.col("chromEnd") - pl.col("chromStart")).max()).item()
         )
 
     if max_jitter is not None:
         length += 2 * max_jitter
 
     bed = with_length(bed, length)
-    contigs = bed["chrom"].unique(maintain_order=True).to_list()
 
     return bed, contigs, length
 
 
 def write_regions(path: Path, bed: pl.DataFrame, contigs: List[str]):
     with pl.StringCache():
         pl.Series(contigs, dtype=pl.Categorical)
@@ -150,203 +177,204 @@
 
 
 def write_variants(
     path: Path,
     bed: pl.DataFrame,
     vcf: Path,
     variants: Variants,
+    region_length: int,
     samples: Optional[List[str]] = None,
-) -> Tuple[pl.DataFrame, int, int, List[str]]:
+):
     if samples is None:
         len(variants.samples)
         sample_idx = None
         _samples = cast(List[str], variants.samples.tolist())
     else:
         _, key_idx, query_idx = np.intersect1d(
             variants.samples, samples, return_indices=True
         )
         if missing := (set(samples) - set(variants.samples)):
             raise ValueError(f"Samples {missing} not found in VCF.")
         sample_idx = key_idx[query_idx]
         len(sample_idx)
         _samples = samples
-    np.save(path / "samples.npy", _samples)
 
     gvl_arrow = re.sub(r"\.[bv]cf(\.gz)?$", ".gvl.arrow", vcf.name)
     recs = pl.read_ipc(vcf.parent / gvl_arrow)
-    recs.select("POS", "ALT", "ILEN").write_ipc(path / "variants.arrow")
 
-    (path / "genotypes").mkdir(parents=True, exist_ok=True)
+    out_dir = path / "genotypes"
+    out_dir.mkdir(parents=True, exist_ok=True)
+
+    recs.select("POS", "ALT", "ILEN").write_ipc(out_dir / "variants.arrow")
 
-    memmap_offsets = {
-        "genotypes": 0,
-        "fv_idxs": 0,
-        "offsets": 0,
-    }
+    v_idx_memmap_offsets = 0
+    offset_memmap_offsets = 0
     last_offset = 0
-    n_variants = 0
-    pbar = tqdm(total=bed["chrom"].n_unique())
-    all_max_ends = []
-    for contig, part in bed.partition_by(
-        "chrom", as_dict=True, include_key=False, maintain_order=True
-    ).items():
-        pbar.set_description(f"Writing genotypes for {contig}")
-        starts = part["chromStart"].to_numpy()
-        ends = part["chromEnd"].to_numpy()
-        n_regions = part.height
+    max_ends = np.empty(bed.height, dtype=np.int32)
+    last_max_end_idx = 0
+    with tqdm(total=bed["chrom"].n_unique()) as pbar:
+        for contig, part in bed.partition_by(
+            "chrom", as_dict=True, include_key=False, maintain_order=True
+        ).items():
+            pbar.set_description(
+                f"Reading genotypes for {part.height} regions on {contig}"
+            )
+            starts = part["chromStart"].to_numpy()
+            ends = part["chromEnd"].to_numpy()
+            n_regions = part.height
+
+            _contig = normalize_contig_name(contig, variants.records.contigs)
+            if _contig is None:
+                genos = SparseGenotypes.empty(n_regions, len(_samples), variants.ploidy)
+            else:
+                multiplier = 2
+                while True:
+                    records = variants.records.vars_in_range(_contig, starts, ends)
+                    # (s p v)
+                    genos = variants.genotypes.read(
+                        _contig,
+                        records.start_idxs,
+                        records.end_idxs,
+                        sample_idx=sample_idx,
+                    )
+                    # (s p v)
+                    ilens = np.where(genos == 1, records.size_diffs, 0)
+                    # (s p r)
+                    ilens = np.add.reduceat(ilens, records.offsets[:-1], axis=-1)
+                    # (s p r)
+                    effective_length = (ends - starts) + ilens
+                    # (s p r)
+                    missing_length = region_length - effective_length
+                    if np.all(missing_length <= 0):
+                        break
+                    # (r)
+                    ends += multiplier * missing_length.max((0, 1))
+
+                pbar.set_description(
+                    f"Sparsifying genotypes for {part.height} regions on {contig}"
+                )
+                genos, c_max_ends = SparseGenotypes.from_dense_with_length(
+                    genos=genos,
+                    # make indices relative to the contig
+                    first_v_idxs=records.start_idxs
+                    - variants.records.contig_offsets[_contig],
+                    offsets=records.offsets.astype(np.int32),
+                    ilens=variants.records.v_diffs[_contig],
+                    positions=variants.records.v_starts[_contig],
+                    starts=starts,
+                    length=region_length,
+                )
+                # make indices absolute
+                genos.variant_idxs += variants.records.contig_offsets[_contig]
+                max_ends[last_max_end_idx : last_max_end_idx + n_regions] = c_max_ends
+                last_max_end_idx += n_regions
 
-        _contig = normalize_contig_name(contig, variants.records.contigs)
-        if _contig is None:
-            records = RecordInfo.empty(n_regions)
-            max_ends = ends.astype(np.int32)
-            genos = np.empty((0, variants.ploidy), np.int8)
-        else:
-            (
-                records,
-                max_ends,
-            ) = variants.records.vars_in_range_for_haplotype_construction(
-                _contig, starts, ends
+            pbar.set_description(
+                f"Writing genotypes for {part.height} regions on {contig}"
             )
-            genos = variants.genotypes.read(
-                _contig, records.start_idxs, records.end_idxs, sample_idx=sample_idx
+            out = np.memmap(
+                out_dir / "variant_idxs.npy",
+                dtype=genos.variant_idxs.dtype,
+                mode="w+" if v_idx_memmap_offsets == 0 else "r+",
+                shape=genos.variant_idxs.shape,
+                offset=v_idx_memmap_offsets,
             )
-            genos = rearrange(genos, "s p v -> (s v) p")
-
-        all_max_ends.append(max_ends)
-        n_variants += len(records.positions)
-
-        out = np.memmap(
-            path / "genotypes" / "genotypes.npy",
-            dtype=genos.dtype,
-            mode="w+" if memmap_offsets["genotypes"] == 0 else "r+",
-            shape=genos.shape,
-            offset=memmap_offsets["genotypes"],
-        )
-        out[:] = genos[:]
-        out.flush()
-        memmap_offsets["genotypes"] += out.nbytes
-
-        out = np.memmap(
-            path / "genotypes" / "first_variant_idxs.npy",
-            dtype=records.start_idxs.dtype,
-            mode="w+" if memmap_offsets["fv_idxs"] == 0 else "r+",
-            shape=records.start_idxs.shape,
-            offset=memmap_offsets["fv_idxs"],
-        )
-        out[:] = records.start_idxs[:]
-        out.flush()
-        memmap_offsets["fv_idxs"] += out.nbytes
-
-        offsets = records.offsets.copy()
-        offsets += last_offset
-        last_offset = offsets[-1]
-        out = np.memmap(
-            path / "genotypes" / "offsets.npy",
-            dtype=offsets.dtype,
-            mode="w+" if memmap_offsets["offsets"] == 0 else "r+",
-            shape=len(offsets) - 1,
-            offset=memmap_offsets["offsets"],
-        )
-        out[:] = offsets[:-1]
-        out.flush()
-        memmap_offsets["offsets"] += out.nbytes
-        pbar.update()
-    pbar.close()
+            out[:] = genos.variant_idxs[:]
+            out.flush()
+            v_idx_memmap_offsets += out.nbytes
+
+            offsets = genos.offsets
+            offsets += last_offset
+            last_offset = offsets[-1]
+            out = np.memmap(
+                out_dir / "offsets.npy",
+                dtype=offsets.dtype,
+                mode="w+" if offset_memmap_offsets == 0 else "r+",
+                shape=len(offsets) - 1,
+                offset=offset_memmap_offsets,
+            )
+            out[:] = offsets[:-1]
+            out.flush()
+            offset_memmap_offsets += out.nbytes
+            pbar.update()
 
     out = np.memmap(
-        path / "genotypes" / "offsets.npy",
+        out_dir / "offsets.npy",
         dtype=offsets.dtype,  # type: ignore
         mode="r+",
         shape=1,
-        offset=memmap_offsets["offsets"],
+        offset=offset_memmap_offsets,
     )
     out[-1] = offsets[-1]  # type: ignore
     out.flush()
 
-    max_ends = np.concatenate(all_max_ends)
     bed = bed.with_columns(chromEnd=pl.lit(max_ends))
-
-    return bed, variants.ploidy, int(n_variants), _samples
+    return bed
 
 
 def write_bigwigs(
     path: Path, bed: pl.DataFrame, bigwigs: BigWigs, samples: Optional[List[str]]
 ) -> int:
     if samples is None:
         _samples = cast(List[str], bigwigs.samples)
     else:
         if missing := (set(samples) - set(bigwigs.samples)):
             raise ValueError(f"Samples {missing} not found in bigwigs.")
         _samples = samples
-    np.save(path / "samples.npy", _samples)
 
-    (path / "intervals").mkdir(parents=True, exist_ok=True)
+    out_dir = path / "intervals" / bigwigs.name
+    out_dir.mkdir(parents=True, exist_ok=True)
 
-    memmap_offsets = {
-        "intervals": 0,
-        "values": 0,
-        "offsets": 0,
-    }
+    interval_offset = 0
+    offset_offset = 0
     last_offset = 0
     n_intervals = 0
     pbar = tqdm(total=bed["chrom"].n_unique())
     for contig, part in bed.partition_by(
         "chrom", as_dict=True, include_key=False, maintain_order=True
     ).items():
-        pbar.set_description(f"Writing intervals for {contig}")
+        pbar.set_description(f"Reading intervals for {part.height} regions on {contig}")
         starts = part["chromStart"].to_numpy()
         ends = part["chromEnd"].to_numpy()
 
         intervals = bigwigs.intervals(contig, starts, ends, sample=_samples)
-        n_intervals += len(intervals.intervals)
 
+        pbar.set_description(f"Writing intervals for {part.height} regions on {contig}")
+        n_intervals += len(intervals.data)
         out = np.memmap(
-            path / "intervals" / "intervals.npy",
-            dtype=intervals.intervals.dtype,
-            mode="w+" if memmap_offsets["intervals"] == 0 else "r+",
-            shape=intervals.intervals.shape,
-            offset=memmap_offsets["intervals"],
+            out_dir / "intervals.npy",
+            dtype=intervals.data.dtype,
+            mode="w+" if interval_offset == 0 else "r+",
+            shape=intervals.data.shape,
+            offset=interval_offset,
         )
-        out[:] = intervals.intervals[:]
+        out[:] = intervals.data[:]
         out.flush()
-        memmap_offsets["intervals"] += intervals.intervals.nbytes
+        interval_offset += out.nbytes
 
-        out = np.memmap(
-            path / "intervals" / "values.npy",
-            dtype=intervals.values.dtype,
-            mode="w+" if memmap_offsets["values"] == 0 else "r+",
-            shape=intervals.values.shape,
-            offset=memmap_offsets["values"],
-        )
-        out[:] = intervals.values[:]
-        out.flush()
-        memmap_offsets["values"] += intervals.values.nbytes
-
-        offsets = np.empty(len(intervals.n_per_query) + 1, dtype=np.uint32)
-        offsets[0] = 0
-        intervals.n_per_query.cumsum(out=offsets[1:])
+        offsets = intervals.offsets
         offsets += last_offset
         last_offset = offsets[-1]
         out = np.memmap(
-            path / "intervals" / "offsets.npy",
+            out_dir / "offsets.npy",
             dtype=offsets.dtype,
-            mode="w+" if memmap_offsets["offsets"] == 0 else "r+",
+            mode="w+" if offset_offset == 0 else "r+",
             shape=len(offsets) - 1,
-            offset=memmap_offsets["offsets"],
+            offset=offset_offset,
         )
         out[:] = offsets[:-1]
         out.flush()
-        memmap_offsets["offsets"] += offsets[:-1].nbytes
+        offset_offset += out.nbytes
         pbar.update()
     pbar.close()
 
     out = np.memmap(
-        path / "intervals" / "offsets.npy",
-        dtype=np.uint32,
+        out_dir / "offsets.npy",
+        dtype=offsets.dtype,  # type: ignore
         mode="r+",
         shape=1,
-        offset=memmap_offsets["offsets"],
+        offset=offset_offset,
     )
-    out[-1] = n_intervals
+    out[-1] = offsets[-1]  # type: ignore
     out.flush()
 
     return n_intervals
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/fasta.py` & `genvarloader-0.3.1/python/genvarloader/fasta.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from functools import partial
 from pathlib import Path
 from typing import Dict, Iterable, Optional, Union, cast
 
 import numpy as np
 import pysam
 import seqpro as sp
@@ -24,37 +25,45 @@
 
     def __init__(
         self,
         name: str,
         path: Union[str, Path],
         pad: Optional[str] = None,
         alphabet: Optional[Union[str, sp.NucleotideAlphabet, sp.AminoAlphabet]] = None,
-        in_memory=False,
+        in_memory: bool = False,
+        cache: bool = False,
     ) -> None:
         """Read sequences from a FASTA file.
 
         Parameters
         ----------
         name : str
             Name of the reader, for example `'seq'`.
         path : Union[str, Path]
             Path to the FASTA file.
         pad : Optional[str], optional
             A single character which, if passed, will pad out-of-bound ranges with this
             value. By default no padding is done and out-of-bound ranges raise an error.
         alphabet : str, sp.NucleotideAlphabet, sp.AminoAlphabet, optional
             Alphabet to use for the sequences. If not passed, defaults to DNA.
+        in_memory : bool, optional
+            Whether to load the sequences into memory. If `True`, the sequences will be
+            loaded into memory and the FASTA file will be closed. If `False`, the sequences
+            will be read from the FASTA file on demand. Defaults to `False`.
+        cache : bool, optional
+            Whether to cache the sequences to disk. If `True`, the sequences will be written
+            to disk in a `.fa.gvl` file. Defaults to `False`. Only used if `in_memory` is `True`.
 
         Raises
         ------
         ValueError
             If pad value is not a single character.
         """
         self.name = name
-        self.path = path
+        self.path = Path(path)
         if pad is None:
             self.pad = pad
         else:
             if len(pad) > 1:
                 raise ValueError("Pad value must be a single character.")
             self.pad = pad.encode("ascii")
 
@@ -89,31 +98,64 @@
             self.rev_strand_fn = rev_strand_fn  # type: ignore[assignment]
         else:
             assert_never(self.alphabet)
 
         self.contigs = self._get_contig_lengths()
 
         self.handle: Optional[pysam.FastaFile] = None
+        fa_extension = re.compile(r"\.(fa|fna|fasta)(\.gz)?$")
+        self.cache_path = Path(fa_extension.sub(".fa.gvl", str(self.path)))
 
         if not in_memory:
             self.sequences = None
         else:
-            self.sequences = self._get_contigs(self.contigs)
+            if cache:
+                if not self.cache_path.exists():
+                    self._write_to_cache()
+                self.sequences = self._get_sequences(self.contigs)
+            else:
+                self.sequences = self._get_sequences(self.contigs)
 
     def _get_contig_lengths(self) -> Dict[str, int]:
         with self._open() as f:
             return {c: f.get_reference_length(c) for c in f.references}
 
-    def _get_contigs(self, contigs: Iterable[str]) -> Dict[str, NDArray[np.bytes_]]:
+    def _get_sequences(
+        self, contigs: Iterable[str], from_fasta=False
+    ) -> Dict[str, NDArray[np.bytes_]]:
         """Load contigs into memory."""
-        with self._open() as f:
-            return {
-                c: np.frombuffer(f.fetch(c).encode("ascii").upper(), "S1")
-                for c in contigs
-            }
+        if from_fasta:
+            with self._open() as f:
+                sequences = {
+                    c: np.frombuffer(f.fetch(c).encode("ascii").upper(), "S1")
+                    for c in contigs
+                }
+        elif self.cache_path.exists():
+            sequences: Dict[str, NDArray[np.bytes_]] = {}
+            for contig in contigs:
+                sequences[contig] = np.load(self.cache_path / f"{contig}.npy")
+        else:
+            with self._open() as f:
+                sequences = {
+                    c: np.frombuffer(f.fetch(c).encode("ascii").upper(), "S1")
+                    for c in contigs
+                }
+        return sequences
+
+    def _write_to_cache(self):
+        """Write contigs to cache."""
+        self.cache_path.mkdir(parents=True, exist_ok=True)
+
+        if self.sequences is None:
+            sequences = self._get_sequences(self.contigs, from_fasta=True)
+        else:
+            sequences = self.sequences
+
+        for contig, seq in sequences.items():
+            np.save(self.cache_path / f"{contig}.npy", seq)
 
     def _open(self):
         return pysam.FastaFile(str(self.path))
 
     def close(self):
         if self.handle is not None:
             self.handle.close()
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/haplotypes.py` & `genvarloader-0.3.1/python/genvarloader/haplotypes.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/intervals.py` & `genvarloader-0.3.1/python/genvarloader/intervals.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/loader.py` & `genvarloader-0.3.1/python/genvarloader/loader.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/torch.py` & `genvarloader-0.3.1/python/genvarloader/torch.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/utils.py` & `genvarloader-0.3.1/python/genvarloader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,7 +417,30 @@
         Normalized contig name.
     """
     for c in contigs:
         # exact match, remove chr, add chr
         if contig == c or contig[3:] == c or f"chr{contig}" == c:
             return c
     return None
+
+
+ITYPE = TypeVar("ITYPE", bound=np.integer)
+
+
+def offsets_to_lengths(offsets: NDArray[ITYPE]) -> NDArray[ITYPE]:
+    """Converts offsets to the number of elements in each group.
+
+    Notes
+    -----
+    This function will silently fail with wraparound values if the offsets are
+    not sorted in ascending order."""
+    return np.diff(offsets)
+
+
+def lengths_to_offsets(
+    lengths: NDArray[np.integer], dtype: type[ITYPE] = np.int32
+) -> NDArray[ITYPE]:
+    """Converts the number of elements in each group to offsets."""
+    offsets = np.empty(len(lengths) + 1, dtype=dtype)
+    offsets[0] = 0
+    np.cumsum(lengths, out=offsets[1:])
+    return offsets
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/variants/__init__.py` & `genvarloader-0.3.1/python/genvarloader/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.0rc9/genvarloader/variants/genotypes.py` & `genvarloader-0.3.1/python/genvarloader/variants/genotypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
 
 class Genotypes(Protocol):
     chunked: bool
     samples: NDArray[np.str_]
     ploidy: int
 
+    @property
+    def n_samples(self) -> int:
+        return len(self.samples)
+
     def read(
         self,
         contig: str,
         start_idxs: ArrayLike,
         end_idxs: ArrayLike,
         sample_idx: Optional[ArrayLike] = None,
         haplotype_idx: Optional[ArrayLike] = None,
@@ -65,17 +69,23 @@
         Returns
         -------
         genotypes : NDArray[np.int8]
             Shape: (samples ploidy variants). Genotypes for each query region.
         """
         ...
 
-    @property
-    def n_samples(self) -> int:
-        return len(self.samples)
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: ArrayLike,
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ): ...
 
 
 class FromRecsGenos(Protocol):
     @classmethod
     def from_recs_genos(
         cls,
         records: Records,
@@ -183,14 +193,25 @@
         genotypes = genotypes[_sample_idx, _haplotype_idx]
         # re-order samples to be in query order
         # if sample_sorter is not None and (np.arange(n_samples) != sample_sorter).any():
         #     genotypes = genotypes[sample_sorter]
 
         return genotypes
 
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: ArrayLike,
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ):
+        raise NotImplementedError
+
     def __del__(self) -> None:
         if self.handle is not None:
             self.handle.close()
 
 
 """
 Implementation note regarding using tensorstore with num_workers > 0
@@ -421,14 +442,25 @@
             ts.d[0].translate_to[0]  # pyright: ignore[reportPossiblyUnboundVariable,reportAttributeAccessIssue]
         ]
 
         genotypes = cast(NDArray[np.int8], genotypes.read().result())
 
         return genotypes
 
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: ArrayLike,
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ):
+        raise NotImplementedError
+
 
 class NumpyGenos(Genotypes, FromRecsGenos):
     chunked = False
 
     def __init__(
         self,
         arrays: Dict[str, NDArray[np.int8]],
@@ -476,14 +508,25 @@
         for s, e, r_s, r_e in zip(start_idxs, end_idxs, rel_starts, rel_ends):
             if s == e:
                 continue
             genos[..., r_s:r_e] = self.arrays[contig][_sample_idx, _haplotype_idx, s:e]
 
         return genos
 
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: ArrayLike,
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ):
+        raise NotImplementedError
+
     def __getitem__(
         self,
         contigs: ArrayLike,
         start_idxs: ArrayLike,
         end_idxs: ArrayLike,
         sample_idxs: ArrayLike,
         haplotype_idxs: ArrayLike,
@@ -554,14 +597,25 @@
             # (s p v)
             genos_ls.append(
                 self.memmaps[contig][_sample_idx, _haplotype_idx, s_idx:e_idx]
             )
         genos = np.concatenate(genos_ls, axis=-1)
         return genos
 
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: ArrayLike,
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ):
+        raise NotImplementedError
+
     @classmethod
     def from_recs_genos(
         cls,
         records: Records,
         genotypes: Genotypes,
         paths: Optional[Dict[str, Path]] = None,
         mem=int(1e9),
@@ -612,51 +666,60 @@
 
         self.paths = vcfs
         samples = None
         for p in self.paths.values():
             if not p.exists():
                 raise FileNotFoundError(f"VCF file {p} not found.")
             if samples is None:
-                samples = np.array(cyvcf2.VCF(str(p)).samples)  # pyright: ignore
+                f = cyvcf2.VCF(str(p))  # type: ignore
+                samples = np.array(f.samples)
+                f.close()
+                del f
         self.samples = samples  # type: ignore
-        self.handles: Optional[Dict[str, cyvcf2.VCF]] = None  # pyright: ignore
+        self.handles: Optional[Dict[str, "cyvcf2.VCF"]] = None
         self.contig_offsets = contig_offsets
 
+    def close(self):
+        if self.handles is not None:
+            for handle in self.handles.values():
+                handle.close()
+
     def read(
         self,
         contig: str,
         start_idxs: ArrayLike,
         end_idxs: ArrayLike,
         sample_idx: Optional[ArrayLike] = None,
         haplotype_idx: Optional[ArrayLike] = None,
     ) -> NDArray[np.int8]:
         start_idxs = np.atleast_1d(np.asarray(start_idxs, dtype=int))
         end_idxs = np.atleast_1d(np.asarray(end_idxs, dtype=int))
 
         if self.handles is None and "_all" not in self.paths:
             self.handles = {
-                c: cyvcf2.VCF(str(p), lazy=True)  # pyright: ignore
+                c: cyvcf2.VCF(str(p), lazy=True)  # type: ignore
                 for c, p in self.paths.items()
             }
         elif self.handles is None:
-            handle = cyvcf2.VCF(str(next(iter(self.paths.values()))), lazy=True)  # pyright: ignore
+            first_path = next(iter(self.paths.values()))
+            handle = cyvcf2.VCF(str(first_path), lazy=True)  # type: ignore
             self.handles = {c: handle for c in handle.seqnames}
 
         if sample_idx is None:
             _sample_idx = slice(None)
         else:
             _sample_idx = np.atleast_1d(np.asarray(sample_idx, dtype=int))
 
         if haplotype_idx is None:
             _haplotype_idx = slice(None)
         else:
             _haplotype_idx = np.atleast_1d(np.asarray(haplotype_idx, dtype=int))
 
-        # (s p v)
         n_variants = (end_idxs - start_idxs).sum()
+        # (s p v)
         genos = np.empty(
             (len(self.samples), self.ploidy, n_variants),
             dtype=np.int8,
         )
 
         if genos.size == 0:
             return genos
@@ -669,23 +732,89 @@
         offset = self.contig_offsets[contig]
         for i, v in enumerate(self.handles[contig](contig), start=offset):
             # (n_queries)
             overlapping_query_intervals = (i >= start_idxs) & (i < end_idxs)
             if overlapping_query_intervals.any():
                 # (n_valid)
                 place_idx = geno_idxs[overlapping_query_intervals]
+                genos[..., place_idx] = v.genotype.array()[:, :2, None]
                 # increment idxs for next iteration
                 geno_idxs[overlapping_query_intervals] += 1
-                genos[..., place_idx] = v.genotype.array()[:, :2, None]
             if (geno_idxs == finish_idxs).all():
                 break
 
         genos = genos[_sample_idx, _haplotype_idx]
         # cyvcf2 encoding: 0, 1, -1 => gvl/pgen encoding: 0, 1, -9
         genos[genos == -1] = -9
 
         return genos
 
+    def read_for_length(
+        self,
+        contig: str,
+        start_idxs: Optional[ArrayLike],
+        init_end_idxs: Optional[ArrayLike],
+        length: int,
+        ilens: NDArray[np.int32],
+        sample_idx: Optional[ArrayLike] = None,
+        haplotype_idx: Optional[ArrayLike] = None,
+    ):
+        raise NotImplementedError
+        start_idxs = np.atleast_1d(np.asarray(start_idxs, dtype=np.int32))
+        init_end_idxs = np.atleast_1d(np.asarray(init_end_idxs, dtype=np.int32))
+
+        if self.handles is None:
+            self.handles = self.init_handles()
+
+        if sample_idx is None:
+            _sample_idx = slice(None)
+        else:
+            _sample_idx = np.atleast_1d(np.asarray(sample_idx, dtype=int))
+
+        if haplotype_idx is None:
+            _haplotype_idx = slice(None)
+        else:
+            _haplotype_idx = np.atleast_1d(np.asarray(haplotype_idx, dtype=int))
+
+        n_variants = (init_end_idxs - start_idxs).sum()
+        genos = np.empty(
+            (len(self.samples), self.ploidy, n_variants),
+            dtype=np.int8,
+        )
+
+        if genos.size == 0:
+            return genos
+
+        geno_idxs = get_rel_starts(start_idxs, init_end_idxs)
+        finish_idxs = np.empty_like(geno_idxs)
+        finish_idxs[:-1] = geno_idxs[1:]
+        finish_idxs[-1] = n_variants
+        offset = self.contig_offsets[contig]
+        for i, v in enumerate(self.handles[contig](contig), start=offset):
+            # (n_queries)
+            overlapping_query_intervals = (i >= start_idxs) & (i < init_end_idxs)
+            if overlapping_query_intervals.any():
+                # (n_valid)
+                place_idx = geno_idxs[overlapping_query_intervals]
+                # increment idxs for next iteration
+                geno_idxs[overlapping_query_intervals] += 1
+                genos[..., place_idx] = v.genotype.array()[:, :2, None]
+            if (geno_idxs == finish_idxs).all():
+                break
+
+    def init_handles(self) -> Dict[str, "cyvcf2.VCF"]:
+        if self.handles is None and "_all" not in self.paths:
+            handles = {
+                c: cyvcf2.VCF(str(p), lazy=True)  # pyright: ignore
+                for c, p in self.paths.items()
+            }
+        elif self.handles is None:
+            handle = cyvcf2.VCF(str(next(iter(self.paths.values()))), lazy=True)  # pyright: ignore
+            handles = {c: handle for c in handle.seqnames}
+        else:
+            handles = self.handles
+        return handles
+
     def __del__(self) -> None:
         if self.handles is not None:
             for handle in self.handles.values():
                 handle.close()
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/variants/records.py` & `genvarloader-0.3.1/python/genvarloader/variants/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict, Iterable, List, Optional, Tuple, Union, overload
+from typing import Dict, Iterable, List, Literal, Optional, Tuple, Union, overload
 
 import numba as nb
 import numpy as np
 import polars as pl
 from attrs import define
 from loguru import logger
 from numpy.typing import ArrayLike, NDArray
 from tqdm.auto import tqdm
-from typing_extensions import Self
+from typing_extensions import Self, assert_never
 
-from ..utils import normalize_contig_name
+from ..utils import lengths_to_offsets, normalize_contig_name, offsets_to_lengths
 
 try:
     import cyvcf2
 
     CYVCF2_INSTALLED = True
 except ImportError:
     CYVCF2_INSTALLED = False
@@ -108,26 +108,18 @@
     @staticmethod
     def concat(*vlen_alleles: "VLenAlleles"):
         if len(vlen_alleles) == 0:
             return VLenAlleles(np.array([0], np.uint32), np.array([], "|S1"))
         elif len(vlen_alleles) == 1:
             return vlen_alleles[0]
 
-        offset_ends = np.array([v.offsets[-1] for v in vlen_alleles[:-1]]).cumsum(
-            dtype=np.uint32
-        )
-        offsets = np.concatenate(
-            [
-                vlen_alleles[0].offsets,
-                *(
-                    v.offsets + last_offset_end
-                    for v, last_offset_end in zip(vlen_alleles[1:], offset_ends)
-                ),
-            ]
+        nuc_per_allele = np.concatenate(
+            [offsets_to_lengths(v.offsets) for v in vlen_alleles]
         )
+        offsets = lengths_to_offsets(nuc_per_allele, np.uint32)
         alleles = np.concatenate([v.alleles for v in vlen_alleles])
         return VLenAlleles(offsets, alleles)
 
 
 @define
 class RecordInfo:
     """Information about sets of records corresponding to range queries.
@@ -162,14 +154,18 @@
     size_diffs: NDArray[np.int32]  # (n_variants)
     refs: VLenAlleles
     alts: VLenAlleles
     start_idxs: NDArray[np.int32]  # (n_queries)
     end_idxs: NDArray[np.int32]  # (n_queries)
     offsets: NDArray[np.uint32]  # (n_queries + 1)
 
+    @property
+    def n_queries(self):
+        return len(self.start_idxs)
+
     @classmethod
     def empty(cls, n_queries: int):
         return cls(
             positions=np.empty(n_queries, np.int32),
             size_diffs=np.empty(n_queries, np.int32),
             refs=VLenAlleles(
                 np.zeros(n_queries + 1, np.uint32), np.empty(n_queries, "S1")
@@ -178,14 +174,48 @@
                 np.zeros(n_queries + 1, np.uint32), np.empty(n_queries, "S1")
             ),
             start_idxs=np.empty(n_queries, np.int32),
             end_idxs=np.empty(n_queries, np.int32),
             offsets=np.zeros(n_queries + 1, np.uint32),
         )
 
+    @staticmethod
+    def concat(
+        *record_infos: "RecordInfo", how: Literal["separate", "merge"] = "separate"
+    ):
+        if len(record_infos) == 0:
+            return RecordInfo.empty(0)
+        elif len(record_infos) == 1:
+            return record_infos[0]
+
+        positions = np.concatenate([r.positions for r in record_infos])
+        size_diffs = np.concatenate([r.size_diffs for r in record_infos])
+        refs = VLenAlleles.concat(*(r.refs for r in record_infos))
+        alts = VLenAlleles.concat(*(r.alts for r in record_infos))
+        start_idxs = np.concatenate([r.start_idxs for r in record_infos])
+        end_idxs = np.concatenate([r.end_idxs for r in record_infos])
+        v_per_query = np.concatenate(
+            [offsets_to_lengths(r.offsets) for r in record_infos]
+        )
+        if how == "separate":
+            offsets = lengths_to_offsets(v_per_query, np.uint32)
+        elif how == "merge":
+            offsets = np.array([0, v_per_query.sum()], np.uint32)
+        else:
+            assert_never(how)
+        return RecordInfo(
+            positions=positions,
+            size_diffs=size_diffs,
+            refs=refs,
+            alts=alts,
+            start_idxs=start_idxs,
+            end_idxs=end_idxs,
+            offsets=offsets,
+        )
+
 
 @define
 class Records:
     contigs: List[str]
     contig_offsets: Dict[str, int]
 
     ## sorted by starts ##
@@ -551,23 +581,22 @@
 
     def vars_in_range(
         self,
         contig: str,
         starts: ArrayLike,
         ends: ArrayLike,
     ) -> RecordInfo:
+        starts = np.atleast_1d(np.asarray(starts, dtype=int))
+        ends = np.atleast_1d(np.asarray(ends, dtype=int))
         n_queries = len(starts)
 
         _contig = normalize_contig_name(contig, self.contigs)
         if _contig is None:
             return RecordInfo.empty(n_queries)
 
-        starts = np.atleast_1d(np.asarray(starts, dtype=int))
-        ends = np.atleast_1d(np.asarray(ends, dtype=int))
-
         _s_idxs = np.searchsorted(self.v_ends[_contig], starts)
         # make idxs absolute
         s_idxs = self.e2s_idx[_contig][_s_idxs] + self.contig_offsets[_contig]
         e_idxs = (
             np.searchsorted(self.v_starts[_contig], ends) + self.contig_offsets[_contig]
         )
```

### Comparing `genvarloader-0.3.0rc9/genvarloader/zarr.py` & `genvarloader-0.3.1/python/genvarloader/zarr.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,16 @@
                         batched(reader.coords["sample"], 10)
                     ):
                         pbar.set_description(f"Reading {contig}")
                         data = reader.read(contig, 0, e, sample=samples)
 
                         if tstore is None:
                             tstore = ts_open(
-                                dtype=data.dtype, shape=data.shape
+                                dtype=data.dtype,
+                                shape=(reader.sizes["sample"], *data.shape[1:]),
                             ).result()
 
                         pbar.set_description(f"Writing {contig}")
                         start = b_idx * 10
                         stop = b_idx * 10 + len(samples)
                         tstore[start:stop].write(data).result()
```

