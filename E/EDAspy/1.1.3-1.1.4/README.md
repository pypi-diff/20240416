# Comparing `tmp/EDAspy-1.1.3.tar.gz` & `tmp/EDAspy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EDAspy-1.1.3.tar", last modified: Fri Sep 29 15:29:58 2023, max compression
+gzip compressed data, was "edaspy-1.1.4.tar", last modified: Tue Apr 16 07:45:03 2024, max compression
```

## Comparing `EDAspy-1.1.3.tar` & `EDAspy-1.1.4.tar`

### file list

```diff
@@ -1,87 +1,304 @@
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.325448 EDAspy-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.197446 EDAspy-1.1.3/EDAspy/
--rw-rw-rw-   0        0        0       82 2023-09-28 10:03:15.000000 EDAspy-1.1.3/EDAspy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.211447 EDAspy-1.1.3/EDAspy/benchmarks/
--rw-rw-rw-   0        0        0      141 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/benchmarks/__init__.py
--rw-rw-rw-   0        0        0      328 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/benchmarks/binary.py
--rw-rw-rw-   0        0        0    13889 2023-03-22 14:02:48.000000 EDAspy-1.1.3/EDAspy/benchmarks/continuous.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.220447 EDAspy-1.1.3/EDAspy/optimization/
--rw-rw-rw-   0        0        0      270 2023-09-28 15:42:54.000000 EDAspy-1.1.3/EDAspy/optimization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.224449 EDAspy-1.1.3/EDAspy/optimization/custom/
--rw-rw-rw-   0        0        0      360 2023-09-28 15:38:46.000000 EDAspy-1.1.3/EDAspy/optimization/custom/__init__.py
--rw-rw-rw-   0        0        0     6162 2023-03-22 13:46:56.000000 EDAspy-1.1.3/EDAspy/optimization/custom/eda_custom.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.238447 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/
--rw-rw-rw-   0        0        0      411 2023-09-28 13:16:08.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/__init__.py
--rw-rw-rw-   0        0        0      345 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/_generation_init.py
--rw-rw-rw-   0        0        0     1475 2023-09-28 14:52:46.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/categorical_geninit.py
--rw-rw-rw-   0        0        0     2200 2023-09-28 09:46:53.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/latin_hypercube_sampling_geninit.py
--rw-rw-rw-   0        0        0     2016 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/multi_gauss_geninit.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uni_bin_geninit.py
--rw-rw-rw-   0        0        0     2069 2023-03-22 11:48:09.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uni_gauss_geninit.py
--rw-rw-rw-   0        0        0     1839 2023-09-28 09:14:32.000000 EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uniform_geninit.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.261447 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/
--rw-rw-rw-   0        0        0      509 2023-09-28 15:11:49.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/__init__.py
--rw-rw-rw-   0        0        0      719 2023-09-29 09:52:30.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/_probabilistic_model.py
--rw-rw-rw-   0        0        0     2267 2023-09-29 15:24:10.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/discrete_bayesian_network.py
--rw-rw-rw-   0        0        0     8579 2023-05-23 10:49:59.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/gaussian_bayesian_network.py
--rw-rw-rw-   0        0        0     3601 2023-09-29 09:45:16.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/kde_bayesian_network.py
--rw-rw-rw-   0        0        0     2366 2023-09-29 12:06:28.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/multivariate_gaussian.py
--rw-rw-rw-   0        0        0     3807 2023-06-28 09:02:13.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/semiparametric_bayesian_network.py
--rw-rw-rw-   0        0        0     2287 2023-09-29 09:50:46.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_binary.py
--rw-rw-rw-   0        0        0     2269 2023-09-29 09:50:24.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_categorical.py
--rw-rw-rw-   0        0        0     2074 2023-09-29 09:50:24.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_gaussian.py
--rw-rw-rw-   0        0        0     1611 2023-09-29 09:50:55.000000 EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_kde.py
--rw-rw-rw-   0        0        0     9370 2023-09-28 10:20:56.000000 EDAspy-1.1.3/EDAspy/optimization/eda.py
--rw-rw-rw-   0        0        0     1400 2023-04-17 15:35:01.000000 EDAspy-1.1.3/EDAspy/optimization/eda_result.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.273447 EDAspy-1.1.3/EDAspy/optimization/multivariate/
--rw-rw-rw-   0        0        0      193 2023-09-28 12:51:12.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/__init__.py
--rw-rw-rw-   0        0        0     4498 2023-09-29 09:08:47.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/ebna.py
--rw-rw-rw-   0        0        0     4708 2023-09-29 09:03:30.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/egna.py
--rw-rw-rw-   0        0        0     4515 2023-09-29 09:04:06.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/emna.py
--rw-rw-rw-   0        0        0     5668 2023-09-29 09:04:18.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/keda.py
--rw-rw-rw-   0        0        0     6019 2023-09-29 09:04:29.000000 EDAspy-1.1.3/EDAspy/optimization/multivariate/speda.py
--rw-rw-rw-   0        0        0     4148 2023-03-22 15:59:36.000000 EDAspy-1.1.3/EDAspy/optimization/tools.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.282447 EDAspy-1.1.3/EDAspy/optimization/univariate/
--rw-rw-rw-   0        0        0      200 2023-09-28 15:42:59.000000 EDAspy-1.1.3/EDAspy/optimization/univariate/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-09-29 09:06:38.000000 EDAspy-1.1.3/EDAspy/optimization/univariate/keda.py
--rw-rw-rw-   0        0        0     4466 2023-09-28 09:44:58.000000 EDAspy-1.1.3/EDAspy/optimization/univariate/umda_binary.py
--rw-rw-rw-   0        0        0     4309 2023-09-29 09:09:31.000000 EDAspy-1.1.3/EDAspy/optimization/univariate/umda_categorical.py
--rw-rw-rw-   0        0        0     5362 2023-09-29 09:07:24.000000 EDAspy-1.1.3/EDAspy/optimization/univariate/umda_continuous.py
--rw-rw-rw-   0        0        0     1500 2023-03-28 13:56:07.000000 EDAspy-1.1.3/EDAspy/optimization/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.205447 EDAspy-1.1.3/EDAspy.egg-info/
--rw-rw-rw-   0        0        0     9702 2023-09-29 15:29:58.000000 EDAspy-1.1.3/EDAspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3030 2023-09-29 15:29:58.000000 EDAspy-1.1.3/EDAspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-29 15:29:58.000000 EDAspy-1.1.3/EDAspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-09-29 15:29:58.000000 EDAspy-1.1.3/EDAspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1066 2023-03-22 11:48:09.000000 EDAspy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     9702 2023-09-29 15:29:58.325448 EDAspy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7621 2023-09-29 12:52:56.000000 EDAspy-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-09-29 15:29:58.326447 EDAspy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1513 2023-09-29 15:27:34.000000 EDAspy-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.284447 EDAspy-1.1.3/tests/
--rw-rw-rw-   0        0        0       70 2023-03-22 14:18:16.000000 EDAspy-1.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.295447 EDAspy-1.1.3/tests/edas_multivariate/
--rw-rw-rw-   0        0        0       57 2023-09-28 15:53:30.000000 EDAspy-1.1.3/tests/edas_multivariate/__init__.py
--rw-rw-rw-   0        0        0     4213 2023-09-28 15:03:59.000000 EDAspy-1.1.3/tests/edas_multivariate/test_ebna.py
--rw-rw-rw-   0        0        0     6723 2023-09-28 10:17:44.000000 EDAspy-1.1.3/tests/edas_multivariate/test_egna.py
--rw-rw-rw-   0        0        0     4952 2023-09-28 10:17:34.000000 EDAspy-1.1.3/tests/edas_multivariate/test_emna.py
--rw-rw-rw-   0        0        0     6368 2023-09-28 10:17:24.000000 EDAspy-1.1.3/tests/edas_multivariate/test_multivariate_keda.py
--rw-rw-rw-   0        0        0     6928 2023-09-28 10:18:31.000000 EDAspy-1.1.3/tests/edas_multivariate/test_speda.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.304448 EDAspy-1.1.3/tests/edas_univariate/
--rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 EDAspy-1.1.3/tests/edas_univariate/__init__.py
--rw-rw-rw-   0        0        0     6148 2023-09-28 11:04:18.000000 EDAspy-1.1.3/tests/edas_univariate/test_umdac.py
--rw-rw-rw-   0        0        0     4193 2023-09-28 15:50:24.000000 EDAspy-1.1.3/tests/edas_univariate/test_umdacat.py
--rw-rw-rw-   0        0        0     4342 2023-09-07 08:55:03.000000 EDAspy-1.1.3/tests/edas_univariate/test_umdad.py
--rw-rw-rw-   0        0        0     5255 2023-09-28 10:19:48.000000 EDAspy-1.1.3/tests/edas_univariate/test_univariate_keda.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.308447 EDAspy-1.1.3/tests/inits/
--rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 EDAspy-1.1.3/tests/inits/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-09-28 14:45:28.000000 EDAspy-1.1.3/tests/inits/test_geninit.py
-drwxrwxrwx   0        0        0        0 2023-09-29 15:29:58.322447 EDAspy-1.1.3/tests/pms/
--rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 EDAspy-1.1.3/tests/pms/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-09-28 14:22:03.000000 EDAspy-1.1.3/tests/pms/test_discrete_bn.py
--rw-rw-rw-   0        0        0     2606 2023-09-28 15:32:55.000000 EDAspy-1.1.3/tests/pms/test_gbn.py
--rw-rw-rw-   0        0        0     1526 2023-09-28 15:05:55.000000 EDAspy-1.1.3/tests/pms/test_kdebn.py
--rw-rw-rw-   0        0        0     3306 2023-09-28 15:32:32.000000 EDAspy-1.1.3/tests/pms/test_spbn.py
--rw-rw-rw-   0        0        0     1410 2023-09-28 15:37:04.000000 EDAspy-1.1.3/tests/pms/test_uni_bin_pm.py
--rw-rw-rw-   0        0        0     1653 2023-09-28 15:41:37.000000 EDAspy-1.1.3/tests/pms/test_uni_cat_pm.py
--rw-rw-rw-   0        0        0      902 2023-09-28 15:35:55.000000 EDAspy-1.1.3/tests/pms/test_uni_gauss_pm.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.057206 edaspy-1.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.410035 edaspy-1.1.4/EDAspy/
+-rw-rw-rw-   0        0        0       82 2024-04-15 17:45:53.000000 edaspy-1.1.4/EDAspy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.425707 edaspy-1.1.4/EDAspy/benchmarks/
+-rw-rw-rw-   0        0        0      141 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/__init__.py
+-rw-rw-rw-   0        0        0      328 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/binary.py
+-rw-rw-rw-   0        0        0    13889 2023-03-22 14:02:48.000000 edaspy-1.1.4/EDAspy/benchmarks/continuous.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.865885 edaspy-1.1.4/EDAspy/benchmarks/input_data/
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_10_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_11_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_12_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_13_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_14_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_15_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_16_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_17_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_18_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_19_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_1_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_20_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_21_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_22_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_23_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_24_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_25_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_26_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_27_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_28_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_29_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_2_D50.txt
+-rw-rw-rw-   0        0        0    25200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D10.txt
+-rw-rw-rw-   0        0        0  2502000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D100.txt
+-rw-rw-rw-   0        0        0      832 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D2.txt
+-rw-rw-rw-   0        0        0   100400 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D20.txt
+-rw-rw-rw-   0        0        0   225600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D30.txt
+-rw-rw-rw-   0        0        0   626000 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_30_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_3_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_4_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_5_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_6_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_7_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_8_D50.txt
+-rw-rw-rw-   0        0        0     2520 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D10.txt
+-rw-rw-rw-   0        0        0   250200 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D100.txt
+-rw-rw-rw-   0        0        0      104 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D2.txt
+-rw-rw-rw-   0        0        0    10040 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D20.txt
+-rw-rw-rw-   0        0        0    22560 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D30.txt
+-rw-rw-rw-   0        0        0    62600 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/M_9_D50.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_1.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_10.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_11.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_12.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_13.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_14.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_15.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_16.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_17.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_18.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_19.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_2.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_20.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_21.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_22.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_23.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_24.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_25.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_26.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_27.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_28.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_29.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_3.txt
+-rw-rw-rw-   0        0        0    25020 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_30.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_4.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_5.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_6.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_7.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_8.txt
+-rw-rw-rw-   0        0        0     2502 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/benchmarks/input_data/shift_data_9.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.897215 edaspy-1.1.4/EDAspy/optimization/
+-rw-rw-rw-   0        0        0      281 2024-03-25 18:21:18.000000 edaspy-1.1.4/EDAspy/optimization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.897215 edaspy-1.1.4/EDAspy/optimization/custom/
+-rw-rw-rw-   0        0        0      382 2024-03-25 18:17:42.000000 edaspy-1.1.4/EDAspy/optimization/custom/__init__.py
+-rw-rw-rw-   0        0        0     6162 2023-03-22 13:46:56.000000 edaspy-1.1.4/EDAspy/optimization/custom/eda_custom.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.928763 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/
+-rw-rw-rw-   0        0        0      411 2023-09-28 13:16:08.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/__init__.py
+-rw-rw-rw-   0        0        0      355 2024-03-25 18:02:01.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/_generation_init.py
+-rw-rw-rw-   0        0        0     1496 2024-04-15 17:30:13.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/categorical_geninit.py
+-rw-rw-rw-   0        0        0     2200 2023-09-28 09:46:53.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/latin_hypercube_sampling_geninit.py
+-rw-rw-rw-   0        0        0     2016 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/multi_gauss_geninit.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uni_bin_geninit.py
+-rw-rw-rw-   0        0        0     2069 2023-03-22 11:48:09.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uni_gauss_geninit.py
+-rw-rw-rw-   0        0        0     1839 2024-03-25 17:44:30.000000 edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uniform_geninit.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.961677 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/
+-rw-rw-rw-   0        0        0      565 2024-03-25 18:17:04.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/__init__.py
+-rw-rw-rw-   0        0        0      719 2024-03-25 18:02:09.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/_probabilistic_model.py
+-rw-rw-rw-   0        0        0     2635 2024-03-25 18:19:13.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/adaptive_univariate_gaussian.py
+-rw-rw-rw-   0        0        0     2370 2024-03-20 18:33:26.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/discrete_bayesian_network.py
+-rw-rw-rw-   0        0        0     8935 2024-03-20 16:01:15.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/gaussian_bayesian_network.py
+-rw-rw-rw-   0        0        0     3601 2023-09-29 09:45:16.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/kde_bayesian_network.py
+-rw-rw-rw-   0        0        0     2366 2023-09-29 12:06:28.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/multivariate_gaussian.py
+-rw-rw-rw-   0        0        0     3807 2023-06-28 09:02:13.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/semiparametric_bayesian_network.py
+-rw-rw-rw-   0        0        0     2287 2023-09-29 09:50:46.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_binary.py
+-rw-rw-rw-   0        0        0     2269 2023-09-29 09:50:24.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_categorical.py
+-rw-rw-rw-   0        0        0     2074 2023-09-29 09:50:24.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_gaussian.py
+-rw-rw-rw-   0        0        0     1611 2023-09-29 09:50:55.000000 edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_kde.py
+-rw-rw-rw-   0        0        0    10150 2024-04-15 17:09:50.000000 edaspy-1.1.4/EDAspy/optimization/eda.py
+-rw-rw-rw-   0        0        0     1400 2023-04-17 15:35:01.000000 edaspy-1.1.4/EDAspy/optimization/eda_result.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.977631 edaspy-1.1.4/EDAspy/optimization/multivariate/
+-rw-rw-rw-   0        0        0      215 2024-03-20 18:48:08.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-03-20 19:16:56.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/boa.py
+-rw-rw-rw-   0        0        0     4643 2024-03-20 19:10:03.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/ebna.py
+-rw-rw-rw-   0        0        0     4778 2024-03-10 11:50:40.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/egna.py
+-rw-rw-rw-   0        0        0     4736 2024-03-10 11:50:24.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/emna.py
+-rw-rw-rw-   0        0        0     5894 2024-03-10 11:50:01.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/keda.py
+-rw-rw-rw-   0        0        0     6245 2024-03-10 11:49:41.000000 edaspy-1.1.4/EDAspy/optimization/multivariate/speda.py
+-rw-rw-rw-   0        0        0     4148 2023-03-22 15:59:36.000000 edaspy-1.1.4/EDAspy/optimization/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.993254 edaspy-1.1.4/EDAspy/optimization/univariate/
+-rw-rw-rw-   0        0        0      224 2024-03-25 18:20:58.000000 edaspy-1.1.4/EDAspy/optimization/univariate/__init__.py
+-rw-rw-rw-   0        0        0     4286 2024-03-10 11:49:18.000000 edaspy-1.1.4/EDAspy/optimization/univariate/keda.py
+-rw-rw-rw-   0        0        0     5728 2024-03-25 18:19:39.000000 edaspy-1.1.4/EDAspy/optimization/univariate/pbil.py
+-rw-rw-rw-   0        0        0     4477 2024-04-15 16:57:27.000000 edaspy-1.1.4/EDAspy/optimization/univariate/umda_binary.py
+-rw-rw-rw-   0        0        0     4321 2024-03-20 19:10:21.000000 edaspy-1.1.4/EDAspy/optimization/univariate/umda_categorical.py
+-rw-rw-rw-   0        0        0     5583 2024-03-10 11:48:17.000000 edaspy-1.1.4/EDAspy/optimization/univariate/umda_continuous.py
+-rw-rw-rw-   0        0        0     1500 2023-03-28 13:56:07.000000 edaspy-1.1.4/EDAspy/optimization/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.057206 edaspy-1.1.4/EDAspy.egg-info/
+-rw-rw-rw-   0        0        0     9809 2024-04-16 07:45:02.000000 edaspy-1.1.4/EDAspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12196 2024-04-16 07:45:02.000000 edaspy-1.1.4/EDAspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:45:02.000000 edaspy-1.1.4/EDAspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-16 07:45:02.000000 edaspy-1.1.4/EDAspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-16 07:45:02.000000 edaspy-1.1.4/EDAspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1066 2023-03-22 11:48:09.000000 edaspy-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     9809 2024-04-16 07:45:03.057206 edaspy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8513 2024-04-15 17:51:55.000000 edaspy-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:45:03.057206 edaspy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2024-04-16 06:52:59.000000 edaspy-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:02.993254 edaspy-1.1.4/tests/
+-rw-rw-rw-   0        0        0       70 2023-03-22 14:18:16.000000 edaspy-1.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.010328 edaspy-1.1.4/tests/edas_multivariate/
+-rw-rw-rw-   0        0        0       57 2023-09-28 15:53:30.000000 edaspy-1.1.4/tests/edas_multivariate/__init__.py
+-rw-rw-rw-   0        0        0     4203 2024-03-25 18:03:34.000000 edaspy-1.1.4/tests/edas_multivariate/test_boa.py
+-rw-rw-rw-   0        0        0     4213 2023-09-28 15:03:59.000000 edaspy-1.1.4/tests/edas_multivariate/test_ebna.py
+-rw-rw-rw-   0        0        0     6723 2023-09-28 10:17:44.000000 edaspy-1.1.4/tests/edas_multivariate/test_egna.py
+-rw-rw-rw-   0        0        0     4952 2023-09-28 10:17:34.000000 edaspy-1.1.4/tests/edas_multivariate/test_emna.py
+-rw-rw-rw-   0        0        0     6368 2023-09-28 10:17:24.000000 edaspy-1.1.4/tests/edas_multivariate/test_multivariate_keda.py
+-rw-rw-rw-   0        0        0     6928 2023-09-28 10:18:31.000000 edaspy-1.1.4/tests/edas_multivariate/test_speda.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.025959 edaspy-1.1.4/tests/edas_univariate/
+-rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 edaspy-1.1.4/tests/edas_univariate/__init__.py
+-rw-rw-rw-   0        0        0     6219 2024-03-25 18:26:36.000000 edaspy-1.1.4/tests/edas_univariate/test_pbil.py
+-rw-rw-rw-   0        0        0     6148 2023-09-28 11:04:18.000000 edaspy-1.1.4/tests/edas_univariate/test_umdac.py
+-rw-rw-rw-   0        0        0     4193 2023-09-28 15:50:24.000000 edaspy-1.1.4/tests/edas_univariate/test_umdacat.py
+-rw-rw-rw-   0        0        0     4342 2023-09-07 08:55:03.000000 edaspy-1.1.4/tests/edas_univariate/test_umdad.py
+-rw-rw-rw-   0        0        0     5255 2023-09-28 10:19:48.000000 edaspy-1.1.4/tests/edas_univariate/test_univariate_keda.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.025959 edaspy-1.1.4/tests/inits/
+-rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 edaspy-1.1.4/tests/inits/__init__.py
+-rw-rw-rw-   0        0        0     3113 2023-09-28 14:45:28.000000 edaspy-1.1.4/tests/inits/test_geninit.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:45:03.057206 edaspy-1.1.4/tests/pms/
+-rw-rw-rw-   0        0        0       57 2023-09-28 15:53:58.000000 edaspy-1.1.4/tests/pms/__init__.py
+-rw-rw-rw-   0        0        0     3228 2024-04-15 17:33:28.000000 edaspy-1.1.4/tests/pms/test_discrete_bn.py
+-rw-rw-rw-   0        0        0     3275 2024-03-12 14:00:13.000000 edaspy-1.1.4/tests/pms/test_gbn.py
+-rw-rw-rw-   0        0        0     1526 2023-09-28 15:05:55.000000 edaspy-1.1.4/tests/pms/test_kdebn.py
+-rw-rw-rw-   0        0        0     3306 2023-09-28 15:32:32.000000 edaspy-1.1.4/tests/pms/test_spbn.py
+-rw-rw-rw-   0        0        0     1410 2023-09-28 15:37:04.000000 edaspy-1.1.4/tests/pms/test_uni_bin_pm.py
+-rw-rw-rw-   0        0        0     1709 2024-04-15 17:34:12.000000 edaspy-1.1.4/tests/pms/test_uni_cat_pm.py
+-rw-rw-rw-   0        0        0      902 2023-09-28 15:35:55.000000 edaspy-1.1.4/tests/pms/test_uni_gauss_pm.py
```

### Comparing `EDAspy-1.1.3/EDAspy/benchmarks/continuous.py` & `edaspy-1.1.4/EDAspy/benchmarks/continuous.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/eda_custom.py` & `edaspy-1.1.4/EDAspy/optimization/custom/eda_custom.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/categorical_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/categorical_geninit.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,10 +39,10 @@
 
         :param size: number of samplings.
         :return: array with the dataset sampled
         :rtype: np.array
         """
         data = {}
         for i in range(self.n_variables):
-            data[i] = np.random.choice(self.possible_values[i], size=size)
+            data[i] = np.random.choice(self.possible_values[i], size=size, p=self.frequency[i])
 
         return pd.DataFrame(data).to_numpy()
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/latin_hypercube_sampling_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/latin_hypercube_sampling_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/multi_gauss_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/multi_gauss_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uni_bin_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uni_bin_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uni_gauss_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uni_gauss_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/initialization_models/uniform_geninit.py` & `edaspy-1.1.4/EDAspy/optimization/custom/initialization_models/uniform_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/_probabilistic_model.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/_probabilistic_model.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/discrete_bayesian_network.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/discrete_bayesian_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,31 +28,32 @@
         super().__init__(variables)
 
         self.variables = variables
         self.pm = BayesianNetwork()
 
         self.id = 7
 
-    def learn(self, dataset: np.array, *args, **kwargs):
+    def learn(self, dataset: np.array, score: str = "bicscore", *args, **kwargs):
         """
         Learn a discrete Bayesian network from the dataset passed as argument.
 
         :param dataset: dataset from which learn the GBN.
