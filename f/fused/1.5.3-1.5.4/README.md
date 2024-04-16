# Comparing `tmp/fused-1.5.3.tar.gz` & `tmp/fused-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fused-1.5.3.tar", max compression
+gzip compressed data, was "fused-1.5.4.tar", max compression
```

## Comparing `fused-1.5.3.tar` & `fused-1.5.4.tar`

### file list

```diff
@@ -1,117 +1,114 @@
--rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.3/README.md
--rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.3/fused/MIGRATION_VERSION
--rw-r--r--   0        0        0     1111 2024-04-09 19:05:19.867615 fused-1.5.3/fused/__init__.py
--rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.3/fused/__main__.py
--rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.3/fused/_auth.py
--rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.3/fused/_cache/__init__.py
--rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.3/fused/_cache/memory.py
--rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.3/fused/_constants.py
--rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.3/fused/_deserialize.py
--rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.3/fused/_deserialize_parquet.py
--rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.3/fused/_environment.py
--rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.3/fused/_experimental.py
--rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.3/fused/_formatter/common.py
--rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.3/fused/_formatter/formatter_dataset.py
--rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.3/fused/_formatter/formatter_eval_result.py
--rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.3/fused/_formatter/formatter_job_config.py
--rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.3/fused/_formatter/formatter_jobs.py
--rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.3/fused/_formatter/formatter_options.py
--rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.3/fused/_formatter/formatter_project.py
--rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.3/fused/_formatter/formatter_templates.py
--rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.3/fused/_formatter/formatter_udf_access_token.py
--rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.3/fused/_formatter/noraise.py
--rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.3/fused/_formatter/template.py
--rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.3/fused/_formatter/udf.py
--rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.3/fused/_global_api.py
--rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.3/fused/_load_udf.py
--rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.3/fused/_magic/__init__.py
--rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.3/fused/_magic/magics.py
--rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.3/fused/_magic/output.py
--rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.3/fused/_options.py
--rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.3/fused/_project.py
--rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.3/fused/_public_api.py
--rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.3/fused/_quick/__init__.py
--rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.3/fused/_quick/udf.py
--rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.3/fused/_raster/__init__.py
--rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.3/fused/_raster/signer.py
--rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.3/fused/_raster/stac.py
--rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.3/fused/_registry.py
--rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.3/fused/_request.py
--rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.3/fused/_run.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.3/fused/_static/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.3/fused/_static/css/__init__.py
--rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.3/fused/_static/css/style.css
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.3/fused/_static/html/__init__.py
--rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.3/fused/_static/html/icons-svg-inline.html
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.3/fused/_static/templates/__init__.py
--rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.3/fused/_str_utils.py
--rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.3/fused/_templates/__init__.py
--rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.3/fused/_templates/loaders.py
--rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.3/fused/_templates/templates.py
--rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.3/fused/_udf/__init__.py
--rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.3/fused/_udf/coerce.py
--rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.3/fused/_udf/context.py
--rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.3/fused/_udf/decorators.py
--rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.3/fused/_udf/execute_v2.py
--rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.3/fused/_udf/load.py
--rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.3/fused/_udf/noop_decorators.py
--rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.3/fused/_udf/state.py
--rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.3/fused/_utils.py
--rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.3/fused/api/__init__.py
--rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.3/fused/api/_open_dataset.py
--rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.3/fused/api/_public_api.py
--rw-r--r--   0        0        0    48807 2024-04-01 21:12:17.248568 fused-1.5.3/fused/api/api.py
--rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.3/fused/api/credentials.py
--rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.3/fused/api/docker_api.py
--rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.3/fused/api/docker_http_api.py
--rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.3/fused/cli.py
--rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.3/fused/core/__init__.py
--rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.3/fused/core/_cache.py
--rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.3/fused/core/_download.py
--rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.3/fused/core/_impl/_context_impl.py
--rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.3/fused/core/_impl/_download_impl.py
--rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.3/fused/core/_impl/_realtime_ops_impl.py
--rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.3/fused/core/_impl/_reimports.py
--rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.3/fused/core/_impl/_table_ops_impl.py
--rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.3/fused/core/_impl/_udf_ops_impl.py
--rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.3/fused/core/_realtime_ops.py
--rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.3/fused/core/_table_ops.py
--rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.3/fused/core/_udf_ops.py
--rw-r--r--   0        0        0      795 2024-02-16 20:07:37.390060 fused-1.5.3/fused/models/__init__.py
--rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.3/fused/models/_codegen/__init__.py
--rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.3/fused/models/_codegen/job.py
--rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.3/fused/models/_codegen/udf.py
--rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.3/fused/models/_inplace.py
--rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.3/fused/models/_project_aware.py
--rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.3/fused/models/api/__init__.py
--rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.3/fused/models/api/_folder.py
--rw-r--r--   0        0        0    34461 2024-03-25 21:04:06.818813 fused-1.5.3/fused/models/api/dataset.py
--rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.3/fused/models/api/enums.py
--rw-r--r--   0        0        0    77407 2024-03-04 17:12:17.771506 fused-1.5.3/fused/models/api/job.py
--rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.3/fused/models/api/udf_access_token.py
--rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.3/fused/models/base.py
--rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.3/fused/models/coerce_dataset.py
--rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.3/fused/models/input.py
--rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.3/fused/models/internal/__init__.py
--rw-r--r--   0        0        0     8519 2023-10-13 17:39:24.951254 fused-1.5.3/fused/models/internal/dataset.py
--rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.3/fused/models/internal/job.py
--rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.3/fused/models/migrations.py
--rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.3/fused/models/request.py
--rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.3/fused/models/schema.py
--rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.3/fused/models/udf/__init__.py
--rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.3/fused/models/udf/_eval_result.py
--rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.3/fused/models/udf/_specialized_udfs.py
--rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.3/fused/models/udf/_udf_registry.py
--rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.3/fused/models/udf/base_udf.py
--rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.3/fused/models/udf/common.py
--rw-r--r--   0        0        0     5927 2024-04-09 19:05:13.177073 fused-1.5.3/fused/models/udf/header.py
--rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.3/fused/models/udf/output.py
--rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.3/fused/models/udf/udf.py
--rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.3/fused/models/urls.py
--rw-r--r--   0        0        0     7940 2023-10-13 17:39:24.956442 fused-1.5.3/fused/models/viz.py
--rw-r--r--   0        0        0      671 2023-10-13 17:39:24.956576 fused-1.5.3/fused/models/viz_colors.py
--rw-r--r--   0        0        0     1126 2023-10-13 17:39:24.956677 fused-1.5.3/fused/models/viz_presets.py
--rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.3/fused/types.py
--rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.3/fused/warnings.py
--rw-r--r--   0        0        0     3111 2024-04-09 19:05:19.861421 fused-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.4/README.md
+-rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.4/fused/MIGRATION_VERSION
+-rw-r--r--   0        0        0     1111 2024-04-16 17:35:47.488366 fused-1.5.4/fused/__init__.py
+-rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.4/fused/__main__.py
+-rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.4/fused/_auth.py
+-rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.4/fused/_cache/__init__.py
+-rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.4/fused/_cache/memory.py
+-rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.4/fused/_constants.py
+-rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.4/fused/_deserialize.py
+-rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.4/fused/_deserialize_parquet.py
+-rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.4/fused/_environment.py
+-rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.4/fused/_experimental.py
+-rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.4/fused/_formatter/common.py
+-rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.4/fused/_formatter/formatter_dataset.py
+-rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.4/fused/_formatter/formatter_eval_result.py
+-rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.4/fused/_formatter/formatter_job_config.py
+-rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.4/fused/_formatter/formatter_jobs.py
+-rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.4/fused/_formatter/formatter_options.py
+-rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.4/fused/_formatter/formatter_project.py
+-rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.4/fused/_formatter/formatter_templates.py
+-rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.4/fused/_formatter/formatter_udf_access_token.py
+-rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.4/fused/_formatter/noraise.py
+-rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.4/fused/_formatter/template.py
+-rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.4/fused/_formatter/udf.py
+-rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.4/fused/_global_api.py
+-rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.4/fused/_load_udf.py
+-rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.4/fused/_magic/__init__.py
+-rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.4/fused/_magic/magics.py
+-rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.4/fused/_magic/output.py
+-rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.4/fused/_options.py
+-rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.4/fused/_project.py
+-rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.4/fused/_public_api.py
+-rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.4/fused/_quick/__init__.py
+-rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.4/fused/_quick/udf.py
+-rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.4/fused/_raster/__init__.py
+-rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.4/fused/_raster/signer.py
+-rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.4/fused/_raster/stac.py
+-rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.4/fused/_registry.py
+-rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.4/fused/_request.py
+-rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.4/fused/_run.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.4/fused/_static/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.4/fused/_static/css/__init__.py
+-rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.4/fused/_static/css/style.css
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.4/fused/_static/html/__init__.py
+-rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.4/fused/_static/html/icons-svg-inline.html
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.4/fused/_static/templates/__init__.py
+-rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.4/fused/_str_utils.py
+-rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.4/fused/_templates/__init__.py
+-rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.4/fused/_templates/loaders.py
+-rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.4/fused/_templates/templates.py
+-rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.4/fused/_udf/__init__.py
+-rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.4/fused/_udf/coerce.py
+-rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.4/fused/_udf/context.py
+-rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.4/fused/_udf/decorators.py
+-rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.4/fused/_udf/execute_v2.py
+-rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.4/fused/_udf/load.py
+-rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.4/fused/_udf/noop_decorators.py
+-rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.4/fused/_udf/state.py
+-rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.4/fused/_utils.py
+-rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.4/fused/api/__init__.py
+-rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.4/fused/api/_open_dataset.py
+-rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.4/fused/api/_public_api.py
+-rw-r--r--   0        0        0    40857 2024-04-16 17:35:39.170109 fused-1.5.4/fused/api/api.py
+-rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.4/fused/api/credentials.py
+-rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.4/fused/api/docker_api.py
+-rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.4/fused/api/docker_http_api.py
+-rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.4/fused/cli.py
+-rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.4/fused/core/__init__.py
+-rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.4/fused/core/_cache.py
+-rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.4/fused/core/_download.py
+-rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.4/fused/core/_impl/_context_impl.py
+-rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.4/fused/core/_impl/_download_impl.py
+-rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.4/fused/core/_impl/_realtime_ops_impl.py
+-rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.4/fused/core/_impl/_reimports.py
+-rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.4/fused/core/_impl/_table_ops_impl.py
+-rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.4/fused/core/_impl/_udf_ops_impl.py
+-rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.4/fused/core/_realtime_ops.py
+-rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.4/fused/core/_table_ops.py
+-rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.4/fused/core/_udf_ops.py
+-rw-r--r--   0        0        0      752 2024-04-16 17:35:39.170492 fused-1.5.4/fused/models/__init__.py
+-rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.4/fused/models/_codegen/__init__.py
+-rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.4/fused/models/_codegen/job.py
+-rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.4/fused/models/_codegen/udf.py
+-rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.4/fused/models/_inplace.py
+-rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.4/fused/models/_project_aware.py
+-rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.4/fused/models/api/__init__.py
+-rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.4/fused/models/api/_folder.py
+-rw-r--r--   0        0        0    30327 2024-04-16 17:35:39.170855 fused-1.5.4/fused/models/api/dataset.py
+-rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.4/fused/models/api/enums.py
+-rw-r--r--   0        0        0    70205 2024-04-16 17:35:39.171363 fused-1.5.4/fused/models/api/job.py
+-rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.4/fused/models/api/udf_access_token.py
+-rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.4/fused/models/base.py
+-rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.4/fused/models/coerce_dataset.py
+-rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.4/fused/models/input.py
+-rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.4/fused/models/internal/__init__.py
+-rw-r--r--   0        0        0     7757 2024-04-16 17:35:39.171815 fused-1.5.4/fused/models/internal/dataset.py
+-rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.4/fused/models/internal/job.py
+-rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.4/fused/models/migrations.py
+-rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.4/fused/models/request.py
+-rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.4/fused/models/schema.py
+-rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.4/fused/models/udf/__init__.py
+-rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.4/fused/models/udf/_eval_result.py
+-rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.4/fused/models/udf/_specialized_udfs.py
+-rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.4/fused/models/udf/_udf_registry.py
+-rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.4/fused/models/udf/base_udf.py
+-rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.4/fused/models/udf/common.py
+-rw-r--r--   0        0        0     5927 2024-04-09 19:05:13.177073 fused-1.5.4/fused/models/udf/header.py
+-rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.4/fused/models/udf/output.py
+-rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.4/fused/models/udf/udf.py
+-rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.4/fused/models/urls.py
+-rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.4/fused/types.py
+-rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.4/fused/warnings.py
+-rw-r--r--   0        0        0     3111 2024-04-16 17:35:47.477699 fused-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.4/PKG-INFO
```

### Comparing `fused-1.5.3/README.md` & `fused-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/__init__.py` & `fused-1.5.4/fused/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 from .core import cache, download, get_chunk_from_table, get_chunks_metadata
 
 # Must be later so that models get imported first
 from . import _experimental as experimental  # isort:skip
 
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-__version__ = "1.5.3"
+__version__ = "1.5.4"
```

### Comparing `fused-1.5.3/fused/_auth.py` & `fused-1.5.4/fused/_auth.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_cache/memory.py` & `fused-1.5.4/fused/_cache/memory.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_deserialize.py` & `fused-1.5.4/fused/_deserialize.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_environment.py` & `fused-1.5.4/fused/_environment.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/common.py` & `fused-1.5.4/fused/_formatter/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_dataset.py` & `fused-1.5.4/fused/_formatter/formatter_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_eval_result.py` & `fused-1.5.4/fused/_formatter/formatter_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_job_config.py` & `fused-1.5.4/fused/_formatter/formatter_job_config.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_jobs.py` & `fused-1.5.4/fused/_formatter/formatter_jobs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_options.py` & `fused-1.5.4/fused/_formatter/formatter_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_project.py` & `fused-1.5.4/fused/_formatter/formatter_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_templates.py` & `fused-1.5.4/fused/_formatter/formatter_templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/formatter_udf_access_token.py` & `fused-1.5.4/fused/_formatter/formatter_udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/noraise.py` & `fused-1.5.4/fused/_formatter/noraise.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/template.py` & `fused-1.5.4/fused/_formatter/template.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_formatter/udf.py` & `fused-1.5.4/fused/_formatter/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_global_api.py` & `fused-1.5.4/fused/_global_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_load_udf.py` & `fused-1.5.4/fused/_load_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_magic/__init__.py` & `fused-1.5.4/fused/_magic/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_magic/magics.py` & `fused-1.5.4/fused/_magic/magics.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_magic/output.py` & `fused-1.5.4/fused/_magic/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_options.py` & `fused-1.5.4/fused/_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_project.py` & `fused-1.5.4/fused/_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_public_api.py` & `fused-1.5.4/fused/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_quick/udf.py` & `fused-1.5.4/fused/_quick/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_raster/signer.py` & `fused-1.5.4/fused/_raster/signer.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_raster/stac.py` & `fused-1.5.4/fused/_raster/stac.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_registry.py` & `fused-1.5.4/fused/_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_request.py` & `fused-1.5.4/fused/_request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_run.py` & `fused-1.5.4/fused/_run.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_static/css/style.css` & `fused-1.5.4/fused/_static/css/style.css`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_static/html/icons-svg-inline.html` & `fused-1.5.4/fused/_static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_str_utils.py` & `fused-1.5.4/fused/_str_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_templates/templates.py` & `fused-1.5.4/fused/_templates/templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/coerce.py` & `fused-1.5.4/fused/_udf/coerce.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/context.py` & `fused-1.5.4/fused/_udf/context.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/decorators.py` & `fused-1.5.4/fused/_udf/decorators.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/execute_v2.py` & `fused-1.5.4/fused/_udf/execute_v2.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/load.py` & `fused-1.5.4/fused/_udf/load.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_udf/state.py` & `fused-1.5.4/fused/_udf/state.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/_utils.py` & `fused-1.5.4/fused/_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/api/_open_dataset.py` & `fused-1.5.4/fused/api/_open_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/api/_public_api.py` & `fused-1.5.4/fused/api/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/api/api.py` & `fused-1.5.4/fused/api/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import shutil
 import time
 import warnings
-import webbrowser
 from functools import lru_cache
 from io import SEEK_SET
 from pathlib import Path
 from tempfile import TemporaryFile
 from typing import Any, BinaryIO, Dict, List, Literal, Optional, Sequence, Union
 
 import geopandas as gpd
@@ -19,21 +18,20 @@
 from fused._auth import CREDENTIALS
 from fused._deserialize import (
     zip_to_join_args,
     zip_to_join_singlefile_args,
     zip_to_map_args,
 )
 from fused._deserialize_parquet import parquet_to_df
-from fused._environment import infer_display_method
 from fused._global_api import set_api, set_api_class
 from fused._options import PROD_DEFAULT_BASE_URL
 from fused._options import options as OPTIONS
 from fused._request import raise_for_status
 from fused.api._open_dataset import post_open_table
-from fused.models import JoinInput, JoinSingleFileInput, MapInput, viz_colors
+from fused.models import JoinInput, JoinSingleFileInput, MapInput
 from fused.models.api import (
     JobConfig,
     JobStepConfig,
     JoinJobStepConfig,
     JoinSinglefileJobStepConfig,
     MapJobStepConfig,
     Table,
@@ -42,15 +40,14 @@
 )
 from fused.models.api._folder import Folder
 from fused.models.internal import Jobs, RunResponse
 from fused.models.internal.job import CoerceableToJobId, _object_to_job_id
 from fused.models.request import WHITELISTED_INSTANCE_TYPES
 from fused.models.udf._udf_registry import UdfRegistry
 from fused.models.udf.base_udf import METADATA_FUSED_ID, METADATA_FUSED_SLUG, BaseUdf
-from fused.models.viz import DatasetViz, DatasetVizV2, VizAppConfig, VizConfig
 from fused.warnings import FusedNonProductionWarning
 
 
 class FusedAPI:
     """API for running jobs in the Fused service."""
 
     base_url: str
@@ -882,228 +879,14 @@
             url=url,
             headers=self._generate_headers(),
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
         return RunResponse.parse_raw(r.content, content_type="json")
 
-    def show(
-        self,
-        path: str,
-        *,
-        open_browser: Optional[bool] = None,
-        show_widget: Optional[bool] = None,
-        iframe_args: Sequence[Any] = ("100%", "600px"),
-        tables: Optional[Sequence[str]] = None,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        app_config: Optional[Union[Dict[str, Any], VizAppConfig]] = None,
-        include_fused_table: bool = False,
-    ) -> str:
-        """Visualize a dataset
-
-        Args:
-            path: The path of the dataset to visualize.
-
-        Keyword Args:
-            open_browser: if True, attempts to open the debugging visualization in a browser window. Defaults to None.
-            show_widget: if True, attempts to open the debugging visualization in a widget within this notebook. Defaults to None.
-            iframe_args: parameters to pass into the generated IFrame. Defaults to ("100%", "600px").
-            tables: tables to load attributes from for visualization. Defaults to None,
-            app_config: additional debugging application configuration options
-            include_fused_table: if True, ensure "fused" is in the list of tables to show.
-
-        Returns:
-            The url to the visualization page.
-        """
-        url = f"{self.base_url}/files/debug"
-
-        if dataset_config is None:
-            dataset_config = VizConfig(selectedColumns={"geometry": True})
-
-            dataset_config.layer_config.root_bboxes.getLineColor = (
-                viz_colors.FUSED_PRIMARY
-            )
-            dataset_config.layer_config.root_bbox_ids.getColor = (
-                viz_colors.FUSED_PRIMARY_DARKER
-            )
-            dataset_config.layer_config.data_text.getColor = (
-                viz_colors.FUSED_PRIMARY_DARKER
-            )
-            dataset_config.layer_config.data_circles.getFillColor = (
-                viz_colors.FUSED_PRIMARY_DARKER
-            )
-            dataset_config.layer_config.root_bboxes_selected.getLineColor = (
-                viz_colors.FUSED_PRIMARY_FADED
-            )
-            dataset_config.layer_config.root_bboxes.getFillColor = (
-                viz_colors.FUSED_PRIMARY_VERY_FADED
-            )
-            dataset_config.layer_config.root_bboxes_selected.getFillColor = (
-                viz_colors.FUSED_PRIMARY_VERY_FADED
-            )
-
-        if isinstance(dataset_config, VizConfig):
-            dataset_config = dataset_config.dict(by_alias=True, exclude_none=True)
-
-        if isinstance(app_config, VizAppConfig):
-            app_config = app_config.dict(by_alias=True, exclude_none=True)
-
-        # If we need to include the fused table (default), and the tables were
-        # specified but not fused, add it.
-        if include_fused_table and tables is not None and "fused" not in tables:
-            tables = [*tables, "fused"]
-
-        body = request_models.DebugDatasetRequest(
-            path=path,
-            tables=tables,
-            dataset_config=dataset_config,
-            app_config=app_config,
-        ).dict()  # type: ignore
-
-        r = requests.post(
-            url=url,
-            json=body,
-            headers=self._generate_headers(),
-            timeout=OPTIONS.request_timeout,
-        )
-        raise_for_status(r)
-        # Returns a string
-        debug_result = r.json()
-        debug_url = debug_result["url"]
-
-        display_method = infer_display_method(
-            open_browser=open_browser, show_widget=show_widget
-        )
-
-        if display_method.open_browser:
-            webbrowser.open(debug_url)
-
-        if display_method.show_widget:
-            from IPython.display import IFrame, display
-
-            display(IFrame(debug_url, *iframe_args))
-
-        return debug_url
-
-    def show_multi(
-        self,
-        datasets: Sequence[DatasetViz],
-        *,
-        open_browser: Optional[bool] = None,
-        show_widget: Optional[bool] = None,
-        iframe_args: Sequence[Any] = ("100%", "600px"),
-        app_config: Optional[Union[Dict[str, Any], VizAppConfig]] = None,
-    ) -> str:
-        """Visualize multiple datasets
-
-        Args:
-            datasets: `DatasetViz` configuration objects.
-
-        Keyword Args:
-            open_browser: if True, attempts to open the debugging visualization in a browser window. Defaults to None.
-            show_widget: if True, attempts to open the debugging visualization in a widget within this notebook. Defaults to None.
-            iframe_args: parameters to pass into the generated IFrame. Defaults to ("100%", "600px").
-            app_config: additional debugging application configuration options
-
-        Returns:
-            The url to the visualization page.
-        """
-        url = f"{self.base_url}/files/multi_debug"
-
-        if isinstance(app_config, VizAppConfig):
-            app_config = app_config.dict(by_alias=True, exclude_none=True)
-
-        body = request_models.DebugMultiDatasetRequest(
-            datasets=[dataset._to_request() for dataset in datasets],
-            app_config=app_config,
-        ).dict()  # type: ignore
-
-        r = requests.post(
-            url=url,
-            json=body,
-            headers=self._generate_headers(),
-            timeout=OPTIONS.request_timeout,
-        )
-        raise_for_status(r)
-        # Returns a string
-        debug_result = r.json()
-        debug_url = debug_result["url"]
-
-        display_method = infer_display_method(
-            open_browser=open_browser, show_widget=show_widget
-        )
-
-        if display_method.open_browser:
-            webbrowser.open(debug_url)
-
-        if display_method.show_widget:
-            from IPython.display import IFrame, display
-
-            display(IFrame(debug_url, *iframe_args))
-
-        return debug_url
-
-    def show_multi_v2(
-        self,
-        datasets: Sequence[DatasetVizV2],
-        *,
-        open_browser: Optional[bool] = None,
-        show_widget: Optional[bool] = None,
-        iframe_args: Sequence[Any] = ("100%", "600px"),
-        app_config: Optional[Union[Dict[str, Any], VizAppConfig]] = None,
-    ) -> str:
-        """Visualize multiple datasets
-
-        Args:
-            datasets: `DatasetVizV2` configuration objects.
-
-        Keyword Args:
-            open_browser: if True, attempts to open the debugging visualization in a browser window. Defaults to None.
-            show_widget: if True, attempts to open the debugging visualization in a widget within this notebook. Defaults to None.
-            iframe_args: parameters to pass into the generated IFrame. Defaults to ("100%", "600px").
-            app_config: additional debugging application configuration options
-
-        Returns:
-            The url to the visualization page.
-        """
-        url = f"{self.base_url}/files/multi_debug_v2"
-
-        if isinstance(app_config, VizAppConfig):
-            app_config = app_config.dict(by_alias=True, exclude_none=True)
-
-        body = request_models.MultiDebugDatasetV2Request(
-            datasets=[dataset._to_request() for dataset in datasets],
-            app_config=app_config,
-        ).dict()  # type: ignore
-
-        r = requests.post(
-            url=url,
-            json=body,
-            headers=CREDENTIALS._authorization_header,
-            timeout=OPTIONS.request_timeout,
-        )
-        raise_for_status(r)
-        # Returns a string
-        debug_result = r.json()
-        debug_url = debug_result["url"]
-
-        display_method = infer_display_method(
-            open_browser=open_browser, show_widget=show_widget
-        )
-
-        if display_method.open_browser:
-            webbrowser.open(debug_url)
-
-        if display_method.show_widget:
-            from IPython.display import IFrame, display
-
-            display(IFrame(debug_url, *iframe_args))
-
-        return debug_url
-
     def _whoami(self) -> Any:
         """
         Returns information on the currently logged in user
         """
         url = f"{self.base_url}/user/self"
 
         r = requests.get(
```

