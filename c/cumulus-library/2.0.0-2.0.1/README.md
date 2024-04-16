# Comparing `tmp/cumulus_library-2.0.0.tar.gz` & `tmp/cumulus_library-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-2.0.0.tar` & `cumulus_library-2.0.1.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-lrwxr-xr-x   0        0        0        0 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      689 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/README.md
--rw-r--r--   0        0        0     6523 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       46 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/base_table_builder.py
--rw-r--r--   0        0        0     2898 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/base_utils.py
--rwxr-xr-x   0        0        0    17396 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/cli.py
--rw-r--r--   0        0        0     7633 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0    14588 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/databases.py
--rw-r--r--   0        0        0      422 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/enums.py
--rw-r--r--   0        0        0      523 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/errors.py
--rw-r--r--   0        0        0      205 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2311 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0     1716 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/protected_table_builder.py
--rw-r--r--   0        0        0        0 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4731 2024-04-04 12:54:43.398847 cumulus_library-2.0.0/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3364 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6024 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0    10722 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/counts.py
--rw-r--r--   0        0        0    14371 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/psm.py
--rw-r--r--   0        0        0     5136 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/psm.sql
--rw-r--r--   0        0        0     7541 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/count.sql.jinja
--rw-r--r--   0        0        0     2311 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/counts_templates.py
--rw-r--r--   0        0        0     1606 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
--rw-r--r--   0        0        0      363 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
--rw-r--r--   0        0        0     3272 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_templates.py
--rw-r--r--   0        0        0     2943 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_condition.py
--rw-r--r--   0        0        0     2710 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_documentreference.py
--rw-r--r--   0        0        0     4562 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_encounter.py
--rw-r--r--   0        0        0     4731 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_medication.py
--rw-r--r--   0        0        0     2241 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_medicationrequest.py
--rw-r--r--   0        0        0     2734 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_observation.py
--rw-r--r--   0        0        0     2039 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_patient.py
--rw-r--r--   0        0        0      867 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/builder_prereq_tables.py
--rw-r--r--   0        0        0     2548 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/condition.sql.jinja
--rw-r--r--   0        0        0      854 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_templates.py
--rw-r--r--   0        0        0     5042 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_utils.jinja
--rw-r--r--   0        0        0     2765 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
--rw-r--r--   0        0        0     4311 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja
--rw-r--r--   0        0        0     5984 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medication.sql.jinja
--rw-r--r--   0        0        0     2058 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
--rw-r--r--   0        0        0     3331 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/observation.sql.jinja
--rw-r--r--   0        0        0     1854 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/patient.sql.jinja
--rw-r--r--   0        0        0     5350 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0      948 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/fhir_lookup_tables.sql
--rw-r--r--   0        0        0     4879 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/fhir_mapping_tables.sql
--rw-r--r--   0        0        0      971 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1163 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/observation_type.sql
--rw-r--r--   0        0        0     7810 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_condition.sql
--rw-r--r--   0        0        0     5116 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
--rw-r--r--   0        0        0    16576 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql
--rw-r--r--   0        0        0     1243 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medication.sql
--rw-r--r--   0        0        0     3286 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
--rw-r--r--   0        0        0     6190 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_observation.sql
--rw-r--r--   0        0        0     8484 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_patient.sql
--rw-r--r--   0        0        0     8008 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
--rw-r--r--   0        0        0    29145 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/count_core.sql
--rw-r--r--   0        0        0     1440 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     2058 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0       69 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/core/version.sql
--rw-r--r--   0        0        0     2580 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/code_definitions.py
--rw-r--r--   0        0        0     2553 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/code_detection.py
--rw-r--r--   0        0        0     1978 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
--rw-r--r--   0        0        0     1618 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
--rw-r--r--   0        0        0      160 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/manifest.toml
--rw-r--r--   0        0        0     4377 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql
--rw-r--r--   0        0        0      863 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     2312 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2024-04-04 12:54:43.402847 cumulus_library-2.0.0/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2024-04-04 12:54:43.434847 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2024-04-04 12:54:43.514847 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      410 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      145 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     3227 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    31623 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/study_parser.py
--rw-r--r--   0        0        0       79 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/alias_table.sql.jinja
--rw-r--r--   0        0        0    11473 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/base_templates.py
--rw-r--r--   0        0        0     2532 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0     1893 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/coding_denormalize.sql.jinja
--rw-r--r--   0        0        0      385 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/column_datatype.sql.jinja
--rw-r--r--   0        0        0      563 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      586 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0      506 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/ctas_empty.sql.jinja
--rw-r--r--   0        0        0       61 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     2534 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      535 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0      439 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
--rw-r--r--   0        0        0       34 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/select_all.sql.jinja
--rw-r--r--   0        0        0      370 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
--rw-r--r--   0        0        0      169 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0      163 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0    10628 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/template_sql/sql_utils.py
--rw-r--r--   0        0        0     3308 2024-04-04 12:54:43.522848 cumulus_library-2.0.0/cumulus_library/upload.py
--rw-r--r--   0        0        0     2316 2024-04-04 12:54:43.526847 cumulus_library-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 cumulus_library-2.0.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      689 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/README.md
+-rw-r--r--   0        0        0     6677 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       46 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/__init__.py
+-rw-r--r--   0        0        0     4837 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/base_table_builder.py
+-rw-r--r--   0        0        0     2898 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/base_utils.py
+-rwxr-xr-x   0        0        0    17396 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/cli.py
+-rw-r--r--   0        0        0     7923 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0    15082 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/databases.py
+-rw-r--r--   0        0        0      422 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/enums.py
+-rw-r--r--   0        0        0      523 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/errors.py
+-rw-r--r--   0        0        0      205 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2311 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0     1716 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/protected_table_builder.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4731 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3364 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6024 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0    10730 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/counts.py
+-rw-r--r--   0        0        0    14371 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/psm.py
+-rw-r--r--   0        0        0     5136 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/psm.sql
+-rw-r--r--   0        0        0     7541 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/count.sql.jinja
+-rw-r--r--   0        0        0     2311 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/counts_templates.py
+-rw-r--r--   0        0        0     1606 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
+-rw-r--r--   0        0        0      363 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
+-rw-r--r--   0        0        0     3272 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_templates.py
+-rw-r--r--   0        0        0     2943 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_condition.py
+-rw-r--r--   0        0        0     2710 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_documentreference.py
+-rw-r--r--   0        0        0     4776 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_encounter.py
+-rw-r--r--   0        0        0     4731 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_medication.py
+-rw-r--r--   0        0        0     2241 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_medicationrequest.py
+-rw-r--r--   0        0        0     2734 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_observation.py
+-rw-r--r--   0        0        0     2039 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_patient.py
+-rw-r--r--   0        0        0      867 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_prereq_tables.py
+-rw-r--r--   0        0        0     2555 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/completion_utils.jinja
+-rw-r--r--   0        0        0     2548 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/condition.sql.jinja
+-rw-r--r--   0        0        0      854 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_templates.py
+-rw-r--r--   0        0        0     5042 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_utils.jinja
+-rw-r--r--   0        0        0     2782 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
+-rw-r--r--   0        0        0     4718 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/encounter.sql.jinja
+-rw-r--r--   0        0        0      274 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/incomplete_encounter.sql.jinja
+-rw-r--r--   0        0        0     5984 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medication.sql.jinja
+-rw-r--r--   0        0        0     2058 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
+-rw-r--r--   0        0        0     3331 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/observation.sql.jinja
+-rw-r--r--   0        0        0     1854 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/patient.sql.jinja
+-rw-r--r--   0        0        0     5350 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0      948 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/fhir_lookup_tables.sql
+-rw-r--r--   0        0        0     4879 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/fhir_mapping_tables.sql
+-rw-r--r--   0        0        0      971 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1163 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/observation_type.sql
+-rw-r--r--   0        0        0     7810 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_condition.sql
+-rw-r--r--   0        0        0     5213 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
+-rw-r--r--   0        0        0    20656 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_encounter.sql
+-rw-r--r--   0        0        0     1243 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medication.sql
+-rw-r--r--   0        0        0     3286 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
+-rw-r--r--   0        0        0     6190 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_observation.sql
+-rw-r--r--   0        0        0     8678 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_patient.sql
+-rw-r--r--   0        0        0     8008 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
+-rw-r--r--   0        0        0    29070 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/count_core.sql
+-rw-r--r--   0        0        0     1440 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     2058 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0       69 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/version.sql
+-rw-r--r--   0        0        0     2580 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/code_definitions.py
+-rw-r--r--   0        0        0     2553 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/code_detection.py
+-rw-r--r--   0        0        0     1978 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
+-rw-r--r--   0        0        0     1618 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
+-rw-r--r--   0        0        0      160 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/manifest.toml
+-rw-r--r--   0        0        0     4622 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/reference_sql/code_detection.sql
+-rw-r--r--   0        0        0      863 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     2312 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2024-04-16 16:14:11.645901 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2024-04-16 16:14:11.729900 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      410 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      145 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     3227 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    31623 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0       79 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/alias_table.sql.jinja
+-rw-r--r--   0        0        0    11473 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/base_templates.py
+-rw-r--r--   0        0        0     2532 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0     1893 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/coding_denormalize.sql.jinja
+-rw-r--r--   0        0        0      385 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/column_datatype.sql.jinja
+-rw-r--r--   0        0        0      563 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      586 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0      506 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/ctas_empty.sql.jinja
+-rw-r--r--   0        0        0       61 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     2534 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      535 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0      439 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/is_table_not_empty.sql.jinja
+-rw-r--r--   0        0        0       34 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/select_all.sql.jinja
+-rw-r--r--   0        0        0      370 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
+-rw-r--r--   0        0        0      169 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0      163 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0    10628 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/sql_utils.py
+-rw-r--r--   0        0        0     3308 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/upload.py
+-rw-r--r--   0        0        0     2316 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 cumulus_library-2.0.1/PKG-INFO
```

### Comparing `cumulus_library-2.0.0/README.md` & `cumulus_library-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/.sqlfluff` & `cumulus_library-2.0.1/cumulus_library/.sqlfluff`

 * *Files 5% similar despite different names*

```diff
@@ -139,15 +139,21 @@
             'class': {
                 'code': True, 'system': True, 'display': False, 'userSelected': True, 'version': True
             }, 
             'subject': {
                 'reference': True, 'display': False, 'type': True
             }, 
             'id': True