+        :param score: score used for the score-based structure learning algorithm
         """
         data = pd.DataFrame(dataset, columns=self.variables, dtype="category")
 
         # initialize model
         self.pm = BayesianNetwork()
 
         # add nodes
         self.pm.add_nodes_from(self.variables)
 
         # learn structure
         es = HillClimbSearch(data)
-        best_structure = es.estimate(scoring_method='bicscore', max_iter=1000, show_progress=False)
+        best_structure = es.estimate(scoring_method=score, max_iter=1000, show_progress=False)
 
         for edge in best_structure.edges():
             self.pm.add_edge(edge[0], edge[1])
 
         # fit model
         self.pm.fit(data, estimator=MaximumLikelihoodEstimator)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/gaussian_bayesian_network.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/gaussian_bayesian_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
             self.vars_1 = list(set(self.variables) - set(self.evidences.keys()))  # not fixed
             self.vars_2 = list(self.evidences.keys())  # evidence
         else:
             self.sample = self._sample_normal
 
         self.id = 4
+        self.fitted = False
 
     def learn(self, dataset: np.array, *args, **kwargs):
         """
         Learn a Gaussian Bayesian network from the dataset passed as argument.
 
         :param dataset: dataset from which learn the GBN.
         """
@@ -71,14 +72,16 @@
             self.pm = hc(data, bn_type=GaussianNetworkType(), arc_blacklist=self.black_list)
         else:
             self.pm = hc(data, bn_type=GaussianNetworkType())
 
         self.pm.fit(data)
         self.top_order = self.pm.graph().topological_sort()
 
+        self.fitted = True
+
     def print_structure(self) -> list:
         """
         Prints the arcs between the nodes that represent the variables in the dataset. This function
         must be used after the learning process.
 
         :return: list of arcs between variables
         :rtype: list