### Comparing `fused-1.5.3/fused/api/credentials.py` & `fused-1.5.4/fused/api/credentials.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/api/docker_api.py` & `fused-1.5.4/fused/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/api/docker_http_api.py` & `fused-1.5.4/fused/api/docker_http_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_cache.py` & `fused-1.5.4/fused/core/_cache.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_download.py` & `fused-1.5.4/fused/core/_download.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_impl/_download_impl.py` & `fused-1.5.4/fused/core/_impl/_download_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_impl/_realtime_ops_impl.py` & `fused-1.5.4/fused/core/_impl/_realtime_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_impl/_table_ops_impl.py` & `fused-1.5.4/fused/core/_impl/_table_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_impl/_udf_ops_impl.py` & `fused-1.5.4/fused/core/_impl/_udf_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_realtime_ops.py` & `fused-1.5.4/fused/core/_realtime_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_table_ops.py` & `fused-1.5.4/fused/core/_table_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/core/_udf_ops.py` & `fused-1.5.4/fused/core/_udf_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/__init__.py` & `fused-1.5.4/fused/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,8 +27,7 @@
     LargeListType,
     ListType,
     PrimitiveDataType,
     Schema,
     StructType,
 )
 from .udf import Chunk, ChunkMetadata, GeoPandasUdfV2, Header