-        }, 
+        },
+        'etl__completion': {
+            'group_name': True,
+        },
+        'etl__completion_encounters': {
+            'group_name': True,
+        },
         'medicationrequest': {
             'id': True, 
             'status': True, 
             'intent': True, 
             'authoredOn': True, 
             'category': {
                 'code': True, 'system': True, 'display': False
```

### Comparing `cumulus_library-2.0.0/cumulus_library/base_table_builder.py` & `cumulus_library-2.0.1/cumulus_library/base_table_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/base_utils.py` & `cumulus_library-2.0.1/cumulus_library/base_utils.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/cli.py` & `cumulus_library-2.0.1/cumulus_library/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/cli_parser.py` & `cumulus_library-2.0.1/cumulus_library/cli_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,16 +72,21 @@
     aws.add_argument(
         "--region",
         help="AWS region data of Athena instance (default: us-east-1)",
         default="us-east-1",
     )
 
 
-def add_db_config(parser: argparse.ArgumentParser) -> None:
-    """Adds arguments related to database backends to a subparser"""
+def add_db_config(parser: argparse.ArgumentParser, input_mode: bool = False) -> None:
+    """
+    Adds arguments related to database backends to a subparser
+
+    Pass input_mode=True if the subparser is for a command that operates on input
+    (e.g. a build operation) rather than output tables (e.g. a clean operation)
+    """
     group = parser.add_argument_group("Database config")
     group.add_argument(
         "--db-type",
         help="Which database backend to use (default athena)",
         choices=["athena", "duckdb"],
         default="athena",
     )
@@ -95,14 +100,21 @@
         # Since we started as an Athena-centric codebase, we mostly keep referring to
         # this as name "schema_name". But to the user, both uses are still conceptually
         # a "database".
         dest="schema_name",
         help="Database name (for Athena) or file (for DuckDB)",
     )
 
+    if input_mode:
+        group.add_argument(
+            "--load-ndjson-dir",
+            help="Load ndjson files from this folder",
+            metavar="DIR",
+        )
+
     # Backend-specific config:
     add_aws_config(parser)
 
 
 def get_parser() -> argparse.ArgumentParser:
     """Provides parser for handling CLI arguments"""
     parser = argparse.ArgumentParser(
@@ -155,29 +167,26 @@
         "build",
         help="Removes and recreates Athena tables & views for specified studies",
     )
     add_target_argument(build)
     add_table_builder_argument(build)
     add_study_dir_argument(build)
     add_verbose_argument(build)
-    add_db_config(build)
+    add_db_config(build, input_mode=True)
     add_data_path_argument(build)
     build.add_argument(
         "--statistics",
         action="store_true",
         help=(
             "Force regenerating statistics data from latest dataset. "
             "Stats are created by default when study is initially run"
         ),
         dest="stats_build",
     )
     build.add_argument(
-        "--load-ndjson-dir", help="Load ndjson files from this folder", metavar="DIR"
-    )
-    build.add_argument(
         "--continue",
         dest="continue_from",
         help=argparse.SUPPRESS,
     )
 
     # Database export
 
@@ -224,15 +233,15 @@
 
     # Generate a study's template-driven sql
     sql = actions.add_parser(
         "generate-sql", help="Generates a study's template-driven sql for reference"
     )
     add_target_argument(sql)
     add_study_dir_argument(sql)
-    add_db_config(sql)
+    add_db_config(sql, input_mode=True)
     add_table_builder_argument(sql)
 
     # Generate markdown tables for documentation
     markdown = actions.add_parser(
         "generate-md", help="Generates markdown tables for study documentation"
     )
     add_target_argument(markdown)
```

### Comparing `cumulus_library-2.0.0/cumulus_library/databases.py` & `cumulus_library-2.0.1/cumulus_library/databases.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,14 +331,33 @@
         # since we're defaulting to athena naming conventions elsewhere,
         # we'll lower case all the keys
         schema = {k.lower(): v for k, v in schema.items()}
 
         return self._parse_found_schema(expected, schema)
 
 
+def _read_rows_from_table_dir(path: str) -> list[dict]:
+    # Grab filenames to load (ignoring .meta files and handling missing folders)
+    folder = Path(path)
+    filenames = []
+    if folder.exists():
+        filenames = sorted(
+            str(x) for x in folder.iterdir() if x.name.endswith(".ndjson")
+        )
+
+    # Read all ndjson directly into memory
+    rows = []
+    for filename in filenames:
+        with open(filename, encoding="utf8") as f:
+            for line in f:
+                rows.append(json.loads(line))
+
+    return rows
+
+
 def read_ndjson_dir(path: str) -> dict[str, pyarrow.Table]:
     """Loads a directory tree of raw ndjson into schema-ful tables.
 
     :param path: a directory path
     :returns: dictionary of table names (like 'documentreference') to table
       data (with schema)
     """
@@ -359,34 +378,31 @@
         "Observation",
         "Patient",
         "Procedure",
         "ServiceRequest",
     ]
     for resource in resources:
         table_name = resource.lower()
