# Comparing `tmp/feeed-1.1.0.tar.gz` & `tmp/feeed-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeed-1.1.0.tar", last modified: Wed Jan 24 08:44:35 2024, max compression
+gzip compressed data, was "feeed-1.2.0.tar", last modified: Mon Apr 15 22:03:19 2024, max compression
```

## Comparing `feeed-1.1.0.tar` & `feeed-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 andreamaldonado   (501) staff       (20)        0 2024-01-24 08:44:35.387179 feeed-1.1.0/
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     1093 2023-08-31 15:22:26.000000 feeed-1.1.0/LICENSE
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      639 2024-01-24 08:44:35.386615 feeed-1.1.0/PKG-INFO
--rw-r--r--   0 andreamaldonado   (501) staff       (20)    20941 2024-01-24 08:29:49.000000 feeed-1.1.0/README.md
-drwxr-xr-x   0 andreamaldonado   (501) staff       (20)        0 2024-01-24 08:44:35.381713 feeed-1.1.0/feeed/
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      207 2023-08-31 15:22:26.000000 feeed-1.1.0/feeed/__init__.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     2492 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/activities.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)    16206 2024-01-23 21:22:13.000000 feeed-1.1.0/feeed/complexity.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     3551 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/end_activities.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     2702 2024-01-24 08:29:49.000000 feeed-1.1.0/feeed/entropies.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      424 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/feature.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     4567 2024-01-24 08:29:49.000000 feeed-1.1.0/feeed/feature_extractor.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      883 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/simple_stats.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     3535 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/start_activities.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     5963 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/time.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     5386 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/trace_length.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     2715 2024-01-23 19:49:55.000000 feeed-1.1.0/feeed/trace_variant.py
-drwxr-xr-x   0 andreamaldonado   (501) staff       (20)        0 2024-01-24 08:44:35.385131 feeed-1.1.0/feeed/utils/
--rw-r--r--   0 andreamaldonado   (501) staff       (20)        0 2023-08-31 15:22:26.000000 feeed-1.1.0/feeed/utils/__init__.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      171 2023-08-31 15:22:26.000000 feeed-1.1.0/feeed/utils/feature_names.py
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      285 2023-08-31 15:22:26.000000 feeed-1.1.0/feeed/utils/sort_alphanumeric.py
-drwxr-xr-x   0 andreamaldonado   (501) staff       (20)        0 2024-01-24 08:44:35.386110 feeed-1.1.0/feeed.egg-info/
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      639 2024-01-24 08:44:35.000000 feeed-1.1.0/feeed.egg-info/PKG-INFO
--rw-r--r--   0 andreamaldonado   (501) staff       (20)      508 2024-01-24 08:44:35.000000 feeed-1.1.0/feeed.egg-info/SOURCES.txt
--rw-r--r--   0 andreamaldonado   (501) staff       (20)        1 2024-01-24 08:44:35.000000 feeed-1.1.0/feeed.egg-info/dependency_links.txt
--rw-r--r--   0 andreamaldonado   (501) staff       (20)       54 2024-01-24 08:44:35.000000 feeed-1.1.0/feeed.egg-info/requires.txt
--rw-r--r--   0 andreamaldonado   (501) staff       (20)        6 2024-01-24 08:44:35.000000 feeed-1.1.0/feeed.egg-info/top_level.txt
--rw-r--r--   0 andreamaldonado   (501) staff       (20)       38 2024-01-24 08:44:35.387317 feeed-1.1.0/setup.cfg
--rw-r--r--   0 andreamaldonado   (501) staff       (20)     1041 2024-01-24 08:34:04.000000 feeed-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:03:19.258611 feeed-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 22:03:17.000000 feeed-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-15 22:03:19.254611 feeed-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23879 2024-04-15 22:03:17.000000 feeed-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:03:19.254611 feeed-1.2.0/feeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/end_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/epa_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/eventropies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/simple_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/start_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/trace_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/trace_variant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:03:19.254611 feeed-1.2.0/feeed/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/utils/feature_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-15 22:03:17.000000 feeed-1.2.0/feeed/utils/sort_alphanumeric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:03:19.254611 feeed-1.2.0/feeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-15 22:03:19.000000 feeed-1.2.0/feeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 22:03:19.000000 feeed-1.2.0/feeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:03:19.000000 feeed-1.2.0/feeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 22:03:19.000000 feeed-1.2.0/feeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 22:03:19.000000 feeed-1.2.0/feeed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 22:03:19.258611 feeed-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 22:03:18.000000 feeed-1.2.0/setup.py
```

### Comparing `feeed-1.1.0/LICENSE` & `feeed-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/README.md` & `feeed-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 To directly use meta feature extraction methods via `import`
 ```shell
 pip install feeed
 ```
 Run:
 ```shell
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/Sepsis.xes'))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/Sepsis.xes'))"
 ```
 
 ## Usage
 Output data contains at least one feature with a `feature_name` and a corresponding value obtained by that feature's specific computation. The schema looks like this:
 ```python
 {
 'log': 'Sepsis'
@@ -34,67 +34,71 @@
 }
 ```
 Every `feature_name` belongs to a `feature_type`, and a `feature_type` can comprise multiple features. The following Feature Types table presents the correspondence between `feature_type` and `feature_name`. 
 
 ### Feature types
 Specific `feature_name`s and `feature_type`s can be selected as in the examples below:
 