@@ -219,7 +222,14 @@
 
         inv_sigma_22 = np.linalg.pinv(sigma_22)  # pseudo-inverse
 
         mu_1_2 = mu_1 + np.dot(sigma_12, np.dot(inv_sigma_22, (np.array(evidence) - mu_2)))
         sigma_1_2 = sigma_11 - np.dot(sigma_12, np.dot(inv_sigma_22, sigma_21))
 
         return mu_1_2, sigma_1_2
+
+    def maximum_a_posteriori(self, evidence, var_names):
+        # TODO: test this
+        assert self.fitted, "The Bayesian network has not been fitted yet. Please, learn it first."
+
+        mu_map, sigma_map = self.inference(evidence=evidence, var_names=var_names)
+        return mu_map
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/kde_bayesian_network.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/kde_bayesian_network.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/multivariate_gaussian.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/multivariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/semiparametric_bayesian_network.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/semiparametric_bayesian_network.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_binary.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_binary.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_categorical.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_categorical.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_gaussian.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/custom/probabilistic_models/univariate_kde.py` & `edaspy-1.1.4/EDAspy/optimization/custom/probabilistic_models/univariate_kde.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/eda.py` & `edaspy-1.1.4/EDAspy/optimization/eda.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,26 +27,33 @@
                  dead_iter: int,
                  n_variables: int,
                  alpha: float = 0.5,
                  elite_factor: float = 0.4,
                  disp: bool = True,
                  parallelize: bool = False,
                  init_data: np.array = None,
+                 w_noise: float = .5,
                  *args, **kwargs):
 
         self.disp = disp
         self.size_gen = size_gen
         self.max_iter = max_iter
         self.alpha = alpha
         self.n_variables = n_variables
         self.truncation_length = int(size_gen * alpha)
         self.elite_factor = elite_factor
         self.elite_length = int(size_gen * elite_factor)
         self.parallelize = parallelize
 
+        # Gaussian white noise definition
+        if (w_noise != 0) and (w_noise is not None):
+            self.w_noise = w_noise
+        else:
+            self.w_noise = 0
+
         assert dead_iter <= self.max_iter, 'dead_iter must be lower than max_iter'
         self.dead_iter = dead_iter
 
         self.best_mae_global = 999999999999
         self.best_ind_global = np.array([0]*self.n_variables)
 
         self.evaluations = np.array(0)
@@ -134,21 +141,23 @@
             "n_variables": self.n_variables,
             "alpha": self.alpha,
             "elite_factor": self.elite_factor,
             "disp": self.disp,
             "parallelize": self.parallelize
         }
 
-    def minimize(self, cost_function: callable, output_runtime: bool = True, *args, **kwargs) -> EdaResult:
+    def minimize(self, cost_function: callable, output_runtime: bool = True, ftol: float = 1e-8,
+                 *args, **kwargs) -> EdaResult:
         """
         Minimize function to execute the EDA optimization. By default, the optimizer is designed to minimize a cost
         function; if maximization is desired, just add a minus sign to your cost function.
 
         :param cost_function: cost function to be optimized and accepts an array as argument.
         :param output_runtime: true if information during runtime is desired.
+        :param ftol: termination tolerance
         :return: EdaResult object with results and information.
         :rtype: EdaResult
         """
 
         history = []
         not_better = 0
 
@@ -156,33 +165,44 @@
         self.generation = self._initialize_generation()
         self._check_generation(cost_function)
 
         # select just one item to be the elite selection if first iteration
         self.elite_temp = np.array([self.generation[0, :]])
         self.evaluations_elite = np.array([self.evaluations.item(0)])
 
-        best_mae_local = best_mae_global = min(self.evaluations)
+        best_mae_local = self.best_mae_global = min(self.evaluations)
         history.append(best_mae_local)
-        best_ind_local = best_ind_global = np.where(self.evaluations == best_mae_local)[0][0]
+        best_ind_local = self.best_ind_global = np.where(self.evaluations == best_mae_local)[0][0]
+
+        if self.w_noise == 0:
+            white_noise = 0
+        elif self.w_noise == -1:
+            white_noise = ""
+        else:
+            white_noise = np.random.normal(0, self.w_noise, size=(self.truncation_length, self.n_variables))
+
+        if output_runtime:
+            print('IT: 0\tBest cost: ', self.best_mae_global)
 
-        for _ in range(self.max_iter - 1):
+        for _ in range(1, self.max_iter):
             self._truncation()
+            self.generation += white_noise  # We add Gaussian white noise for avoiding genetic drift (optional)
             self._update_pm()
 
             self._new_generation()
             self._check_generation(cost_function)
 
             best_mae_local = min(self.evaluations)
             history.append(best_mae_local)
 
             best_ind_local = np.where(self.evaluations == best_mae_local)[0][0]
             best_ind_local = self.generation[best_ind_local]
 
             # update the best values ever
-            if best_mae_local < self.best_mae_global:
+            if best_mae_local < self.best_mae_global * (1 + ftol):
                 self.best_mae_global = best_mae_local
                 self.best_ind_global = best_ind_local
                 not_better = 0
 
             else:
                 not_better += 1
                 if not_better == self.dead_iter:
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/eda_result.py` & `edaspy-1.1.4/EDAspy/optimization/eda_result.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/multivariate/ebna.py` & `edaspy-1.1.4/EDAspy/optimization/multivariate/ebna.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ..custom.initialization_models import CategoricalSampling
 
 
 class EBNA(EDA):
     """
     Estimation of Bayesian Networks Algorithm. This type of Estimation-of-Distribution Algorithm uses
     a Discrete Bayesian Network from where new solutions are sampled. This multivariate probabilistic
-    model is updated in each iteration with the best individuals of the previous generation.
+    model is updated in each iteration with the best individuals of the previous generation. The main
+    difference towards BOA is that a Bayesian Information Criterion Score is used for the structure
+    learning process.
 
     Example:
 
         This example uses some uses a toy example to show how to use the EBNA implementation.
 
         .. code-block:: python
 
@@ -88,13 +90,13 @@
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=elite_factor, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=-1)
 
         self.vars = [str(i) for i in range(n_variables)]
         # self.landscape_bounds = landscape_bounds
         self.pm = BN(self.vars)
         self.init = CategoricalSampling(self.n_variables, possible_values=possible_values, frequency=frequency)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/multivariate/egna.py` & `edaspy-1.1.4/EDAspy/optimization/multivariate/egna.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,24 @@
     """
 
     def __init__(self,
                  size_gen: int,
                  max_iter: int,
                  dead_iter: int,
                  n_variables: int,
-                 lower_bound: Union[np.array, List[float], float],
-                 upper_bound: Union[np.array, List[float], float],
+                 lower_bound: Union[np.array, List[float], float] = None,
+                 upper_bound: Union[np.array, List[float], float] = None,
                  alpha: float = 0.5,
                  elite_factor: float = 0.4,
                  disp: bool = True,
                  black_list: list = None,
                  white_list: list = None,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size. Number of individuals in each generation.
         :param max_iter: Maximum number of iterations during runtime.
         :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finish.
         :param n_variables: Number of variables to be optimized.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
@@ -77,13 +78,13 @@
         initializer is used.
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=elite_factor, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=w_noise)
 
         self.vars = [str(i) for i in range(n_variables)]
         # self.landscape_bounds = landscape_bounds
         self.pm = GBN(self.vars, black_list=black_list, white_list=white_list)
         self.init = UniformGenInit(self.n_variables, lower_bound=lower_bound, upper_bound=upper_bound)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/multivariate/emna.py` & `edaspy-1.1.4/EDAspy/optimization/multivariate/emna.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,23 +46,24 @@
     """
 
     def __init__(self,
                  size_gen: int,
                  max_iter: int,
                  dead_iter: int,
                  n_variables: int,
-                 lower_bound: Union[np.array, List[float], float],
-                 upper_bound: Union[np.array, List[float], float],
+                 lower_bound: Union[np.array, List[float], float] = None,
+                 upper_bound: Union[np.array, List[float], float] = None,
                  alpha: float = 0.5,
                  elite_factor: float = 0.4,
                  disp: bool = True,
                  lower_factor: float = 0.5,
                  upper_factor: float = 100,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size. Number of individuals in each generation.
         :param max_iter: Maximum number of iterations during runtime.
         :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finish.
         :param n_variables: Number of variables to be optimized.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
@@ -70,19 +71,21 @@
         :param elite_factor: Percentage of previous population selected to add to new generation (elite approach).
         :param lower_factor: Lower bound imposed in std of the variables to not converge to std=0.
         :param upper_factor: Upper bound imposed in std of the variables.
         :param disp: Set to True to print convergence messages.
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
+        :param w_noise: Intensity of the Gaussian white noise added to each generation in order to avoid genetic drift.
+        :type w_noise: float
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=elite_factor, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=w_noise)
 
         self.lower_bound = lower_factor
         self.upper_bound = upper_factor
 
         self.pm = MultiGauss(list(range(n_variables)), lower_factor, upper_factor)
         self.init = UniformGenInit(self.n_variables, lower_bound=lower_bound, upper_bound=upper_bound)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/multivariate/keda.py` & `edaspy-1.1.4/EDAspy/optimization/multivariate/speda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from ..eda import EDA
-from ..custom.probabilistic_models import KDEBN
+from ..custom.probabilistic_models import SPBN
 from ..custom.initialization_models import UniformGenInit
 
 import numpy as np
 from typing import Union, List
 
 
-class MultivariateKEDA(EDA):
+class SPEDA(EDA):
     """