-from .viz import VizConfig, VizLayerConfig
```

### Comparing `fused-1.5.3/fused/models/_codegen/job.py` & `fused-1.5.4/fused/models/_codegen/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/_codegen/udf.py` & `fused-1.5.4/fused/models/_codegen/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/api/dataset.py` & `fused-1.5.4/fused/models/api/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 import warnings
 from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
-from typing import Any, Dict, List, Literal, Optional, Sequence, Set, Tuple, Union
+from typing import Dict, List, Literal, Optional, Sequence, Set, Tuple, Union
 
 import geopandas as gpd
 import pandas as pd
 import pyarrow as pa
 from pydantic import Field, PrivateAttr, StrictStr, root_validator, validator
 
 from fused._constants import DEFAULT_TABLE_NAMES
@@ -32,15 +32,14 @@
     DatasetOutput,
     DatasetOutputV2,
 )
 from fused.models.schema import Schema
 from fused.models.udf.common import ChunkMetadata
 from fused.models.udf.udf import EMPTY_UDF, BaseUdf
 from fused.models.urls import DatasetUrl
-from fused.models.viz import VizConfig
 from fused.warnings import FusedDefaultWarning, FusedRefreshingWarning
 
 from ..request import WHITELISTED_INSTANCE_TYPES
 
 
 class JobMetadata(FusedBaseModel):
     ec2_instance_type: Optional[WHITELISTED_INSTANCE_TYPES] = None