-| Feature Type     | Feature Names                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| Feature Type     | Feature Names                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 |------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | simple_stats     | n_traces, n_unique_traces, ratio_unique_traces_per_trace                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | trace_length     | trace_len_min, trace_len_max, trace_len_mean, trace_len_median, trace_len_mode, trace_len_std, trace_len_variance, trace_len_q1, trace_len_q3, trace_len_iqr, trace_len_geometric_mean, trace_len_geometric_std, trace_len_harmonic_mean, trace_len_skewness, trace_len_kurtosis, trace_len_coefficient_variation, trace_len_entropy, trace_len_hist1, trace_len_hist2, trace_len_hist3, trace_len_hist4, trace_len_hist5, trace_len_hist6, trace_len_hist7, trace_len_hist8, trace_len_hist9, trace_len_hist10, trace_len_skewness_hist, trace_len_kurtosis_hist |
 | trace_variant    | ratio_most_common_variant, ratio_top_1_variants, ratio_top_5_variants, ratio_top_10_variants, ratio_top_20_variants, ratio_top_50_variants, ratio_top_75_variants, mean_variant_occurrence, std_variant_occurrence, skewness_variant_occurrence, kurtosis_variant_occurrence                                                                                                                                                                                                                                                                                      |
 | activities       | n_unique_activities, activities_min, activities_max, activities_mean, activities_median, activities_std, activities_variance, activities_q1, activities_q3, activities_iqr, activities_skewness, activities_kurtosis                                                                                                                                                                                                                                                                                                                                              |
 | start_activities | n_unique_start_activities, start_activities_min, start_activities_max, start_activities_mean, start_activities_median, start_activities_std, start_activities_variance, start_activities_q1, start_activities_q3, start_activities_iqr, start_activities_skewness, start_activities_kurtosis                                                                                                                                                                                                                                                                      |
 | end_activities   | n_unique_end_activities, end_activities_min, end_activities_max, end_activities_mean, end_activities_median, end_activities_std, end_activities_variance, end_activities_q1, end_activities_q3, end_activities_iqr, end_activities_skewness, end_activities_kurtosis                                                                                                                                                                                                                                                                                              |