-
-        # Grab filenames to load (ignoring .meta files and handling missing folders)
-        folder = Path(f"{path}/{table_name}")
-        filenames = []
-        if folder.exists():
-            filenames = sorted(
-                str(x) for x in folder.iterdir() if x.name.endswith(".ndjson")
-            )
-
-        # Read all ndjson directly into memory
-        rows = []
-        for filename in filenames:
-            with open(filename, encoding="utf8") as f:
-                for line in f:
-                    rows.append(json.loads(line))
+        rows = _read_rows_from_table_dir(f"{path}/{table_name}")
 
         # Make a pyarrow table with full schema from the data
         schema = cumulus_fhir_support.pyarrow_schema_from_rows(resource, rows)
         all_tables[table_name] = pyarrow.Table.from_pylist(rows, schema)
 
+    # And now some special support for a few ETL tables.
+    metadata_tables = [
+        "etl__completion",
+        "etl__completion_encounters",
+    ]
+    for metadata_table in metadata_tables:
+        rows = _read_rows_from_table_dir(f"{path}/{metadata_table}")
+        if rows:
+            # Auto-detecting the schema works for these simple tables
+            all_tables[metadata_table] = pyarrow.Table.from_pylist(rows)
+
     return all_tables
 
 
 def create_db_backend(args: dict[str, str]) -> DatabaseBackend:
     db_type = args["db_type"]
     database = args["schema_name"]
     load_ndjson_dir = args.get("load_ndjson_dir")