@@ -395,63 +394,14 @@
         map_config = MapJobStepConfig(
             udf=parsed_udf,
             input=dataset_input,
             output=output,
         )
         return map_config
 
-    def show(
-        self,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        *,
-        open_browser: Optional[bool] = None,
-        show_widget: Optional[bool] = None,
-        iframe_args: Sequence[Any] = ("100%", "600px"),
-        app_config: Optional[Dict[str, Any]] = None,
-        _rgb_table: Optional[bool] = None,
-    ) -> str:
-        """Open a debugging visualization of this dataset
-
-        Args:
-            dataset_config: additional dataset configuration options
-
-        Keyword Args:
-            open_browser: if True, attempts to open the debugging visualization in a browser window. Defaults to None.
-            show_widget: if True, attempts to open the debugging visualization in a widget within this notebook. Defaults to None.
-            iframe_args: parameters to pass into the generated IFrame. Defaults to ("100%", "600px").
-            app_config: additional debugging application configuration options
-
-        Returns:
-            The url to the hosted visualization.
-        """
-        dataset = self._dataset
-        include_fused_table = False
-        if dataset is None and self.url:
-            # TODO: Improve this and don't use a fake dataset. This will not work
-            # if e.g. the table is at the root of a volume.
-            dataset_base_path = self.url.rstrip("/").rsplit("/", maxsplit=1)[0]
-            dataset = Dataset(base_path=dataset_base_path, tables={self.name: self})
-        elif dataset is not None:
-            include_fused_table = "fused" in dataset.tables
-
-        if dataset is not None:
-            assert self.name, "Cannot visualize a table without a name set."
-            return dataset.show(
-                open_browser=open_browser,
-                show_widget=show_widget,
-                iframe_args=iframe_args,
-                tables=[self.name],
-                dataset_config=dataset_config,
-                app_config=app_config,
-                _rgb_table=self.name if _rgb_table else None,
-                include_fused_table=include_fused_table,
-            )
-
-        raise NotImplementedError("self._dataset is not set and no URL is set")
-
     def _repr_html_(self) -> str:
         return fused_table_repr(self)
 
     def refresh(self, fetch_samples: Optional[bool] = None) -> Table:
         """Returns this table with updated metadata"""
         should_fetch_samples = False
         if fetch_samples is not None:
@@ -834,60 +784,14 @@
                             file_id=file_id,
                             chunk_id=chunk_id,
                         )
                         chunk_dfs.append(chunk_df)
 
         return pd.concat(chunk_dfs)
 
-    def show(
-        self,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        *,
-        open_browser: Optional[bool] = None,
-        show_widget: Optional[bool] = None,
-        iframe_args: Sequence[Any] = ("100%", "600px"),
-        tables: Optional[Sequence[str]] = None,
-        app_config: Optional[Dict[str, Any]] = None,
-        _rgb_table: Optional[str] = None,
-        include_fused_table: bool = True,
-    ) -> str:
-        """Open a debugging visualization of this dataset
-
-        Args:
-            dataset_config: additional dataset configuration options
-
-        Keyword Args:
-            open_browser: if True, attempts to open the debugging visualization in a browser window. Defaults to None.
-            show_widget: if True, attempts to open the debugging visualization in a widget within this notebook. Defaults to None.
-            iframe_args: parameters to pass into the generated IFrame. Defaults to ("100%", "600px").
-            tables: tables to load attributes from for visualization
-            app_config: additional debugging application configuration options
-            include_fused_table: if True, ensure "fused" is in the list of tables to show.
-
-        Returns:
-            The url to the hosted visualization.
-        """
-        if _rgb_table is not None:
-            # HACK, this needs to import here because it will recurse into this function
-            # All other options are disregarded.
-            from fused.models.viz_presets import _show_naip_preset
-
-            return _show_naip_preset(self, _rgb_table)
-
-        return self._api.show(
-            self.base_path,
-            open_browser=open_browser,
-            show_widget=show_widget,
-            iframe_args=iframe_args,
-            tables=tables,
-            dataset_config=dataset_config,
-            app_config=app_config,
-            include_fused_table=include_fused_table,
-        )
-
     def _repr_html_(self) -> str:
         return fused_dataset_repr(self)
 
     def _validate_output(self, output_table: Optional[str]):
         if output_table and output_table in self.tables:
             raise ValueError(
                 f"Table {output_table} already exists. If you have removed it, you will need to refresh the dataset."
```

### Comparing `fused-1.5.3/fused/models/api/job.py` & `fused-1.5.4/fused/models/api/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     fused_map_repr,
     fused_udf_step_repr,
 )
 from fused._str_utils import append_url_part, is_url
 from fused._udf.execute_v2 import execute_against_sample, validate_imports_whitelist
 from fused.warnings import FusedDefaultWarning, FusedIgnoredWarning, FusedTypeWarning
 
