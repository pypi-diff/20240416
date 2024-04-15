# Comparing `tmp/stabilizer_timelime-0.1.2.tar.gz` & `tmp/stabilizer_timelime-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.1.2.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.1.3.tar", max compression
```

## Comparing `stabilizer_timelime-0.1.2.tar` & `stabilizer_timelime-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.2/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.2/README.md
--rw-r--r--   0        0        0      774 2024-04-15 19:35:38.007374 stabilizer_timelime-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.2/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0       34 2024-04-12 21:50:28.597160 stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/__init__.py
--rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/slurpdata.py
--rw-r--r--   0        0        0      438 2024-04-15 19:26:58.504536 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/__init__.py
--rw-r--r--   0        0        0     1189 2024-04-15 16:24:28.643589 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/config.py
--rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/.DS_Store
--rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS.py
--rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
--rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/DE.py
--rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
--rw-r--r--   0        0        0    10624 2024-04-15 19:30:51.521486 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
--rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Stats_files.py
--rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__init__.py
--rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
--rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
--rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
--rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
--rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
--rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
--rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
--rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
--rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
--rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
--rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
--rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
--rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
--rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
--rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
--rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
--rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
--rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
--rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
--rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
--rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
--rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
--rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
--rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
--rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
--rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
--rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     3268 2024-04-15 19:27:21.411760 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
--rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch.py
--rw-r--r--   0        0        0    11349 2024-04-15 19:28:16.647125 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
--rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
--rw-r--r--   0        0        0     9281 2024-04-15 19:29:17.579849 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
--rw-r--r--   0        0        0     3906 2024-04-15 17:03:28.530047 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
--rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/learners.py
--rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/optimizer.py
--rw-r--r--   0        0        0    13666 2024-04-15 19:31:02.203042 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
--rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
--rw-r--r--   0        0        0     7408 2024-04-14 17:09:44.278177 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/utils.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.3/LICENSE
+-rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.3/README.md
+-rw-r--r--   0        0        0      774 2024-04-15 21:47:47.293198 stabilizer_timelime-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.3/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.1.3/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.3/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      466 2024-04-15 19:47:05.100154 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10624 2024-04-15 19:30:51.521486 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
+-rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
+-rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
+-rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
+-rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
+-rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
+-rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
+-rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
+-rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
+-rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
+-rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
+-rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
+-rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
+-rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
+-rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
+-rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
+-rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
+-rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
+-rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
+-rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
+-rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
+-rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
+-rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
+-rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
+-rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11413 2024-04-15 21:46:52.663909 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9282 2024-04-15 19:40:19.503100 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     4056 2024-04-15 21:39:00.614598 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
+-rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.3/PKG-INFO
```

### Comparing `stabilizer_timelime-0.1.2/LICENSE` & `stabilizer_timelime-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/pyproject.toml` & `stabilizer_timelime-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/slurpdata.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/config.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,19 @@
 class Config:
     def __init__(self, goals:list=DEFAULT_GOALS, month:int=12, data_path:str="data/data_use/", branching_factor:int=7, data_meta:str=None, domain:list=None, seed=12345) -> None:
         self.goals = goals
         self.no_goals = len(goals)
         self.month = month
         self.data_path = data_path
         self.branching_factor = branching_factor
-        self.data_meta = data_meta
-        self.domain = domain
         self.seed = seed
         
     def __str__(self) -> str:
         res = "Configuration:\n"
-        res += "Goal: " + " ,".join(self.goals) + "\n"
+        res += "Goals: " + " ,".join(self.goals) + "\n"
         res += "Number of Goals: " + str(self.no_goals) + "\n"
-        res += "Data Path: " + str(self.data_path) + "\n"
         res += "Branching Factor: " + str(self.branching_factor) + "\n"
-        res += "Meta File Path: " + str(self.data_meta) + "\n"
-        res += "Domain: " +  " ,".join(self.domain) + "\n"
         res += "Seed: " + str(self.seed) + "\n"