-    Kernel Estimation of Distribution Algorithm [1]. This type of Estimation-of-Distribution
-    Algorithm uses a KDE Bayesian network [2] which allows dependencies between variables which have
-    been estimated using KDE. This multivariate probabilistic model is updated in each iteration
-    with the best individuals of the previous generations.
+    Semiparametric Estimation of Distribution Algorithm [1]. This type of Estimation-of-Distribution
+    Algorithm uses a semiparametric Bayesian network [2] which allows dependencies between variables
+    which have been estimated using KDE with variables which fits a Gaussian distribution. By this
+    way, it avoid the assumption of Gaussianity in the variables of the optimization problem. This
+    multivariate probabilistic model is updated in each iteration with the best individuals of the
+    previous generations.
+
+    SPEDA has shown to improve the results for more complex optimization problem compared to the
+    univariate EDAs that can be found implemented in this package, multivariate EDAs such as
+    EGNA, or EMNA, and other population-based algorithms. See [1] for numerical results.
 
     Example:
 
         This example uses some very well-known benchmarks from CEC14 conference to be solved using
-        a Kernel Estimation of Distribution Algorithm (KEDA).
+        a Semiparametric Estimation of Distribution Algorithm (SPEDA).
 
         .. code-block:: python
 
-            from EDAspy.optimization import MultivariateKEDA
+            from EDAspy.optimization import SPEDA
             from EDAspy.benchmarks import ContinuousBenchmarkingCEC14
 
             benchmarking = ContinuousBenchmarkingCEC14(10)
 
-            keda = MultivariateKEDA(size_gen=300, max_iter=100, dead_iter=20, n_variables=10,
-                                    lower_bound=-100, upper_bound=100, l=10)
+            speda = SPEDA(size_gen=300, max_iter=100, dead_iter=20, n_variables=10, lower_bound=-100,
+                          upper_bound=100, l=10)
 
-            eda_result = keda.minimize(benchmarking.cec14_4, True)
+            eda_result = speda.minimize(benchmarking.cec14_4, True)
 
     References:
 
         [1]: Vicente P. Soloviev, Concha Bielza and Pedro Larrañaga. Semiparametric Estimation
         of Distribution Algorithm for continuous optimization. 2022
 
         [2]: Atienza, D., Bielza, C., & Larrañaga, P. (2022). PyBNesian: an extensible Python package
@@ -44,52 +50,54 @@
     """
 
     def __init__(self,
                  size_gen: int,
                  max_iter: int,
                  dead_iter: int,
                  n_variables: int,
-                 lower_bound: Union[np.array, List[float], float],
-                 upper_bound: Union[np.array, List[float], float],
-                 l: float,
+                 lower_bound: Union[np.array, List[float], float] = None,
+                 upper_bound: Union[np.array, List[float], float] = None,
+                 l: float = 10,
                  alpha: float = 0.5,
                  disp: bool = True,
                  black_list: list = None,
                  white_list: list = None,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size. Number of individuals in each generation.
         :param max_iter: Maximum number of iterations during runtime.
-        :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finishes.
+        :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finish.
         :param n_variables: Number of variables to be optimized.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
         :param alpha: Percentage of population selected to update the probabilistic model.
-        :param l: this implementation is an archive-base approach. Thus, in each generation updates the
-        probabilistic model with the best solutions of the previous l generations. If this characteristic is not
-        desired, then l=1.
+        :param l: SPEDA is an archive-base approach. Thus, in each generation updates the probabilistic model with
+        the best solutions of the previous l generations.
         :param alpha: Percentage of population selected to update the probabilistic model in each generation.
         :param disp: Set to True to print convergence messages.
-        :param black_list: list of tuples with the forbidden arcs in the KDEBN during runtime.
-        :param white_list: list of tuples with the mandatory arcs in the KDEBN during runtime.
+        :param black_list: list of tuples with the forbidden arcs in the SPBN during runtime.
+        :param white_list: list of tuples with the mandatory arcs in the SPBN during runtime.
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
+        :param w_noise: Intensity of the Gaussian white noise added to each generation in order to avoid genetic drift.
+        :type w_noise: float
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=alpha, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=w_noise)
 
         self.vars = [str(i) for i in range(n_variables)]
         # self.landscape_bounds = landscape_bounds
-        self.pm = KDEBN(self.vars, black_list=black_list, white_list=white_list)
+        self.pm = SPBN(self.vars, black_list=black_list, white_list=white_list)
 
         self.l_len = l*int(size_gen*self.alpha)  # maximum number of individuals in the archive
         self.archive = np.empty((0, self.n_variables))
 
         # In this implementation the individuals of the first generation are sampled from a uniform distribution
         # to not skew the following estimation of distributions.
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/multivariate/speda.py` & `edaspy-1.1.4/EDAspy/optimization/multivariate/keda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from ..eda import EDA
-from ..custom.probabilistic_models import SPBN
+from ..custom.probabilistic_models import KDEBN
 from ..custom.initialization_models import UniformGenInit
 
 import numpy as np
 from typing import Union, List
 
 
-class SPEDA(EDA):
+class MultivariateKEDA(EDA):
     """
-    Semiparametric Estimation of Distribution Algorithm [1]. This type of Estimation-of-Distribution
-    Algorithm uses a semiparametric Bayesian network [2] which allows dependencies between variables
-    which have been estimated using KDE with variables which fits a Gaussian distribution. By this
-    way, it avoid the assumption of Gaussianity in the variables of the optimization problem. This
-    multivariate probabilistic model is updated in each iteration with the best individuals of the
-    previous generations.
-
-    SPEDA has shown to improve the results for more complex optimization problem compared to the
-    univariate EDAs that can be found implemented in this package, multivariate EDAs such as
-    EGNA, or EMNA, and other population-based algorithms. See [1] for numerical results.
+    Kernel Estimation of Distribution Algorithm [1]. This type of Estimation-of-Distribution
+    Algorithm uses a KDE Bayesian network [2] which allows dependencies between variables which have
+    been estimated using KDE. This multivariate probabilistic model is updated in each iteration
+    with the best individuals of the previous generations.
 
     Example:
 
         This example uses some very well-known benchmarks from CEC14 conference to be solved using
-        a Semiparametric Estimation of Distribution Algorithm (SPEDA).
+        a Kernel Estimation of Distribution Algorithm (KEDA).
 
         .. code-block:: python
 
-            from EDAspy.optimization import SPEDA
+            from EDAspy.optimization import MultivariateKEDA
             from EDAspy.benchmarks import ContinuousBenchmarkingCEC14
 
             benchmarking = ContinuousBenchmarkingCEC14(10)
 
-            speda = SPEDA(size_gen=300, max_iter=100, dead_iter=20, n_variables=10, lower_bound=-100,
-                          upper_bound=100, l=10)
+            keda = MultivariateKEDA(size_gen=300, max_iter=100, dead_iter=20, n_variables=10,
+                                    lower_bound=-100, upper_bound=100, l=10)
 
-            eda_result = speda.minimize(benchmarking.cec14_4, True)
+            eda_result = keda.minimize(benchmarking.cec14_4, True)
 
     References:
 
         [1]: Vicente P. Soloviev, Concha Bielza and Pedro Larrañaga. Semiparametric Estimation
         of Distribution Algorithm for continuous optimization. 2022
 
         [2]: Atienza, D., Bielza, C., & Larrañaga, P. (2022). PyBNesian: an extensible Python package
@@ -50,51 +44,55 @@
     """
 
     def __init__(self,
                  size_gen: int,
                  max_iter: int,
                  dead_iter: int,
                  n_variables: int,
-                 lower_bound: Union[np.array, List[float], float],
-                 upper_bound: Union[np.array, List[float], float],
-                 l: float,
+                 lower_bound: Union[np.array, List[float], float] = None,
+                 upper_bound: Union[np.array, List[float], float] = None,
+                 l: float = 10,
                  alpha: float = 0.5,
                  disp: bool = True,
                  black_list: list = None,
                  white_list: list = None,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size. Number of individuals in each generation.
         :param max_iter: Maximum number of iterations during runtime.
-        :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finish.
+        :param dead_iter: Stopping criteria. Number of iterations with no improvement after which, the algorithm finishes.
         :param n_variables: Number of variables to be optimized.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
         :param alpha: Percentage of population selected to update the probabilistic model.
-        :param l: SPEDA is an archive-base approach. Thus, in each generation updates the probabilistic model with
-        the best solutions of the previous l generations.
+        :param l: this implementation is an archive-base approach. Thus, in each generation updates the
+        probabilistic model with the best solutions of the previous l generations. If this characteristic is not
+        desired, then l=1.
         :param alpha: Percentage of population selected to update the probabilistic model in each generation.
         :param disp: Set to True to print convergence messages.
-        :param black_list: list of tuples with the forbidden arcs in the SPBN during runtime.
-        :param white_list: list of tuples with the mandatory arcs in the SPBN during runtime.
+        :param black_list: list of tuples with the forbidden arcs in the KDEBN during runtime.
+        :param white_list: list of tuples with the mandatory arcs in the KDEBN during runtime.
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
+        :param w_noise: Intensity of the Gaussian white noise added to each generation in order to avoid genetic drift.
+        :type w_noise: float
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=alpha, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=w_noise)
 
         self.vars = [str(i) for i in range(n_variables)]
         # self.landscape_bounds = landscape_bounds
-        self.pm = SPBN(self.vars, black_list=black_list, white_list=white_list)
+        self.pm = KDEBN(self.vars, black_list=black_list, white_list=white_list)
 
         self.l_len = l*int(size_gen*self.alpha)  # maximum number of individuals in the archive
         self.archive = np.empty((0, self.n_variables))
 
         # In this implementation the individuals of the first generation are sampled from a uniform distribution
         # to not skew the following estimation of distributions.
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/tools.py` & `edaspy-1.1.4/EDAspy/optimization/tools.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy/optimization/univariate/keda.py` & `edaspy-1.1.4/EDAspy/optimization/univariate/keda.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,34 +48,37 @@
                  n_variables: int,
                  lower_bound: Union[np.array, List[float], float],
                  upper_bound: Union[np.array, List[float], float],
                  alpha: float = 0.5,
                  elite_factor: float = 0.4,
                  disp: bool = True,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size of each generation.
         :param max_iter: Maximum number of function evaluations.
         :param dead_iter: Stopping criteria. Number of iterations after with no improvement after which EDA stops.
         :param n_variables: Number of variables to be optimized.
         :param alpha: Percentage of population selected to update the probabilistic model.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
         :param elite_factor: Percentage of previous population selected to add to new generation (elite approach).
         :param disp: Set to True to print convergence messages.
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
+        :param w_noise: Intensity of the Gaussian white noise added to each generation in order to avoid genetic drift.
+        :type w_noise: float
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
 
         # self.landscape_bounds = landscape_bounds
         self.names_vars = list(range(n_variables))
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter, n_variables=n_variables,
                          alpha=alpha, elite_factor=elite_factor, disp=disp, parallelize=parallelize,
-                         init_data=init_data)
+                         init_data=init_data, w_noise=w_noise)
 
         self.init = UniformGenInit(n_variables=n_variables, lower_bound=lower_bound, upper_bound=upper_bound)
         self.pm = UniKDE(self.names_vars)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/univariate/umda_binary.py` & `edaspy-1.1.4/EDAspy/optimization/univariate/umda_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter, n_variables=n_variables,
                          alpha=alpha, elite_factor=elite_factor, disp=disp, parallelize=parallelize,
-                         init_data=init_data)
+                         init_data=init_data, w_noise=0)
 
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
         self.vector = vector
 
         self.names_vars = list(range(self.n_variables))
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/univariate/umda_categorical.py` & `edaspy-1.1.4/EDAspy/optimization/univariate/umda_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,13 +84,13 @@
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
         """
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter,
                          n_variables=n_variables, alpha=alpha, elite_factor=elite_factor, disp=disp,