```

### Comparing `cumulus_library-2.0.0/cumulus_library/errors.py` & `cumulus_library-2.0.1/cumulus_library/errors.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-2.0.1/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/protected_table_builder.py` & `cumulus_library-2.0.1/cumulus_library/protected_table_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/schema/columns.py` & `cumulus_library-2.0.1/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/schema/typesystem.py` & `cumulus_library-2.0.1/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/schema/valueset.py` & `cumulus_library-2.0.1/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/counts.py` & `cumulus_library-2.0.1/cumulus_library/statistics/counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,19 @@
 
     def get_where_clauses(
         self, clause: list | str | None = None, min_subject: int = 10
     ) -> str:
         """Convenience method for constructing arbitrary where clauses.
 
         :param clause: either a string or a list of sql where statements
-        :param min_subject: if clause is none, the bin size for a cnt_subject filter
+        :param min_subject: if clause is none, the bin size for a cnt_subject_ref filter
             (deprecated, use count_[fhir_resource](min_subject) instead)
         """
         if clause is None:
-            return [f"cnt_subject >= {min_subject}"]
+            return [f"cnt_subject_ref >= {min_subject}"]
         elif isinstance(clause, str):
             return [clause]
         elif isinstance(clause, list):
             return clause
         else:
             raise CountsBuilderError(f"get_where_clauses invalid clause {clause}")
