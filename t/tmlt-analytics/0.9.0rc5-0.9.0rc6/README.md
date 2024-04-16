# Comparing `tmp/tmlt_analytics-0.9.0rc5.tar.gz` & `tmp/tmlt_analytics-0.9.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.9.0rc5.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.9.0rc6.tar", max compression
```

## Comparing `tmlt_analytics-0.9.0rc5.tar` & `tmlt_analytics-0.9.0rc6.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0    11358 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/LICENSE
--rw-r--r--   0        0        0    20138 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/LICENSE.docs
--rw-r--r--   0        0        0      121 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/NOTICE
--rw-r--r--   0        0        0     3303 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/README.md
--rw-r--r--   0        0        0     1231 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1078 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/logo.png
--rw-r--r--   0        0        0      133 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/build-info.html
--rw-r--r--   0        0        0      491 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/layout.html
--rw-r--r--   0        0        0      106 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/package-name.html
--rw-r--r--   0        0        0    22344 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/changelog.rst
--rw-r--r--   0        0        0     8408 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/conf.py
--rw-r--r--   0        0        0    10498 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/aws-glue.rst
--rw-r--r--   0        0        0     1599 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3005 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1225 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6475 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5897 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4733 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1706 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/setup.rst
--rw-r--r--   0        0        0     6911 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/databricks.rst
--rw-r--r--   0        0        0      339 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/index.rst
--rw-r--r--   0        0        0     4895 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/installation.rst
--rw-r--r--   0        0        0     4126 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/troubleshooting.rst
--rw-r--r--   0        0        0   118378 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0   344848 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_books_borrowed_by_zip.png
--rw-r--r--   0        0        0    34101 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    30778 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/chart_total_books_borrowed_in_zipcodes.png
--rw-r--r--   0        0        0    20226 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    18639 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/flat_map_row_example.svg
--rw-r--r--   0        0        0    23590 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0   116752 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/glue_graph.png
--rw-r--r--   0        0        0    14685 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_api.svg
--rw-r--r--   0        0        0      609 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_howto_guides.svg
--rw-r--r--   0        0        0     1196 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    23369 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/intuitive_noise_visualization.png
--rw-r--r--   0        0        0    30903 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/logo.png
--rw-r--r--   0        0        0    85314 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/mock_checkout_logs.svg
--rw-r--r--   0        0        0    59239 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/private_join_example.svg
--rw-r--r--   0        0        0    35838 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/private_join_tables.svg
--rw-r--r--   0        0        0    32227 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/public_join_example_zips.svg
--rw-r--r--   0        0        0    64480 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping-varied-budgets.png
--rw-r--r--   0        0        0    27218 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping.png
--rw-r--r--   0        0        0     5717 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/index.rst
--rw-r--r--   0        0        0      662 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     3245 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/privacy-policy.rst
--rw-r--r--   0        0        0     2100 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3516 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/templates/python/module.rst
--rw-r--r--   0        0        0      396 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11868 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8665 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6589 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7849 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0    12509 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/understanding-sensitivity.rst
--rw-r--r--   0        0        0     8467 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9126 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7219 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18785 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0     1133 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/index.rst
--rw-r--r--   0        0        0    12370 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     8434 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    15155 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16248 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     6579 2024-04-08 13:11:25.732937 tmlt_analytics-0.9.0rc5/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/__init__.py
--rw-r--r--   0        0        0    11799 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/conftest.py
--rw-r--r--   0        0        0      115 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/__init__.py
--rw-r--r--   0        0        0     3447 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/conftest.py
--rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/__init__.py
--rw-r--r--   0        0        0     2323 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0     6598 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_count_distinct_optimization.py
--rw-r--r--   0        0        0     9173 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_id_col_operations.py
--rw-r--r--   0        0        0    22198 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    14273 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     3969 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    26385 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    45748 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6122 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    18977 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0    10496 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     4465 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/test_budgets.py
--rw-r--r--   0        0        0     2279 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/__init__.py
--rw-r--r--   0        0        0     4726 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_builder.py
--rw-r--r--   0        0        0     7322 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_mixins.py
--rw-r--r--   0        0        0      298 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    65734 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    60081 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24188 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36803 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    15631 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_catalog.py
--rw-r--r--   0        0        0      724 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21123 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_keyset.py
--rw-r--r--   0        0        0    14053 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3751 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5480 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     2931 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40466 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    56419 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16768 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     5021 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    87198 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5372 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      741 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_utils.py
--rw-r--r--   0        0        0       85 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test_requirements.txt
--rw-r--r--   0        0        0      681 2024-04-08 13:11:25.736937 tmlt_analytics-0.9.0rc5/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     5573 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_base_builder.py
--rw-r--r--   0        0        0     3666 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16206 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     6824 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     6583 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     4838 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    60500 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py
--rw-r--r--   0        0        0    63111 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py
--rw-r--r--   0        0        0    11321 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7778 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0     5993 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    47962 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0      393 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12795 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3980 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10581 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0      487 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_type_checking.py
--rw-r--r--   0        0        0      452 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_utils.py
--rw-r--r--   0        0        0    12094 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      374 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      458 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      802 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12758 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11801 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0    10828 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5429 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   133339 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41985 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    73619 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3913 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     6292 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     4743 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc5/setup.py
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/LICENSE
+-rw-r--r--   0        0        0    20138 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/LICENSE.docs
+-rw-r--r--   0        0        0      121 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/NOTICE
+-rw-r--r--   0        0        0     3303 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/README.md
+-rw-r--r--   0        0        0     1231 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1078 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_static/logo.png
+-rw-r--r--   0        0        0      133 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      491 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_templates/layout.html
+-rw-r--r--   0        0        0      106 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/_templates/package-name.html
+-rw-r--r--   0        0        0    22389 2024-04-12 12:49:30.960477 tmlt_analytics-0.9.0rc6/doc/changelog.rst
+-rw-r--r--   0        0        0     8408 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/conf.py
+-rw-r--r--   0        0        0    10498 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/aws-glue.rst
+-rw-r--r--   0        0        0     1599 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3005 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1225 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6475 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5897 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4733 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1706 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0     6911 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/databricks.rst
+-rw-r--r--   0        0        0      339 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/index.rst
+-rw-r--r--   0        0        0     4895 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/installation.rst
+-rw-r--r--   0        0        0     4126 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/howto-guides/troubleshooting.rst
+-rw-r--r--   0        0        0   118378 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0   344848 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_books_borrowed_by_zip.png
+-rw-r--r--   0        0        0    34101 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2024-04-12 12:49:30.964477 tmlt_analytics-0.9.0rc6/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    30778 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_total_books_borrowed_in_zipcodes.png
+-rw-r--r--   0        0        0    20226 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    18639 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/flat_map_row_example.svg
+-rw-r--r--   0        0        0    23590 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0   116752 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/glue_graph.png
+-rw-r--r--   0        0        0    14685 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/index_api.svg
+-rw-r--r--   0        0        0      609 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/index_howto_guides.svg
+-rw-r--r--   0        0        0     1196 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    23369 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/intuitive_noise_visualization.png
+-rw-r--r--   0        0        0    30903 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/logo.png
+-rw-r--r--   0        0        0    85314 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/mock_checkout_logs.svg
+-rw-r--r--   0        0        0    59239 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/private_join_example.svg
+-rw-r--r--   0        0        0    35838 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/private_join_tables.svg
+-rw-r--r--   0        0        0    32227 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/public_join_example_zips.svg
+-rw-r--r--   0        0        0    64480 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/tuning-parameters-error-vs-clamping-varied-budgets.png
+-rw-r--r--   0        0        0    27218 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/images/tuning-parameters-error-vs-clamping.png
+-rw-r--r--   0        0        0     5717 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/index.rst
+-rw-r--r--   0        0        0      662 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     3245 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/privacy-policy.rst
+-rw-r--r--   0        0        0     2100 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3516 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/templates/python/module.rst
+-rw-r--r--   0        0        0      396 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11868 2024-04-12 12:49:30.968477 tmlt_analytics-0.9.0rc6/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8665 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6589 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7849 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0    12509 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/topic-guides/understanding-sensitivity.rst
+-rw-r--r--   0        0        0     8467 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9126 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7219 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18785 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0     1133 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    12370 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     8434 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    15155 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16248 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     6717 2024-04-12 12:50:14.072751 tmlt_analytics-0.9.0rc6/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/__init__.py
+-rw-r--r--   0        0        0    11799 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/conftest.py
+-rw-r--r--   0        0        0      115 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/__init__.py
+-rw-r--r--   0        0        0     3586 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/conftest.py
+-rw-r--r--   0        0        0      108 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/__init__.py
+-rw-r--r--   0        0        0     2323 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0     6598 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_count_distinct_optimization.py
+-rw-r--r--   0        0        0     9173 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_id_col_operations.py
+-rw-r--r--   0        0        0    22159 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14234 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     3969 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    26385 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    45765 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6122 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    18977 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0    10496 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     4465 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/test_budgets.py
+-rw-r--r--   0        0        0     2279 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/__init__.py
+-rw-r--r--   0        0        0     4726 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/base_builder/test_builder.py
+-rw-r--r--   0        0        0     7322 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/base_builder/test_mixins.py
+-rw-r--r--   0        0        0      298 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    65734 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    60081 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24188 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36803 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    15631 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      724 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21123 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    14053 2024-04-12 12:49:30.972477 tmlt_analytics-0.9.0rc6/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3751 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5480 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     2931 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40466 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    56425 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16768 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     5021 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    87198 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5372 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      741 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test/unit/test_utils.py
+-rw-r--r--   0        0        0       85 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/test_requirements.txt
+-rw-r--r--   0        0        0      681 2024-04-12 12:50:14.076752 tmlt_analytics-0.9.0rc6/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     5573 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_base_builder.py
+-rw-r--r--   0        0        0     3666 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16206 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     6824 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     6583 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     4838 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    60500 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py
+-rw-r--r--   0        0        0    63111 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py
+-rw-r--r--   0        0        0    11321 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7778 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0     5993 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    47962 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0      393 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12795 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3980 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10581 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0      487 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_type_checking.py
+-rw-r--r--   0        0        0      452 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/_utils.py
+-rw-r--r--   0        0        0    12094 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      374 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      458 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      802 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12758 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11801 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0    10828 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5429 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   133372 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41985 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    73670 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3913 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     6292 2024-04-12 12:49:30.976477 tmlt_analytics-0.9.0rc6/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     4743 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc6/setup.py
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc6/PKG-INFO
```

### Comparing `tmlt_analytics-0.9.0rc5/LICENSE` & `tmlt_analytics-0.9.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/LICENSE.docs` & `tmlt_analytics-0.9.0rc6/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/README.md` & `tmlt_analytics-0.9.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/_static/css/custom.css` & `tmlt_analytics-0.9.0rc6/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/_static/favicon.ico` & `tmlt_analytics-0.9.0rc6/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/_static/js/version-banner.js` & `tmlt_analytics-0.9.0rc6/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/_static/logo.png` & `tmlt_analytics-0.9.0rc6/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/changelog.rst` & `tmlt_analytics-0.9.0rc6/doc/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Changed
 ~~~~~~~
 
 - :class:`~tmlt.analytics.keyset.KeySet` equality is now performed without
   converting the underlying dataframe to Pandas.
 - :meth:`~tmlt.analytics.session.Session.partition_and_create`: the ``column`` and ``splits``
   arguments are now annotated as required.