-                         parallelize=parallelize, init_data=init_data)
+                         parallelize=parallelize, init_data=init_data, w_noise=-1)
 
         self.vars = [str(i) for i in range(n_variables)]
         # self.landscape_bounds = landscape_bounds
         self.pm = UniCategorical(self.vars)
         self.init = CategoricalSampling(self.n_variables, possible_values=possible_values, frequency=frequency)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/univariate/umda_continuous.py` & `edaspy-1.1.4/EDAspy/optimization/univariate/umda_continuous.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,23 +54,24 @@
     """
 
     def __init__(self,
                  size_gen: int,
                  max_iter: int,
                  dead_iter: int,
                  n_variables: int,
-                 lower_bound: Union[np.array, List[float], float],
-                 upper_bound: Union[np.array, List[float], float],
+                 lower_bound: Union[np.array, List[float], float] = None,
+                 upper_bound: Union[np.array, List[float], float] = None,
                  alpha: float = 0.5,
                  vector: np.array = None,
                  lower_factor: float = 0.5,
                  elite_factor: float = 0.4,
                  disp: bool = True,
                  parallelize: bool = False,
-                 init_data: np.array = None):
+                 init_data: np.array = None,
+                 w_noise: float = .5):
         r"""
         :param size_gen: Population size of each generation.
         :param max_iter: Maximum number of function evaluations.
         :param dead_iter: Stopping criteria. Number of iterations after with no improvement after which EDA stops.
         :param n_variables: Number of variables to be optimized.
         :param lower_bound: lower bound for the uniform distribution sampling.
         :param upper_bound: lower bound for the uniform distribution sampling.
@@ -78,25 +79,27 @@
         :param vector: Array with shape (2, n_variables) where rows are mean and std of the parameters to be optimized.
         :param lower_factor: Lower bound imposed in std of the variables to not converge to std=0.
         :param elite_factor: Percentage of previous population selected to add to new generation (elite approach).
         :param disp: Set to True to print convergence messages.
         :param parallelize: True if the evaluation of the solutions is desired to be parallelized in multiple cores.
         :param init_data: Numpy array containing the data the EDA is desired to be initialized from. By default, an
         initializer is used.