```

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/psm.py` & `cumulus_library-2.0.1/cumulus_library/statistics/psm.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/psm.sql` & `cumulus_library-2.0.1/cumulus_library/statistics/psm.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/count.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/count.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/counts_templates.py` & `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/counts_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/statistics/statistics_templates/psm_templates.py` & `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_condition.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_condition.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_documentreference.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_documentreference.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_encounter.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_encounter.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,21 @@
         ],
         "subject": [
             "reference",
             "display",
             "type",
         ],
         "id": [],
-    }
+    },
+    "etl__completion": {
+        "group_name": [],
+    },
+    "etl__completion_encounters": {
+        "group_name": [],
+    },
 }
 
 
 @dataclass(kw_only=True)
 class EncConfig(sql_utils.CodeableConceptConfig):
     """Convenience wrapper for CodeableConceptConfig"""
 
@@ -122,10 +128,11 @@
         self.denormalize_codes(
             schema,
             cursor,
         )
         validated_schema = core_templates.validate_schema(
             cursor, schema, expected_table_cols, parser
         )
-        self.queries.append(
-            core_templates.get_core_template("encounter", validated_schema)
-        )
+        self.queries += [
+            core_templates.get_core_template("encounter", validated_schema),
+            core_templates.get_core_template("incomplete_encounter", validated_schema),
+        ]
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_medication.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_medication.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_medicationrequest.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_medicationrequest.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_observation.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_observation.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_patient.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_patient.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/builder_prereq_tables.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/builder_prereq_tables.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/condition.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/condition.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_templates.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/core_utils.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/documentreference.sql.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 {% if schema["documentreference"]["context"]["encounter"] %}
         context_encounter.encounter.reference AS encounter_ref
     FROM temp_documentreference AS tdr,
          unnest(context.encounter) AS context_encounter (encounter) --noqa
 
 {% else %}
-        '' AS encounter_ref
+        cast('' AS varchar) AS encounter_ref
     FROM temp_documentreference AS tdr
     WHERE 1=0 -- forces an empty table
 
 {% endif %}
 )
 
 SELECT DISTINCT
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/encounter.sql.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 {% import 'core_utils.jinja' as utils %}
+{% import 'completion_utils.jinja' as completion_utils %}
 {#- Unlike some of the other core templates, in order to get easier access
 to the nested dates in the period, we'll do the preliminary querying in
 two steps.
 
 TODO: profile speed vs a single step, consider extending date col methods
 to traverse nested elements if performance is impacted-#}
 CREATE TABLE core__encounter AS
-WITH temp_encounter_nullable AS (
+WITH
+
+temp_encounter_completion AS {{ completion_utils.complete_encounters(schema) }},
+
+temp_encounter_nullable AS (
     SELECT DISTINCT
         {{- utils.basic_cols(
                 'encounter',
                 'e',
                 [
                     'id'
                 ], 
@@ -47,14 +52,20 @@
                     ('period', 'start', 'period_start_month', 'month'),
                     ('period', 'start', 'period_start_year', 'year'),
                 ],
                 schema
             ) 
         }}
     FROM encounter AS e
+    LEFT JOIN temp_encounter_completion AS tec ON tec.id = e.id
+    WHERE (
+        -- NULL completion just means it's a row that isn't completion-tracked
+        -- (likely a legacy row), so allow it in.
+        tec.is_complete IS NULL OR tec.is_complete
+    )
 ),
 
 temp_encounter AS (
     SELECT DISTINCT
         e.id,
         e.status,
         e.class,
@@ -64,16 +75,16 @@
         e.period_end_day,
         e.period_start_week,
         e.period_start_month,
         e.period_start_year,
         edt.code AS type_code,
         edt.code_system AS type_code_system,
         edt.display AS type_display,
-        eds.code AS seviceType_code,
-        eds.code_system AS seviceType_code_system,
+        eds.code AS serviceType_code,
+        eds.code_system AS serviceType_code_system,
         eds.display AS serviceType_display,
         edp.code AS priority_code,
         edp.code_system AS priority_code_system,
         edp.display AS priority_display,
         edr.code AS reasonCode_code,
         edr.code_system AS reasonCode_code_system,
         edr.display AS reasonCode_display,
@@ -93,16 +104,16 @@
     e.id,
     e.status,
     ac.code AS class_code,
     ac.display AS class_display,
     e.type_code,
     e.type_code_system,
     e.type_display,
-    e.seviceType_code,
-    e.seviceType_code_system,
+    e.serviceType_code,
+    e.serviceType_code_system,
     e.serviceType_display,
     e.priority_code,
     e.priority_code_system,
     e.priority_display,
     e.reasonCode_code,
     e.reasonCode_code_system,
     e.reasonCode_display,
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medication.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medication.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/observation.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/observation.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/core_templates/patient.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/patient.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/count_core.py` & `cumulus_library-2.0.1/cumulus_library/studies/core/count_core.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/fhir_lookup_tables.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/fhir_lookup_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/fhir_mapping_tables.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/fhir_mapping_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/manifest.toml` & `cumulus_library-2.0.1/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/observation_type.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/observation_type.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_condition.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_documentreference.sql`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
         dr.id,
         dr.type,
         dr.status,
         cast(NULL as timestamp) AS "date",
         dr.docStatus,
         dr.context,
         dr.subject.reference AS subject_ref,