+- Upgrades to version 0.13.0 of Tumult Core.
 
 Removed
 ~~~~~~~
 - *Backwards-incompatible*: The ``stability`` and ``grouping_column`` parameters to :meth:`Session.from_dataframe <tmlt.analytics.session.Session.from_dataframe>` and :meth:`Session.Builder.with_private_dataframe <tmlt.analytics.session.Session.Builder.with_private_dataframe>` have been removed (deprecated since Tumult Analytics 0.7.0).
   As a result, the ``protected_change`` parameter to those methods is now required.
 
 Fixed
```

### Comparing `tmlt_analytics-0.9.0rc5/doc/conf.py` & `tmlt_analytics-0.9.0rc6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/aws-glue.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/aws-glue.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/bigquery-setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/docker-image.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/index.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/inputs-outputs.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/parameters.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/parameters.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/running-the-program.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/setup.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/bigquery/setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/databricks.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/databricks.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/installation.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/howto-guides/troubleshooting.rst` & `tmlt_analytics-0.9.0rc6/doc/howto-guides/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/api_diagram.svg` & `tmlt_analytics-0.9.0rc6/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_books_borrowed_by_zip.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_books_borrowed_by_zip.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_education.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_filters_education.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_total_books_borrowed_in_zipcodes.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_total_books_borrowed_in_zipcodes.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.9.0rc6/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.9.0rc6/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.9.0rc6/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/flat_map_row_example.svg` & `tmlt_analytics-0.9.0rc6/doc/images/flat_map_row_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.9.0rc6/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/glue_graph.png` & `tmlt_analytics-0.9.0rc6/doc/images/glue_graph.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.9.0rc6/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/index_api.svg` & `tmlt_analytics-0.9.0rc6/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/index_howto_guides.svg` & `tmlt_analytics-0.9.0rc6/doc/images/index_howto_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/index_more.svg` & `tmlt_analytics-0.9.0rc6/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.9.0rc6/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/index_tutorials.svg` & `tmlt_analytics-0.9.0rc6/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/intuitive_noise_visualization.png` & `tmlt_analytics-0.9.0rc6/doc/images/intuitive_noise_visualization.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/logo.png` & `tmlt_analytics-0.9.0rc6/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/mock_checkout_logs.svg` & `tmlt_analytics-0.9.0rc6/doc/images/mock_checkout_logs.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/private_join_example.svg` & `tmlt_analytics-0.9.0rc6/doc/images/private_join_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/private_join_tables.svg` & `tmlt_analytics-0.9.0rc6/doc/images/private_join_tables.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/public_join_example_zips.svg` & `tmlt_analytics-0.9.0rc6/doc/images/public_join_example_zips.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping-varied-budgets.png` & `tmlt_analytics-0.9.0rc6/doc/images/tuning-parameters-error-vs-clamping-varied-budgets.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping.png` & `tmlt_analytics-0.9.0rc6/doc/images/tuning-parameters-error-vs-clamping.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/index.rst` & `tmlt_analytics-0.9.0rc6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/intersphinx_mapping.json` & `tmlt_analytics-0.9.0rc6/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/privacy-policy.rst` & `tmlt_analytics-0.9.0rc6/doc/privacy-policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/templates/python/class.rst` & `tmlt_analytics-0.9.0rc6/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/templates/python/module.rst` & `tmlt_analytics-0.9.0rc6/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/privacy-budgets.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/privacy-promise.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/spark.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/understanding-sensitivity.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/understanding-sensitivity.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.9.0rc6/doc/topic-guides/working-with-sessions.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/clamping-bounds.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/first-steps.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/groupby-queries.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/index.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/more-with-privacy-ids.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/privacy-budget-basics.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/privacy-id-basics.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.9.0rc6/doc/tutorials/simple-transformations.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/pyproject.toml` & `tmlt_analytics-0.9.0rc6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 readme = "README.md"
 authors = []
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.9.0-rc.5"
+version = "0.9.0-rc.6"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -37,31 +37,32 @@
   { include = "tmlt" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.1, <3.12.0"
 
-# When updating Core, PySpark, Pandas or SymPy, remember to update
+#####################################################################
+# When upating Core, PySpark, Pandas or SymPy, remember to update
 # test_multi_deps in the Noxfile.
-
-"tmlt.core" = "^0.12.0"
-
+"tmlt.core" = "^0.13.0"
 pandas = [
   { version = ">=1.2.0,<1.4.0", python = "<3.8" },
   { version = ">=1.2.0,<2.0.0", python = ">=3.8,<3.10" },
   { version = ">=1.4.0,<2.0.0", python = ">=3.10,<3.11" },
   { version = ">=1.5.0,<2.0.0", python = ">=3.11" },
 ]
 pyspark = [
   { version = "^3.0.0,<3.4.0", extras = ["sql"], python = "<3.8" },
   { version = "^3.0.0,<3.6.0", extras = ["sql"], python = ">=3.8,<3.11" },
   { version = "^3.4.0,<3.6.0", extras = ["sql"], python = ">=3.11" },
 ]
 sympy = "^1.8,<1.10"
+#####################################################################
+
 typeguard = "^2.12.1,<2.13.0"
 typing-extensions = "^4.1.0"
 
 [tool.poetry.group.fix-lock.dependencies]
 # This is a hack to convince Poetry to allow different versions of various
 # transitive dependencies on different Python versions, as there is not a single
 # version of these dependencies that works across our entire supported Python
```

### Comparing `tmlt_analytics-0.9.0rc5/test/conftest.py` & `tmlt_analytics-0.9.0rc6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/conftest.py` & `tmlt_analytics-0.9.0rc6/test/system/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,19 @@
     """
     if not collection:
         return None
 
     if isinstance(value, (int, float)):
         return min(collection, key=lambda c: abs(value - c))
     elif isinstance(value, tuple):
-        return min(
-            collection, key=lambda c: sum(abs(t[0] - t[1]) for t in zip(value, c))
+        for candidate in collection:
+            if value == pytest.approx(candidate, nan_ok=True):
+                return candidate
+        raise AssertionError(
+            "No element of the collection is approximately equal to the value"
         )
     else:
         raise AssertionError("Unknown input data type")
 
 
 @pytest.fixture(scope="module")
 def _session_data(spark):
```

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/conftest.py` & `tmlt_analytics-0.9.0rc6/test/system/session/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_count_distinct_optimization.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_count_distinct_optimization.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_id_col_operations.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_id_col_operations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2024
 
 import statistics
 from typing import List, Optional, Set, Tuple
 
+import pandas as pd
 import pytest
 
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
@@ -269,40 +270,38 @@
     assert len(res) == 1
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison. Our variance algorithm always
     # produces (width of bounds / 2)**2 as the variance of an empty collection
     # of rows, so fill that in to prevent pvariance from raising an exception in
     # that case.
     value = res["n_variance"][0]
-    closest = closest_value(value, {statistics.pvariance(n) if n else 25 for n in ns})
-    assert value == pytest.approx(closest)
+    closest = closest_value(value, {pd.Series(n).var() for n in ns})
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS_GROUPED))
 def test_variance_grouped(
     base_query: QueryBuilder, ns: Set[Tuple[Tuple[int, ...], Tuple[int, ...]]], session
 ):
     """Grouped variances on tables with IDs work using L0 + L-inf."""
     res = session.evaluate(
         base_query.groupby(_KEYSET).variance("n", 0, 10),
         session.remaining_privacy_budget,
     ).toPandas()
-    expected_variances = {
-        tuple(statistics.pvariance(g) if len(g) > 1 else 25 for g in n) for n in ns
-    }
+    expected_variances = {tuple(pd.Series(g).var() for g in n) for n in ns}
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison.
     value = tuple(
         res.loc[res["group"] == group]["n_variance"].values[0] for group in ["A", "B"]
     )
     closest = closest_value(value, expected_variances)
-    assert value == pytest.approx(closest)
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS))
 def test_stdev(base_query: QueryBuilder, ns: Set[Tuple[int, ...]], session):
@@ -313,37 +312,35 @@
     assert len(res) == 1
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison. Our stdev algorithm always
     # produces (width of bounds / 2) as the stdev (before noise) if no data
     # points are available, so fill that in to prevent pstdev from raising an
     # exception in that case.
     value = res["n_stdev"][0]
-    closest = closest_value(value, {statistics.pstdev(n) if n else 25 for n in ns})
-    assert value == pytest.approx(closest)
+    closest = closest_value(value, {pd.Series(n).std() for n in ns})
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS_GROUPED))
 def test_stdev_grouped(
     base_query: QueryBuilder, ns: Set[Tuple[Tuple[int, ...], Tuple[int, ...]]], session
 ):
     """Grouped stdevs on tables with IDs work using L0 + L-inf."""
     res = session.evaluate(
         base_query.groupby(_KEYSET).stdev("n", 0, 10), session.remaining_privacy_budget
     ).toPandas()
-    expected_stdevs = {
-        tuple(statistics.pstdev(g) if len(g) > 1 else 5 for g in n) for n in ns
-    }
+    expected_stdevs = {tuple(pd.Series(g).std() for g in n) for n in ns}
     value = tuple(
         res.loc[res["group"] == group]["n_stdev"].values[0] for group in ["A", "B"]
     )
     closest = closest_value(value, expected_stdevs)
-    assert value == pytest.approx(closest)
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 def test_mismatched_grouping_columns(session):
     """Constraints with different grouping columns can't be used for truncation."""
```

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_l1_truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2024
 
 import statistics
 from typing import List, Set, Tuple
 
+import pandas as pd
 import pytest
 
 from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
@@ -215,40 +216,38 @@
     assert len(res) == 1
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison. Our variance algorithm always
     # produces (width of bounds / 2)**2 as the variance of an empty collection
     # of rows, so fill that in to prevent pvariance from raising an exception in
     # that case.
     value = res["n_variance"][0]
-    closest = closest_value(value, {statistics.pvariance(n) if n else 25 for n in ns})
-    assert value == pytest.approx(closest)
+    closest = closest_value(value, {pd.Series(n).var() for n in ns})
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS_GROUPED))
 def test_variance_grouped(
     base_query: QueryBuilder, ns: Set[Tuple[Tuple[int, ...], Tuple[int, ...]]], session
 ):
     """Grouped variances on tables with IDs work using MaxRowsPerID."""
     res = session.evaluate(
         base_query.groupby(_KEYSET).variance("n", 0, 10),
         session.remaining_privacy_budget,
     ).toPandas()
-    expected_variances = {
-        tuple(statistics.pvariance(g) if len(g) > 1 else 25 for g in n) for n in ns
-    }
+    expected_variances = {tuple(pd.Series(g).var() for g in n) for n in ns}
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison.
     value = tuple(
         res.loc[res["group"] == group]["n_variance"].values[0] for group in ["A", "B"]
     )
     closest = closest_value(value, expected_variances)
-    assert value == pytest.approx(closest)
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS))
 def test_stdev(base_query: QueryBuilder, ns: Set[Tuple[int, ...]], session):
@@ -259,37 +258,35 @@
     assert len(res) == 1
     # There's some floating-point imprecision at play here, so find the closest
     # value and use approx() for the comparison. Our stdev algorithm always
     # produces (width of bounds / 2) as the stdev (before noise) if no data
     # points are available, so fill that in to prevent pstdev from raising an
     # exception in that case.
     value = res["n_stdev"][0]
-    closest = closest_value(value, {statistics.pstdev(n) if n else 25 for n in ns})
-    assert value == pytest.approx(closest)
+    closest = closest_value(value, {pd.Series(n).std() for n in ns})
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize(
     "session", [INF_BUDGET, INF_BUDGET_ZCDP], indirect=True, ids=["puredp", "zcdp"]
 )
 @pytest.mark.parametrize("base_query,ns", zip(_BASE_QUERIES, _BASE_QUERY_NS_GROUPED))
 def test_stdev_grouped(
     base_query: QueryBuilder, ns: Set[Tuple[Tuple[int, ...], Tuple[int, ...]]], session
 ):
     """Grouped stdevs on tables with IDs work using MaxRowsPerID."""
     res = session.evaluate(
         base_query.groupby(_KEYSET).stdev("n", 0, 10), session.remaining_privacy_budget
     ).toPandas()
-    expected_stdevs = {
-        tuple(statistics.pstdev(g) if len(g) > 1 else 5 for g in n) for n in ns
-    }
+    expected_stdevs = {tuple(pd.Series(g).std() for g in n) for n in ns}
     value = tuple(
         res.loc[res["group"] == group]["n_stdev"].values[0] for group in ["A", "B"]
     )
     closest = closest_value(value, expected_stdevs)
-    assert value == pytest.approx(closest)
+    assert value == pytest.approx(closest, nan_ok=True)
 
 
 @pytest.mark.parametrize("session", [INF_BUDGET], indirect=True, ids=["puredp"])
 @pytest.mark.parametrize(
     "query,expected_noise",
     [
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count(), [1]),
```

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.9.0rc6/test/system/session/ids/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.9.0rc6/test/system/session/mixed/test_mixed_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/rows/conftest.py` & `tmlt_analytics-0.9.0rc6/test/system/session/rows/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2024
 
 # pylint: disable=no-self-use
 
 from typing import Any, Dict, List, Optional, Union
 
+import numpy as np
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
 from tmlt.core.measurements.interactive_measurements import PrivacyAccountantState
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
 from tmlt.core.utils.exact_number import ExactNumber
 from tmlt.core.utils.parameters import calculate_noise_scale
@@ -133,15 +134,15 @@
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="B",
                     low=0,
                     high=1,
                     mechanism=StdevMechanism.GAUSSIAN,
                     output_column="B_stdev",
                 ),