+        :param w_noise: Intensity of the Gaussian white noise added to each generation in order to avoid genetic drift.
+        :type w_noise: float
         :type lower_bound: List of lower bounds of size equal to number of variables OR single bound to all dimensions.
         :type upper_bound: List of upper bounds of size equal to number of variables OR single bound to all dimensions.
         """
 
         self.vector = vector
         self.lower_bound = lower_factor
         self.names_vars = list(range(n_variables))
 
         super().__init__(size_gen=size_gen, max_iter=max_iter, dead_iter=dead_iter, n_variables=n_variables,
                          alpha=alpha, elite_factor=elite_factor, disp=disp, parallelize=parallelize,
-                         init_data=init_data)
+                         init_data=init_data, w_noise=w_noise)
 
         if self.vector is not None:
             assert self.vector.shape == (2, n_variables)
             self.init = UniGaussGenInit(n_variables, means_vector=self.vector[0, :], stds_vector=self.vector[1, :])
         else:
             self.init = UniformGenInit(self.n_variables, lower_bound=lower_bound, upper_bound=upper_bound)
```

### Comparing `EDAspy-1.1.3/EDAspy/optimization/utils.py` & `edaspy-1.1.4/EDAspy/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/EDAspy.egg-info/PKG-INFO` & `edaspy-1.1.4/EDAspy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,160 @@
 Metadata-Version: 2.1
 Name: EDAspy
-Version: 1.1.3
+Version: 1.1.4
 Summary: EDAspy is a Python package that implements Estimation of Distribution Algorithms. EDAspy allows toeither use already existing implementations or customize the EDAs baseline easily building it bymodules so new research can be easily developed. It also has several benchmarks for comparisons.
 Home-page: https://github.com/VicentePerezSoloviev/EDAspy
+Download-URL: https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.4.tar.gz
 Author: Vicente P. Soloviev
 Author-email: vicente.perez.soloviev@gmail.com
 License: MIT
-Download-URL: https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.2.tar.gz
-Description: # <img src='https://raw.githubusercontent.com/VicentePerezSoloviev/EDAspy/master/Logo%20EDAspy.png' align="right" height="150"/>
-        
-        [![PyPI](https://img.shields.io/pypi/v/edaspy)](https://pypi.python.org/pypi/EDAspy/)
-        [![PyPI license](https://img.shields.io/pypi/l/EDAspy.svg)](https://pypi.python.org/pypi/EDAspy/)
-        [![Downloads](https://static.pepy.tech/badge/edaspy)](https://pepy.tech/project/edaspy)
-        [![Documentation Status](https://readthedocs.org/projects/edaspy/badge/?version=latest)](https://edaspy.readthedocs.io/en/latest/?badge=latest)
-        
-        # EDAspy
-        
-        ## Introduction
-        
-        EDAspy presents some implementations of the Estimation of Distribution Algorithms (EDAs) [1]. EDAs are a type of
-        evolutionary algorithms. Depending on the type of the probabilistic model embedded in the EDA, and the type of
-        variables considered, we will use a different EDA implementation.
-        
-        The pseudocode of EDAs is the following:
-        
-        1. Random initialization of the population.
-        
-        2. Evaluate each individual of the population.
-        
-        3. Select the top best individuals according to cost function evaluation.
-        
-        4. Learn a probabilistic model from the best individuals selected.
-        
-        5. Sampled another population.
-        
-        6. If stopping criteria is met, finish; else, go to 2.
-        
-        EDAspy allows to create a custom version of the EDA. Using the modular probabilistic models and the initializators, this can be embedded into the EDA baseline and used for different purposes. If this fits you, take a look on the examples section to the EDACustom example.
-        
-        EDAspy also incorporates a set of benchmarks in order to compare the algorithms trying to minimize these cost functions.
-        
-        The following implementations are available in EDAspy:
-        
-        * UMDAd: Univariate Marginal Distribution Algorithm binary [2]. It can be used as a simple example of EDA where the variables are binary and there are not dependencies between variables. Some usages include feature selection, for example.
-        
-        
-        * UMDAc: Univariate Marginal Distribution Algorithm continuous [3]. In this EDA all the variables assume a Gaussian distribution and there are not dependencies considered between the variables. Some usages include hyperparameter optimization, for example.
-        
-        
-        * UnivariateKEDA: Univariate Kernel Estimation of Distribution Algorithm [4]. Each variables distribution is estimated using Kernel Density Estimation.
-        
-        
-        * UMDAcat: Univariate Marginal Distribution Algorithm categorical [2]. UMDA variant for categorical data, where more than two possible values per dimension are used (otherwise, use binary version).
-        
-        
-        * EGNA: Estimation of Gaussian Distribution Algorithm [5][6]. This is a complex implementation in which dependencies between the variables are considered during the optimization. In each iteration, a Gaussian Bayesian network is learned and sampled. The variables in the model are assumed to be Gaussian and also de dependencies between them. This implementation is focused in continuous optimization.
-        
-        
-        * EMNA: Estimation of Multivariate Normal Algorithm [1]. This is a similar implementation to EGNA, in which instead of using a Gaussian Bayesian network, a multivariate Gaussian distribution is iteratively learned and sampled. As in EGNA, the dependencies between variables are considered and assumed to be linear Gaussian. This implementation is focused in continuous optimization.
-        
-        
-        * SPEDA: Semiparametric Estimation of Distribution Algorithm [7]. This multivariate EDA allows estimating the density of a variable using either KDE or Gaussians, and allow dependencies between both types of variables. It is an archive-based approach where the probabilistic model is updated given the best individuals of l previous generations.
-        
-        
-        * MultivariateKEDA: Special case of SPEDA approach in which all nodes are restricted to be estimated using KDE (Gaussian nodes are forbidden) [7]. It is also an archive-based approach.
-        
-        
-        * EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed. 
-        
-        
-        Some tools are also available in EDAspy such as the Bayesian network structure plotting, for visualizing the graph learnt in some of the implementations, if needed.
-        
-        
-        Although some categorical EDAs are implemented, the package is focused in continuous optimization. Below, we show a CPU time analysis for the different approaches implemented for continuous optimization. Note that the CPU time can be reduced using parallelization (available as a parameter in the EDA initialization). Reference [7] shows a comparison about the performance of the algorithms in terms of cost function minimization. 
-        
-        <img src='cpu_comparison_continuous_opt.jpeg' alt="CPU time comparison for continuous optimization" title="CPU time comparison for continuous optimization"/>
-        
-        ## Examples
-        
-        Some examples are available in https://github.com/VicentePerezSoloviev/EDAspy/tree/master/notebooks
-        
-        ## Getting started
-        
-        For installing EDAspy from Pypi execute the following command using pip:
-        
-        ```bash
-            pip install EDAspy
-        ```
-        
-        ## Build from Source
-        
-        ### Prerequisites
-        
-        - Python >= 3.0
-        - Pybnesian, numpy, pandas.
-        
-        ### Building
-        
-        Clone the repository:
-        
-        ```bash
-            git clone https://github.com/VicentePerezSoloviev/EDAspy.git
-            cd EDAspy
-            git checkout v1.1.2 # You can checkout a specific version if you want
-            python setup.py install
-        ```
-        ## Testing 
-        
-        The library contains tests that can be executed using `pytest <https://docs.pytest.org/>`_. Install it using 
-        pip:
-        
-        ```bash
-          pip install pytest
-        ```
-        
-        Run the tests with:
-        
-        ```bash
-          pytest
-        ```
-        
-        ## Bibliography
-        
-        [1] LarraÃ±aga, P., & Lozano, J. A. (Eds.). (2001). Estimation of distribution algorithms: A new tool for evolutionary computation (Vol. 2). Springer Science & Business Media.
-        
-        [2] MÃ¼hlenbein, H., & Paass, G. (1996). From recombination of genes to the estimation of distributions I. Binary parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 178-187). Springer Berlin Heidelberg.
-        
-        [3] MÃ¼hlenbein, H., Bendisch, J., & Voigt, H. M. (1996). From recombination of genes to the estimation of distributions II. Continuous parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 188-197). Springer Berlin Heidelberg.
-        
-        [4] Luo, N., & Qian, F. (2009, August). Evolutionary algorithm using kernel density estimation model in continuous domain. In 2009 7th Asian Control Conference (pp. 1526-1531). IEEE.
-        
-        [5] Larranaga, P. (2000). Optimization in continuous domains by learning and simulation of Gaussian networks. In Proc. of the 2000 Genetic and Evolutionary Computation Conference Workshop Program.
-        
-        [6] Soloviev, V. P., LarraÃ±aga, P., & Bielza, C. (2022). Estimation of distribution algorithms using Gaussian Bayesian networks to solve industrial optimization problems constrained by environment variables. Journal of Combinatorial Optimization, 44(2), 1077-1098.
-        
-        [7] Soloviev, Vicente P.& Bielza, Concha & LarraÃ±aga, Pedro (2023). Semiparametric Estimation of Distribution Algorithms for continuous optimization. IEEE Transactions on Evolutionary Computation.
-        
 Keywords: EDA,estimation,bayesian,evolutionary,algorithm,optimization,time_series,feature,selection,semiparametric,Gaussian
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: networkx
+Requires-Dist: pandas
+Requires-Dist: pgmpy
+Requires-Dist: pyarrow==9.0.0
+Requires-Dist: pybnesian==0.4.3
+Requires-Dist: scipy
+Requires-Dist: multiprocess
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+
+# <img src='https://raw.githubusercontent.com/VicentePerezSoloviev/EDAspy/master/Logo%20EDAspy.png' align="right" height="150"/>
+
+[![PyPI](https://img.shields.io/pypi/v/edaspy)](https://pypi.python.org/pypi/EDAspy/)
+[![PyPI license](https://img.shields.io/pypi/l/EDAspy.svg)](https://pypi.python.org/pypi/EDAspy/)
+[![Downloads](https://static.pepy.tech/badge/edaspy)](https://pepy.tech/project/edaspy)
+[![Documentation Status](https://readthedocs.org/projects/edaspy/badge/?version=latest)](https://edaspy.readthedocs.io/en/latest/?badge=latest)
+
+# EDAspy
+
+## Introduction
+
+EDAspy presents some implementations of the Estimation of Distribution Algorithms (EDAs) [1]. EDAs are a type of
+evolutionary algorithms. Depending on the type of the probabilistic model embedded in the EDA, and the type of
+variables considered, we will use a different EDA implementation.
+
+The pseudocode of EDAs is the following:
+
+1. Random initialization of the population.
+
+2. Evaluate each individual of the population.
+
+3. Select the top best individuals according to cost function evaluation.
+
+4. Learn a probabilistic model from the best individuals selected.
+
+5. Sampled another population.
+
+6. If stopping criteria is met, finish; else, go to 2.
+
+EDAspy allows to create a custom version of the EDA. Using the modular probabilistic models and the initializators, this can be embedded into the EDA baseline and used for different purposes. If this fits you, take a look on the examples section to the EDACustom example.
+
+EDAspy also incorporates a set of benchmarks in order to compare the algorithms trying to minimize these cost functions.
+
+The following implementations are available in EDAspy:
+
+* UMDAd: Univariate Marginal Distribution Algorithm binary [2]. It can be used as a simple example of EDA where the variables are binary and there are not dependencies between variables. Some usages include feature selection, for example.
+
+
+* UMDAc: Univariate Marginal Distribution Algorithm continuous [3]. In this EDA all the variables assume a Gaussian distribution and there are not dependencies considered between the variables. Some usages include hyperparameter optimization, for example.
+
+
+* UnivariateKEDA: Univariate Kernel Estimation of Distribution Algorithm [4]. Each variables distribution is estimated using Kernel Density Estimation.
+
+
+* UMDAcat: Univariate Marginal Distribution Algorithm categorical [2]. UMDA variant for categorical data, where more than two possible values per dimension are used (otherwise, use binary version).
+
+
+* EGNA: Estimation of Gaussian Distribution Algorithm [5][6]. This is a complex implementation in which dependencies between the variables are considered during the optimization. In each iteration, a Gaussian Bayesian network is learned and sampled. The variables in the model are assumed to be Gaussian and also de dependencies between them. This implementation is focused in continuous optimization.
+
+
+* EMNA: Estimation of Multivariate Normal Algorithm [1]. This is a similar implementation to EGNA, in which instead of using a Gaussian Bayesian network, a multivariate Gaussian distribution is iteratively learned and sampled. As in EGNA, the dependencies between variables are considered and assumed to be linear Gaussian. This implementation is focused in continuous optimization.
+
+
+* SPEDA: Semiparametric Estimation of Distribution Algorithm [7]. This multivariate EDA allows estimating the density of a variable using either KDE or Gaussians, and allow dependencies between both types of variables. It is an archive-based approach where the probabilistic model is updated given the best individuals of l previous generations.
+
+
+* MultivariateKEDA: Special case of SPEDA approach in which all nodes are restricted to be estimated using KDE (Gaussian nodes are forbidden) [7]. It is also an archive-based approach.
+
+
+* EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed.
+
+
+* BOA: Bayesian Optimization Algorithm [8]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where Bayesian Dirichlet score is used, in contrast to EBNA.
+
+
+* PBIL: Population-based incremental learning [9]. This version is a modification of UMDA strategy, where the mean of the Gaussian distribution is computed not only considering the best individuals, but also the worst one. 
+
+Some tools are also available in EDAspy such as the Bayesian network structure plotting, for visualizing the graph learnt in some of the implementations, if needed.
+
+
+Although some categorical EDAs are implemented, the package is focused in continuous optimization. Below, we show a CPU time analysis for the different approaches implemented for continuous optimization. Note that the CPU time can be reduced using parallelization (available as a parameter in the EDA initialization). Reference [7] shows a comparison about the performance of the algorithms in terms of cost function minimization. 
+
+<img src='cpu_comparison_continuous_opt.jpeg' alt="CPU time comparison for continuous optimization" title="CPU time comparison for continuous optimization"/>
+
+## Examples
+
+Some examples are available in https://github.com/VicentePerezSoloviev/EDAspy/tree/master/notebooks
+
+## Getting started
+
+For installing EDAspy from Pypi execute the following command using pip:
+
+```bash
+    pip install EDAspy
+```
+
+## Build from Source
+
+### Prerequisites
+
+- C++ 17 compatible compiler.
+- CMake (it is needed for pybnesian dependencies).
+- OpenCL 1.2 headers/library available.
+- Python >=3.8, <3.11
+- pgmpy, scipy, pyarrow, pybnesian, numpy, pandas, multiprocessing.
+
+### Installation
+We provide a detailed [installation guide](INSTALLATION.md) for EDAspy.
+
+## Testing 
+
+The library contains tests that can be executed using `pytest <https://docs.pytest.org/>`_. Install it using 
+pip:
+
+```bash
+  pip install pytest
+```
+
+Run the tests with:
+
+```bash
+  pytest
+```
+
+## Bibliography
+
+[1] LarraÃ±aga, P., & Lozano, J. A. (Eds.). (2001). Estimation of distribution algorithms: A new tool for evolutionary computation (Vol. 2). Springer Science & Business Media.
+
+[2] MÃ¼hlenbein, H., & Paass, G. (1996). From recombination of genes to the estimation of distributions I. Binary parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 178-187). Springer Berlin Heidelberg.
+
+[3] MÃ¼hlenbein, H., Bendisch, J., & Voigt, H. M. (1996). From recombination of genes to the estimation of distributions II. Continuous parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 188-197). Springer Berlin Heidelberg.
+
+[4] Luo, N., & Qian, F. (2009, August). Evolutionary algorithm using kernel density estimation model in continuous domain. In 2009 7th Asian Control Conference (pp. 1526-1531). IEEE.
+
+[5] Larranaga, P. (2000). Optimization in continuous domains by learning and simulation of Gaussian networks. In Proc. of the 2000 Genetic and Evolutionary Computation Conference Workshop Program.
+
+[6] Soloviev, V. P., LarraÃ±aga, P., & Bielza, C. (2022). Estimation of distribution algorithms using Gaussian Bayesian networks to solve industrial optimization problems constrained by environment variables. Journal of Combinatorial Optimization, 44(2), 1077-1098.
+
+[7] Soloviev, Vicente P.& Bielza, Concha & LarraÃ±aga, Pedro (2023). Semiparametric Estimation of Distribution Algorithms for continuous optimization. IEEE Transactions on Evolutionary Computation.
+
+[8] Martin Pelikan, David E. Goldberg, and Erick CantÃº-Paz (1999). BOA: the Bayesian optimization algorithm. In Proc. of the Genetic and Evolutionary Computation Congress (pp. 525â€“532).
+
+[9] Sebag, M., & Ducoulombier, A. (1998, September). Extending population-based incremental learning to continuous search spaces. In International Conference on Parallel Problem Solving from Nature (pp. 418-427). Springer.
```

### Comparing `EDAspy-1.1.3/LICENSE` & `edaspy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/PKG-INFO` & `edaspy-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,160 @@
 Metadata-Version: 2.1
 Name: EDAspy
-Version: 1.1.3
+Version: 1.1.4
 Summary: EDAspy is a Python package that implements Estimation of Distribution Algorithms. EDAspy allows toeither use already existing implementations or customize the EDAs baseline easily building it bymodules so new research can be easily developed. It also has several benchmarks for comparisons.
 Home-page: https://github.com/VicentePerezSoloviev/EDAspy
+Download-URL: https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.4.tar.gz
 Author: Vicente P. Soloviev
 Author-email: vicente.perez.soloviev@gmail.com
 License: MIT
-Download-URL: https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.2.tar.gz
-Description: # <img src='https://raw.githubusercontent.com/VicentePerezSoloviev/EDAspy/master/Logo%20EDAspy.png' align="right" height="150"/>
-        
-        [![PyPI](https://img.shields.io/pypi/v/edaspy)](https://pypi.python.org/pypi/EDAspy/)
-        [![PyPI license](https://img.shields.io/pypi/l/EDAspy.svg)](https://pypi.python.org/pypi/EDAspy/)
-        [![Downloads](https://static.pepy.tech/badge/edaspy)](https://pepy.tech/project/edaspy)
-        [![Documentation Status](https://readthedocs.org/projects/edaspy/badge/?version=latest)](https://edaspy.readthedocs.io/en/latest/?badge=latest)
-        
-        # EDAspy
-        
-        ## Introduction
-        
-        EDAspy presents some implementations of the Estimation of Distribution Algorithms (EDAs) [1]. EDAs are a type of
-        evolutionary algorithms. Depending on the type of the probabilistic model embedded in the EDA, and the type of
-        variables considered, we will use a different EDA implementation.
-        
-        The pseudocode of EDAs is the following:
-        
-        1. Random initialization of the population.
-        
-        2. Evaluate each individual of the population.
-        
-        3. Select the top best individuals according to cost function evaluation.
-        
-        4. Learn a probabilistic model from the best individuals selected.
-        
-        5. Sampled another population.
-        
-        6. If stopping criteria is met, finish; else, go to 2.
-        
-        EDAspy allows to create a custom version of the EDA. Using the modular probabilistic models and the initializators, this can be embedded into the EDA baseline and used for different purposes. If this fits you, take a look on the examples section to the EDACustom example.
-        
-        EDAspy also incorporates a set of benchmarks in order to compare the algorithms trying to minimize these cost functions.
-        
-        The following implementations are available in EDAspy:
-        
-        * UMDAd: Univariate Marginal Distribution Algorithm binary [2]. It can be used as a simple example of EDA where the variables are binary and there are not dependencies between variables. Some usages include feature selection, for example.
-        
-        
-        * UMDAc: Univariate Marginal Distribution Algorithm continuous [3]. In this EDA all the variables assume a Gaussian distribution and there are not dependencies considered between the variables. Some usages include hyperparameter optimization, for example.
-        
-        
-        * UnivariateKEDA: Univariate Kernel Estimation of Distribution Algorithm [4]. Each variables distribution is estimated using Kernel Density Estimation.
-        
-        
-        * UMDAcat: Univariate Marginal Distribution Algorithm categorical [2]. UMDA variant for categorical data, where more than two possible values per dimension are used (otherwise, use binary version).
-        
-        
-        * EGNA: Estimation of Gaussian Distribution Algorithm [5][6]. This is a complex implementation in which dependencies between the variables are considered during the optimization. In each iteration, a Gaussian Bayesian network is learned and sampled. The variables in the model are assumed to be Gaussian and also de dependencies between them. This implementation is focused in continuous optimization.
-        
-        
-        * EMNA: Estimation of Multivariate Normal Algorithm [1]. This is a similar implementation to EGNA, in which instead of using a Gaussian Bayesian network, a multivariate Gaussian distribution is iteratively learned and sampled. As in EGNA, the dependencies between variables are considered and assumed to be linear Gaussian. This implementation is focused in continuous optimization.
-        
-        
-        * SPEDA: Semiparametric Estimation of Distribution Algorithm [7]. This multivariate EDA allows estimating the density of a variable using either KDE or Gaussians, and allow dependencies between both types of variables. It is an archive-based approach where the probabilistic model is updated given the best individuals of l previous generations.
-        
-        
-        * MultivariateKEDA: Special case of SPEDA approach in which all nodes are restricted to be estimated using KDE (Gaussian nodes are forbidden) [7]. It is also an archive-based approach.
-        
-        
-        * EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed. 
-        
-        
-        Some tools are also available in EDAspy such as the Bayesian network structure plotting, for visualizing the graph learnt in some of the implementations, if needed.
-        
-        
-        Although some categorical EDAs are implemented, the package is focused in continuous optimization. Below, we show a CPU time analysis for the different approaches implemented for continuous optimization. Note that the CPU time can be reduced using parallelization (available as a parameter in the EDA initialization). Reference [7] shows a comparison about the performance of the algorithms in terms of cost function minimization. 
-        
-        <img src='cpu_comparison_continuous_opt.jpeg' alt="CPU time comparison for continuous optimization" title="CPU time comparison for continuous optimization"/>
-        
-        ## Examples
-        
-        Some examples are available in https://github.com/VicentePerezSoloviev/EDAspy/tree/master/notebooks
-        
-        ## Getting started
-        
-        For installing EDAspy from Pypi execute the following command using pip:
-        
-        ```bash
-            pip install EDAspy
-        ```
-        
-        ## Build from Source
-        
-        ### Prerequisites
-        
-        - Python >= 3.0
-        - Pybnesian, numpy, pandas.
-        
-        ### Building
-        
-        Clone the repository:
-        
-        ```bash
-            git clone https://github.com/VicentePerezSoloviev/EDAspy.git
-            cd EDAspy
-            git checkout v1.1.2 # You can checkout a specific version if you want
-            python setup.py install
-        ```
-        ## Testing 
-        
-        The library contains tests that can be executed using `pytest <https://docs.pytest.org/>`_. Install it using 
-        pip:
-        
-        ```bash
-          pip install pytest
-        ```
-        
-        Run the tests with:
-        
-        ```bash
-          pytest
-        ```
-        
-        ## Bibliography
-        
-        [1] LarraÃ±aga, P., & Lozano, J. A. (Eds.). (2001). Estimation of distribution algorithms: A new tool for evolutionary computation (Vol. 2). Springer Science & Business Media.
-        
-        [2] MÃ¼hlenbein, H., & Paass, G. (1996). From recombination of genes to the estimation of distributions I. Binary parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 178-187). Springer Berlin Heidelberg.
-        
-        [3] MÃ¼hlenbein, H., Bendisch, J., & Voigt, H. M. (1996). From recombination of genes to the estimation of distributions II. Continuous parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 188-197). Springer Berlin Heidelberg.
-        
-        [4] Luo, N., & Qian, F. (2009, August). Evolutionary algorithm using kernel density estimation model in continuous domain. In 2009 7th Asian Control Conference (pp. 1526-1531). IEEE.
-        
-        [5] Larranaga, P. (2000). Optimization in continuous domains by learning and simulation of Gaussian networks. In Proc. of the 2000 Genetic and Evolutionary Computation Conference Workshop Program.
-        
-        [6] Soloviev, V. P., LarraÃ±aga, P., & Bielza, C. (2022). Estimation of distribution algorithms using Gaussian Bayesian networks to solve industrial optimization problems constrained by environment variables. Journal of Combinatorial Optimization, 44(2), 1077-1098.
-        
-        [7] Soloviev, Vicente P.& Bielza, Concha & LarraÃ±aga, Pedro (2023). Semiparametric Estimation of Distribution Algorithms for continuous optimization. IEEE Transactions on Evolutionary Computation.
-        
 Keywords: EDA,estimation,bayesian,evolutionary,algorithm,optimization,time_series,feature,selection,semiparametric,Gaussian
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: networkx
+Requires-Dist: pandas
+Requires-Dist: pgmpy
+Requires-Dist: pyarrow==9.0.0
+Requires-Dist: pybnesian==0.4.3
+Requires-Dist: scipy
+Requires-Dist: multiprocess
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+
+# <img src='https://raw.githubusercontent.com/VicentePerezSoloviev/EDAspy/master/Logo%20EDAspy.png' align="right" height="150"/>
+
+[![PyPI](https://img.shields.io/pypi/v/edaspy)](https://pypi.python.org/pypi/EDAspy/)
+[![PyPI license](https://img.shields.io/pypi/l/EDAspy.svg)](https://pypi.python.org/pypi/EDAspy/)
+[![Downloads](https://static.pepy.tech/badge/edaspy)](https://pepy.tech/project/edaspy)
+[![Documentation Status](https://readthedocs.org/projects/edaspy/badge/?version=latest)](https://edaspy.readthedocs.io/en/latest/?badge=latest)
+
+# EDAspy
+
+## Introduction
+
+EDAspy presents some implementations of the Estimation of Distribution Algorithms (EDAs) [1]. EDAs are a type of
+evolutionary algorithms. Depending on the type of the probabilistic model embedded in the EDA, and the type of
+variables considered, we will use a different EDA implementation.
+
+The pseudocode of EDAs is the following:
+
+1. Random initialization of the population.
+
+2. Evaluate each individual of the population.
+
+3. Select the top best individuals according to cost function evaluation.
+
+4. Learn a probabilistic model from the best individuals selected.
+
+5. Sampled another population.
+
+6. If stopping criteria is met, finish; else, go to 2.
+
+EDAspy allows to create a custom version of the EDA. Using the modular probabilistic models and the initializators, this can be embedded into the EDA baseline and used for different purposes. If this fits you, take a look on the examples section to the EDACustom example.
+
+EDAspy also incorporates a set of benchmarks in order to compare the algorithms trying to minimize these cost functions.
+
+The following implementations are available in EDAspy:
+
+* UMDAd: Univariate Marginal Distribution Algorithm binary [2]. It can be used as a simple example of EDA where the variables are binary and there are not dependencies between variables. Some usages include feature selection, for example.
+
+
+* UMDAc: Univariate Marginal Distribution Algorithm continuous [3]. In this EDA all the variables assume a Gaussian distribution and there are not dependencies considered between the variables. Some usages include hyperparameter optimization, for example.
+
+
+* UnivariateKEDA: Univariate Kernel Estimation of Distribution Algorithm [4]. Each variables distribution is estimated using Kernel Density Estimation.
+
+
+* UMDAcat: Univariate Marginal Distribution Algorithm categorical [2]. UMDA variant for categorical data, where more than two possible values per dimension are used (otherwise, use binary version).
+
+
+* EGNA: Estimation of Gaussian Distribution Algorithm [5][6]. This is a complex implementation in which dependencies between the variables are considered during the optimization. In each iteration, a Gaussian Bayesian network is learned and sampled. The variables in the model are assumed to be Gaussian and also de dependencies between them. This implementation is focused in continuous optimization.
+
+
+* EMNA: Estimation of Multivariate Normal Algorithm [1]. This is a similar implementation to EGNA, in which instead of using a Gaussian Bayesian network, a multivariate Gaussian distribution is iteratively learned and sampled. As in EGNA, the dependencies between variables are considered and assumed to be linear Gaussian. This implementation is focused in continuous optimization.
+
+
+* SPEDA: Semiparametric Estimation of Distribution Algorithm [7]. This multivariate EDA allows estimating the density of a variable using either KDE or Gaussians, and allow dependencies between both types of variables. It is an archive-based approach where the probabilistic model is updated given the best individuals of l previous generations.
+
+
+* MultivariateKEDA: Special case of SPEDA approach in which all nodes are restricted to be estimated using KDE (Gaussian nodes are forbidden) [7]. It is also an archive-based approach.
+
+
+* EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed.
+
+
+* BOA: Bayesian Optimization Algorithm [8]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where Bayesian Dirichlet score is used, in contrast to EBNA.
+
+
+* PBIL: Population-based incremental learning [9]. This version is a modification of UMDA strategy, where the mean of the Gaussian distribution is computed not only considering the best individuals, but also the worst one. 
+
+Some tools are also available in EDAspy such as the Bayesian network structure plotting, for visualizing the graph learnt in some of the implementations, if needed.
+
+
+Although some categorical EDAs are implemented, the package is focused in continuous optimization. Below, we show a CPU time analysis for the different approaches implemented for continuous optimization. Note that the CPU time can be reduced using parallelization (available as a parameter in the EDA initialization). Reference [7] shows a comparison about the performance of the algorithms in terms of cost function minimization. 
+
+<img src='cpu_comparison_continuous_opt.jpeg' alt="CPU time comparison for continuous optimization" title="CPU time comparison for continuous optimization"/>
+
+## Examples
+
+Some examples are available in https://github.com/VicentePerezSoloviev/EDAspy/tree/master/notebooks
+
+## Getting started
+
+For installing EDAspy from Pypi execute the following command using pip:
+
+```bash
+    pip install EDAspy
+```
+
+## Build from Source
+
+### Prerequisites
+
+- C++ 17 compatible compiler.
+- CMake (it is needed for pybnesian dependencies).
+- OpenCL 1.2 headers/library available.
+- Python >=3.8, <3.11
+- pgmpy, scipy, pyarrow, pybnesian, numpy, pandas, multiprocessing.
+
+### Installation
+We provide a detailed [installation guide](INSTALLATION.md) for EDAspy.
+
+## Testing 
+
+The library contains tests that can be executed using `pytest <https://docs.pytest.org/>`_. Install it using 
+pip:
+
+```bash
+  pip install pytest
+```
+
+Run the tests with:
+
+```bash
+  pytest
+```
+
+## Bibliography
+
+[1] LarraÃ±aga, P., & Lozano, J. A. (Eds.). (2001). Estimation of distribution algorithms: A new tool for evolutionary computation (Vol. 2). Springer Science & Business Media.
+
+[2] MÃ¼hlenbein, H., & Paass, G. (1996). From recombination of genes to the estimation of distributions I. Binary parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 178-187). Springer Berlin Heidelberg.
+
+[3] MÃ¼hlenbein, H., Bendisch, J., & Voigt, H. M. (1996). From recombination of genes to the estimation of distributions II. Continuous parameters. In Parallel Problem Solving from Natureâ€”PPSN IV: International Conference on Evolutionary Computationâ€”The 4th International Conference on Parallel Problem Solving from Nature Berlin, Germany, September 22â€“26, 1996 Proceedings 4 (pp. 188-197). Springer Berlin Heidelberg.
+
+[4] Luo, N., & Qian, F. (2009, August). Evolutionary algorithm using kernel density estimation model in continuous domain. In 2009 7th Asian Control Conference (pp. 1526-1531). IEEE.
+
+[5] Larranaga, P. (2000). Optimization in continuous domains by learning and simulation of Gaussian networks. In Proc. of the 2000 Genetic and Evolutionary Computation Conference Workshop Program.
+
+[6] Soloviev, V. P., LarraÃ±aga, P., & Bielza, C. (2022). Estimation of distribution algorithms using Gaussian Bayesian networks to solve industrial optimization problems constrained by environment variables. Journal of Combinatorial Optimization, 44(2), 1077-1098.
+
+[7] Soloviev, Vicente P.& Bielza, Concha & LarraÃ±aga, Pedro (2023). Semiparametric Estimation of Distribution Algorithms for continuous optimization. IEEE Transactions on Evolutionary Computation.
+
+[8] Martin Pelikan, David E. Goldberg, and Erick CantÃº-Paz (1999). BOA: the Bayesian optimization algorithm. In Proc. of the Genetic and Evolutionary Computation Congress (pp. 525â€“532).
+
+[9] Sebag, M., & Ducoulombier, A. (1998, September). Extending population-based incremental learning to continuous search spaces. In International Conference on Parallel Problem Solving from Nature (pp. 418-427). Springer.
```

### Comparing `EDAspy-1.1.3/README.md` & `edaspy-1.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -53,17 +53,22 @@
 
 * SPEDA: Semiparametric Estimation of Distribution Algorithm [7]. This multivariate EDA allows estimating the density of a variable using either KDE or Gaussians, and allow dependencies between both types of variables. It is an archive-based approach where the probabilistic model is updated given the best individuals of l previous generations.
 
 
 * MultivariateKEDA: Special case of SPEDA approach in which all nodes are restricted to be estimated using KDE (Gaussian nodes are forbidden) [7]. It is also an archive-based approach.
 
 
-* EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed. 
+* EBNA: Estimation of Bayesian Network Algorithm [1]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where conditional dependencies between variables can be analyzed.
 
 
+* BOA: Bayesian Optimization Algorithm [8]. This version of EDAs is used for categorical data. The probabilistic model used is a Categorical Bayesian network, where Bayesian Dirichlet score is used, in contrast to EBNA.
+
+
+* PBIL: Population-based incremental learning [9]. This version is a modification of UMDA strategy, where the mean of the Gaussian distribution is computed not only considering the best individuals, but also the worst one. 
+
 Some tools are also available in EDAspy such as the Bayesian network structure plotting, for visualizing the graph learnt in some of the implementations, if needed.
 
 
 Although some categorical EDAs are implemented, the package is focused in continuous optimization. Below, we show a CPU time analysis for the different approaches implemented for continuous optimization. Note that the CPU time can be reduced using parallelization (available as a parameter in the EDA initialization). Reference [7] shows a comparison about the performance of the algorithms in terms of cost function minimization. 
 
 <img src='cpu_comparison_continuous_opt.jpeg' alt="CPU time comparison for continuous optimization" title="CPU time comparison for continuous optimization"/>
 
@@ -79,27 +84,23 @@
     pip install EDAspy
 ```
 
 ## Build from Source
 
 ### Prerequisites
 
-- Python >= 3.0
-- Pybnesian, numpy, pandas.
-
-### Building
+- C++ 17 compatible compiler.
+- CMake (it is needed for pybnesian dependencies).
+- OpenCL 1.2 headers/library available.
+- Python >=3.8, <3.11
+- pgmpy, scipy, pyarrow, pybnesian, numpy, pandas, multiprocessing.
 
-Clone the repository:
+### Installation
+We provide a detailed [installation guide](INSTALLATION.md) for EDAspy.
 
-```bash
-    git clone https://github.com/VicentePerezSoloviev/EDAspy.git
-    cd EDAspy
-    git checkout v1.1.2 # You can checkout a specific version if you want
-    python setup.py install
-```
 ## Testing 
 
 The library contains tests that can be executed using `pytest <https://docs.pytest.org/>`_. Install it using 
 pip:
 
 ```bash
   pip install pytest
@@ -122,7 +123,11 @@
 [4] Luo, N., & Qian, F. (2009, August). Evolutionary algorithm using kernel density estimation model in continuous domain. In 2009 7th Asian Control Conference (pp. 1526-1531). IEEE.
 
 [5] Larranaga, P. (2000). Optimization in continuous domains by learning and simulation of Gaussian networks. In Proc. of the 2000 Genetic and Evolutionary Computation Conference Workshop Program.
 
 [6] Soloviev, V. P., Larrañaga, P., & Bielza, C. (2022). Estimation of distribution algorithms using Gaussian Bayesian networks to solve industrial optimization problems constrained by environment variables. Journal of Combinatorial Optimization, 44(2), 1077-1098.
 
 [7] Soloviev, Vicente P.& Bielza, Concha & Larrañaga, Pedro (2023). Semiparametric Estimation of Distribution Algorithms for continuous optimization. IEEE Transactions on Evolutionary Computation.
+
+[8] Martin Pelikan, David E. Goldberg, and Erick Cantú-Paz (1999). BOA: the Bayesian optimization algorithm. In Proc. of the Genetic and Evolutionary Computation Congress (pp. 525–532).
+
+[9] Sebag, M., & Ducoulombier, A. (1998, September). Extending population-based incremental learning to continuous search spaces. In International Conference on Parallel Problem Solving from Nature (pp. 418-427). Springer.
```

### Comparing `EDAspy-1.1.3/setup.py` & `edaspy-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = '1.1.3'  # also defined in EDAspy/__init__.py and in conf.py (docs)
+__version__ = '1.1.4'  # also defined in EDAspy/__init__.py and in conf.py (docs)
 
 setuptools.setup(
     name="EDAspy",
     version=__version__,
     author="Vicente P. Soloviev",
     author_email="vicente.perez.soloviev@gmail.com",
     description="EDAspy is a Python package that implements Estimation of Distribution Algorithms. EDAspy allows to"
                 "either use already existing implementations or customize the EDAs baseline easily building it by"
                 "modules so new research can be easily developed. It also has several benchmarks for comparisons.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    download_url="https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.2.tar.gz",
+    download_url="https://github.com/VicentePerezSoloviev/EDAspy/archive/1.1.4.tar.gz",
     url="https://github.com/VicentePerezSoloviev/EDAspy",
     packages=setuptools.find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=['EDA', 'estimation', 'bayesian', 'evolutionary', 'algorithm', 'optimization', 'time_series', 'feature',
               'selection', 'semiparametric', 'Gaussian'],
-    python_requires='>=3.8',
+    python_requires='>=3.8, <3.11',
+    setup_requires=["networkx", "pandas", "pgmpy", "pyarrow==9.0.0", "pybnesian==0.4.3", "scipy", "multiprocess",
+                    "matplotlib", "numpy"],
+    install_requires=["networkx", "pandas", "pgmpy", "pyarrow==9.0.0", "pybnesian==0.4.3", "scipy", "multiprocess",
+                      "matplotlib", "numpy"],
     license="MIT",
     include_package_data=True,
     package_data={'': ['benchmarks/input_data/*.txt']}
 )
```

### Comparing `EDAspy-1.1.3/tests/edas_multivariate/test_ebna.py` & `edaspy-1.1.4/tests/edas_multivariate/test_ebna.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_multivariate/test_egna.py` & `edaspy-1.1.4/tests/edas_multivariate/test_egna.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_multivariate/test_emna.py` & `edaspy-1.1.4/tests/edas_multivariate/test_emna.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_multivariate/test_multivariate_keda.py` & `edaspy-1.1.4/tests/edas_multivariate/test_multivariate_keda.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_multivariate/test_speda.py` & `edaspy-1.1.4/tests/edas_multivariate/test_speda.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_univariate/test_umdac.py` & `edaspy-1.1.4/tests/edas_univariate/test_umdac.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_univariate/test_umdacat.py` & `edaspy-1.1.4/tests/edas_univariate/test_umdacat.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_univariate/test_umdad.py` & `edaspy-1.1.4/tests/edas_univariate/test_umdad.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/edas_univariate/test_univariate_keda.py` & `edaspy-1.1.4/tests/edas_univariate/test_univariate_keda.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/inits/test_geninit.py` & `edaspy-1.1.4/tests/inits/test_geninit.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/pms/test_discrete_bn.py` & `edaspy-1.1.4/tests/pms/test_discrete_bn.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 
 
 class TestBN(TestCase):
 
     np.random.seed(42)
 
-    def test_sample(self):
+    def test_sample_bic(self):
         """
         Test if the samplings order is the same as the input used.
         """
         variables = ['A', 'B', 'C']
         possible_values = np.array([
             ['q', 'w', 'e'],
             ['a', 's', 'd', 'f'],
@@ -24,15 +24,46 @@
             [.4, .6]], dtype=object
         )
 
         init = CategoricalSampling(n_variables=len(variables), possible_values=possible_values, frequency=frequency)
         data = init.sample(100)
 
         bn = BN(variables=variables)
-        bn.learn(data)
+        bn.learn(data, score="bicscore")
+
+        samples = bn.sample(100)
+
+        for i in range(len(variables)):
+            # check if unique values are the same
+            assert len(set(possible_values[i]) - set(samples[:, i])) + \
+                   len(set(samples[:, i]) - set(possible_values[i])) == 0, "Unique values and possible " \
+                                                                           "values do not match"
+
+    def test_sample_bdeu(self):
+        """
+        Test if the samplings order is the same as the input used.
+        """
+        variables = ['A', 'B', 'C']
+        possible_values = np.array([
+            ['q', 'w', 'e'],
+            ['a', 's', 'd', 'f'],
+            ['b', 'v']], dtype=object
+        )
+
+        frequency = np.array([
+            [.25, .5, .25],
+            [.25, .25, .25, .25],
+            [.4, .6]], dtype=object
+        )
+
+        init = CategoricalSampling(n_variables=len(variables), possible_values=possible_values, frequency=frequency)
+        data = init.sample(100)
+
+        bn = BN(variables=variables)
+        bn.learn(data, score="bdeuscore")
 
         samples = bn.sample(100)
 
         for i in range(len(variables)):
             # check if unique values are the same
             assert len(set(possible_values[i]) - set(samples[:, i])) + \
                    len(set(samples[:, i]) - set(possible_values[i])) == 0, "Unique values and possible " \
@@ -42,21 +73,21 @@
         """
         Test if the samplings size is the expected.
         """
         variables = ['A', 'B', 'C']
         possible_values = np.array([
             ['q', 'w', 'e'],
             ['a', 's', 'd', 'f'],
-            ['b', 'v']]
+            ['b', 'v']], dtype=object
         )
 
         frequency = np.array([
             [0.2, 0.5, 0.3],
             [.25, .25, .25, .25],
-            [.1, .9]]
+            [.1, .9]], dtype=object
         )
 
         n_rows = 100
 
         init = CategoricalSampling(n_variables=len(variables), possible_values=possible_values, frequency=frequency)
         data = init.sample(n_rows)
```

### Comparing `EDAspy-1.1.3/tests/pms/test_gbn.py` & `edaspy-1.1.4/tests/pms/test_gbn.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,7 +69,30 @@
         white_list = [('1', '2'), ('4', '5'), ('29', '15'), ('16', '7')]
 
         gbn = GBN(var_names + ['pre1', 'pre2'], black_list=black_list, white_list=white_list)
         gbn.learn(data)
 
         assert all(elem in gbn.print_structure() for elem in white_list)
         assert not all(elem in gbn.print_structure() for elem in black_list)
+
+    def test_map(self):
+        """
+        Test if the MAP output matches the results from the ranges of the variables
+        """
+
+        n_rows, n_vars = 10, 3
+        var_names = ['A', 'B', 'C']
+
+        data = pd.DataFrame(np.random.random((n_rows, n_vars)), columns=var_names)
+        data['A'] *= 10
+        data['A'] = abs(data['A'])
+        data['B'] *= 100
+        data['B'] = abs(data['B'])
+        data['C'] *= 1000
+        data['C'] = abs(data['C'])
+
+        gbn = GBN(var_names)
+        gbn.learn(data)
+
+        print(gbn.maximum_a_posteriori([8, 108], ["A", "B"]))
+
+        print(gbn.maximum_a_posteriori([8, 1100], ["A", "C"]))
```

### Comparing `EDAspy-1.1.3/tests/pms/test_kdebn.py` & `edaspy-1.1.4/tests/pms/test_kdebn.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/pms/test_spbn.py` & `edaspy-1.1.4/tests/pms/test_spbn.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/pms/test_uni_bin_pm.py` & `edaspy-1.1.4/tests/pms/test_uni_bin_pm.py`

 * *Files identical despite different names*

### Comparing `EDAspy-1.1.3/tests/pms/test_uni_cat_pm.py` & `edaspy-1.1.4/tests/pms/test_uni_cat_pm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 class TestUniCategoricalPM(TestCase):
 
     def test_print_structure_uni_gauss(self):
         variables = ['A', 'B', 'C']
         possible_values = np.array([
             ['q', 'w', 'e'],
             ['a', 's', 'd', 'f'],
-            ['b', 'v']]
+            ['b', 'v']], dtype=object
         )
 
         frequency = np.array([
             [0.2, 0.5, 0.3],
             [.25, .25, .25, .25],
-            [.1, .9]]
+            [.1, .9]], dtype=object
         )
 
         n_rows = 100
 
         init = CategoricalSampling(n_variables=len(variables), possible_values=possible_values, frequency=frequency)
         data = init.sample(n_rows)
 
@@ -34,21 +34,21 @@
         """
         Test if the samplings size is the expected.
         """
         variables = ['A', 'B', 'C']
         possible_values = np.array([
             ['q', 'w', 'e'],
             ['a', 's', 'd', 'f'],
-            ['b', 'v']]
+            ['b', 'v']], dtype=object
         )
 
         frequency = np.array([
             [0.2, 0.5, 0.3],
             [.25, .25, .25, .25],
-            [.1, .9]]
+            [.1, .9]], dtype=object
         )
 
         n_rows = 100
 
         init = CategoricalSampling(n_variables=len(variables), possible_values=possible_values, frequency=frequency)
         data = init.sample(n_rows)
```

### Comparing `EDAspy-1.1.3/tests/pms/test_uni_gauss_pm.py` & `edaspy-1.1.4/tests/pms/test_uni_gauss_pm.py`

 * *Files identical despite different names*