-| entropies        | entropy_trace, entropy_prefix, entropy_global_block, entropy_lempel_ziv, entropy_k_block_diff_1, entropy_k_block_diff_3, entropy_k_block_diff_5, entropy_k_block_ratio_1, entropy_k_block_ratio_3, entropy_k_block_ratio_5, entropy_knn_3, entropy_knn_5, entropy_knn_7                                                                                                                                                                                                                                                                                           |
-| complexity       | variant_entropy, normalized_variant_entropy, sequence_entropy, normalized_sequence_entropy, sequence_entropy_linear_forgetting, normalized_sequence_entropy_linear_forgetting, sequence_entropy_exponential_forgetting, normalized_sequence_entropy_exponential_forgetting
-| time_based       | accumulated_time, execution_time, remaining_time, waiting_time (with each: min, max, mean, median, mode, std, variance, q1, q3, iqr, geometric_mean, geometric_std, harmonic_mean, skewness, kurtosis, coefficient_variation, entropy, skewness_hist, kurtosis_hist resulting in e.g. accumulated_time_min)|
+| eventropies[[4]](#references)   | eventropy_trace, eventropy_prefix, eventropy_prefix_flattened, eventropy_global_block, eventropy_global_block_flattened, eventropy_lempel_ziv, eventropy_lempel_ziv_flattened, eventropy_k_block_diff_1, eventropy_k_block_diff_3, eventropy_k_block_diff_5, eventropy_k_block_ratio_1, eventropy_k_block_ratio_3, eventropy_k_block_ratio_5, eventropy_knn_3, eventropy_knn_5, eventropy_knn_7                                                                                                                                                                 |
+| epa_based[[5]](#references)       | epa_variant_entropy, epa_normalized_variant_entropy, epa_sequence_entropy, epa_normalized_sequence_entropy, epa_sequence_entropy_linear_forgetting, epa_normalized_sequence_entropy_linear_forgetting, epa_sequence_entropy_exponential_forgetting, epa_normalized_sequence_entropy_exponential_forgetting
+| time_based       | accumulated_time, execution_time, remaining_time, within_day (with each: min, max, mean, median, mode, std, variance, q1, q3, iqr, geometric_mean, geometric_std, harmonic_mean, skewness, kurtosis, coefficient_variation, entropy, skewness_hist, kurtosis_hist resulting in e.g. accumulated_time_min)|
 
 ### Examples
 For the following examples we used Sepsis event data[1].
 #### Example 1:
 Passing sublist of feature_names, e.g. ['start_activities_min', 'end_activities_max'], to get a list of values for those features only.
 ```shell
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/Sepsis.xes',  ['start_activities_min', 'end_activities_max']))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/Sepsis.xes',  ['start_activities_min', 'end_activities_max']))"
 ```
 outputs
 ```python
 SUCCESSFULLY: 2 features for SEPSIS.xes took 0:00:00.342855 sec.
 {'log': 'SEPSIS', 'start_activities_min': 6, 'end_activities_max': 393}
 ```
 
 #### Example 2:
 Passing sublist of feature_types, e.g. ['start_activities'], to get a list of values for the feature type 'start_activities' only
 ```shell
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/Sepsis.xes',  ['start_activities']))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/Sepsis.xes',  ['start_activities']))"
 ```
 outputs
 ```python
 SUCCESSFULLY: 12 features for Sepsis.xes took 0:00:01.946063 sec.
 {'log': 'Sepsis', 'n_unique_start_activities': 6, 'start_activities_iqr': 9.25, 'start_activities_kurtosis': 1.199106773708694, 'start_activities_max': 995, 'start_activities_mean': 175.0, 'start_activities_median': 12.0, 'start_activities_min': 6, 'start_activities_q1': 7.75, 'start_activities_q3': 17.0, 'start_activities_skewness': 1.7883562472303318, 'start_activities_std': 366.73787187399483, 'start_activities_variance': 134496.66666666666}
 ```
 
 #### Example 3:
 By not passing any list of feature_types to get the full list of all feature values for all feature_types,
 from the shell
 ```shell
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/Sepsis.xes'))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/Sepsis.xes'))"
+```
+For the order of feature_names as in [Feature Type table](#feature-types):
+```python
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/Sepsis.xes', ['n_traces', 'n_unique_traces', 'ratio_unique_traces_per_trace', 'trace_len_min', 'trace_len_max', 'trace_len_mean', 'trace_len_median', 'trace_len_mode', 'trace_len_std', 'trace_len_variance', 'trace_len_q1', 'trace_len_q3', 'trace_len_iqr', 'trace_len_geometric_mean', 'trace_len_geometric_std', 'trace_len_harmonic_mean', 'trace_len_skewness', 'trace_len_kurtosis', 'trace_len_coefficient_variation', 'trace_len_entropy', 'trace_len_hist1', 'trace_len_hist2', 'trace_len_hist3', 'trace_len_hist4', 'trace_len_hist5', 'trace_len_hist6', 'trace_len_hist7', 'trace_len_hist8', 'trace_len_hist9', 'trace_len_hist10', 'trace_len_skewness_hist', 'trace_len_kurtosis_hist', 'ratio_most_common_variant', 'ratio_top_1_variants', 'ratio_top_5_variants', 'ratio_top_10_variants', 'ratio_top_20_variants', 'ratio_top_50_variants', 'ratio_top_75_variants', 'mean_variant_occurrence', 'std_variant_occurrence', 'skewness_variant_occurrence', 'kurtosis_variant_occurrence', 'n_unique_activities', 'activities_min', 'activities_max', 'activities_mean', 'activities_median', 'activities_std', 'activities_variance', 'activities_q1', 'activities_q3', 'activities_iqr', 'activities_skewness', 'activities_kurtosis', 'n_unique_start_activities', 'start_activities_min', 'start_activities_max', 'start_activities_mean', 'start_activities_median', 'start_activities_std', 'start_activities_variance', 'start_activities_q1', 'start_activities_q3', 'start_activities_iqr', 'start_activities_skewness', 'start_activities_kurtosis', 'n_unique_end_activities', 'end_activities_min', 'end_activities_max', 'end_activities_mean', 'end_activities_median', 'end_activities_std', 'end_activities_variance', 'end_activities_q1', 'end_activities_q3', 'end_activities_iqr', 'end_activities_skewness', 'end_activities_kurtosis', 'eventropy_trace', 'eventropy_prefix', 'eventropy_global_block', 'eventropy_lempel_ziv', 'eventropy_k_block_diff_1', 'eventropy_k_block_diff_3', 'eventropy_k_block_diff_5', 'eventropy_k_block_ratio_1', 'eventropy_k_block_ratio_3', 'eventropy_k_block_ratio_5', 'eventropy_knn_3', 'eventropy_knn_5', 'eventropy_knn_7', 'epa_variant_entropy', 'epa_normalized_variant_entropy', 'epa_sequence_entropy', 'epa_normalized_sequence_entropy', 'epa_sequence_entropy_linear_forgetting', 'epa_normalized_sequence_entropy_linear_forgetting', 'epa_sequence_entropy_exponential_forgetting', 'epa_normalized_sequence_entropy_exponential_forgetting', 'accumulated_time', 'execution_time', 'remaining_time', 'within_day']))"
 ```
 or in a python script
 ```python
 from feeed.feature_extractor import extract_features
 
-features = extract_features("test_logs/Sepsis.xes")
+features = extract_features("test_data/Sepsis.xes")
 
 ```
 outputs
 ```python
-SUCCESSFULLY: 176 features for SEPSIS.xes took 0:00:32.267865 sec.
-{'log': 'SEPSIS', 'n_traces': 1050, 'n_unique_traces': 846, 'ratio_unique_traces_per_trace': 0.8057142857142857, 'trace_len_coefficient_variation': 0.7916391922924689, 'trace_len_entropy': 6.769403523350811, 'trace_len_geometric_mean': 12.281860759040903, 'trace_len_geometric_std': 1.7464004837799154, 'trace_len_harmonic_mean': 10.47731701485374, 'trace_len_hist1': 0.048613291470434326, 'trace_len_hist10': 0.00010465724751439027, 'trace_len_hist2': 0.005285190999476714, 'trace_len_hist3': 0.0005756148613291472, 'trace_len_hist4': 0.0002093144950287807, 'trace_len_hist5': 0.00010465724751439036, 'trace_len_hist6': 0.0, 'trace_len_hist7': 5.232862375719522e-05, 'trace_len_hist8': 0.0, 'trace_len_hist9': 0.0, 'trace_len_iqr': 7.0, 'trace_len_kurtosis': 87.0376906898399, 'trace_len_kurtosis_hist': 4.931206347805768, 'trace_len_max': 185, 'trace_len_mean': 14.48952380952381, 'trace_len_median': 13.0, 'trace_len_min': 3, 'trace_len_mode': 8, 'trace_len_q1': 9.0, 'trace_len_q3': 16.0, 'trace_len_skewness': 7.250526815880918, 'trace_len_skewness_hist': 2.6128507781562513, 'trace_len_std': 11.470474925273926, 'trace_len_variance': 131.57179501133788, 'kurtosis_variant_occurrence': 217.44268017168216, 'mean_variant_occurrence': 1.2411347517730495, 'ratio_most_common_variant': 0.03333333333333333, 'ratio_top_10_variants': 0.2742857142857143, 'ratio_top_1_variants': 0.12, 'ratio_top_20_variants': 0.35523809523809524, 'ratio_top_50_variants': 0.5971428571428572, 'ratio_top_5_variants': 0.21523809523809523, 'ratio_top_75_variants': 0.7980952380952381, 'skewness_variant_occurrence': 13.637101374069475, 'std_variant_occurrence': 1.7594085182491936, 'activities_iqr': 983.5, 'activities_kurtosis': 1.05777753209275, 'activities_max': 3383, 'activities_mean': 950.875, 'activities_median': 788.0, 'activities_min': 6, 'activities_q1': 101.75, 'activities_q3': 1085.25, 'activities_skewness': 1.3912385607018212, 'activities_std': 1008.5815457239935, 'activities_variance': 1017236.734375, 'n_unique_activities': 16, 'n_unique_start_activities': 6, 'start_activities_iqr': 9.25, 'start_activities_kurtosis': 1.199106773708694, 'start_activities_max': 995, 'start_activities_mean': 175.0, 'start_activities_median': 12.0, 'start_activities_min': 6, 'start_activities_q1': 7.75, 'start_activities_q3': 17.0, 'start_activities_skewness': 1.7883562472303318, 'start_activities_std': 366.73787187399483, 'start_activities_variance': 134496.66666666666, 'end_activities_iqr': 39.5, 'end_activities_kurtosis': 2.5007579343413617, 'end_activities_max': 393, 'end_activities_mean': 75.0, 'end_activities_median': 32.5, 'end_activities_min': 2, 'end_activities_q1': 14.0, 'end_activities_q3': 53.5, 'end_activities_skewness': 2.004413358907822, 'end_activities_std': 112.91400014423114, 'end_activities_variance': 12749.57142857143, 'n_unique_end_activities': 14, 'entropy_global_block': 14.501, 'entropy_k_block_diff_1': -0.019, 'entropy_k_block_diff_3': 1.837, 'entropy_k_block_diff_5': 1.712, 'entropy_k_block_ratio_1': 2.262, 'entropy_k_block_ratio_3': 3.238, 'entropy_k_block_ratio_5': 2.538, 'entropy_knn_3': 4.956, 'entropy_knn_5': 4.49, 'entropy_knn_7': 4.191, 'entropy_lempel_ziv': 1.727, 'entropy_prefix': 10.227, 'entropy_trace': 9.334, 'normalized_sequence_entropy': 0.5223430410751398, 'normalized_sequence_entropy_exponential_forgetting': 0.29950463593968696, 'normalized_sequence_entropy_linear_forgetting': 0.21936523360299368, 'normalized_variant_entropy': 0.6957588422064969, 'sequence_entropy': 76528.6794749776, 'sequence_entropy_exponential_forgetting': 43880.53919110408, 'sequence_entropy_linear_forgetting': 32139.284589305265, 'variant_entropy': 40624.49329803771, 'accumulated_time_min': 0.0, 'accumulated_time_max': 36488789.0, 'accumulated_time_mean': 396893.5456158801, 'accumulated_time_median': 11924.0, 'accumulated_time_mode': 0.0, 'accumulated_time_std': 1603193.2693230412, 'accumulated_time_variance': 2570228658802.701, 'accumulated_time_q1': 1138.5, 'accumulated_time_q3': 273793.5, 'accumulated_time_iqr': 272655.0, 'accumulated_time_geometric_mean': 10904.332835327954, 'accumulated_time_geometric_std': 44.90292804116573, 'accumulated_time_harmonic_mean': 0.0, 'accumulated_time_skewness': 11.401470845961647, 'accumulated_time_kurtosis': 172.5725804780399, 'accumulated_time_coefficient_variation': 4.039353340541942, 'accumulated_time_entropy': 7.7513093893416505, 'accumulated_time_skewness_hist': 2.6663623098416838, 'accumulated_time_kurtosis_hist': 5.1101603988544575, 'execution_time_min': 0.0, 'execution_time_max': 36051318.0, 'execution_time_mean': 169759.47397134217, 'execution_time_median': 188.0, 'execution_time_mode': 0.0, 'execution_time_std': 1442884.0333929851, 'execution_time_variance': 2081914333820.4087, 'execution_time_q1': 0.0, 'execution_time_q3': 18623.25, 'execution_time_iqr': 18623.25, 'execution_time_geometric_mean': 199.88320191111325, 'execution_time_geometric_std': 127.92792986844444, 'execution_time_harmonic_mean': 0.0, 'execution_time_skewness': 14.528527518337812, 'execution_time_kurtosis': 250.488253204707, 'execution_time_coefficient_variation': 8.499578843161146, 'execution_time_entropy': 6.221052534222753, 'execution_time_skewness_hist': 2.666603580180752, 'execution_time_kurtosis_hist': 5.110914600502133, 'remaining_time_min': 0.0, 'remaining_time_max': 36488789.0, 'remaining_time_mean': 2796232.825161036, 'remaining_time_median': 619470.0, 'remaining_time_mode': 0.0, 'remaining_time_std': 5281078.119895241, 'remaining_time_variance': 27889786108436.258, 'remaining_time_q1': 202862.5, 'remaining_time_q3': 2487420.0, 'remaining_time_iqr': 2284557.5, 'remaining_time_geometric_mean': 224736.22203397762, 'remaining_time_geometric_std': 70.1715364379747, 'remaining_time_harmonic_mean': 0.0, 'remaining_time_skewness': 3.1659682263680318, 'remaining_time_kurtosis': 11.666720436340661, 'remaining_time_coefficient_variation': 1.8886403422401359, 'remaining_time_entropy': 8.55331137332654, 'remaining_time_skewness_hist': 2.61693528788402, 'remaining_time_kurtosis_hist': 4.950830339077765, 'within_day_min': 0.0, 'within_day_max': 86390.0, 'within_day_mean': 41330.543183909555, 'within_day_median': 37800.0, 'within_day_mode': 21600.0, 'within_day_std': 20590.894075207798, 'within_day_variance': 423984918.8164276, 'within_day_q1': 23113.75, 'within_day_q3': 57600.0, 'within_day_iqr': 34486.25, 'within_day_geometric_mean': 35069.233548115764, 'within_day_geometric_std': 1.9726454507370417, 'within_day_harmonic_mean': 0.0, 'within_day_skewness': 0.3603519661740256, 'within_day_kurtosis': -0.9142275965359778, 'within_day_coefficient_variation': 0.49820042247168106, 'within_day_entropy': 9.501009299480838, 'within_day_skewness_hist': 1.7511033515349685, 'within_day_kurtosis_hist': 2.6115894228132266}
+SUCCESSFULLY: 179 features for Sepsis.xes took 0:00:14.875727 sec.
+{'log': 'Sepsis', 'n_traces': 1050, 'n_unique_traces': 846, 'ratio_unique_traces_per_trace': 0.8057142857142857, 'trace_len_coefficient_variation': 0.7916391922924689, 'trace_len_entropy': 6.769403523350811, 'trace_len_geometric_mean': 12.281860759040903, 'trace_len_geometric_std': 1.7464004837799154, 'trace_len_harmonic_mean': 10.47731701485374, 'trace_len_hist1': 0.048613291470434326, 'trace_len_hist10': 0.00010465724751439027, 'trace_len_hist2': 0.005285190999476714, 'trace_len_hist3': 0.0005756148613291472, 'trace_len_hist4': 0.0002093144950287807, 'trace_len_hist5': 0.00010465724751439036, 'trace_len_hist6': 0.0, 'trace_len_hist7': 5.232862375719522e-05, 'trace_len_hist8': 0.0, 'trace_len_hist9': 0.0, 'trace_len_iqr': 7.0, 'trace_len_kurtosis': 87.0376906898399, 'trace_len_kurtosis_hist': 4.931206347805768, 'trace_len_max': 185, 'trace_len_mean': 14.48952380952381, 'trace_len_median': 13.0, 'trace_len_min': 3, 'trace_len_mode': 8, 'trace_len_q1': 9.0, 'trace_len_q3': 16.0, 'trace_len_skewness': 7.250526815880918, 'trace_len_skewness_hist': 2.6128507781562513, 'trace_len_std': 11.470474925273926, 'trace_len_variance': 131.57179501133788, 'kurtosis_variant_occurrence': 217.44268017168216, 'mean_variant_occurrence': 1.2411347517730495, 'ratio_most_common_variant': 0.03333333333333333, 'ratio_top_10_variants': 0.2742857142857143, 'ratio_top_1_variants': 0.12, 'ratio_top_20_variants': 0.35523809523809524, 'ratio_top_50_variants': 0.5971428571428572, 'ratio_top_5_variants': 0.21523809523809523, 'ratio_top_75_variants': 0.7980952380952381, 'skewness_variant_occurrence': 13.637101374069475, 'std_variant_occurrence': 1.7594085182491936, 'activities_iqr': 983.5, 'activities_kurtosis': 1.05777753209275, 'activities_max': 3383, 'activities_mean': 950.875, 'activities_median': 788.0, 'activities_min': 6, 'activities_q1': 101.75, 'activities_q3': 1085.25, 'activities_skewness': 1.3912385607018212, 'activities_std': 1008.5815457239935, 'activities_variance': 1017236.734375, 'n_unique_activities': 16, 'n_unique_start_activities': 6, 'start_activities_iqr': 9.25, 'start_activities_kurtosis': 1.199106773708694, 'start_activities_max': 995, 'start_activities_mean': 175.0, 'start_activities_median': 12.0, 'start_activities_min': 6, 'start_activities_q1': 7.75, 'start_activities_q3': 17.0, 'start_activities_skewness': 1.7883562472303318, 'start_activities_std': 366.73787187399483, 'start_activities_variance': 134496.66666666666, 'end_activities_iqr': 39.5, 'end_activities_kurtosis': 2.5007579343413617, 'end_activities_max': 393, 'end_activities_mean': 75.0, 'end_activities_median': 32.5, 'end_activities_min': 2, 'end_activities_q1': 14.0, 'end_activities_q3': 53.5, 'end_activities_skewness': 2.004413358907822, 'end_activities_std': 112.91400014423114, 'end_activities_variance': 12749.57142857143, 'n_unique_end_activities': 14, 'eventropy_global_block': 14.501, 'eventropy_global_block_flattened': 14.655, 'eventropy_k_block_diff_1': 3.238, 'eventropy_k_block_diff_3': 1.712, 'eventropy_k_block_diff_5': 1.104, 'eventropy_k_block_ratio_1': 3.238, 'eventropy_k_block_ratio_3': 2.262, 'eventropy_k_block_ratio_5': 1.871, 'eventropy_knn_3': 4.956, 'eventropy_knn_5': 4.49, 'eventropy_knn_7': 4.191, 'eventropy_lempel_ziv': 1.727, 'eventropy_lempel_ziv_flattened': 1.888, 'eventropy_prefix': 10.227, 'eventropy_prefix_flattened': 10.595, 'eventropy_trace': 9.334, 'epa_normalized_sequence_entropy': 0.5223430410751398, 'epa_normalized_sequence_entropy_exponential_forgetting': 0.29950463593968696, 'epa_normalized_sequence_entropy_linear_forgetting': 0.21936523360299368, 'epa_normalized_variant_entropy': 0.6957588422064969, 'epa_sequence_entropy': 76528.6794749776, 'epa_sequence_entropy_exponential_forgetting': 43880.53919110408, 'epa_sequence_entropy_linear_forgetting': 32139.284589305265, 'epa_variant_entropy': 40624.49329803771, 'accumulated_time_min': 0.0, 'accumulated_time_max': 36488789.0, 'accumulated_time_mean': 396893.5456158801, 'accumulated_time_median': 11924.0, 'accumulated_time_mode': 0.0, 'accumulated_time_std': 1603193.2693230412, 'accumulated_time_variance': 2570228658802.701, 'accumulated_time_q1': 1138.5, 'accumulated_time_q3': 273793.5, 'accumulated_time_iqr': 272655.0, 'accumulated_time_geometric_mean': 10904.332835327954, 'accumulated_time_geometric_std': 44.90292804116573, 'accumulated_time_harmonic_mean': 0.0, 'accumulated_time_skewness': 11.401470845961647, 'accumulated_time_kurtosis': 172.5725804780399, 'accumulated_time_coefficient_variation': 4.039353340541942, 'accumulated_time_entropy': 7.7513093893416505, 'accumulated_time_skewness_hist': 2.6663623098416838, 'accumulated_time_kurtosis_hist': 5.1101603988544575, 'execution_time_min': 0.0, 'execution_time_max': 36051318.0, 'execution_time_mean': 169759.47397134217, 'execution_time_median': 188.0, 'execution_time_mode': 0.0, 'execution_time_std': 1442884.0333929851, 'execution_time_variance': 2081914333820.4087, 'execution_time_q1': 0.0, 'execution_time_q3': 18623.25, 'execution_time_iqr': 18623.25, 'execution_time_geometric_mean': 199.88320191111325, 'execution_time_geometric_std': 127.92792986844444, 'execution_time_harmonic_mean': 0.0, 'execution_time_skewness': 14.528527518337812, 'execution_time_kurtosis': 250.488253204707, 'execution_time_coefficient_variation': 8.499578843161146, 'execution_time_entropy': 6.221052534222753, 'execution_time_skewness_hist': 2.666603580180752, 'execution_time_kurtosis_hist': 5.110914600502133, 'remaining_time_min': 0.0, 'remaining_time_max': 36488789.0, 'remaining_time_mean': 2796232.825161036, 'remaining_time_median': 619470.0, 'remaining_time_mode': 0.0, 'remaining_time_std': 5281078.119895241, 'remaining_time_variance': 27889786108436.258, 'remaining_time_q1': 202862.5, 'remaining_time_q3': 2487420.0, 'remaining_time_iqr': 2284557.5, 'remaining_time_geometric_mean': 224736.22203397762, 'remaining_time_geometric_std': 70.1715364379747, 'remaining_time_harmonic_mean': 0.0, 'remaining_time_skewness': 3.1659682263680318, 'remaining_time_kurtosis': 11.666720436340661, 'remaining_time_coefficient_variation': 1.8886403422401359, 'remaining_time_entropy': 8.55331137332654, 'remaining_time_skewness_hist': 2.61693528788402, 'remaining_time_kurtosis_hist': 4.950830339077765, 'within_day_min': 0.0, 'within_day_max': 86390.0, 'within_day_mean': 41330.543183909555, 'within_day_median': 37800.0, 'within_day_mode': 21600.0, 'within_day_std': 20590.894075207798, 'within_day_variance': 423984918.8164276, 'within_day_q1': 23113.75, 'within_day_q3': 57600.0, 'within_day_iqr': 34486.25, 'within_day_geometric_mean': 35069.233548115764, 'within_day_geometric_std': 1.9726454507370417, 'within_day_harmonic_mean': 0.0, 'within_day_skewness': 0.3603519661740256, 'within_day_kurtosis': -0.9142275965359778, 'within_day_coefficient_variation': 0.49820042247168106, 'within_day_entropy': 9.501009299480838, 'within_day_skewness_hist': 1.7511033515349685, 'within_day_kurtosis_hist': 2.6115894228132266}
 ```
 
 ## Extending Features
 This tutorial is for extending this tool to include additional features (e.g. time-based). As an example for this tutorial, we focus on the example of time-based features. The `feeed/time.py` script contains the class `TimeBased`, which extracts features from timestamps. FEEED focuses and extracts features of the whole log only (e.g., time within the day).
 
 ### Assumptions and conditions
 To include new features in this repo, first consider the following:
@@ -150,19 +154,19 @@
 
 ```
 ### Testing the new implementation
 
 After implementing the new feature; including it in the list of `feeed/feature_extractor.py` and importing the new method accordingly, you can quickly test it by running the:
 
 ```bash
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/SEPSIS.xes', ['new_feature_type']))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/SEPSIS.xes', ['new_feature_type']))"
 ```
 and
 ```bash
-python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_logs/SEPSIS.xes', ['new_feature_name_1', 'new_feature_name_2']))"
+python -c "from feeed.feature_extractor import extract_features; print(extract_features('test_data/SEPSIS.xes', ['new_feature_name_1', 'new_feature_name_2']))"
 ```
 
 ### Update documentation
 When updating results and table in the documentation, please note that the features are sorted by their type and types are sorted chronologically.
 
 Finally, consider submitting a pull request to our repository. We are looking forward to your new features! :)
```

### Comparing `feeed-1.1.0/feeed/activities.py` & `feeed-1.2.0/feeed/activities.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/complexity.py` & `feeed-1.2.0/feeed/epa_based.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import math
 import pandas as pd
 import pm4py
+import functools
 
 from .feature import Feature
 
 class Event:
     __slots__ = "case_id", "activity", "timestamp", "predecessor", "event_id"
     _counter = 0
 
@@ -157,15 +158,15 @@
         )
 
     def get_timespan(self):
         return (self.get_last_timestamp() - self.get_first_timestamp()).total_seconds()
 
     def to_plain_log(self):
         return sorted(
-            Complexity.flatten([node.sequence for node in self.nodes if node != self.root]),
+            Epa_based.flatten([node.sequence for node in self.nodes if node != self.root]),
             key=lambda event: event.timestamp,
         )
 
     def to_pm4py_log(self):
         traces = {}
         for event in sorted(
             self.to_plain_log(), key=lambda event: (event.case_id, event.timestamp)
@@ -177,26 +178,27 @@
             pm4py_event = pm4py.objects.log.obj.Event()
             pm4py_event["concept:name"] = event.activity
             pm4py_event["time:timestamp"] = event.timestamp
             traces[event.case_id].append(pm4py_event)
         return pm4py.objects.log.obj.EventLog(traces.values())
 
 
-class Complexity(Feature):
-    def __init__(self, feature_names='complexity'):
-        self.feature_type = "complexity"
-        self.available_class_methods = dict(inspect.getmembers(Complexity, predicate=inspect.ismethod))
+class Epa_based(Feature):
+    def __init__(self, feature_names='epa_based'):
+        self.feature_type = "epa_based"
+        # listing class methods in the order they were defined so that the cache can be reset in the last class method without looking it up
+        self.available_class_methods = {name: method.__get__(self, Epa_based) for name, method in vars(Epa_based).items() if isinstance(method, classmethod)}
         if self.feature_type in feature_names:
-            self.feature_names = [*self.available_class_methods.keys()]
+            self.feature_names = [method for method in self.available_class_methods.keys() if not method.startswith('_')]
         else:
             self.feature_names = feature_names
 
     def log_to_epa(pm4py_log):
-        log = Complexity.generate_log(pm4py_log)
-        epa = Complexity.build_graph(log)
+        log = Epa_based.generate_log(pm4py_log)
+        epa = Epa_based.build_graph(log)
         return epa
 
     def generate_log(pm4py_log, verbose=False):
         log = []
         for trace in pm4py_log:
             for event in trace:
                 try:
@@ -242,24 +244,24 @@
 
         return log
 
     def flatten(in_list):
         out_list = []
         for item in in_list:
             if isinstance(item, list):
-                out_list.extend(Complexity.flatten(item))
+                out_list.extend(Epa_based.flatten(item))
             else:
                 out_list.append(item)
         return out_list
 
 
     def build_graph(log, verbose=False, accepting=False):
         def add_events_to_graph(pa, log, verbose=False):
             for event in log:
-                Complexity.add_event_to_graph(event, pa, verbose=verbose)
+                Epa_based.add_event_to_graph(event, pa, verbose=verbose)
             pa.nodes.sort(key=lambda node: (node.c, node.j))
             return pa
         if len(log) == 0:
             raise Exception("Cannot build EPA from an empty log")
         if verbose:
             print("Building the prefix automaton...")
 
@@ -313,42 +315,42 @@
 
         for key in c_index:
             c_index[key].sort(key=lambda node: node.j)
 
         return c_index
 
     def graph_complexity(pa):
-        pa.c_index = Complexity.create_c_index(pa)
+        pa.c_index = Epa_based.create_c_index(pa)
         graph_complexity = math.log(len(pa.nodes) - 1) * (len(pa.nodes) - 1)
         normalize = graph_complexity
         for i in list(pa.c_index.keys())[1:]:
             e = len(pa.c_index[i])
             graph_complexity -= math.log(e) * e
 
         return graph_complexity, (graph_complexity / normalize)
 
     def log_complexity(pa, forgetting=None, k=1):
-        pa.c_index = Complexity.create_c_index(pa)
-        normalize = sum([len(AT.sequence) for AT in Complexity.flatten(pa.activity_types.values())])
+        pa.c_index = Epa_based.create_c_index(pa)
+        normalize = sum([len(AT.sequence) for AT in Epa_based.flatten(pa.activity_types.values())])
         normalize = normalize * math.log(normalize)
         if not forgetting:
             length = 0
-            for AT in Complexity.flatten(pa.activity_types.values()):
+            for AT in Epa_based.flatten(pa.activity_types.values()):
                 length += len(AT.sequence)
             log_complexity = math.log(length) * length
             for i in list(pa.c_index.keys())[1:]:
                 e = sum([len(AT.sequence) for AT in pa.c_index[i]])
                 log_complexity -= math.log(e) * e
 
             return log_complexity, (log_complexity / normalize)
         elif forgetting == "linear":
             last_timestamp = pa.get_last_timestamp()
             timespan = pa.get_timespan()
             log_complexity_linear = 0
-            for AT in Complexity.flatten(pa.activity_types.values()):
+            for AT in Epa_based.flatten(pa.activity_types.values()):
                 for event in AT.sequence:
                     try:
                         log_complexity_linear += (
                             1 - (last_timestamp - event.timestamp).total_seconds() / timespan
                         )
                     except ValueError:
                         log_complexity_linear += (
@@ -367,23 +369,26 @@
                                 - (last_timestamp - event.timestamp).total_seconds() / timespan
                             )
                         except ValueError:
                             e += (
                                     1
                                     - (last_timestamp - event.timestamp).total_seconds() / (timespan+1e-6)
                             )
-                log_complexity_linear -= math.log(e) * e
+                try:
+                    log_complexity_linear -= math.log(e) * e
+                except ValueError:
+                    log_complexity_linear -= math.log(1e-6) * 1e-6
 
             return log_complexity_linear, (log_complexity_linear / normalize)
 
         elif forgetting == "exp":
             last_timestamp = pa.get_last_timestamp()
             timespan = pa.get_timespan()
             log_complexity_exp = 0
-            for AT in Complexity.flatten(pa.activity_types.values()):
+            for AT in Epa_based.flatten(pa.activity_types.values()):
                 for event in AT.sequence:
                     try:
                         log_complexity_exp += math.exp(
                             (-(last_timestamp - event.timestamp).total_seconds() / timespan) * k
                         )
                     except ValueError:
                         log_complexity_exp += math.exp(
@@ -403,52 +408,103 @@
                             )
                         except ValueError:
                             e += math.exp(
                                 (-(last_timestamp - event.timestamp).total_seconds() / (timespan+1e-6))
                                 * k
                             )
 
-                log_complexity_exp -= math.log(e) * e
+                try:
+                    log_complexity_exp -= math.log(e) * e
+                except ValueError:
+                    log_complexity_exp -= math.log(1e-6) * 1e-6
+
             return log_complexity_exp, (log_complexity_exp / normalize)
         else:
             return None, None
 
+    _cached_epa = None
+    _cached_graph_complexity = None
+    _cached_log_complexity = None
+    _cached_log_complexity_linear = None
+    _cached_log_complexity_exp = None
+
+    # Helper functions (start with _)
     @classmethod
-    def variant_entropy(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.graph_complexity(epa)[0]
+    def _calculate_epa(cls, log):
+        if cls._cached_epa is None:
+            cls._cached_epa = Epa_based.log_to_epa(log)
+        return cls._cached_epa
 
     @classmethod
-    def normalized_variant_entropy(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.graph_complexity(epa)[1]
+    def _calculate_graph_complexity(cls, log):
+        if cls._cached_graph_complexity is None:
+            epa = cls._calculate_epa(log)
+            cls._cached_graph_complexity = Epa_based.graph_complexity(epa)
+        return cls._cached_graph_complexity
 
     @classmethod
-    def sequence_entropy(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa)[0]
+    def _calculate_log_complexity(cls, log):
+        if cls._cached_log_complexity is None:
+            epa = cls._calculate_epa(log)
+            cls._cached_log_complexity = Epa_based.log_complexity(epa)
+        return cls._cached_log_complexity
 
     @classmethod
-    def normalized_sequence_entropy(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa)[1]
+    def _calculate_log_complexity_linear(cls, log):
+        if cls._cached_log_complexity_linear is None:
+            epa = cls._calculate_epa(log)
+            cls._cached_log_complexity_linear = Epa_based.log_complexity(epa, "linear")
+        return cls._cached_log_complexity_linear
 
     @classmethod
-    def sequence_entropy_linear_forgetting(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa, "linear")[0]
+    def _calculate_log_complexity_exp(cls, log):
+        if cls._cached_log_complexity_exp is None:
+            epa = cls._calculate_epa(log)
+            cls._cached_log_complexity_exp = Epa_based.log_complexity(epa, "exp")
+        return cls._cached_log_complexity_exp
 
     @classmethod
-    def normalized_sequence_entropy_linear_forgetting(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa, "linear")[1]
+    def epa_variant_entropy(cls, log):
+        graph_complexity = cls._calculate_graph_complexity(log)
+        return graph_complexity[0]
 
     @classmethod
-    def sequence_entropy_exponential_forgetting(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa, "exp")[0]
+    def epa_normalized_variant_entropy(cls, log):
+        graph_complexity = cls._calculate_graph_complexity(log)
+        return graph_complexity[1]
 
     @classmethod
-    def normalized_sequence_entropy_exponential_forgetting(cls, log):
-        epa = Complexity.log_to_epa(log)
-        return Complexity.log_complexity(epa, "exp")[1]
+    def epa_sequence_entropy(cls, log):
+        log_complexity = cls._calculate_log_complexity(log)
+        return log_complexity[0]
 
+    @classmethod
+    def epa_normalized_sequence_entropy(cls, log):
+        log_complexity = cls._calculate_log_complexity(log)
+        return log_complexity[1]
+
+    @classmethod
+    def epa_sequence_entropy_linear_forgetting(cls, log):
+        log_complexity = cls._calculate_log_complexity_linear(log)
+        return log_complexity[0]
+
+    @classmethod
+    def epa_normalized_sequence_entropy_linear_forgetting(cls, log):
+        log_complexity = cls._calculate_log_complexity_linear(log)
+        return log_complexity[1]
+
+    @classmethod
+    def epa_sequence_entropy_exponential_forgetting(cls, log):
+        log_complexity = cls._calculate_log_complexity_exp(log)
+        return log_complexity[0]
+
+    @classmethod
+    def epa_normalized_sequence_entropy_exponential_forgetting(cls, log):
+        log_complexity = cls._calculate_log_complexity_exp(log)
+        
+        #reset the cache
+        cls._cached_epa = None
+        cls._cached_graph_complexity = None
+        cls._cached_log_complexity = None
+        cls._cached_log_complexity_linear = None
+        cls._cached_log_complexity_exp = None
+        return log_complexity[1]
```

### Comparing `feeed-1.1.0/feeed/end_activities.py` & `feeed-1.2.0/feeed/end_activities.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/feature_extractor.py` & `feeed-1.2.0/feeed/feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import subprocess
 from .simple_stats import SimpleStats as simple_stats
 from .trace_length import TraceLength as trace_length
 from .trace_variant import TraceVariant as trace_variant
 from .activities import Activities as activities
 from .start_activities import StartActivities as start_activities
 from .end_activities import EndActivities as end_activities
-from .entropies import Entropies as entropies
-from .complexity import Complexity as complexity
+from .eventropies import Eventropies as eventropies
+from .epa_based import Epa_based as epa_based
 from .time import TimeBased as time_based
 
 from datetime import datetime as dt
 from pm4py.objects.log.importer.xes import importer as xes_importer
 
 FEATURE_TYPES = [
     "simple_stats",
     "trace_length",
     "trace_variant",
     "activities",
     "start_activities",
     "end_activities",
-    "entropies",
-    "complexity",
+    "eventropies",
+    "epa_based",
     "time_based",
     ]
 
 
 def feature_type(feature_name):
     available_features = []
     for feature_type in FEATURE_TYPES:
@@ -98,18 +98,15 @@
     features = {"log": log_name.split(".xes")[0]}
     start_log = dt.now()
 
     for i, ft_name in enumerate(feature_types):
         start_feat = dt.now()
         ft_type = feature_type(ft_name)
 
-        if ft_type == "entropies":
-            feature_values = eval(f"{ft_type}(feature_names =['{ft_name}']).extract(event_logs_path)")
-        else:
-            feature_values = eval(f"{ft_type}(feature_names=['{ft_name}']).extract(log)")
+        feature_values = eval(f"{ft_type}(feature_names=['{ft_name}']).extract(log)")
         features = {**features, **feature_values}
 
         log_info =  f"     INFO: {log_name} starting at {len(features)}, {ft_name} from {ft_type} took {dt.now()-start_feat} sec, "
         if i == len(feature_types) - 1:
             print(log_info + "last feature.")
         else:
             print(log_info + f"next {feature_types[(i+1)%len(feature_types)]}...")
```

### Comparing `feeed-1.1.0/feeed/simple_stats.py` & `feeed-1.2.0/feeed/simple_stats.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/start_activities.py` & `feeed-1.2.0/feeed/start_activities.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/time.py` & `feeed-1.2.0/feeed/time.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/trace_length.py` & `feeed-1.2.0/feeed/trace_length.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/feeed/trace_variant.py` & `feeed-1.2.0/feeed/trace_variant.py`

 * *Files identical despite different names*

### Comparing `feeed-1.1.0/setup.py` & `feeed-1.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
         name = 'feeed',
-        version = '1.1.0',
+        version = '1.2.0',
         description = 'Feature Extraction from Event Data',
         author = 'Andrea Maldonado, Gabriel Tavares',
         author_email = 'andreamalher.works@gmail.com, gabrielmrqstvrs@gmail.com',
         license = 'MIT',
         url='https://github.com/lmu-dbs/feeed.git',
         install_requires=[
-            'pandas==2.0.0',
             'tqdm==4.65.0',
             'pm4py==2.7.2',
             'scipy>=1.10.1',
+            'Levenshtein==0.23.0',
             ],
         packages = ['feeed', 'feeed.utils'],
         classifiers=[
             'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
             'Intended Audience :: Science/Research',      # Define that your audience are developers
             'Topic :: Software Development',
             'License :: OSI Approved :: MIT License',   # Again, pick a license
             'Programming Language :: Python :: 3.9',
     ],
-)
+)
```