-                pd.DataFrame({"A": ["0", "1"], "B_stdev": [0.471405, 0.0]}),
+                pd.DataFrame({"A": ["0", "1"], "B_stdev": [0.5, np.nan]}),
             ),
         ],
     )
     def test_queries_privacy_budget_infinity_rhozcdp(
         self,
         query_expr: QueryExpr,
         expected_expr: Optional[QueryExpr],
```

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_infs_nulls.py` & `tmlt_analytics-0.9.0rc6/test/system/session/rows/test_add_max_rows_infs_nulls.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_invalid.py` & `tmlt_analytics-0.9.0rc6/test/system/session/rows/test_invalid.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/test_budgets.py` & `tmlt_analytics-0.9.0rc6/test/system/session/test_budgets.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.9.0rc6/test/system/session/test_invalid_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_builder.py` & `tmlt_analytics-0.9.0rc6/test/unit/base_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_mixins.py` & `tmlt_analytics-0.9.0rc6/test/unit/base_builder/test_mixins.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.9.0rc6/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_binning_spec.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_binning_spec.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_catalog.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_cleanup.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_constraints.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_keyset.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_neighboring_relations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_noise_info.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_protected_change.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_query_builder.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_query_expr_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright Tumult Labs 2024
 
 # pylint: disable=protected-access, no-self-use
 
 import datetime
 from typing import Dict, List, Union
 
+import numpy as np
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.functions import col
 from pyspark.sql.types import (
     DateType,
@@ -156,28 +157,28 @@
                 child=PrivateSource("private"),
                 groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                 measure_column="X",
                 low=0.0,
                 high=1.0,
             )
         ],
-        [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471405, 0.5]})],
+        [pd.DataFrame({"A": ["0", "1"], "stdev": [0.5, np.nan]})],
     ),
     (  # BoundedVariance
         [
             GroupByBoundedVariance(
                 child=PrivateSource("private"),
                 groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                 measure_column="X",
                 low=0.0,
                 high=1.0,
                 output_column="var",
             )
         ],
-        [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.25]})],
+        [pd.DataFrame({"A": ["0", "1"], "var": [0.25, np.nan]})],
     ),
     (  # BoundedSum
         [
             GroupByBoundedSum(
                 child=PrivateSource("private"),
                 groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                 measure_column="X",
@@ -806,78 +807,78 @@
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="X",
                     low=0.0,
                     high=1.0,
                     mechanism=StdevMechanism.LAPLACE,
                 ),
                 PureDP(),
-                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471405, 0.5]})],
+                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.5, np.nan]})],
             ),
             (  # BoundedSTDEV on integer valued measure column with LAPLACE
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="B",
                     low=0,
                     high=1,
                     mechanism=StdevMechanism.LAPLACE,
                 ),
                 PureDP(),
-                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471405, 0.0]})],
+                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.5, np.nan]})],
             ),
             (  # BoundedSTDEV on integer valued measure column with GAUSSIAN
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="B",
                     low=0,
                     high=1,
                     mechanism=StdevMechanism.GAUSSIAN,
                 ),
                 RhoZCDP(),
-                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471405, 0.0]})],
+                [pd.DataFrame({"A": ["0", "1"], "stdev": [0.5, np.nan]})],
             ),
             (  # BoundedVariance on floating-point valued measure column with LAPLACE
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="X",
                     low=0.0,
                     high=1.0,
                     output_column="var",
                     mechanism=VarianceMechanism.LAPLACE,
                 ),
                 PureDP(),
-                [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.25]})],
+                [pd.DataFrame({"A": ["0", "1"], "var": [0.25, np.nan]})],
             ),
             (  # BoundedVariance on integer valued measure column with LAPLACE
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="B",
                     low=0,
                     high=1,
                     output_column="var",
                     mechanism=VarianceMechanism.LAPLACE,
                 ),
                 PureDP(),
-                [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.0]})],
+                [pd.DataFrame({"A": ["0", "1"], "var": [0.25, np.nan]})],
             ),
             (  # BoundedVariance on integer valued measure column with GAUSSIAN
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="B",
                     low=0,
                     high=1,
                     output_column="var",
                     mechanism=VarianceMechanism.GAUSSIAN,
                 ),
                 RhoZCDP(),
-                [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.0]})],
+                [pd.DataFrame({"A": ["0", "1"], "var": [0.25, np.nan]})],
             ),
             (  # BoundedSum on floating-point valued measure column with LAPLACE
                 GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                     measure_column="X",
                     low=0.0,
@@ -966,30 +967,30 @@
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         mechanism=StdevMechanism.GAUSSIAN,
                     ),
                     RhoZCDP(),
-                    [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471404, 0.5]})],
+                    [pd.DataFrame({"A": ["0", "1"], "stdev": [0.5, np.nan]})],
                 ]
             ),
             (  # BoundedVariance on floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedVariance(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         output_column="var",
                         mechanism=VarianceMechanism.GAUSSIAN,
                     ),
                     RhoZCDP(),
-                    [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.25]})],
+                    [pd.DataFrame({"A": ["0", "1"], "var": [0.25, np.nan]})],
                 ]
             ),
             (  # BoundedSum on floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedSum(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
```

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_query_expression.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_query_expression.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_query_expression_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_schema.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_session.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_table_identifiers.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/test/unit/test_utils.py` & `tmlt_analytics-0.9.0rc6/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/__init__.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """`Tumult Labs' <https://tmlt.io>`_ differentially private analytics library."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2024
 
 # These gets automatically replaced by the version number during the release process
 # by poetry-dynamic-versioning.
-__version__ = "0.9.0-rc.5"
-__version_tuple__ = (0, 9, 0, "rc", 5)
+__version__ = "0.9.0-rc.6"
+__version_tuple__ = (0, 9, 0, "rc", 6)
 
 from typing import List
 
 from tmlt.core.utils.configuration import check_java11
 
 __all__: List[str] = []
```

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_base_builder.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_base_builder.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_coerce_spark_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_neighboring_relation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_schema.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_table_identifier.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_table_reference.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/binning_spec.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_base.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_simplify.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/constraints/_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/keyset.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/query_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2290,15 +2290,15 @@
             >>> # Answering the query with infinite privacy budget
             >>> answer = sess.evaluate(
             ...     query,
             ...     PureDPBudget(float("inf"))
             ... )
             >>> answer.toPandas()
                B_variance
-            0    0.666667
+            0         1.0
 
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
@@ -2373,16 +2373,16 @@
             ... )
             >>> # Answering the query with infinite privacy budget
             >>> answer = sess.evaluate(
             ...     query,
             ...     PureDPBudget(float("inf"))
             ... )
             >>> answer.toPandas()
-                B_stdev
-            0  0.816497
+               B_stdev
+            0      1.0
 
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
@@ -3105,14 +3105,15 @@
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import tmlt.analytics.session
             >>> import pandas as pd
+            >>> import numpy as np
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
             ... )
@@ -3143,15 +3144,15 @@
             >>> # Answering the query with infinite privacy budget
             >>> answer = sess.evaluate(
             ...     query,
             ...     PureDPBudget(float("inf"))
             ... )
             >>> answer.sort("A").toPandas()
                A  B_variance
-            0  0         1.0
+            0  0         NaN
             1  1         1.0
 
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
@@ -3238,15 +3239,15 @@
             >>> # Answering the query with infinite privacy budget
             >>> answer = sess.evaluate(
             ...     query,
             ...     PureDPBudget(float("inf"))
             ... )
             >>> answer.sort("A").toPandas()
                A  B_stdev
-            0  0      1.0
+            0  0      NaN
             1  1      1.0
 
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
```

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/query_expr.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/session.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,19 @@
 from pyspark.sql import SparkSession  # pylint: disable=unused-import
 from pyspark.sql import DataFrame
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.interactive_measurements import (
     InactiveAccountantError,
-    InsufficientBudgetError,
     PrivacyAccountant,
     PrivacyAccountantState,
     SequentialComposition,
 )
-from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.measures import ApproxDP, InsufficientBudgetError, PureDP, RhoZCDP
 from tmlt.core.metrics import (
     DictMetric,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -1086,15 +1085,17 @@
                 )
             try:
                 answers = self._accountant.measure(
                     measurement, d_out=adjusted_budget.value
                 )
             except InsufficientBudgetError as err:
                 msg = _format_insufficient_budget_msg(
-                    err.requested_budget, err.remaining_budget, privacy_budget
+                    err.requested_budget.value,
+                    err.remaining_budget.value,
+                    privacy_budget,
                 )
                 raise RuntimeError(
                     "Cannot answer query without exceeding the Session privacy budget."
                     + msg
                 ) from err
 
             if len(answers) != 1:
@@ -1490,15 +1491,15 @@
             ... )
             >>> count_answer.toPandas() # doctest: +NORMALIZE_WHITESPACE, +ELLIPSIS
                count
             0    ...
 
         Args:
             source_id: The private source to partition.
-            privacy_budget: Amount of privacy budget to pass to each new session.
+            privacy_budget: Privacy budget to pass to each new session.
             column: The name of the column partitioning on.
             splits: Mapping of split name to value of partition.
                 Split name is ``source_id`` in new session.
         """
         # pylint: enable=line-too-long
         # If you remove this if-block, mypy will complain
         if not (
@@ -1545,15 +1546,15 @@
                 "This session is no longer active. Either it was manually stopped"
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
             ) from e
         except InsufficientBudgetError as err:
             msg = _format_insufficient_budget_msg(
-                err.requested_budget, err.remaining_budget, privacy_budget
+                err.requested_budget.value, err.remaining_budget.value, privacy_budget
             )
             raise RuntimeError(
                 "Cannot perform this partition without exceeding "
                 "the Session privacy budget." + msg
             ) from err
 
         # We now have split accountants, and names for each.
```

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/tmlt/analytics/utils.py` & `tmlt_analytics-0.9.0rc6/tmlt/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.9.0rc5/setup.py` & `tmlt_analytics-0.9.0rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
  'tmlt.analytics.constraints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['sympy>=1.8,<1.10',
- 'tmlt.core>=0.12.0,<0.13.0',
+ 'tmlt.core>=0.13.0,<0.14.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=4.1.0,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['pandas>=1.2.0,<1.4.0',
                              'pyspark[sql]>=3.0.0,<3.4.0'],
  ':python_version >= "3.10" and python_version < "3.11"': ['pandas>=1.4.0,<2.0.0'],
  ':python_version >= "3.11"': ['pandas>=1.5.0,<2.0.0',
                                'pyspark[sql]>=3.4.0,<3.6.0'],
  ':python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.2.0,<2.0.0'],
  ':python_version >= "3.8" and python_version < "3.11"': ['pyspark[sql]>=3.0.0,<3.6.0']}
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.9.0rc5',
+    'version': '0.9.0rc6',
     'description': "Tumult's differential privacy analytics API",
     'long_description': "[![PyPI - Version](https://img.shields.io/pypi/v/tmlt-analytics?color=006dad)](https://pypi.org/project/tmlt-analytics/) |\n[![Documentation - Latest](https://img.shields.io/badge/documentation-latest-cc3d56)](https://docs.tmlt.dev/analytics/latest/) |\n[![Join our Slack!](https://img.shields.io/badge/Join%20our%20Slack!-634ad3?logo=slack)](https://tmlt.dev/slack)\n\n# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Demo video\n\nWant to see Tumult Analytics in action? Check out this video introducing the\ninterface fundamentals:\n\n[![Screenshot of the demo video](https://img.youtube.com/vi/SNfbYOp0CEs/0.jpg)](https://www.youtube.com/watch?v=SNfbYOp0CEs)\n\nA selection of more advanced features is shown on the second part of this demo,\nin a [separate video](https://www.youtube.com/watch?v=BRUPlfwzHHo).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions, feedback, or feature requests, please reach out to us on [Slack](https://tmlt.dev/slack).\n\n## Contributing\n\nWe do not yet have a process in place to accept external contributions, but we are open to collaboration opportunities.\nIf you are interested in contributing, please let us know [via Slack](https://tmlt.dev/slack).\n\nSee [CONTRIBUTING.md](https://gitlab.com/tumult-labs/analytics/-/blob/dev/CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nTumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nTumult Analytics' documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
```

### Comparing `tmlt_analytics-0.9.0rc5/PKG-INFO` & `tmlt_analytics-0.9.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.9.0rc5
+Version: 0.9.0rc6
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.12.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -24,15 +24,15 @@
 Requires-Dist: pandas (>=1.2.0,<2.0.0); python_version >= "3.8" and python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0); python_version >= "3.10" and python_version < "3.11"
 Requires-Dist: pandas (>=1.5.0,<2.0.0); python_version >= "3.11"
 Requires-Dist: pyspark[sql] (>=3.0.0,<3.4.0); python_version < "3.8"
 Requires-Dist: pyspark[sql] (>=3.0.0,<3.6.0); python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: pyspark[sql] (>=3.4.0,<3.6.0); python_version >= "3.11"
 Requires-Dist: sympy (>=1.8,<1.10)
-Requires-Dist: tmlt.core (>=0.12.0,<0.13.0)
+Requires-Dist: tmlt.core (>=0.13.0,<0.14.0)
 Requires-Dist: typeguard (>=2.12.1,<2.13.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Project-URL: Documentation, https://docs.tmlt.dev/analytics/latest
 Project-URL: Repository, https://gitlab.com/tumult-labs/analytics
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tmlt-analytics?color=006dad)](https://pypi.org/project/tmlt-analytics/) |
```