-from ...models import viz_colors
 from ...models.schema import Schema
 from .._codegen import (
     create_directory_and_zip,
     extract_parameters,
     generate_meta_json,
     generate_readme,
     stringify_input,
@@ -56,15 +55,14 @@
     DatasetOutputBase,
     DatasetOutputV2,
     RunResponse,
 )
 from ..request import WHITELISTED_INSTANCE_TYPES
 from ..udf import EMPTY_UDF, BaseUdf
 from ..udf._eval_result import MultiUdfEvaluationResult, UdfEvaluationResult
-from ..viz import DatasetVizV2, VizAppConfig, VizConfig
 
 if TYPE_CHECKING:
     import geopandas as gpd
     import pandas as pd
     import pyarrow as pa
 
     from ...models.coerce_dataset import CoerceableToDatasetInput
@@ -1110,47 +1108,14 @@
                 url=self.output.url,
                 file_id=file_id,
                 chunk_id=chunk_id,
             )
         else:
             raise ValueError("Unknown output type or no output URL is set")
 
-    def show(
-        self,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        **kwargs,
-    ) -> str:
-        """Visualize the map operation
-
-        Args:
-            dataset_config: Customization of how to load and display the dataset.
-            **kwargs: Will be passed through to the underlying API viz method.
-        """
-        if isinstance(self.input, DatasetInput):
-            raise ValueError(
-                "Cannot run `show` on an old job input -- set a URL input instead."
-            )
-
-        if self.input is None or (
-            isinstance(self.input, DatasetInputV2) and not self.input.tables
-        ):
-            raise ValueError(
-                "Cannot run `show` when no input is set -- call `set_input` first."
-            )
-
-        return self._api.show_multi_v2(
-            datasets=[
-                DatasetVizV2(
-                    dataset=self.input,
-                    dataset_config=dataset_config,
-                ),
-            ],
-            **kwargs,
-        )
-
     def _repr_html_(self) -> str:
         return fused_map_repr(self)
 
     def run_realtime(
         self,
         df_left: Optional[
             Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
@@ -1419,139 +1384,14 @@
                 url=self.output.url,
                 file_id=file_id,
                 chunk_id=chunk_id,
             )
         else:
             raise ValueError("Unknown output type or no output URL is set")
 
-    def show(
-        self,
-        dataset_config_left: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        dataset_config_right: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        app_config: Optional[Union[Dict[str, Any], VizAppConfig]] = None,
-        **kwargs,
-    ) -> str:
-        """Visualize the join operation
-
-        Args:
-            dataset_config_left: Customization of how to load and display the left dataset.
-            dataset_config_right: Customization of how to load and display the right dataset.
-            app_config: Customization of the app.
-            **kwargs: Will be passed through to the underlying API show method.
-        """
-        if not isinstance(app_config, VizAppConfig):
-            if isinstance(app_config, dict):
-                app_config = VizAppConfig(**app_config)
-            elif app_config is None:
-                app_config = VizAppConfig()
-
-        app_config.show_toolbar_stats = True
-
-        if not isinstance(dataset_config_left, VizConfig):
-            if isinstance(dataset_config_left, dict):
-                dataset_config_left = VizConfig(**dataset_config_left)
-            elif dataset_config_left is None:
-                dataset_config_left = VizConfig(name="left")
-
-        if not isinstance(dataset_config_right, VizConfig):
-            if isinstance(dataset_config_right, dict):
-                dataset_config_right = VizConfig(**dataset_config_right)
-            elif dataset_config_right is None:
-                dataset_config_right = VizConfig(name="right")
-
-        dataset_config_left.selected_columns = {"geometry": True}
-        dataset_config_left.show_bboxes = True
-        dataset_config_left.show_bbox_ids = True
-        dataset_config_left.layer_config.root_heatmap.visible = False
-        dataset_config_left.layer_config.root_bboxes.getLineColor = (
-            viz_colors.FUSED_PRIMARY
-        )
-        dataset_config_left.layer_config.root_bbox_ids.getColor = (
-            viz_colors.FUSED_PRIMARY_DARKER
-        )
-        dataset_config_left.layer_config.data_text.getColor = (
-            viz_colors.FUSED_PRIMARY_DARKER
-        )
-        dataset_config_left.layer_config.data_circles.getFillColor = (
-            viz_colors.FUSED_PRIMARY_DARKER
-        )
-        dataset_config_left.layer_config.root_bboxes_selected.getLineColor = (
-            viz_colors.FUSED_PRIMARY_FADED
-        )
-        dataset_config_left.layer_config.root_bboxes.getFillColor = (
-            viz_colors.FUSED_PRIMARY_VERY_FADED
-        )
-        dataset_config_left.layer_config.root_bboxes_selected.getFillColor = (
-            viz_colors.FUSED_PRIMARY_VERY_FADED
-        )
-
-        dataset_config_right.selected_columns = {"geometry": True}
-        dataset_config_right.show_bboxes = True
-        dataset_config_right.show_bbox_ids = True
-        dataset_config_right.layer_config.root_heatmap.visible = False
-        dataset_config_right.layer_config.root_bboxes.getLineColor = (
-            viz_colors.FUSED_SECONDARY
-        )
-        dataset_config_right.layer_config.root_bbox_ids.getColor = (
-            viz_colors.FUSED_SECONDARY_DARKER
-        )
-        dataset_config_right.layer_config.data_text.getColor = (
-            viz_colors.FUSED_SECONDARY_DARKER
-        )
-        dataset_config_right.layer_config.data_circles.getFillColor = (
-            viz_colors.FUSED_SECONDARY_DARKER
-        )
-        dataset_config_right.layer_config.root_bboxes_selected.getLineColor = (
-            viz_colors.FUSED_SECONDARY_FADED
-        )
-        dataset_config_right.layer_config.root_bboxes.getFillColor = (
-            viz_colors.FUSED_SECONDARY_VERY_FADED
-        )
-        dataset_config_right.layer_config.root_bboxes_selected.getFillColor = (
-            viz_colors.FUSED_SECONDARY_VERY_FADED
-        )
-
-        if isinstance(self.input_left, DatasetInput) or isinstance(
-            self.input_right, DatasetInput
-        ):
-            raise ValueError(
-                "Cannot run `show` on an old job input -- set a URL input instead."
-            )
-
-        if (
-            self.input_left is None
-            or self.input_right is None
-            or (
-                isinstance(self.input_left, DatasetInputV2)
-                and not self.input_left.tables
-            )
-            or (
-                isinstance(self.input_right, DatasetInputV2)
-                and not self.input_right.tables
-            )
-        ):
-            raise ValueError(
-                "Cannot run `show` when no input is set -- call `set_input` first."
-            )
-
-        return self._api.show_multi_v2(
-            datasets=[
-                DatasetVizV2(
-                    dataset=self.input_left,
-                    dataset_config=dataset_config_left,
-                ),
-                DatasetVizV2(
-                    dataset=self.input_right,
-                    dataset_config=dataset_config_right,
-                ),
-            ],
-            app_config=app_config,
-            **kwargs,
-        )
-
     def _repr_html_(self) -> str:
         return fused_join_repr(self)
 
     def run_realtime(
         self,
         df_left: Optional[
             Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
@@ -1826,47 +1666,14 @@
                 url=self.output.url,
                 file_id=file_id,
                 chunk_id=chunk_id,
             )
         else:
             raise ValueError("Unknown output type or no output URL is set")
 
-    def show(
-        self,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        **kwargs,
-    ) -> str:
-        """Visualize the operation
-
-        Args:
-            dataset_config: Customization of how to load and display the dataset.
-            **kwargs: Will be passed through to the underlying API viz method.
-        """
-        if isinstance(self.input_left, DatasetInput):
-            raise ValueError(
-                "Cannot run `show` on an old job input -- set a URL input instead."
-            )
-
-        if self.input_left is None or (
-            isinstance(self.input_left, DatasetInputV2) and not self.input_left.tables
-        ):
-            raise ValueError(
-                "Cannot run `show` when no input is set -- call `set_input` first."
-            )
-
-        return self._api.show_multi_v2(
-            datasets=[
-                DatasetVizV2(
-                    dataset=self.input_left,
-                    dataset_config=dataset_config,
-                ),
-            ],
-            **kwargs,
-        )
-
     def _repr_html_(self) -> str:
         return fused_join_singlefile_repr(self)
 
 
 class JobConfig(FusedBaseModel):
     name: Optional[StrictStr] = None
     """The name of the job."""
```

### Comparing `fused-1.5.3/fused/models/api/udf_access_token.py` & `fused-1.5.4/fused/models/api/udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/base.py` & `fused-1.5.4/fused/models/base.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/coerce_dataset.py` & `fused-1.5.4/fused/models/coerce_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/input.py` & `fused-1.5.4/fused/models/input.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/internal/dataset.py` & `fused-1.5.4/fused/models/internal/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import annotations
 
 import warnings
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
+from typing import Dict, List, Optional, Type
 from urllib.parse import urlparse
 
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
 from fused._constants import DEFAULT_TABLE_NAMES
 from fused._str_utils import append_url_part
 from fused.warnings import FusedDeprecationWarning
 
 from .._project_aware import FusedProjectAware
 from ..base import FusedBaseModel
 from ..urls import DatasetUrl
 
-if TYPE_CHECKING:
-    from ..viz import VizConfig
-
 
 class DatasetInputBase(FusedBaseModel):
     type: Optional[str] = None
 
     _registered_subtypes: Dict[str, Type["DatasetInputBase"]] = dict()
 
     def __init_subclass__(cls, type=None):
@@ -122,38 +119,14 @@
         """Create a DatasetInputV2 that reads a single table from a URL."""
         return cls(
             # The specific operation isn't important, ZIP is just a convenient default.
             operation=DatasetInputV2Type.ZIP,
             tables=[DatasetInputV2Table(url=url, cache_locally=cache_locally)],
         )
 
-    def show(
-        self,
-        dataset_config: Optional[Union[Dict[str, Any], VizConfig]] = None,
-        **kwargs,
-    ) -> str:
-        """Visualize the input
-
-        Args:
-            dataset_config: Customization of how to load and display the dataset.
-            **kwargs: Will be passed through to the underlying API viz method.
-        """
-        # Needed for circular import reasons
-        from ..viz import DatasetVizV2
-
-        return self._api.show_multi_v2(
-            datasets=[
-                DatasetVizV2(
-                    dataset=self,
-                    dataset_config=dataset_config,
-                ),
-            ],
-            **kwargs,
-        )
-
 
 class SampleStrategy(str, Enum):
     """How to generate output samples"""
 
     EMPTY = "empty"
     """Do not generate a sample"""
     FIRST_CHUNK = "first_chunk"
```

### Comparing `fused-1.5.3/fused/models/internal/job.py` & `fused-1.5.4/fused/models/internal/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/migrations.py` & `fused-1.5.4/fused/models/migrations.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/request.py` & `fused-1.5.4/fused/models/request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/schema.py` & `fused-1.5.4/fused/models/schema.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/_eval_result.py` & `fused-1.5.4/fused/models/udf/_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/_specialized_udfs.py` & `fused-1.5.4/fused/models/udf/_specialized_udfs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/_udf_registry.py` & `fused-1.5.4/fused/models/udf/_udf_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/base_udf.py` & `fused-1.5.4/fused/models/udf/base_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/common.py` & `fused-1.5.4/fused/models/udf/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/header.py` & `fused-1.5.4/fused/models/udf/header.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/output.py` & `fused-1.5.4/fused/models/udf/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/udf/udf.py` & `fused-1.5.4/fused/models/udf/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/models/urls.py` & `fused-1.5.4/fused/models/urls.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/fused/warnings.py` & `fused-1.5.4/fused/warnings.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.3/pyproject.toml` & `fused-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fused"
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "1.5.3"
+version = "1.5.4"
 description = ""
 authors = []
 readme = "README.md"
 packages = [{ include = "fused" }]
 
 [project.urls]
 Homepage = "https://www.fused.io"
```

### Comparing `fused-1.5.3/PKG-INFO` & `fused-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fused
-Version: 1.5.3
+Version: 1.5.4
 Summary: 
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