-        cast(NULL as varchar) AS encounter_ref,
         dr.context.period.start AS author_date,
         date_trunc('day', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_day,
         date_trunc('week', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_week,
         date_trunc('month', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_month,
@@ -159,14 +158,25 @@
         cdrt.display as type_display,
         cdrc.code as category_code,
         cdrf.code as format_code
     FROM documentreference AS dr
     LEFT JOIN core__documentreference_dn_type AS cdrt ON dr.id = cdrt.id
     LEFT JOIN core__documentreference_dn_category AS cdrc ON dr.id = cdrc.id
     LEFT JOIN core__documentreference_dn_format AS cdrf ON dr.id = cdrf.id
+),
+
+temp_encounters AS (
+    SELECT
+        tdr.id,
+
+
+        context_encounter.encounter.reference AS encounter_ref
+    FROM temp_documentreference AS tdr,
+         unnest(context.encounter) AS context_encounter (encounter) --noqa
+
 
 )
 
 SELECT DISTINCT
     tdr.id,
     tdr.status,
     tdr.type_code,
@@ -177,12 +187,12 @@
     tdr."date",
     tdr.author_day,
     tdr.author_week,
     tdr.author_month,
     tdr.author_year,
     tdr.format_code,
     tdr.subject_ref,
-    coalesce(tdr.encounter_ref, context_encounter.encounter.reference) as encounter_ref,
+    te.encounter_ref,
     concat('DocumentReference/', tdr.id) AS documentreference_ref
-FROM temp_documentreference AS tdr,
-    unnest(context.encounter) AS context_encounter (encounter) --noqa
+FROM temp_documentreference AS tdr
+LEFT JOIN temp_encounters AS te ON tdr.id = te.id
 WHERE date(tdr.author_day) BETWEEN date('2016-06-01') AND current_date;
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_encounter.sql`

 * *Files 24% similar despite different names*

```diff
@@ -473,16 +473,62 @@
         display
     FROM union_table
 );
 
 
 -- ###########################################################
 
+
 CREATE TABLE core__encounter AS
-WITH temp_encounter_nullable AS (
+WITH
+
+temp_encounter_completion AS (
+    WITH
+    -- Start by grabbing group names and exports times for each Encounter.
+    temp_completion_times AS (
+        SELECT
+            ece.encounter_id,
+            -- note that we don't chop the export time down to a DATE,
+            -- as is typical in the core study
+            min(from_iso8601_timestamp(ece.export_time)) AS earliest_export
+        FROM etl__completion_encounters AS ece
+        GROUP BY ece.encounter_id
+    ),
+
+    -- Then examine all tables that are at least as recently loaded as the
+    -- Encounter. (This is meant to detect Conditions that maybe aren't
+    -- loaded into Athena yet for the Encounter.)
+    -- Make sure that we have all the tables we care about.
+    temp_completed_tables AS (
+        SELECT
+            ece.encounter_id,
+            (
+                BOOL_OR(ec.table_name = 'condition')
+                AND BOOL_OR(ec.table_name = 'documentreference')
+                AND BOOL_OR(ec.table_name = 'medicationrequest')
+                AND BOOL_OR(ec.table_name = 'observation')
+            ) AS is_complete
+        FROM etl__completion_encounters AS ece
+        INNER JOIN temp_completion_times AS tct ON tct.encounter_id = ece.encounter_id
+        INNER JOIN etl__completion AS ec ON ec.group_name = ece.group_name
+        WHERE tct.earliest_export <= from_iso8601_timestamp(ec.export_time)
+        GROUP BY ece.encounter_id
+    )
+
+    -- Left join back with main completion_encounters table,
+    -- to catch rows that are completion-tracked but not in
+    -- temp_completed_tables.
+    SELECT
+        ece.encounter_id AS id,
+        (is_complete IS NOT NULL AND is_complete) AS is_complete
+    FROM etl__completion_encounters AS ece
+    LEFT JOIN temp_completed_tables AS tct ON tct.encounter_id = ece.encounter_id
+),
+
+temp_encounter_nullable AS (
     SELECT DISTINCT
         e.id,
         e.status,
         e.class,
         e.subject.reference AS subject_ref,
         e.period,
         date(from_iso8601_timestamp(e.period.start)) AS period_start,
@@ -493,14 +539,20 @@
         date_trunc('week', date(from_iso8601_timestamp(e."period"."start")))
             AS period_start_week,
         date_trunc('month', date(from_iso8601_timestamp(e."period"."start")))
             AS period_start_month,
         date_trunc('year', date(from_iso8601_timestamp(e."period"."start")))
             AS period_start_year
     FROM encounter AS e
+    LEFT JOIN temp_encounter_completion AS tec ON tec.id = e.id
+    WHERE (
+        -- NULL completion just means it's a row that isn't completion-tracked
+        -- (likely a legacy row), so allow it in.
+        tec.is_complete IS NULL OR tec.is_complete
+    )
 ),
 
 temp_encounter AS (
     SELECT DISTINCT
         e.id,
         e.status,
         e.class,
@@ -510,16 +562,16 @@
         e.period_end_day,
         e.period_start_week,
         e.period_start_month,
         e.period_start_year,
         edt.code AS type_code,
         edt.code_system AS type_code_system,
         edt.display AS type_display,
-        eds.code AS seviceType_code,
-        eds.code_system AS seviceType_code_system,
+        eds.code AS serviceType_code,
+        eds.code_system AS serviceType_code_system,
         eds.display AS serviceType_display,
         edp.code AS priority_code,
         edp.code_system AS priority_code_system,
         edp.display AS priority_display,
         edr.code AS reasonCode_code,
         edr.code_system AS reasonCode_code_system,
         edr.display AS reasonCode_display,
@@ -527,28 +579,28 @@
         edd.code_system AS dischargeDisposition_code_system,
         edd.display AS dischargeDisposition_display
 
     FROM temp_encounter_nullable AS e
     LEFT JOIN core__encounter_dn_priority AS edt ON e.id = edt.id
     LEFT JOIN core__encounter_dn_servicetype AS eds ON e.id = eds.id
     LEFT JOIN core__encounter_dn_priority AS edp ON e.id = edp.id
-    LEFT JOIN core__encounter_dn_reasonCode AS edr ON e.id = edr.id
-    LEFT JOIN core__encounter_dn_dischargeDisposition AS edd ON e.id = edd.id
+    LEFT JOIN core__encounter_dn_reasoncode AS edr ON e.id = edr.id
+    LEFT JOIN core__encounter_dn_dischargedisposition AS edd ON e.id = edd.id
 )
 
 SELECT DISTINCT
     e.id,
     e.status,
     ac.code AS class_code,
     ac.display AS class_display,
     e.type_code,
     e.type_code_system,
     e.type_display,
-    e.seviceType_code,
-    e.seviceType_code_system,
+    e.serviceType_code,
+    e.serviceType_code_system,
     e.serviceType_display,
     e.priority_code,
     e.priority_code_system,
     e.priority_display,
     e.reasonCode_code,
     e.reasonCode_code_system,
     e.reasonCode_display,
@@ -570,7 +622,59 @@
 FROM temp_encounter AS e
 LEFT JOIN core__fhir_mapping_expected_act_encounter_code_v3 AS eac
     ON e.class.code = eac.found
 LEFT JOIN core__fhir_act_encounter_code_v3 AS ac ON eac.expected = ac.code
 INNER JOIN core__patient AS p ON e.subject_ref = p.subject_ref
 WHERE
     e.period_start_day BETWEEN date('2016-06-01') AND current_date;
+
+-- ###########################################################
+
+
+CREATE TABLE core__incomplete_encounter AS
+WITH
+temp_encounter_completion AS (
+    WITH
+    -- Start by grabbing group names and exports times for each Encounter.
+    temp_completion_times AS (
+        SELECT
+            ece.encounter_id,
+            -- note that we don't chop the export time down to a DATE,
+            -- as is typical in the core study
+            min(from_iso8601_timestamp(ece.export_time)) AS earliest_export
+        FROM etl__completion_encounters AS ece
+        GROUP BY ece.encounter_id
+    ),
+
+    -- Then examine all tables that are at least as recently loaded as the
+    -- Encounter. (This is meant to detect Conditions that maybe aren't
+    -- loaded into Athena yet for the Encounter.)
+    -- Make sure that we have all the tables we care about.
+    temp_completed_tables AS (
+        SELECT
+            ece.encounter_id,
+            (
+                BOOL_OR(ec.table_name = 'condition')
+                AND BOOL_OR(ec.table_name = 'documentreference')
+                AND BOOL_OR(ec.table_name = 'medicationrequest')
+                AND BOOL_OR(ec.table_name = 'observation')
+            ) AS is_complete
+        FROM etl__completion_encounters AS ece
+        INNER JOIN temp_completion_times AS tct ON tct.encounter_id = ece.encounter_id
+        INNER JOIN etl__completion AS ec ON ec.group_name = ece.group_name
+        WHERE tct.earliest_export <= from_iso8601_timestamp(ec.export_time)
+        GROUP BY ece.encounter_id
+    )
+
+    -- Left join back with main completion_encounters table,
+    -- to catch rows that are completion-tracked but not in
+    -- temp_completed_tables.
+    SELECT
+        ece.encounter_id AS id,
+        (is_complete IS NOT NULL AND is_complete) AS is_complete
+    FROM etl__completion_encounters AS ece
+    LEFT JOIN temp_completed_tables AS tct ON tct.encounter_id = ece.encounter_id
+)
+
+SELECT DISTINCT tec.id
+FROM temp_encounter_completion AS tec
+WHERE NOT tec.is_complete
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medication.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medication.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_observation.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_patient.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_patient.sql`

 * *Files 4% similar despite different names*

```diff
@@ -262,29 +262,38 @@
         date(from_iso8601_timestamp(p.birthDate)) AS birthDate,
         er.race_display,
         ee.ethnicity_display
     FROM
         patient AS p
     LEFT JOIN core__patient_ext_race AS er ON p.id = er.id
     LEFT JOIN core__patient_ext_ethnicity AS ee ON p.id = ee.id
+),
+
+-- Grab a single address to use for this patient, if present
+temp_address AS (
+    SELECT
+        tp.id,
+        
+        
+        
+        substr(max(t_address.addr_row.postalcode), 1, 3) AS postalcode3
+    FROM
+        temp_patient AS tp,
+        unnest(tp.address) AS t_address (addr_row)
+    GROUP BY tp.id
 )
 
 SELECT DISTINCT
     tp.id,
     tp.gender,
     tp.birthDate,
-    CASE
-        WHEN
-            t_address.addr_row.postalcode IS NOT NULL
-            THEN substr(t_address.addr_row.postalcode, 1, 3)
-        ELSE 'None'
-    END AS postalCode_3,
+    coalesce(ta.postalcode3, 'cumulus__none') AS postalCode_3,
     concat('Patient/', tp.id) AS subject_ref,
     coalesce(tp.race_display, 'unknown') AS race_display,
     coalesce(tp.ethnicity_display, 'unknown') AS ethnicity_display
 FROM
-    temp_patient AS tp,
-    unnest(tp.address) AS t_address (addr_row)
+    temp_patient AS tp
+LEFT JOIN temp_address AS ta ON tp.id = ta.id
 
 WHERE
     tp.birthDate IS NOT NULL
     AND tp.gender IS NOT NULL;
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/reference_sql/count_core.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/count_core.sql`

 * *Files 3% similar despite different names*

```diff
@@ -9,86 +9,86 @@
 CREATE TABLE core__count_condition_month AS (
     WITH
     filtered_table AS (
         SELECT
             s.subject_ref,
             s.encounter_ref,
             --noqa: disable=RF03, AL02
-            s."category_code" AS cond_category_code,
-            s."recordedDate_month" AS cond_month,
-            s."code_display" AS cond_code_display
+            s."category_code",
+            s."recordedDate_month",
+            s."code_display"
             --noqa: enable=RF03, AL02
         FROM core__condition AS s
     ),
     
     null_replacement AS (
         SELECT
             subject_ref,
             encounter_ref,
             coalesce(
-                cast(cond_category_code AS varchar),
+                cast(category_code AS varchar),
                 'cumulus__none'
-            ) AS cond_category_code,
+            ) AS category_code,
             coalesce(
-                cast(cond_month AS varchar),
+                cast(recordedDate_month AS varchar),
                 'cumulus__none'
-            ) AS cond_month,
+            ) AS recordedDate_month,
             coalesce(
-                cast(cond_code_display AS varchar),
+                cast(code_display AS varchar),
                 'cumulus__none'
-            ) AS cond_code_display
+            ) AS code_display
         FROM filtered_table
     ),
     secondary_powerset AS (
         SELECT
             count(DISTINCT encounter_ref) AS cnt_encounter_ref,
-            "cond_category_code",
-            "cond_month",
-            "cond_code_display",
+            "category_code",
+            "recordedDate_month",
+            "code_display",
             concat_ws(
                 '-',
-                COALESCE("cond_category_code",''),
-                COALESCE("cond_month",''),
-                COALESCE("cond_code_display",'')
+                COALESCE("category_code",''),
+                COALESCE("recordedDate_month",''),
+                COALESCE("code_display",'')
             ) AS id
         FROM null_replacement
         GROUP BY
             cube(
-            "cond_category_code",
-            "cond_month",
-            "cond_code_display"
+            "category_code",
+            "recordedDate_month",
+            "code_display"
             )
     ),
 
     powerset AS (
         SELECT
             count(DISTINCT subject_ref) AS cnt_subject_ref,
-            "cond_category_code",
-            "cond_month",
-            "cond_code_display",
+            "category_code",
+            "recordedDate_month",
+            "code_display",
             concat_ws(
                 '-',
-                COALESCE("cond_category_code",''),
-                COALESCE("cond_month",''),
-                COALESCE("cond_code_display",'')
+                COALESCE("category_code",''),
+                COALESCE("recordedDate_month",''),
+                COALESCE("code_display",'')
             ) AS id
         FROM null_replacement
         GROUP BY
             cube(
-            "cond_category_code",
-            "cond_month",
-            "cond_code_display"
+            "category_code",
+            "recordedDate_month",
+            "code_display"
             )
     )
 
     SELECT
         s.cnt_encounter_ref AS cnt,