-
+        res += "Data Path: " + str(self.data_path) + "\n"
         res = "="*50 + "\n" + res + "="*50 + "\n"
 
         return res
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/.DS_Store` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS_regression.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/CFS_regression.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/DE.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/DE.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Stats_files.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/Stats_files.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/attribute_selector.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/attribute_selector.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,15 @@
 def calculate_median(repo_pool, path, goal, config):
     feature_selected = []
     repos = []
     for repo in sorted(repo_pool):
         try:
             data = utils.data_goal_arrange(repo, path, goal, config)
             data = data.iloc[:,:-1]
-            # print("data values: ",data['license'][0])
-            # print("data: ", data.median())
             data_median = data.median().values.tolist()
-            # data_median.append(data['license'][0])
-            # print("data median: ",data_median)
             feature_selected.append(data_median)
             repos.append(repo)
         except Exception as e:
             print(e)
             continue
     return feature_selected, repos
 
@@ -43,15 +39,16 @@
         if not filename.startswith('.'):
             repo_pool.append(os.path.join(filename))
 
     for _goal in range(no_goals):
         goal = utils.get_goal(_goal, config)
         print("goal: ",goal)
         df_cols = utils.data_goal_arrange(repo_pool[0], path, _goal, config).columns[:-1]
-        feature_selected, repos = calculate_median(repo_pool, path, _goal)
+        feature_selected, repos = calculate_median(repo_pool, path, _goal, config)
+        print(feature_selected, repos)
         median_df = pd.DataFrame(feature_selected, columns = df_cols, index = repos)
         median_df.to_csv('results/attribute/'+str(seed)+'/data_attribute_' + goal + '.csv')
 
 
 if __name__ == '__main__':
     repo_pool = []
    
@@ -97,10 +94,10 @@
                 repo_pool.append(os.path.join(filename))
 
         for _goal in range(no_goals):
             goal = utils.get_goal(_goal, DEFAULT_CONFIG)
             print("goal: ",goal)
             df_cols = utils.data_goal_arrange(repo_pool[0], path, _goal, DEFAULT_CONFIG).columns[:-1]
             print("df_cols: ",len(df_cols))
-            feature_selected, repos = calculate_median(repo_pool, path, _goal)
+            feature_selected, repos = calculate_median(repo_pool, path, _goal, DEFAULT_CONFIG)
             median_df = pd.DataFrame(feature_selected, columns = df_cols, index = repos)
             median_df.to_csv('results/attribute/'+str(seed)+'/data_attribute_' + goal + '.csv')
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/birch.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 import timeit
 import random
 
 
 import matplotlib.pyplot as plt
 
 from . import birch
-from predictor_advance_v1 import *
+from .predictor_advance_v1 import *
 from . import utils
-import CFS_regression as CFS
+from . import CFS_regression as CFS
 
 
 from multiprocessing import Pool, cpu_count
 from threading import Thread
 from multiprocessing import Queue
 
 # import metrices
@@ -190,14 +190,16 @@
         meta_path = 'results/attribute/'+str(seed)+'/data_attribute_' + goal + '.csv'
         data_store_path = 'results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/'
         attr_df = pd.read_csv(meta_path, index_col=0)
 
         attr_df_index = list(attr_df.index)
         sample_size = attr_df.shape[0]
 
+        print("Training size: ", int(sample_size*0.8))
+
         training_projects = random.sample(attr_df_index, int(sample_size*0.8)) 
         test_projects = []
         test_len=0
         for project in attr_df_index:
             if project not in training_projects:
                 test_projects.append(project) #todo use seed rand
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/default_bellwether.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/default_bellwether.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import timeit
 
 
 import matplotlib.pyplot as plt
 
 from . import birch
-from predictor_advance_v1 import *
+from .predictor_advance_v1 import *
 from . import utils
 
 
 from multiprocessing import  cpu_count
 from threading import Thread
 
 # import metrices
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/init_datafiles.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/init_datafiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 
 DEFAULT_CONFIG = Config()
 
 def create_folders(config=DEFAULT_CONFIG):
     folders_to_create = ["data/data_use/","results/attribute/", "results/with_CFS_DE/", "meta_data/"]
 
     for folder in folders_to_create:
-        shutil.rmtree(folder)
+        shutil.rmtree(folder, ignore_errors=True)
         Path(folder).mkdir(parents=True, exist_ok=True)
     
-    shutil.rmtree("data/data_use_{0}_months/".format(config.month))
+    shutil.rmtree("data/data_use_{0}_months/".format(config.month), ignore_errors=True)
     Path("data/data_use_{0}_months/".format(config.month)).mkdir(parents=True, exist_ok=True)
 
-    attr_seed = os.path.join("results/attribute/", config.seed)
+    attr_seed = os.path.join("results/attribute/", str(config.seed))
     Path(attr_seed).mkdir(parents=True, exist_ok=True)
 
-    cfs_seed = os.path.join("results/with_CFS_DE/", config.seed)
+    cfs_seed = os.path.join("results/with_CFS_DE/", str(config.seed))
     Path(cfs_seed).mkdir(parents=True, exist_ok=True)
 
     subfolders = ['Stats_new', 'month_{0}_models'.format(config.month)]
 
     for subfolder in subfolders:
         subfolder_path = os.path.join(cfs_seed, subfolder)
         if subfolder!='Stats_new':
@@ -86,20 +86,22 @@
 
             num_rows = df.shape[0]
 
             if num_rows>config.month:
                 shutil.copy(filepath, os.path.join(destination_folder, filename))
 
 def move_back_2_data_use(config=DEFAULT_CONFIG):
-    shutil.rmtree("data/data_use/")
-    Path("data/data_use/").mkdir(parents=True, exist_ok=True)
-
     source_dir = "data/data_use_{0}_months/".format(config.month)
     dest_dir = "data/data_use/"
 
+    for file_name in os.listdir(dest_dir):
+        file_path = os.path.join(dest_dir, file_name)
+
+        os.remove(file_path)
+
     cols = ["dates"] + config.goals
 
     # Loop through all files in the source directory
     for file_name in os.listdir(source_dir):
         file_path = os.path.join(source_dir, file_name)
         
         # Check if the file is a CSV file
@@ -114,14 +116,17 @@
             shutil.copy(file_path, os.path.join(dest_dir, file_name))
 
 
 def init_datafiles(config=DEFAULT_CONFIG):
     # Create necessary folders
     create_folders(config)
 
+    # Copy data files to data_use/
+    copy_source_2_data_use(config)
+
     # Rename data files
     rename_data_files()
 
     # Only take data for x months
     move_x_months_data(config)
 
     # Move data back to data_use/ with some cleaning
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/learners.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/learners.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/optimizer.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/optimizer.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from utils import *
+from .utils import *
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor
-from optimizer import *
+from .optimizer import *
 from .predictor_baseline import *
 import pandas as pd
 
-from learners import SK_DTR, SK_RRF
-from DE import DE_Tune_ML
+from .learners import SK_DTR, SK_RRF
+from .DE import DE_Tune_ML
 import traceback
 
 from ..config import Config
 DEFAULT_CONFIG = Config()
 
 def tune_learner(learner, train_X, train_Y, tune_X, tune_Y, goal,
                  target_class=None):
```

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/utils.py` & `stabilizer_timelime-0.1.3/stabilizer_timelime/src/stabilizer/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         F1 = 0
     else:
         F1 = 2 * (Recall * Precision) / (Recall + Precision)
     return [Accuracy, Precision, Recall, F1]
 
 
 def data_goal_arrange(repo_name, directory, goal, config):
-    print(directory,repo_name)
     df_raw = pd.read_csv(directory + repo_name, sep=',')
     df_raw = df_raw.drop(columns=['dates'])
     last_col = get_goal(goal, config)
     cols = list(df_raw.columns.values)
     cols.pop(cols.index(last_col))
     df_adjust = df_raw[cols+[last_col]]
```

### Comparing `stabilizer_timelime-0.1.2/PKG-INFO` & `stabilizer_timelime-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.1.2
+Version: 0.1.3
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