-        p."cond_category_code",
-        p."cond_month",
-        p."cond_code_display"
+        p."category_code",
+        p."recordedDate_month",
+        p."code_display"
     FROM powerset AS p
     JOIN secondary_powerset AS s on s.id = p.id
     WHERE 
         cnt_subject_ref >= 10
 );
 
 -- ###########################################################
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/setup.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/core/study_period.sql` & `cumulus_library-2.0.1/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/discovery/code_definitions.py` & `cumulus_library-2.0.1/cumulus_library/studies/discovery/code_definitions.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/discovery/code_detection.py` & `cumulus_library-2.0.1/cumulus_library/studies/discovery/code_detection.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py` & `cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql` & `cumulus_library-2.0.1/cumulus_library/studies/discovery/reference_sql/code_detection.sql`

 * *Files 2% similar despite different names*

```diff
@@ -49,25 +49,21 @@
     table_2.col_2.system
 FROM documentreference,
 UNNEST(category) AS table_1 (col_1),
 UNNEST(col_1.coding) as table_2 (col_2)
 
 UNION
 
-SELECT *
-FROM (
-    VALUES (
-        'encounter',
-        'class',
-        '',
-        '',
-        ''
-    )
-)
-    AS t (table_name, column_name, code, display, system)
+SELECT DISTINCT
+    'encounter' AS table_name,
+    'class' AS column_name,
+    class.code,
+    class.display,
+    class.system
+FROM encounter
 
 UNION
 
 SELECT DISTINCT
     'encounter' AS table_name,
     'type' AS column_name,
     table_2.col_2.code,
@@ -155,14 +151,25 @@
     )
 )
     AS t (table_name, column_name, code, display, system)
 
 UNION
 
 SELECT DISTINCT
+    'medicationrequest' AS table_name,
+    'medicationcodeableconcept' AS column_name,
+    table_1.col_1.code,
+    table_1.col_1.display,
+    table_1.col_1.system
+FROM medicationrequest,
+UNNEST(medicationcodeableconcept.coding) AS table_1 (col_1)
+
+UNION
+
+SELECT DISTINCT
     'observation' AS table_name,
     'category' AS column_name,
     table_2.col_2.code,
     table_2.col_2.display,
     table_2.col_2.system
 FROM observation,
 UNNEST(category) AS table_1 (col_1),
```

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/template/counts.sql` & `cumulus_library-2.0.1/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-2.0.1/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/template/manifest.toml` & `cumulus_library-2.0.1/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/template/setup.sql` & `cumulus_library-2.0.1/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-2.0.1/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/study_parser.py` & `cumulus_library-2.0.1/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/base_templates.py` & `cumulus_library-2.0.1/cumulus_library/template_sql/base_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/coding_denormalize.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/coding_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/insert_into.sql.jinja` & `cumulus_library-2.0.1/cumulus_library/template_sql/insert_into.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/template_sql/sql_utils.py` & `cumulus_library-2.0.1/cumulus_library/template_sql/sql_utils.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/cumulus_library/upload.py` & `cumulus_library-2.0.1/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/pyproject.toml` & `cumulus_library-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.0/PKG-INFO` & `cumulus_library-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 2.0.0
+Version: 2.0.1
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

