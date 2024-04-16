# Comparing `tmp/dvcx-0.73.0.tar.gz` & `tmp/dvcx-0.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.73.0.tar", last modified: Mon Apr  8 16:48:49 2024, max compression
+gzip compressed data, was "dvcx-0.74.0.tar", last modified: Tue Apr 16 08:37:58 2024, max compression
```

## Comparing `dvcx-0.73.0.tar` & `dvcx-0.74.0.tar`

### file list

```diff
@@ -1,227 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:49.006125 dvcx-0.73.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 16:48:43.000000 dvcx-0.73.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 16:48:43.000000 dvcx-0.73.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-08 16:48:43.000000 dvcx-0.73.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 16:48:43.000000 dvcx-0.73.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 16:48:43.000000 dvcx-0.73.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 16:48:43.000000 dvcx-0.73.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-08 16:48:43.000000 dvcx-0.73.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-08 16:48:43.000000 dvcx-0.73.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 16:48:49.002125 dvcx-0.73.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-08 16:48:43.000000 dvcx-0.73.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-08 16:48:43.000000 dvcx-0.73.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.966125 dvcx-0.73.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-08 16:48:43.000000 dvcx-0.73.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-08 16:48:43.000000 dvcx-0.73.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:48:49.006125 dvcx-0.73.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.954125 dvcx-0.73.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.974125 dvcx-0.73.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.974125 dvcx-0.73.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70456 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.978125 dvcx-0.73.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.978125 dvcx-0.73.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33347 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.982125 dvcx-0.73.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.982125 dvcx-0.73.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    55045 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.990125 dvcx-0.73.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.990125 dvcx-0.73.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34571 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.994125 dvcx-0.73.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.994125 dvcx-0.73.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.024024 dvcx-0.74.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 08:37:52.000000 dvcx-0.74.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 08:37:52.000000 dvcx-0.74.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-16 08:37:52.000000 dvcx-0.74.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-16 08:37:52.000000 dvcx-0.74.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 08:37:52.000000 dvcx-0.74.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 08:37:52.000000 dvcx-0.74.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-16 08:37:52.000000 dvcx-0.74.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-16 08:37:52.000000 dvcx-0.74.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 08:37:58.024024 dvcx-0.74.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-16 08:37:52.000000 dvcx-0.74.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-16 08:37:52.000000 dvcx-0.74.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-16 08:37:52.000000 dvcx-0.74.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-16 08:37:52.000000 dvcx-0.74.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:37:58.024024 dvcx-0.74.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.976024 dvcx-0.74.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.992024 dvcx-0.74.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.996024 dvcx-0.74.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72831 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.996024 dvcx-0.74.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.000024 dvcx-0.74.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44816 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.000024 dvcx-0.74.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57791 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35621 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114379 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/utils.py
```

### Comparing `dvcx-0.73.0/.cruft.json` & `dvcx-0.74.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.74.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.74.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.github/workflows/benchmarks.yml` & `dvcx-0.74.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.github/workflows/release.yml` & `dvcx-0.74.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.github/workflows/tests.yml` & `dvcx-0.74.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.gitignore` & `dvcx-0.74.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/.pre-commit-config.yaml` & `dvcx-0.74.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/CODE_OF_CONDUCT.rst` & `dvcx-0.74.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/CONTRIBUTING.rst` & `dvcx-0.74.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/LICENSE` & `dvcx-0.74.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/LICENSES/Apache-2.0.txt` & `dvcx-0.74.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.74.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/LICENSES/Python-2.0.txt` & `dvcx-0.74.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/PKG-INFO` & `dvcx-0.74.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.73.0
+Version: 0.74.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -61,14 +61,15 @@
 Requires-Dist: pytest-benchmark[histogram]; extra == "tests"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "tests"
 Requires-Dist: pytest-xdist>=3.3.1; extra == "tests"
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
+Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
```

### Comparing `dvcx-0.73.0/README.rst` & `dvcx-0.74.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/docs/udfs.md` & `dvcx-0.74.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/blip2_image_desc_lib.py` & `dvcx-0.74.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/common_sql_functions.py` & `dvcx-0.74.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/dir_expansion.py` & `dvcx-0.74.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/hf_pipeline.py` & `dvcx-0.74.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/llava2_image_desc_lib.py` & `dvcx-0.74.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/loader.py` & `dvcx-0.74.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/neurips/README` & `dvcx-0.74.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/neurips/distance_to_query.py` & `dvcx-0.74.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/neurips/llm_chat.py` & `dvcx-0.74.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/neurips/single_query.py` & `dvcx-0.74.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/neurips/text_loaders.py` & `dvcx-0.74.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/openai_image_desc_lib.py` & `dvcx-0.74.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/openimage-detect.py` & `dvcx-0.74.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/pose_detection.py` & `dvcx-0.74.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/torch-loader.py` & `dvcx-0.74.0/examples/torch-loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import torch
 from torch import nn, optim
 from torch.utils.data import DataLoader
 from torchvision.transforms import v2
 
 from dvcx.lib.param import Image, Label
-from dvcx.lib.pytorch import PytorchDataset
 from dvcx.query import C, DatasetQuery, udf
 from dvcx.sql.types import String
 
 STORAGE = "gcs://dvcx-datalakes/dogs-and-cats/"
 
 # Define transformation for data preprocessing
 transform = v2.Compose(
     [
+        v2.ToTensor(),
         v2.Resize((64, 64)),
         v2.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
     ]
 )
 
 
 CLASSES = ["cat", "dog"]
@@ -46,28 +46,18 @@
         x = x.view(-1, 64 * 8 * 8)
         x = torch.relu(self.fc1(x))
         x = self.fc2(x)
         return x
 
 
 if __name__ == "__main__":
-    q = (
-        DatasetQuery(STORAGE)
-        .filter(C.name.glob("*.jpg"))
-        .add_signals(extract_label)
-        .save("cats-and-dogs")
-    )
+    q = DatasetQuery(STORAGE).filter(C.name.glob("*.jpg")).add_signals(extract_label)
 
     train_loader = DataLoader(
-        PytorchDataset(
-            params=[Image(), Label("label", CLASSES)],
-            name="cats-and-dogs",
-            cache=True,
-            transform=transform,
-        ),
+        q.to_pytorch(Image(), Label("label", CLASSES), cache=True, transform=transform),
         batch_size=16,
     )
 
     model = CNN()
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.Adam(model.parameters(), lr=0.001)
```

### Comparing `dvcx-0.73.0/examples/udfs/batching.py` & `dvcx-0.74.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/udfs/image_transformation.py` & `dvcx-0.74.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/udfs/parallel.py` & `dvcx-0.74.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/udfs/simple.py` & `dvcx-0.74.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/udfs/stateful.py` & `dvcx-0.74.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/udfs/stateful_similarity.py` & `dvcx-0.74.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/unstructured-text.py` & `dvcx-0.74.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/wds.py` & `dvcx-0.74.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/wds_filtered.py` & `dvcx-0.74.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/wds_meta.py` & `dvcx-0.74.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/zalando/zalando_clip.py` & `dvcx-0.74.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.74.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/noxfile.py` & `dvcx-0.74.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/pyproject.toml` & `dvcx-0.74.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
   "pytest-benchmark[histogram]",
   "pytest-asyncio>=0.23.2",
   "pytest-xdist>=3.3.1",
   "virtualenv",
   "dulwich",
   "hypothesis",
   "numpy",
+  "open_clip_torch",
   "aiotools>=1.7.0",
   "requests-mock"
 ]
 dev = [
   "dvcx[tests]",
   "mypy==1.9.0",
   "types-python-dateutil",
@@ -139,14 +140,15 @@
 pretty = true
 check_untyped_defs = false
 # Warnings
 warn_no_return = true
 warn_redundant_casts = true
 warn_unreachable = true
 ignore_missing_imports = true
+disable_error_code = "annotation-unchecked"
 files = ["src", "tests"]
 
 [tool.codespell]
 ignore-words-list = " "
 
 [tool.ruff]
 output-format = "full"
```

### Comparing `dvcx-0.73.0/src/dvcx/asyn.py` & `dvcx-0.74.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/cache.py` & `dvcx-0.74.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/catalog/catalog.py` & `dvcx-0.74.0/src/dvcx/catalog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 import posixpath
 import subprocess
 import sys
 import time
 import traceback
 from ast import Attribute, Call, Expr, Import, Load, Name, alias
 from collections.abc import Iterable, Iterator, Mapping, Sequence
+from contextlib import contextmanager, nullcontext
 from copy import copy
 from dataclasses import dataclass
 from pathlib import Path
 from random import shuffle
+from threading import Thread
 from typing import (
+    IO,
     TYPE_CHECKING,
     Any,
+    Callable,
     NamedTuple,
     NoReturn,
     Optional,
     Union,
 )
 from uuid import uuid4
 
@@ -38,14 +42,15 @@
 from dvcx.cache import DVCXCache
 from dvcx.client import Client
 from dvcx.config import get_remote_config, read_config
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.dataset import (
     DATASET_PREFIX,
     QUERY_DATASET_NAME_PREFIX,
+    TEMP_DATASET_NAME_PREFIX,
     DatasetDependency,
     DatasetRecord,
     DatasetRow,
     DatasetStats,
     create_dataset_uri,
     parse_dataset_uri,
 )
@@ -109,14 +114,40 @@
 PULL_DATASET_CHECK_STATUS_INTERVAL = 20  # interval to check export status in Studio
 
 
 def _raise_remote_error(error_message: str) -> NoReturn:
     raise DVCXError(f"Error from server: {error_message}")
 
 
+def noop(_: str):
+    pass
+
+
+@contextmanager
+def print_and_capture(
+    stream: "IO[str]", callback: Callable[[str], None] = noop
+) -> "Iterator[list[str]]":
+    lines: list[str] = []
+    append = lines.append
+
+    def loop() -> None:
+        for line in iter(stream.readline, ""):
+            print(line, end="")
+            callback(line)
+            append(line)
+
+    thread = Thread(target=loop, daemon=True)
+    thread.start()
+
+    try:
+        yield lines
+    finally:
+        thread.join()
+
+
 class QueryResult(NamedTuple):
     dataset: Optional[DatasetRecord]
     version: Optional[int]
     output: str
     preview: Optional[list[dict]]
 
 
@@ -575,14 +606,30 @@
             result.warehouse = None
         return result
 
     @classmethod
     def generate_query_dataset_name(cls) -> str:
         return f"{QUERY_DATASET_NAME_PREFIX}_{uuid4().hex}"
 
+    @classmethod
+    def generate_temp_dataset_name(cls, query_session_uuid: str) -> str:
+        """
+        Temp or ephemeral datasets are the ones created without specified name
+        with DatasetQuery, e.g ds = DatasetQuery(path="s3://ldb-public").save().
+        They are useful for optimization purposes and should be removed when
+        query ends.
+        Temp dataset has specific name that starts with ds_temp keyword and then
+        follows by unique query uuid. Finally it ends with unique uuid to make
+        sure it's generally unique. Examples:
+        ds_temp_afcc3350-8dee-4342-9a84-1556fc0fae45_03c071eb-6728-4192-b7dd-624b4148e8b4
+        ds_temp_2801235b-63c7-4c5a-9555-4b962d2a5dff
+        """
+
+        return f"{TEMP_DATASET_NAME_PREFIX}{query_session_uuid}_{uuid4().hex}"
+
     def compile_query_script(self, script: str, save=False) -> str:
         wrapper_function = "query_wrapper_print"
         if save:
             wrapper_function = "query_wrapper_save"
 
         code_ast = ast.parse(script)
         if code_ast.body:
@@ -1102,14 +1149,25 @@
         ensure that they are cleaned up as soon as they are no longer
         needed. When running the same `DatasetQuery` multiple times we
         may use the same temporary table names.
         """
         self.warehouse.cleanup_temp_tables(names)
         self.id_generator.delete_uris(names)
 
+    def cleanup_temp_datasets(self, query_session_uuid: Optional[str] = None) -> None:
+        """
+        This method removes temporary datasets for specific query session uuid
+        or in general
+        """
+        prefix = TEMP_DATASET_NAME_PREFIX
+        if query_session_uuid:
+            prefix = f"{prefix}{query_session_uuid}"
+        for dataset in self.metastore.list_datasets_by_prefix(prefix):
+            self.remove_dataset(dataset.name, force=True)
+
     def create_dataset_from_sources(
         self,
         name: str,
         sources: list[str],
         client_config=None,
         recursive=False,
     ) -> DatasetRecord:
@@ -1704,23 +1762,25 @@
             ds = DatasetQuery(path=source, catalog=self)
         udf = import_object(udf_location)
         if params:
             args, kwargs = parse_params_string(params)
             udf = udf(*args, **kwargs)
         ds.add_signals(udf, parallel=parallel).save(target_name)
 
-    def query(  # noqa: PLR0912
+    def query(
         self,
         query_script: str,
         envs: Optional[Mapping[str, str]] = None,
         python_executable: Optional[str] = None,
         save: bool = False,
         preview_limit: Optional[int] = 10,
         preview_offset: int = 0,
         preview_columns: Optional[list[str]] = None,
+        capture_output: bool = True,
+        output_hook: Callable[[str], None] = noop,
     ) -> QueryResult:
         """
         Method to run custom user Python script to run a query and, as result,
         creates new dataset from the results of a query.
         Returns tuple of result dataset and script output.
 
         Constraints on query script:
@@ -1736,86 +1796,101 @@
 
         Example of query script:
             from dvcx.query import DatasetQuery, C
             DatasetQuery('s3://ldb-public/remote/datasets/mnist-tiny/').filter(
                 C.size > 1000
             )
         """
-        if envs is None:
-            envs = os.environ
-
         try:
             query_script_compiled = self.compile_query_script(query_script, save=save)
         except Exception as exc:
             raise QueryScriptCompileError(
                 f"Query script failed to compile, reason: {exc}"
             ) from exc
 
-        if not python_executable:
-            python_executable = sys.executable
+        r, w = os.pipe()
+        if os.name == "nt":
+            import msvcrt
+
+            os.set_inheritable(w, True)
+
+            startupinfo = subprocess.STARTUPINFO()  # type: ignore[attr-defined]
+            handle = msvcrt.get_osfhandle(w)  # type: ignore[attr-defined]
+            startupinfo.lpAttributeList["handle_list"].append(handle)
+            kwargs: dict[str, Any] = {"startupinfo": startupinfo}
+        else:
+            handle = w
+            kwargs = {"pass_fds": [w]}
 
-        envs = dict(envs)
+        envs = dict(envs or os.environ)
+        query_session_uuid = uuid4().hex
         envs.update(
             {
                 "DVCX_QUERY_PREVIEW_ARGS": json.dumps(
                     {
                         "limit": preview_limit,
                         "offset": preview_offset,
                         "columns": preview_columns,
                     }
-                )
-            }
+                ),
+                "DVCX_QUERY_SESSION_UUID": query_session_uuid,
+                "PYTHONUNBUFFERED": "1",
+                "DVCX_OUTPUT_FD": str(handle),
+            },
         )
-        result = subprocess.run(
+
+        python_executable = python_executable or sys.executable
+        with subprocess.Popen(
             [python_executable, "-c", query_script_compiled],  # noqa: S603
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,  # merging stderr to stdout
             env=envs,
-            check=False,
-        )
-
-        script_output = ""  # stdout + stderr from user script itself
+            stdout=subprocess.PIPE if capture_output else None,
+            stderr=subprocess.STDOUT if capture_output else None,
+            bufsize=1,
+            text=True,
+            **kwargs,
+        ) as proc:
+            os.close(w)
+
+            out = proc.stdout
+            _lines: list[str] = []
+            ctx = print_and_capture(out, output_hook) if out else nullcontext(_lines)
+
+            with ctx as lines, open(r) as f:
+                response_text = ""
+                while proc.poll() is None:
+                    response_text += f.readline()
+                    time.sleep(0.1)
+                response_text += f.readline()
 
-        # finding returning dataset name and version from script
-        dataset_name = None
-        dataset_version = None
-        records = None
-        if result.stdout:
-            for line in result.stdout.decode("utf-8").splitlines():
-                if len(line.split(PYTHON_SCRIPT_WRAPPER_CODE)) == 4:
-                    dataset_name = line.split(PYTHON_SCRIPT_WRAPPER_CODE)[1]
-                    dataset_version = int(line.split(PYTHON_SCRIPT_WRAPPER_CODE)[2])
-                elif (
-                    not records
-                    and line.startswith("__ds_records__")
-                    and line.endswith("__ds_records__")
-                ):
-                    _, record, _ = line.split("__ds_records__", 2)
-                    records = json.loads(record.strip())
-                else:
-                    # collecting script output as well to save it to the database
-                    # later on for debugging
-                    script_output += line + "\n"
-
-        if result.returncode:
-            if result.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
+        try:
+            response = json.loads(response_text)
+        except ValueError:
+            response = {}
+        records = response.get("preview", None)
+        dataset_name, dataset_version = response.get("dataset", (None, None))
+
+        script_output = "".join(lines)
+
+        self.cleanup_temp_datasets(query_session_uuid)
+        if proc.returncode:
+            if proc.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
                 raise QueryScriptCancelError(
                     "Query script was canceled by user",
-                    return_code=result.returncode,
+                    return_code=proc.returncode,
                     output=script_output,
                 )
-            if result.returncode == QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE:
+            if proc.returncode == QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE:
                 raise QueryScriptRunError(
                     "Last line in a script was not an instance of DatasetQuery",
-                    return_code=result.returncode,
+                    return_code=proc.returncode,
                     output=script_output,
                 )
             raise QueryScriptRunError(
-                f"Query script exited with error code {result.returncode}",
-                return_code=result.returncode,
+                f"Query script exited with error code {proc.returncode}",
+                return_code=proc.returncode,
                 output=script_output,
             )
 
         if not save:
             return QueryResult(
                 dataset=None, version=None, output=script_output, preview=records
             )
```

### Comparing `dvcx-0.73.0/src/dvcx/catalog/datasource.py` & `dvcx-0.74.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/catalog/formats.py` & `dvcx-0.74.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/catalog/loader.py` & `dvcx-0.74.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/cli.py` & `dvcx-0.74.0/src/dvcx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from multiprocessing import freeze_support
 from typing import TYPE_CHECKING, Optional, Union
 
 import shtab
 
 from dvcx import __version__, utils
 from dvcx.cli_utils import BooleanOptionalAction, CommaSeparatedArgs
-from dvcx.error import QueryScriptRunError
 from dvcx.utils import DVCXDir
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
 
 logger = logging.getLogger("dvcx")
 
@@ -797,39 +796,31 @@
     script: str,
     dataset_name: str,
     parallel: Optional[int] = None,
     limit: int = 10,
     offset: int = 0,
     columns: Optional[list[str]] = None,
     no_collapse: bool = False,
-    show_error: bool = False,
 ) -> None:
     from dvcx.utils import show_records
 
     with open(script, encoding="utf-8") as f:
         script_content = f.read()
 
     if parallel is not None:
         # This also sets this environment variable for any subprocesses
         os.environ["DVCX_SETTINGS_PARALLEL"] = str(parallel)
 
-    try:
-        result = catalog.query(
-            script_content,
-            preview_limit=limit,
-            preview_offset=offset,
-            preview_columns=columns,
-        )
-    except QueryScriptRunError as e:
-        if show_error:
-            print(e.output, end="")
-        raise
-
-    if result.output:
-        print(result.output)
+    result = catalog.query(
+        script_content,
+        preview_limit=limit,
+        preview_offset=offset,
+        preview_columns=columns,
+        capture_output=False,
+    )
     show_records(result.preview, collapse_columns=not no_collapse)
 
 
 def clear_cache(catalog: "Catalog"):
     catalog.cache.clear()
 
 
@@ -998,15 +989,14 @@
                 catalog,
                 args.script,
                 args.parallel,
                 limit=args.limit,
                 offset=args.offset,
                 columns=args.columns,
                 no_collapse=args.no_collapse,
-                show_error=args.verbose,
             )
         elif args.command == "apply-udf":
             catalog.apply_udf(
                 args.udf, args.source, args.target, args.parallel, args.udf_params
             )
         elif args.command == "clear-cache":
             clear_cache(catalog)
```

### Comparing `dvcx-0.73.0/src/dvcx/cli_utils.py` & `dvcx-0.74.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/azure.py` & `dvcx-0.74.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/fileslice.py` & `dvcx-0.74.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/fsspec.py` & `dvcx-0.74.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/gcs.py` & `dvcx-0.74.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/local.py` & `dvcx-0.74.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/client/s3.py` & `dvcx-0.74.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/config.py` & `dvcx-0.74.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.74.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.74.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.74.0/src/dvcx/data_storage/metastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,18 @@
         """
 
     @abstractmethod
     def list_datasets(self) -> Iterator[DatasetRecord]:
         """Lists all datasets."""
 
     @abstractmethod
+    def list_datasets_by_prefix(self, prefix: str) -> Iterator["DatasetRecord"]:
+        """Lists all datasets which names start with prefix."""
+
+    @abstractmethod
     def get_dataset(self, name: str) -> DatasetRecord:
         """Gets a single dataset by name."""
 
     @abstractmethod
     def update_dataset_status(
         self,
         dataset: DatasetRecord,
@@ -1052,14 +1056,52 @@
         versions = []
         for r in rows:
             versions.append(self.dataset_class.parse(*r))
         if not versions:
             return None
         return reduce(lambda ds, version: ds.merge_versions(version), versions)
 
+    def _parse_datasets(self, rows) -> Iterator["DatasetRecord"]:
+        # grouping rows by dataset id
+        for _, g in groupby(rows, lambda r: r[0]):
+            dataset = self._parse_dataset(list(g))
+            if dataset:
+                yield dataset
+
+    def _base_dataset_query(self):
+        d = self._datasets
+        dv = self._datasets_versions
+        query = self._datasets_select(
+            *(getattr(d.c, f) for f in self._dataset_fields),
+            *(getattr(dv.c, f) for f in self._dataset_version_fields),
+        )
+        j = d.join(dv, d.c.id == dv.c.dataset_id, isouter=True)
+        return query.select_from(j)
+
+    def list_datasets(self) -> Iterator["DatasetRecord"]:
+        """Lists all datasets."""
+        yield from self._parse_datasets(self.db.execute(self._base_dataset_query()))
+
+    def list_datasets_by_prefix(
+        self, prefix: str, conn=None
+    ) -> Iterator["DatasetRecord"]:
+        query = self._base_dataset_query()
+        query = query.where(self._datasets.c.name.startswith(prefix))
+        yield from self._parse_datasets(self.db.execute(query))
+
+    def get_dataset(self, name: str, conn=None) -> DatasetRecord:
+        """Gets a single dataset by name"""
+        d = self._datasets
+        query = self._base_dataset_query()
+        query = query.where(d.c.name == name)  # type: ignore [attr-defined]
+        ds = self._parse_dataset(self.db.execute(query, conn=conn))
+        if not ds:
+            raise DatasetNotFoundError(f"Dataset {name} not found.")
+        return ds
+
     def remove_dataset_version(
         self, dataset: DatasetRecord, version: int
     ) -> DatasetRecord:
         """
         Deletes one single dataset version.
         If it was last version, it removes dataset completely
         """
@@ -1083,48 +1125,14 @@
             # had only one version, fully deleting dataset
             self.db.execute(self._datasets_delete().where(d.c.id == dataset.id))
 
         result_ds = copy.deepcopy(dataset)
         result_ds.remove_version(version)
         return result_ds
 
-    def list_datasets(self) -> Iterator["DatasetRecord"]:
-        """Lists all datasets."""
-        d = self._datasets
-        dv = self._datasets_versions
-        query = self._datasets_select(
-            *(getattr(d.c, f) for f in self._dataset_fields),
-            *(getattr(dv.c, f) for f in self._dataset_version_fields),
-        )
-        j = d.join(dv, d.c.id == dv.c.dataset_id, isouter=True)
-
-        query = query.select_from(j)
-        rows = self.db.execute(query)
-
-        for _, g in groupby(rows, lambda r: r[0]):
-            dataset = self._parse_dataset(list(g))
-            if dataset:
-                dataset.sort_versions()
-                yield dataset
-
-    def get_dataset(self, name: str, conn=None) -> DatasetRecord:
-        """Gets a single dataset by name"""
-        d = self._datasets
-        dv = self._datasets_versions
-        query = self._datasets_select(
-            *(getattr(d.c, f) for f in self._dataset_fields),
-            *(getattr(dv.c, f) for f in self._dataset_version_fields),
-        ).where(d.c.name == name)  # type: ignore [attr-defined]
-        j = d.join(dv, d.c.id == dv.c.dataset_id, isouter=True)
-        query = query.select_from(j)
-        ds = self._parse_dataset(self.db.execute(query, conn=conn))
-        if not ds:
-            raise DatasetNotFoundError(f"Dataset {name} not found.")
-        return ds
-
     def update_dataset_status(
         self,
         dataset: DatasetRecord,
         status: int,
         version: Optional[int] = None,
         error_message="",
         error_stack="",
```

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/schema.py` & `dvcx-0.74.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.74.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.74.0/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.74.0/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -863,24 +863,14 @@
         n = self.nodes_table(uri, partial_id)
         query = select(sa.func.count(), sa.func.sum(n.c.size)).select_from(
             n.get_table()
         )
         (res,) = self.db.execute(query)
         return res[0], res[1]
 
-    def return_ds_hook(self, name: str, version: int) -> None:
-        """
-        Hook to be run when a return ds is ready to be saved in a
-        DatasetQuery script.
-        """
-        print(
-            f"{PYTHON_SCRIPT_WRAPPER_CODE}{name}{PYTHON_SCRIPT_WRAPPER_CODE}"
-            f"{version}{PYTHON_SCRIPT_WRAPPER_CODE}"
-        )
-
     def create_udf_table(
         self,
         name: str,
         custom_columns: Sequence["sa.Column"] = (),
     ) -> "sa.Table":
         """
         Create a temporary table for storing custom signals generated by a UDF.
```

### Comparing `dvcx-0.73.0/src/dvcx/dataset.py` & `dvcx-0.74.0/src/dvcx/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 T = TypeVar("T", bound="DatasetRecord")
 V = TypeVar("V", bound="DatasetVersion")
 DD = TypeVar("DD", bound="DatasetDependency")
 
 DATASET_PREFIX = "ds://"
 QUERY_DATASET_NAME_PREFIX = "ds_query_"
+TEMP_DATASET_NAME_PREFIX = "ds_temp_"
 
 
 def parse_dataset_uri(uri: str) -> tuple[str, Optional[int]]:
     """
     Parse dataser uri to extract name and version out of it (if version is defined)
     Example:
         Input: ds://zalando@v3
@@ -381,22 +382,17 @@
         if not other.versions:
             # nothing to merge
             return self
         if not self.versions:
             self.versions = []
 
         self.versions = list(set(self.versions + other.versions))
+        self.versions.sort(key=lambda v: v.version)
         return self
 
-    def sort_versions(self, reverse=False) -> None:
-        """Sorts versions by version number"""
-        if not self.versions:
-            return
-        self.versions.sort(key=lambda v: v.version, reverse=reverse)
-
     def has_version(self, version: int) -> bool:
         return version in self.versions_values
 
     def is_valid_next_version(self, version: int) -> bool:
         """
         Checks if a number can be a valid next latest version for dataset.
         The only rule is that it cannot be lower than current latest version
```

### Comparing `dvcx-0.73.0/src/dvcx/error.py` & `dvcx-0.74.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.74.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/dataset.py` & `dvcx-0.74.0/src/dvcx/lib/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         cache: bool = False,
-    ):
+    ) -> "Self":
         """Create a new dataframe by applying a function to each row to create new
         columns. The function should return a list of new column values corresponding
         to column names defined in the `output` parameter.
 
         Input-output relationship: 1:1
 
         Parameters:
@@ -98,15 +98,15 @@
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         cache: bool = False,
-    ):
+    ) -> "Self":
         """Create a new dataframe by applying a function to each row to generate a new
         set of rows and columns.
 
         Input-output relationship: 1:N
 
         This method is similar to `map()`, uses the same list of parameters, but with
         two key differences:
@@ -139,15 +139,15 @@
         output=None,
         partition_by: Optional[PartitionByType] = None,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         batch=1,
         cache: bool = False,
-    ):
+    ) -> "Self":
         """Create a new dataframe by aggregating a group of rows using a specified
         function, resulting in a new set of rows and columns.
 
         Input-output relationship: N:M
 
         This method bears similarity to `generate()`, employing a comparable set of
         parameters, yet differs in two crucial aspects:
@@ -176,15 +176,15 @@
         params=None,
         output=None,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         batch=1000,
         cache: bool = False,
-    ):
+    ) -> "Self":
         """This is a batch version of map(). It accepts the same parameters plus an
         additional parameter:
 
         `batch` (int), which sets the batch size. The default batch size is 1000.
 
         Input-output relationship: N:N
         """
@@ -206,15 +206,15 @@
         params=None,
         output=None,
         partition_by: Optional[PartitionByType] = None,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         cache: bool = False,
-    ):
+    ) -> "Self":
         """Warning: experimental functionality!
         Create a new dataframe by applying a function to group of rows to create new
         columns. The function should return a nested list of new column values
         corresponding to columns defined in the `output` parameter.
 
         Input-output relationship: N:N
 
@@ -240,16 +240,23 @@
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
             partition_by=partition_by,
         )
 
     def _udf_to_obj(
-        self, udf, target_class, name, params=None, output=None, batch=1, cache=False
-    ):
+        self,
+        udf,
+        target_class: type[UDFBase],
+        name: str,
+        params=None,
+        output=None,
+        batch: int = 1,
+        cache: bool = False,
+    ) -> UDFBase:
         if isinstance(udf, UDFBase):
             if not isinstance(udf, target_class):
                 cls_name = target_class.__name__
                 raise TypeError(
                     f"{name}: expected an instance derived from {cls_name}"
                     f", but received {udf.name}"
                 )
@@ -267,30 +274,30 @@
 
                 if cache:
                     udf.enable_caching()
 
             return udf
 
         if inspect.isfunction(udf):
-            return target_class.create_from_func(udf, params, output, batch)
+            return target_class.from_func(udf, params, output, batch)
 
         if isinstance(udf, type):
             raise TypeError(
                 f"{name} error: The class '{udf}' needs to be instantiated"
                 f" as an object before you can use it as UDF"
             )
 
         if not callable(udf):
             raise TypeError(f"{name} error: instance {udf} must be callable for UDF")
 
-        return target_class.create_from_func(udf, params, output, batch)
+        return target_class.from_func(udf, params, output, batch)
 
     def _validate_args(
         self, name, parallel, workers, min_task_size=None, partition_by=None
-    ):
+    ) -> None:
         msg = None
         if not isinstance(parallel, int) and parallel is not None:
             msg = (
                 f"'parallel' argument must be int or None"
                 f", {parallel.__class__.__name__} was given"
             )
         elif not isinstance(workers, bool) and not isinstance(workers, int):
```

### Comparing `dvcx-0.73.0/src/dvcx/lib/feature.py` & `dvcx-0.74.0/src/dvcx/lib/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     list: Array,
     dict: JSON,
 }
 
 FeatureClass = type["Feature"]
 FeatureClassSeq = Sequence[FeatureClass]
 
-
 # Disable Pydantic warning, see https://github.com/iterative/dvcx/issues/1285
 warnings.filterwarnings(
     "ignore",
     message="Field name .* shadows an attribute in parent",
     category=UserWarning,
 )
 
@@ -91,14 +90,25 @@
         if orig == dict:
             return JSON
 
         args = get_args(typ)
         if orig == Union and len(args) == 2 and (type(None) in args):
             return Feature._convert_type(args[0])
 
+        # Special case for list in JSON: Union[dict, list[dict]]
+        if orig == Union and len(args) >= 2:
+            args_no_nones = [arg for arg in args if arg != type(None)]
+            if len(args_no_nones) == 2:
+                args_no_dicts = [arg for arg in args_no_nones if arg != dict]
+                if len(args_no_dicts) == 1:
+                    if get_origin(args_no_dicts[0]) == list:
+                        arg = get_args(args_no_dicts[0])
+                        if len(arg) == 1 and arg[0] == dict:
+                            return JSON
+
         raise RuntimeError(f"Cannot recognize type {typ}")
 
     @staticmethod
     def _iter_fields(fields):
         for name, f_info in fields.items():
             yield name, f_info.annotation, f_info.is_required()
```

### Comparing `dvcx-0.73.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.74.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/file.py` & `dvcx-0.74.0/src/dvcx/lib/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,22 @@
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     version: str = Field(default="")
     etag: str = Field(default="")
     size: int = Field(default=0)
     vtype: str = Field(default="")
-    location: Optional[dict] = Field(default=None)
+    location: Optional[Union[dict, list[dict]]] = Field(default=None)
 
     _unique_id_keys = ["source", "parent", "name", "etag", "size", "vtype", "location"]
 
     @staticmethod
-    def to_dict(v: Optional[Union[str, dict]]) -> Optional[dict]:
+    def to_dict(
+        v: Optional[Union[str, dict, list[dict]]],
+    ) -> Optional[Union[str, dict, list[dict]]]:
         if v is None or v == "":
             return None
         if isinstance(v, str):
             try:
                 return json.loads(v)
             except Exception as e:
                 raise ValueError(
@@ -103,24 +105,24 @@
 
 
 class FileInfo(FileFeature):
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     size: int = Field(default=0)
-    location: Optional[dict] = Field(default=None)
+    location: Optional[Union[dict, list[dict]]] = Field(default=None)
     vtype: str = Field(default="")
     dir_type: int = Field(default=0)
     owner_name: str = Field(default="")
     owner_id: str = Field(default="")
     is_latest: bool = Field(default=True)
     last_modified: datetime = Field(default=datetime.min)
     version: str = Field(default="")
     etag: str = Field(default="")
     checksum: str = Field(default="")
-    anno: Optional[dict] = Field(default=None)
+    anno: Optional[Union[dict, list[dict]]] = Field(default=None)
     random: int = Field(default_factory=lambda: getrandbits(63))
 
     @field_validator("location", "anno", mode="before")
     @classmethod
     def validate_location(cls, v):
         return File.to_dict(v)
```

### Comparing `dvcx-0.73.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.74.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.74.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.74.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/image_transform.py` & `dvcx-0.74.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.74.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/udf.py` & `dvcx-0.74.0/src/dvcx/lib/udf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import inspect
 import types
 from abc import ABC
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 from dvcx.catalog import get_catalog
 from dvcx.query import udf
 from dvcx.query.schema import DatasetRow
 from dvcx.sql.types import Int, String
 
+if TYPE_CHECKING:
+    from dvxc.query.udf import UDFWrapper
+    from typing_extensions import Self
+
 
 class UDFBase(ABC):
     DEF_OUTPUT_NAME = "result"
     DEF_OUTPUT_TYPE = String
 
     def __init__(self, params=None, output=None, batch=1):
         sign_params, sign_output = self._get_signature(self.process)
@@ -48,15 +52,15 @@
     def set_catalog(self, catalog):
         self._catalog = catalog.copy(db=False)
 
     @property
     def catalog(self):
         return self._catalog
 
-    def to_udf_wrapper(self):
+    def to_udf_wrapper(self) -> "UDFWrapper":
         udf_wrapper = udf(params=self.params, output=self.output, batch=self.batch)
         return udf_wrapper(self)
 
     def setup(self):  # noqa: B027
         """Initialization process executed on each worker before processing begins.
         This is needed for tasks like pre-loading ML models prior to scoring.
         """
@@ -128,47 +132,45 @@
             res_len = len(res)
             if out_len != res_len:
                 raise ValueError(
                     f"{self.name} returned {res_len} values"
                     f" while {out_len} expected. Inputs: {args} Result: {res}"
                 )
 
-    @staticmethod
-    def _create_from_func(
-        target_class, func: Callable, params=None, output=None, batch=1
-    ):
-        if not issubclass(target_class, UDFBase):
-            raise ValueError(
-                f"cannot create UDF from function {func}: "
-                f" not supported target class {target_class}"
-            )
+    @classmethod
+    def _from_func(cls, func: Callable, params=None, output=None, batch=1) -> "Self":
         sign_params, sign_output = UDFBase._get_signature(func)
-        udf = target_class(params or sign_params, output or sign_output, batch=batch)
-        udf.process = lambda *args, **kwargs: func(*args, **kwargs)
+        udf = cls(params or sign_params, output or sign_output, batch=batch)
+        udf.process = func  # type: ignore[method-assign]
         return udf
 
+    @classmethod
+    def from_func(
+        cls, func: Callable, params=None, output=None, batch: int = 1
+    ) -> "UDFBase":
+        return cls._from_func(func, params, output, batch)
+
 
 class Mapper(UDFBase):
     def __init__(self, params=None, output=None, batch=1):
         if batch > 1:
             raise ValueError("Mapper does not support batch")
-
         super().__init__(params, output)
 
     def validate_results(self, results, *args, **kwargs):
         self._validate_result_type(results, *args)
         self._validate_result_length(results, *args)
         return results
 
-    @staticmethod
-    def create_from_func(func, params=None, output=None, batch=1):
+    @classmethod
+    def from_func(cls, func, params=None, output=None, batch=1) -> "Mapper":
         if batch == 1:
-            return UDFBase._create_from_func(Mapper, func, params, output)
+            return super()._from_func(func, params, output)
         else:
-            return UDFBase._create_from_func(BatchMapper, func, params, output, batch)
+            return super(Mapper, BatchMapper)._from_func(func, params, output, batch)
 
 
 class BatchMapper(Mapper):
     def __init__(self, params=None, output=None, batch=1000):
         if batch == 1:
             raise ValueError(f"{self.name} must be batch UDF")
         UDFBase.__init__(self, params, output, batch)
@@ -196,18 +198,14 @@
         if isinstance(results, types.GeneratorType):
             results = tuple(results)
 
         self._validate_result_type(results, *args)
         self._validate_result_batch_length(results, *args)
         return results
 
-    @staticmethod
-    def create_from_func(func, params=None, output=None, batch=1):
-        return UDFBase._create_from_func(Generator, func, params, output)
-
 
 class Aggregator(UDFBase):
     def __init__(self, params=None, output=None, batch=1):
         output = output or {}
         super().__init__(params, DatasetRow.schema | output, batch)
 
     def validate_results(self, results, *args, **kwargs):
@@ -217,26 +215,18 @@
                 yield r
             return
 
         self._validate_result_type(results, *args)
         self._validate_result_batch_length(results, *args)
         return results
 
-    @staticmethod
-    def create_from_func(func, params=None, output=None, batch=1):
-        return UDFBase._create_from_func(Aggregator, func, params, output, batch)
-
 
 class GroupMapper(UDFBase):
     def __init__(self, params=None, output=None, batch=1):
         if batch > 1:
             raise ValueError("GroupMapper does not support batch")
         super().__init__(params, output)
 
     def validate_results(self, results, *args, **kwargs):
         self._validate_result_type(results, *args)
         self._validate_result_length(results, *args)
         return results
-
-    @staticmethod
-    def create_from_func(func, params=None, output=None):
-        return UDFBase._create_from_func(GroupMapper, func, params, output)
```

### Comparing `dvcx-0.73.0/src/dvcx/lib/unstructured.py` & `dvcx-0.74.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/utils.py` & `dvcx-0.74.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/webdataset.py` & `dvcx-0.74.0/src/dvcx/lib/webdataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import json
 import tarfile
 from collections.abc import Sequence
 from typing import Optional, Union, get_args, get_origin
 
 from pydantic import Field
 
@@ -153,28 +154,35 @@
             raise CoreFileNotFoundError(
                 self._tar_stream, self._core_extensions, self.state.stem
             )
 
         wds = self._wds_class(**self.state.data)
 
         new_parent = f"{self._tar_stream.get_full_name()}"
-        etag = self._tar_stream.etag + "-" + str(self.state.core_file.mtime)
+        core_file = self.state.core_file
+        etag_string = "-".join(
+            [self._tar_stream.etag, core_file.name, str(core_file.mtime)]
+        )
+        etag = hashlib.md5(etag_string.encode(), usedforsecurity=False).hexdigest()
+
         f_info = FileInfo(
-            name=self.state.core_file.name,
+            name=core_file.name,
             source=self._tar_stream.source,
             parent=new_parent,
-            size=self.state.core_file.size,
+            size=core_file.size,
             etag=etag,
             vtype="tar",
-            location={
-                "parent": new_parent,
-                "size": self.state.core_file.size,
-                "offset": self.state.core_file.offset,
-                "etag": etag,
-            },
+            location=[
+                {
+                    "parent": new_parent,
+                    "size": core_file.size,
+                    "offset": core_file.offset,
+                    "etag": etag,
+                }
+            ],
         )
 
         self.state = BuilderState()
 
         return f_info, wds
 
     def _get_type(self, ext):
```

### Comparing `dvcx-0.73.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.74.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.74.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/listing.py` & `dvcx-0.74.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/node.py` & `dvcx-0.74.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.74.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.74.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/progress.py` & `dvcx-0.74.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/query/batch.py` & `dvcx-0.74.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/query/builtins.py` & `dvcx-0.74.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/query/dataset.py` & `dvcx-0.74.0/src/dvcx/query/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,25 @@
     Any,
     Callable,
     Optional,
     Protocol,
     TypeVar,
     Union,
 )
+from uuid import uuid4
 
 import attrs
 import sqlalchemy
 from attrs import frozen
 from dill import dumps
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.elements import ColumnClause, ColumnElement
 from sqlalchemy.sql.expression import label
 from sqlalchemy.sql.schema import TableClause
+from sqlalchemy.sql.selectable import Select
 
 from dvcx.asyn import ASYNC_WORKERS, AsyncMapper, OrderedMapper
 from dvcx.catalog import (
     QUERY_SCRIPT_CANCELED_EXIT_CODE,
     QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE,
     get_catalog,
 )
@@ -53,31 +55,31 @@
 
 from .schema import C, UDFParamSpec, normalize_param
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
     from sqlalchemy.sql.elements import ClauseElement
     from sqlalchemy.sql.schema import Table
-    from sqlalchemy.sql.selectable import GenerativeSelect, Select
+    from sqlalchemy.sql.selectable import GenerativeSelect
     from typing_extensions import Concatenate, ParamSpec, Self
 
     from dvcx.catalog import Catalog
     from dvcx.data_storage import AbstractWarehouse
     from dvcx.dataset import DatasetRecord
+    from dvcx.lib.pytorch import PytorchDataset
 
     from .udf import UDFResult
 
     P = ParamSpec("P")
 
 
 INSERT_BATCH_SIZE = 10000
 
 PartitionByType = Union[ColumnElement, Sequence[ColumnElement]]
 JoinPredicateType = Union[str, ColumnClause, ColumnElement]
-S = TypeVar("S", bound="Select[Any]")
 # dependency can be either dataset_name + dataset_version tuple or just storage uri
 # depending what type of dependency we are adding
 DatasetDependencyType = Union[tuple[str, int], StorageURI]
 
 logger = logging.getLogger("dvcx")
 
 
@@ -105,26 +107,26 @@
         cloned.version = None
         return cloned
 
     return _inner
 
 
 class QueryGeneratorFunc(Protocol):
-    def __call__(self, *columns: ColumnElement) -> "Select": ...
+    def __call__(self, *columns: ColumnElement) -> Select: ...
 
 
 @frozen
 class QueryGenerator:
     func: QueryGeneratorFunc
     columns: tuple[ColumnElement, ...]
 
-    def exclude(self, column_names) -> "Select":
+    def exclude(self, column_names) -> Select:
         return self.func(*(c for c in self.columns if c.name not in column_names))
 
-    def select(self, column_names=None) -> "Select":
+    def select(self, column_names=None) -> Select:
         if column_names is None:
             return self.func(*self.columns)
         return self.func(*(c for c in self.columns if c.name in column_names))
 
 
 @frozen
 class StepResult:
@@ -221,32 +223,33 @@
     Yield items from generator then execute a function and yield
     its result.
     """
     yield from generator
     yield func() or []
 
 
+@frozen
 class DatasetDiffOperation(Step):
     """
     Abstract class for operations that are calculation some kind of diff between
     datasets queries like subtract, changed etc.
     """
 
     dq: "DatasetQuery"
     catalog: "Catalog"
 
-    def clone(self):
+    def clone(self) -> "Self":
         return self.__class__(self.dq, self.catalog)
 
     @abstractmethod
     def query(
         self,
-        source_query: sqlalchemy.sql.selectable.Select,
-        target_query: sqlalchemy.sql.selectable.Select,
-    ) -> sqlalchemy.sql.selectable.Select:
+        source_query: Select,
+        target_query: Select,
+    ) -> Select:
         """
         Should return select query that calculates desired diff between dataset queries
         """
 
     def apply(self, query_generator):
         source_query = query_generator.exclude(("id", "parent_id"))
         target_query = self.dq.apply_steps().select()
@@ -291,18 +294,15 @@
                 .subtract(ds)
                 .add_signals(calc_embeddings) # calculae embeddings only on new rows
                 .union(ds) # union with old dataset that's missing new rows
                 .save("dogs_cats_updated")
             )
     """
 
-    dq: "DatasetQuery"
-    catalog: "Catalog"
-
-    def query(self, source_query, target_query) -> sqlalchemy.sql.selectable.Select:
+    def query(self, source_query: Select, target_query: Select) -> Select:
         return self.catalog.warehouse.subtract_query(source_query, target_query)
 
 
 @frozen
 class Changed(DatasetDiffOperation):
     """
     Calculates rows that are changed in a source query compared to target query
@@ -316,18 +316,15 @@
                 .add_signals(calc_embeddings) # calculae embeddings only on changed rows
                 .union(ds) # union with old dataset that's missing updated rows
                 .save("dogs_cats_updated")
             )
 
     """
 
-    dq: "DatasetQuery"
-    catalog: "Catalog"
-
-    def query(self, source_query, target_query) -> sqlalchemy.sql.selectable.Select:
+    def query(self, source_query: Select, target_query: Select) -> Select:
         return self.catalog.warehouse.changed_query(source_query, target_query)
 
 
 def adjust_outputs(
     warehouse: "AbstractWarehouse", row: dict[str, Any], udf: UDFBase
 ) -> dict[str, Any]:
     """
@@ -390,26 +387,24 @@
     parallel: Optional[int] = None
     workers: Union[bool, int] = False
     min_task_size: Optional[int] = None
     is_generator = False
     cache: bool = False
 
     @abstractmethod
-    def create_udf_table(self, udf) -> "Table":
+    def create_udf_table(self) -> "Table":
         """Method that creates a table where temp udf results will be saved"""
 
-    def process_input_query(
-        self, query: "Select[Any]"
-    ) -> tuple["Select[Any]", list["Table"]]:
+    def process_input_query(self, query: Select) -> tuple[Select, list["Table"]]:
         """Apply any necessary processing to the input query"""
         return query, []
 
     @abstractmethod
     def create_result_query(
-        self, udf_table, query, udf
+        self, udf_table: "Table", query: Select
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
         """
         Method that should return query to fetch results from udf and columns
         to select
         """
 
     def udf_table_name(self) -> str:
@@ -419,17 +414,17 @@
     def custom_columns_created(self) -> dict[str, SQLType]:
         return {
             col_name: col_type
             for (col_name, col_type) in self.udf.output.items()
             if col_name not in DATASET_CORE_COLUMN_NAMES
         }
 
-    def populate_udf_table(self, udf_table, query, udf) -> None:
+    def populate_udf_table(self, udf_table: "Table", query: Select) -> None:
         use_partitioning = self.partition_by is not None
-        batching = udf.properties.get_batching(use_partitioning)
+        batching = self.udf.properties.get_batching(use_partitioning)
         workers = self.workers
         if (
             not workers
             and os.environ.get("DVCX_DISTRIBUTED")
             and os.environ.get("DVCX_SETTINGS_WORKERS")
         ):
             # Enable distributed processing by default if the module is available,
@@ -440,28 +435,28 @@
 
         try:
             if workers:
                 from dvcx.catalog.loader import get_distributed_class
 
                 distributor = get_distributed_class(min_task_size=self.min_task_size)
                 distributor(
-                    udf,
+                    self.udf,
                     self.catalog,
                     udf_table,
                     query,
                     workers,
                     processes,
                     is_generator=self.is_generator,
                     use_partitioning=use_partitioning,
                     cache=self.cache,
                 )
             elif processes:
                 # Parallel processing (faster for more CPU-heavy UDFs)
                 udf_info = {
-                    "udf": udf,
+                    "udf": self.udf,
                     "catalog_init": self.catalog.get_init_params(),
                     "id_generator_clone_params": (
                         self.catalog.id_generator.clone_params()
                     ),
                     "metastore_clone_params": self.catalog.metastore.clone_params(),
                     "warehouse_clone_params": self.catalog.warehouse.clone_params(),
                     "table": udf_table,
@@ -481,16 +476,18 @@
                     check=False,
                 )
                 if result.returncode != 0:
                     raise RuntimeError("UDF Execution Failed!")
             else:
                 # Otherwise process single-threaded (faster for smaller UDFs)
                 # Optionally instantiate the UDF instance if a class is provided.
-                if isinstance(udf, UDFFactory):
-                    udf = udf()
+                if isinstance(self.udf, UDFFactory):
+                    udf = self.udf()
+                else:
+                    udf = self.udf
 
                 udf_inputs = batching(
                     self.catalog.warehouse.dataset_select_paginated, query
                 )
                 udf_results = (
                     udf(
                         self.catalog,
@@ -506,15 +503,15 @@
             self.catalog.warehouse.close()
             sys.exit(QUERY_SCRIPT_CANCELED_EXIT_CODE)
         except Exception:
             # Close any open database connections if an error is encountered
             self.catalog.warehouse.close()
             raise
 
-    def create_partitions_table(self, query) -> "Table":
+    def create_partitions_table(self, query: Select) -> "Table":
         """
         Create temporary table with group by partitions.
         """
         assert self.partition_by is not None
 
         if isinstance(self.partition_by, Sequence):
             list_partition_by = self.partition_by
@@ -533,27 +530,27 @@
         ]
         self.catalog.warehouse.db.execute(
             tbl.insert().from_select(cols, query.with_only_columns(*cols))
         )
 
         return tbl
 
-    def clone(self, partition_by: Optional[PartitionByType] = None):
+    def clone(self, partition_by: Optional[PartitionByType] = None) -> "Self":
         if partition_by is not None:
             return self.__class__(
                 self.udf,
                 self.catalog,
                 partition_by=partition_by,
                 parallel=self.parallel,
                 workers=self.workers,
                 min_task_size=self.min_task_size,
             )
         return self.__class__(self.udf, self.catalog)
 
-    def apply(self, query_generator):
+    def apply(self, query_generator: QueryGenerator) -> "StepResult":
         query = query_generator.select()
         temp_tables = []
 
         # Apply partitioning if needed.
         if self.partition_by is not None:
             partition_tbl = self.create_partitions_table(query)
             temp_tables.append(partition_tbl.name)
@@ -562,45 +559,40 @@
             query = (
                 sqlalchemy.select(*subq.c)
                 .select_from(subq)
                 .outerjoin(partition_tbl, partition_tbl.c.id == subq.c.id)
                 .add_columns(*partition_columns())
             )
 
-        if isinstance(self.udf, UDFClassWrapper):
-            udf = self.udf()
-        else:
-            udf = self.udf
-
         query, tables = self.process_input_query(query)
         for t in tables:
             temp_tables.append(t.name)
-        udf_table = self.create_udf_table(udf)
+        udf_table = self.create_udf_table()
         temp_tables.append(udf_table.name)
-        self.populate_udf_table(udf_table, query, udf)
-        q, cols = self.create_result_query(udf_table, query, udf)
+        self.populate_udf_table(udf_table, query)
+        q, cols = self.create_result_query(udf_table, query)
 
         return step_result(q, cols, temp_table_names=temp_tables)
 
 
 @frozen
 class UDFSignal(UDF):
     is_generator = False
 
-    def create_udf_table(self, udf) -> "Table":
+    def create_udf_table(self) -> "Table":
         udf_output_columns: list[sqlalchemy.Column[Any]] = [
             sqlalchemy.Column(col_name, col_type)
-            for (col_name, col_type) in udf.output.items()
+            for (col_name, col_type) in self.udf.output.items()
         ]
 
         return self.catalog.warehouse.create_udf_table(
             self.udf_table_name(), udf_output_columns
         )
 
-    def create_pre_udf_table(self, query: S) -> "Table":
+    def create_pre_udf_table(self, query: Select) -> "Table":
         columns = [
             sqlalchemy.Column(c.name, c.type)
             for c in query.selected_columns
             if c.name != "id"
         ]
         table = self.catalog.warehouse.create_udf_table(self.udf_table_name(), columns)
         select_q = query.with_only_columns(
@@ -615,29 +607,27 @@
         )
 
         self.catalog.warehouse.db.execute(
             table.insert().from_select(list(select_q.selected_columns), select_q)
         )
         return table
 
-    def process_input_query(
-        self, query: "Select[Any]"
-    ) -> tuple["Select[Any]", list["Table"]]:
+    def process_input_query(self, query: Select) -> tuple[Select, list["Table"]]:
         if os.getenv("DVCX_DISABLE_QUERY_CACHE", "") not in ("", "0"):
             return query, []
         table = self.create_pre_udf_table(query)
-        q: Select[Any] = sqlalchemy.select(*table.c).select_from(table)
+        q: Select = sqlalchemy.select(*table.c).select_from(table)
         if query._order_by_clauses:
             # we are adding ordering only if it's explicitly added by user in
             # query part before adding signals
             q = q.order_by(table.c.id)
         return q, [table]
 
     def create_result_query(
-        self, udf_table, query, udf
+        self, udf_table, query
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
         subq = query.subquery()
         original_cols = [c for c in subq.c if c.name not in partition_col_names]
 
         # new signal columns that are added to udf_table
         signal_cols = [c for c in udf_table.c if c.name != "id"]
         signal_name_cols = {c.name: c for c in signal_cols}
@@ -681,33 +671,30 @@
 
 @frozen
 class RowGenerator(UDF):
     """Extend dataset with new rows."""
 
     is_generator = True
 
-    def create_udf_table(self, udf) -> "Table":
+    def create_udf_table(self) -> "Table":
         table_name = self.udf_table_name()
-        if isinstance(udf, UDFFactory):
-            udf = udf()
-
         custom_udf_output_columns: list[sqlalchemy.Column] = [
             sqlalchemy.Column(col_name, col_type)
-            for (col_name, col_type) in udf.output.items()
+            for (col_name, col_type) in self.udf.output.items()
             if col_name not in DATASET_CORE_COLUMN_NAMES
         ]
 
         return self.catalog.warehouse.create_dataset_rows_table(
             table_name,
             custom_columns=custom_udf_output_columns,
             if_not_exists=False,
         )
 
     def create_result_query(
-        self, udf_table, query, udf
+        self, udf_table, query: Select
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
         if not query._order_by_clauses:
             # if we are not selecting all rows in UDF, we need to ensure that
             # we get the same rows as we got as inputs of UDF since selecting
             # without ordering can be non deterministic in some databases
             c = query.selected_columns
             query = query.order_by(c.source, c.parent, c.name, c.version, c.etag)
@@ -724,15 +711,15 @@
             return sqlalchemy.select(*cols).select_from(udf_table_query)
 
         return q, udf_table_query.columns
 
 
 @frozen
 class SQLClause(Step, ABC):
-    def apply(self, query_generator):
+    def apply(self, query_generator: QueryGenerator) -> StepResult:
         query = query_generator.select()
         new_query = self.apply_sql_clause(query)
 
         def q(*columns):
             return new_query.with_only_columns(*columns)
 
         return step_result(q, new_query.selected_columns)
@@ -742,68 +729,68 @@
         pass
 
 
 @frozen
 class SQLSelect(SQLClause):
     args: tuple[Union[str, ColumnElement], ...]
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query) -> Select:
         subquery = query.subquery()
 
         args = [subquery.c[str(c)] if isinstance(c, (str, C)) else c for c in self.args]
         if not args:
             args = subquery.c
 
         return sqlalchemy.select(*args).select_from(subquery)
 
 
 @frozen
 class SQLSelectExcept(SQLClause):
     args: tuple[str, ...]
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query: Select) -> Select:
         subquery = query.subquery()
         names = set(self.args)
         args = [c for c in subquery.c if c.name not in names]
         return sqlalchemy.select(*args).select_from(subquery)
 
 
 @frozen
 class SQLMutate(SQLClause):
     args: tuple[ColumnElement, ...]
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query: Select) -> Select:
         subquery = query.subquery()
         return sqlalchemy.select(*subquery.c, *self.args).select_from(subquery)
 
 
 @frozen
 class SQLFilter(SQLClause):
     expressions: tuple[ColumnElement, ...]
 
     def __and__(self, other):
         return self.__class__(self.expressions + other)
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query: Select) -> Select:
         return query.filter(*self.expressions)
 
 
 @frozen
 class SQLOrderBy(SQLClause):
     args: tuple[ColumnElement, ...]
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query: Select) -> Select:
         return query.order_by(*self.args)
 
 
 @frozen
 class SQLLimit(SQLClause):
     n: int
 
-    def apply_sql_clause(self, query):
+    def apply_sql_clause(self, query: Select) -> Select:
         return query.limit(self.n)
 
 
 @frozen
 class SQLOffset(SQLClause):
     offset: int
 
@@ -818,15 +805,15 @@
 
 
 @frozen
 class SQLUnion(Step):
     query1: "DatasetQuery"
     query2: "DatasetQuery"
 
-    def apply(self, query_generator):
+    def apply(self, query_generator: QueryGenerator) -> StepResult:
         q1 = self.query1.apply_steps().select().subquery()
         q2 = self.query2.apply_steps().select().subquery()
         columns1, columns2 = fill_columns(q1.columns, q2.columns)
 
         def q(*columns):
             names = {c.name for c in columns}
             col1 = [c for c in columns1 if c.name in names]
@@ -882,15 +869,15 @@
                         " part of the join"
                     )
                 else:
                     continue
             else:
                 self.validate_expression(c, q1, q2)
 
-    def apply(self, query_generator):
+    def apply(self, query_generator: QueryGenerator) -> StepResult:
         q1 = self.query1.apply_steps().select().subquery(self.query1.table.name)
         q2 = self.query2.apply_steps().select().subquery(self.query2.table.name)
 
         q1_columns = list(q1.c)
         q1_column_names = {c.name for c in q1_columns}
         q2_columns = [
             c
@@ -944,18 +931,18 @@
 
 @frozen
 class GroupBy(Step):
     """Group rows by a specific column."""
 
     cols: PartitionByType
 
-    def clone(self):
+    def clone(self) -> "Self":
         return self.__class__(self.cols)
 
-    def apply(self, query_generator):
+    def apply(self, query_generator: QueryGenerator) -> StepResult:
         query = query_generator.select()
         grouped_query = query.group_by(*self.cols)
 
         def q(*columns):
             return grouped_query.with_only_columns(*columns)
 
         return step_result(q, grouped_query.selected_columns)
@@ -1005,14 +992,16 @@
         self._chunk_total: Optional[int] = None
         self.temp_table_names: list[str] = []
         self.dependencies: set[DatasetDependencyType] = set()
         self.table = self.get_table()
         self.starting_step: StartingStep
         self.name: Optional[str] = None
         self.version: Optional[int] = None
+        # if run with Catalog.query(...) it will have this env variable defined
+        self.query_session_uuid = os.getenv("DVCX_QUERY_SESSION_UUID", None)
 
         if path:
             self.starting_step = IndexingStep(
                 path, self.catalog, {"client_config": client_config}, recursive
             )
         elif name:
             version = version or self.catalog.get_dataset(name).latest_version
@@ -1186,14 +1175,45 @@
                 "To install run:\n\n"
                 "  pip install 'dvcx[pandas]'\n"
             ) from exc
 
         records = self.to_records()
         return pd.DataFrame.from_records(records)
 
+    def to_pytorch(
+        self,
+        *params: UDFParamSpec,
+        transform=None,
+        workers: int = ASYNC_WORKERS,
+        cache: bool = False,
+    ) -> "PytorchDataset":
+        try:
+            import torch  # noqa: F401
+        except ImportError as exc:
+            raise ImportError(
+                "Missing required dependency 'torch' for DatasetQuery.to_pytorch()"
+            ) from exc
+        from dvcx.lib.pytorch import PytorchDataset
+
+        if self.attached:
+            ds = self
+        else:
+            ds_name = self.catalog.generate_query_dataset_name()
+            ds = self.save(ds_name)
+        assert ds.name is not None  # for mypy
+        return PytorchDataset(
+            params,
+            ds.name,
+            ds.version,
+            transform=transform,
+            workers=workers,
+            cache=cache,
+            catalog=self.catalog,
+        )
+
     def shuffle(self) -> "DatasetQuery":
         # ToDo: implement shaffle based on seed and/or generating random column
         return self.order_by(C.random)
 
     def show(self, limit=20) -> None:
         df = self.limit(limit).to_pandas()
         no_footer = re.sub(r"\n\[\d+ rows x \d+ columns\]$", "", str(df))
@@ -1418,14 +1438,17 @@
         For distributed processing with the appropriate distributed module installed,
         workers can optionally be specified as >= 1 for a specific number of workers,
         or set to True for the default of all nodes in the cluster.
         As well, a custom minimum task size (min_task_size) can be provided to send
         at least that minimum number of rows to each distributed worker, mostly useful
         if there are a very large number of small tasks to process.
         """
+        if isinstance(udf, UDFClassWrapper):
+            # This is a bare decorated class, "instantiate" it now.
+            udf = udf()
         query = self.clone()
         query.steps.append(
             UDFSignal(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
                 parallel=parallel,
@@ -1454,14 +1477,17 @@
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
         cache: bool = False,
     ) -> "Self":
+        if isinstance(udf, UDFClassWrapper):
+            # This is a bare decorated class, "instantiate" it now.
+            udf = udf()
         query = self.clone()
         steps = query.steps
         steps.append(
             RowGenerator(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
@@ -1491,22 +1517,30 @@
                     StorageURI(dataset.name),
                     version,
                     storage.uri,
                     storage.timestamp_str,
                 )
 
     def save(
-        self, name: str, version: Optional[int] = None, **kwargs
+        self, name: Optional[str] = None, version: Optional[int] = None, **kwargs
     ) -> "DatasetQuery":
         """Save the query as a dataset."""
         try:
-            if version and self.catalog.get_dataset(name).has_version(version):
+            if name and version and self.catalog.get_dataset(name).has_version(version):
                 raise RuntimeError(f"Dataset {name} already has version {version}")
         except DatasetNotFoundError:
             pass
+        if not name and version:
+            raise RuntimeError("Cannot set version for temporary datasets")
+
+        if not name:
+            # missing name means this is temp dataset
+            if not self.query_session_uuid:
+                raise RuntimeError("Temporary dataset must be created using session")
+            name = self.catalog.generate_temp_dataset_name(self.query_session_uuid)
 
         try:
             query = self.apply_steps()
 
             missing_default_columns = [
                 c_name
                 for c_name in DATASET_CORE_COLUMN_NAMES
@@ -1563,35 +1597,47 @@
             self._add_dependencies(dataset, version)  # type: ignore [arg-type]
         finally:
             self.cleanup()
 
         return DatasetQuery(name=name, version=version, catalog=self.catalog)
 
 
+def _get_output_fd_for_write() -> Union[str, int]:
+    handle = os.getenv("DVCX_OUTPUT_FD")
+    if not handle:
+        return os.devnull
+
+    if os.name != "nt":
+        return int(handle)
+
+    import msvcrt
+
+    return msvcrt.open_osfhandle(int(handle), os.O_WRONLY)  # type: ignore[attr-defined]
+
+
 def query_wrapper_save(dataset_query: DatasetQuery) -> DatasetQuery:
     """
     Wrapper function that wraps the last statement of user query script for creating
     new dataset
     Last statement MUST be instance of DatasetQuery, otherwise script exits with
     error code 10
     """
     if not isinstance(dataset_query, DatasetQuery):
         sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
 
-    if isinstance(dataset_query, DatasetQuery):
-        if dataset_query.attached:
-            dataset_query.catalog.warehouse.return_ds_hook(
-                dataset_query.name,  # type: ignore [arg-type]
-                dataset_query.version,  # type: ignore [arg-type]
-            )
-        else:
-            ds_name = dataset_query.catalog.generate_query_dataset_name()
-            dataset_query.catalog.warehouse.return_ds_hook(ds_name, 1)
-            dataset_query.save(ds_name)
+    if dataset_query.attached:
+        name = dataset_query.name
+        version = dataset_query.version
+    else:
+        name = dataset_query.catalog.generate_query_dataset_name()
+        dataset_query.save(name)
+        version = 1
 
+    with open(_get_output_fd_for_write(), mode="w") as out:
+        print(json.dumps({"dataset": (name, version)}), file=out)
     return dataset_query
 
 
 def query_wrapper_print(dataset_query: DatasetQuery) -> DatasetQuery:
     """
     Wrapper function that wraps the last statement of user query script for printing
     results in console.
@@ -1619,17 +1665,47 @@
         columns.insert(0, "id")
 
     preview_query = (
         dataset_query.select(*columns)
         .limit(preview_args.get("limit", 10))
         .offset(preview_args.get("offset", 0))
     )
-    records = json.dumps(preview_query.to_records(), default=_json_serialize)
-    print("__ds_records__", records, "__ds_records__", sep="")
+
+    with open(_get_output_fd_for_write(), mode="w") as out:
+        d = {"preview": preview_query.to_records()}
+        print(json.dumps(d, default=_json_serialize), file=out)
     return dataset_query
 
 
 def _random_string(length: int) -> str:
     return "".join(
         random.choice(string.ascii_letters + string.digits)  # noqa: S311
         for i in range(length)
     )
+
+
+class Session:
+    """
+    Object that injects it's unique uuid to DatasetQuery instances created
+    through it. This is needed for things like temp datasets.
+    """
+
+    def __init__(self, catalog: Optional["Catalog"] = None):
+        self.uuid = uuid4().hex
+        self.catalog = catalog or get_catalog()
+
+    def DatasetQuery(self, *args, **kwargs) -> DatasetQuery:  # noqa: N802
+        ds = DatasetQuery(*args, **kwargs)
+        ds.query_session_uuid = self.uuid
+        return ds
+
+    def cleanup(self) -> None:
+        self.catalog.cleanup_temp_datasets(self.uuid)
+
+
+@contextlib.contextmanager
+def session(catalog: Optional["Catalog"] = None):
+    session = Session(catalog=catalog)
+    try:
+        yield session
+    finally:
+        session.cleanup()
```

### Comparing `dvcx-0.73.0/src/dvcx/query/dispatch.py` & `dvcx-0.74.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/query/schema.py` & `dvcx-0.74.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/query/udf.py` & `dvcx-0.74.0/src/dvcx/query/udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         method: Optional[str] = None,
     ):
         self.udf_class = udf_class
         self.udf_method = method
         self.properties = properties
         self.output = properties.output
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> "UDFFactory":
         return UDFFactory(
             self.udf_class,
             args,
             kwargs,
             self.properties,
             self.udf_method,
         )
@@ -229,9 +229,8 @@
         udf_func = self.udf_class(*self.args, **self.kwargs)
         if self.udf_method:
             udf_func = getattr(udf_func, self.udf_method)
 
         return UDFWrapper(udf_func, self.properties)
 
 
-# UDFs can be callables or classes that instantiate into callables
-UDFType = Union[UDFBase, UDFFactory, UDFClassWrapper]
+UDFType = Union[UDFBase, UDFFactory]
```

### Comparing `dvcx-0.73.0/src/dvcx/remote/studio.py` & `dvcx-0.74.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/default/base.py` & `dvcx-0.74.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/functions/array.py` & `dvcx-0.74.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/functions/path.py` & `dvcx-0.74.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/selectable.py` & `dvcx-0.74.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.74.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.74.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/types.py` & `dvcx-0.74.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/sql/utils.py` & `dvcx-0.74.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/storage.py` & `dvcx-0.74.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx/utils.py` & `dvcx-0.74.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.74.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.73.0
+Version: 0.74.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -61,14 +61,15 @@
 Requires-Dist: pytest-benchmark[histogram]; extra == "tests"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "tests"
 Requires-Dist: pytest-xdist>=3.3.1; extra == "tests"
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
+Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
```

### Comparing `dvcx-0.73.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.74.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 .github/workflows/update-template.yaml
 .reuse/dep5
 LICENSES/Apache-2.0.txt
 LICENSES/BSD-3-Clause.txt
 LICENSES/Python-2.0.txt
 docs/udfs.md
 examples/blip2_image_desc_lib.py
+examples/clip.py
 examples/common_sql_functions.py
 examples/dir_expansion.py
 examples/hf_pipeline.py
 examples/iptc_exif_xmp_lib.py
 examples/llava2_image_desc_lib.py
 examples/loader.py
 examples/openai_image_desc_lib.py
```

### Comparing `dvcx-0.73.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.74.0/src/dvcx.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -52,13 +52,14 @@
 pytest-benchmark[histogram]
 pytest-asyncio>=0.23.2
 pytest-xdist>=3.3.1
 virtualenv
 dulwich
 hypothesis
 numpy
+open_clip_torch
 aiotools>=1.7.0
 requests-mock
 
 [vector]
 numpy
 scipy
```

### Comparing `dvcx-0.73.0/tests/benchmarks/conftest.py` & `dvcx-0.74.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/conftest.py` & `dvcx-0.74.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/data.py` & `dvcx-0.74.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/func/test_catalog.py` & `dvcx-0.74.0/tests/func/test_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import io
+import json
 import os
+from contextlib import suppress
 from pathlib import Path
 from textwrap import dedent
-from unittest.mock import patch
 from urllib.parse import urlparse
+from uuid import uuid4
 
 import pytest
 import yaml
 from fsspec.implementations.local import LocalFileSystem
 
 from dvcx.catalog import indexer_formats, parse_edvcx_file
+from dvcx.dataset import TEMP_DATASET_NAME_PREFIX
 from dvcx.error import (
+    DatasetNotFoundError,
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
     StorageNotFoundError,
 )
 
 from ..data import ENTRIES
@@ -29,61 +34,57 @@
 
 @pytest.fixture
 def pre_created_ds_name():
     return "pre_created_dataset"
 
 
 @pytest.fixture
-def mock_subprocess_run(cloud_test_catalog, listed_bucket):
-    from subprocess import CompletedProcess
-
-    with patch("subprocess.run") as mock_run:
-        # create dataset which would be created in subprocess
-        ds_name = cloud_test_catalog.catalog.generate_query_dataset_name()
-        ds_version = 1
-        cloud_test_catalog.catalog.create_dataset_from_sources(
-            ds_name,
-            [f"{cloud_test_catalog.src_uri}/dogs/*"],
-            recursive=True,
-        )
-        res = CompletedProcess([], 0)
-        std = f"__ds__{ds_name}__ds__{ds_version}__ds__\nuser log 1\nuser log 2"
-        res.stdout = str.encode(std)
-        mock_run.return_value = res
-
-        yield mock_run
+def mock_os_pipe(mocker):
+    r, w = os.pipe()
+    mocker.patch("os.pipe", return_value=(r, w))
+
+    try:
+        yield (r, w)
+    finally:
+        with suppress(OSError):
+            os.close(r)
+        with suppress(OSError):
+            os.close(w)
 
 
 @pytest.fixture
-def mock_subprocess_run_error_exit_code(cloud_test_catalog):
-    from subprocess import CompletedProcess
-
-    with patch("subprocess.run") as mock_run:
-        mock_run.return_value = CompletedProcess([], 1)
-        yield mock_run
+def mock_popen(mocker):
+    m = mocker.patch(
+        "subprocess.Popen", returncode=0, stdout=io.StringIO(), stderr=io.StringIO()
+    )
+    m.return_value.__enter__.return_value = m
+    # keep in sync with the returncode
+    m.poll.side_effect = lambda: m.returncode if m.poll.call_count > 1 else None
+    return m
 
 
 @pytest.fixture
-def mock_subprocess_run_error_exit_code_10(cloud_test_catalog):
-    from subprocess import CompletedProcess
-
-    with patch("subprocess.run") as mock_run:
-        mock_run.return_value = CompletedProcess([], 10)
-        yield mock_run
-
+def mock_popen_dataset_created(
+    mock_popen, cloud_test_catalog, mock_os_pipe, listed_bucket
+):
+    # create dataset which would be created in subprocess
+    ds_name = cloud_test_catalog.catalog.generate_query_dataset_name()
+    ds_version = 1
+    cloud_test_catalog.catalog.create_dataset_from_sources(
+        ds_name,
+        [f"{cloud_test_catalog.src_uri}/dogs/*"],
+        recursive=True,
+    )
 
-@pytest.fixture
-def mock_subprocess_run_dataset_not_created(cloud_test_catalog):
-    from subprocess import CompletedProcess
+    _, w = mock_os_pipe
+    with open(w, mode="w", closefd=False) as f:
+        f.write(json.dumps({"dataset": (ds_name, ds_version)}))
 
-    with patch("subprocess.run") as mock_run:
-        res = CompletedProcess([], 0)
-        res.stdout = b"random str"
-        mock_run.return_value = res
-        yield mock_run
+    mock_popen.configure_mock(stdout=io.StringIO("user log 1\nuser log 2"))
+    yield mock_popen
 
 
 @pytest.fixture
 def fake_index(catalog):
     src = "s3://whatever"
     make_index(catalog, src, ENTRIES)
     return src
@@ -928,15 +929,45 @@
 def test_index_error(cloud_test_catalog):
     protocol = cloud_test_catalog.src_uri.split("://", 1)[0]
     # XXX: different clients raise inconsistent exceptions
     with pytest.raises(Exception):  # noqa: B017
         cloud_test_catalog.catalog.index([f"{protocol}://does_not_exist"])
 
 
-def test_query(cloud_test_catalog, mock_subprocess_run):
+def test_generate_temp_dataset_name_with_query_session_uuid(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+    query_session_uuid = uuid4().hex
+    name = catalog.generate_temp_dataset_name(query_session_uuid)
+    assert name.startswith(f"{TEMP_DATASET_NAME_PREFIX}{query_session_uuid}")
+
+
+def test_clean_temp_dataset(cloud_test_catalog):
+    # if temp dataset is created by using dvcx as a lib in client's code, it
+    # needs to be created using sessions which will inject it's unique query
+    # session uuid
+    catalog = cloud_test_catalog.catalog
+    query_session_uuid = uuid4().hex
+
+    ds_name = catalog.generate_temp_dataset_name(query_session_uuid)
+    dataset = catalog.create_dataset_from_sources(
+        ds_name,
+        [f"{cloud_test_catalog.src_uri}/dogs/*"],
+        recursive=True,
+    )
+    assert dataset.name == ds_name
+
+    catalog.cleanup_temp_datasets("wrong_uuid")
+    catalog.get_dataset(ds_name)
+
+    catalog.cleanup_temp_datasets(query_session_uuid)
+    with pytest.raises(DatasetNotFoundError):
+        catalog.get_dataset(ds_name)
+
+
+def test_query(cloud_test_catalog, mock_popen_dataset_created):
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
     DatasetQuery({src_uri!r})
     """
@@ -959,33 +990,31 @@
 
     query_script = "syntax error"
 
     with pytest.raises(QueryScriptCompileError):
         catalog.query(query_script)
 
 
-def test_query_subprocess_wrong_return_code(
-    cloud_test_catalog, mock_subprocess_run_error_exit_code
-):
+def test_query_subprocess_wrong_return_code(mock_popen, cloud_test_catalog):
+    mock_popen.configure_mock(returncode=1)
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""
 from dvcx.query import DatasetQuery, C
 DatasetQuery('{src_uri}')
     """
 
     with pytest.raises(QueryScriptRunError) as exc_info:
         catalog.query(query_script)
         assert str(exc_info.value).startswith("Query script exited with error code 1")
 
 
-def test_query_last_statement_not_expression(
-    cloud_test_catalog, mock_subprocess_run_error_exit_code_10
-):
+def test_query_last_statement_not_expression(mock_popen, cloud_test_catalog):
+    mock_popen.configure_mock(returncode=10)
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""
 from dvcx.query import DatasetQuery, C
 ds = DatasetQuery('{src_uri}')
     """
@@ -994,17 +1023,16 @@
         catalog.query(query_script)
         assert str(exc_info.value).startswith(
             "Query script failed to compile, "
             "reason: Last line in a script was not an expression"
         )
 
 
-def test_query_last_statement_not_ds_query_instance(
-    cloud_test_catalog, mock_subprocess_run_error_exit_code_10
-):
+def test_query_last_statement_not_ds_query_instance(mock_popen, cloud_test_catalog):
+    mock_popen.configure_mock(returncode=10)
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""
 from dvcx.query import DatasetQuery, C
 ds = DatasetQuery('{src_uri}')
 5
@@ -1013,27 +1041,27 @@
     with pytest.raises(QueryScriptRunError) as exc_info:
         catalog.query(query_script)
         assert str(exc_info.value).startswith(
             "Last line in a script was not an instance of DatasetQuery"
         )
 
 
-def test_query_dataset_not_returned(
-    cloud_test_catalog, mock_subprocess_run_dataset_not_created
-):
+def test_query_dataset_not_returned(mock_popen, cloud_test_catalog):
+    mock_popen.configure_mock(stdout=io.StringIO("random str"))
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""
 from dvcx.query import DatasetQuery, C
 DatasetQuery('{src_uri}')
     """
 
-    with pytest.raises(QueryScriptDatasetNotFound):
+    with pytest.raises(QueryScriptDatasetNotFound) as e:
         catalog.query(query_script, save=True)
+    assert e.value.output == "random str"
 
 
 def test_storage_stats(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     with pytest.raises(StorageNotFoundError):
```

### Comparing `dvcx-0.73.0/tests/func/test_client.py` & `dvcx-0.74.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/func/test_dataset_query.py` & `dvcx-0.74.0/tests/func/test_dataset_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,29 @@
 import sqlalchemy
 from dateutil.parser import isoparse
 from sqlalchemy import tuple_
 
 from dvcx.catalog import indexer_formats
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.warehouse import RANDOM_BITS
-from dvcx.dataset import DatasetDependencyType
+from dvcx.dataset import TEMP_DATASET_NAME_PREFIX, DatasetDependencyType
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetInvalidVersionError, DatasetNotFoundError
-from dvcx.lib.param import Label
+from dvcx.lib.param import Label, Text
 from dvcx.node import Node
-from dvcx.query import C, DatasetQuery, DatasetRow, LocalFilename, Object, Stream, udf
+from dvcx.query import (
+    C,
+    DatasetQuery,
+    DatasetRow,
+    LocalFilename,
+    Object,
+    Stream,
+    session,
+    udf,
+)
 from dvcx.query.builtins import checksum, index_tar
 from dvcx.query.dataset import QueryStep
 from dvcx.sql import functions
 from dvcx.sql.functions.array import cosine_distance, euclidean_distance
 from dvcx.sql.types import (
     JSON,
     Array,
@@ -236,14 +245,34 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
+def test_saving_temp_dataset(cloud_test_catalog, dogs_cats_dataset):
+    catalog = cloud_test_catalog.catalog
+    ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
+    ds.query_session_uuid = uuid.uuid4().hex
+
+    ds2 = ds.save()
+    assert ds2.name.startswith(TEMP_DATASET_NAME_PREFIX)
+    assert isinstance(ds2, DatasetQuery)
+    assert (
+        {row.name for row in catalog.ls_dataset_rows(dogs_cats_dataset.name, 1)}
+        == {row.name for row in catalog.ls_dataset_rows(ds2.name, ds2.version)}
+        == {"cat1", "cat2", "dog1", "dog2", "dog3", "dog4"}
+    )
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
 def test_query_specific_dataset_set_proper_dataset_name_version(
     cloud_test_catalog, dogs_cats_dataset
 ):
     catalog = cloud_test_catalog.catalog
     ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
     assert ds.name == dogs_cats_dataset.name
     assert ds.version == 1
@@ -1251,14 +1280,39 @@
         .filter(C("label").in_(["cat", "dog"]))
         .save("cats-dogs")
     )
     results = list(ds.order_by("name").extract(Label("label", ["cat", "dog"])))
     assert results == [(0,)] * 2 + [(1,)] * 4
 
 
+# Test hf and non-hf tokenizers
+@pytest.mark.parametrize("tokenizer_model", ["ViT-B-32", "hf-hub:timm/ViT-B-16-SigLIP"])
+@pytest.mark.parametrize(
+    "cloud_type, version_aware",
+    [("file", False)],
+    indirect=True,
+)
+def test_text_param(cloud_test_catalog, listed_bucket, tokenizer_model):
+    import open_clip
+    import torch
+
+    ctc = cloud_test_catalog
+
+    @udf(params=("name",), output={"text": String})
+    def extract_text(name):
+        return (name,)
+
+    ds = DatasetQuery(ctc.src_uri, catalog=ctc.catalog).add_signals(extract_text)
+
+    tokenizer = open_clip.get_tokenizer(tokenizer_model)
+
+    for row in ds.extract(Text("text", tokenizer)):
+        assert row[0].dtype == torch.int64
+
+
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
 def test_union(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
@@ -3126,14 +3180,58 @@
     import pandas as pd
 
     df = simple_ds_query.to_pandas()
     expected = pd.DataFrame.from_records(SIMPLE_DS_QUERY_RECORDS)
     assert (df == expected).all(axis=None)
 
 
+@pytest.mark.parametrize("use_cache", [False, True])
+@pytest.mark.parametrize("cloud_type,version_aware", [("file", False)], indirect=True)
+def test_to_pytorch(cloud_test_catalog, dogs_dataset, use_cache):
+    from torch.utils.data import IterableDataset
+
+    catalog = cloud_test_catalog.catalog
+    q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
+    results = set()
+    pt_dataset = q.to_pytorch("name", Stream(), cache=use_cache)
+    assert isinstance(pt_dataset, IterableDataset)
+    for name, stream in pt_dataset:
+        with stream:
+            value = stream.read().decode("utf-8")
+        results.add((name, value))
+    assert results == {
+        ("dog1", "woof"),
+        ("dog2", "arf"),
+        ("dog3", "bark"),
+        ("dog4", "ruff"),
+    }
+
+
+@pytest.mark.parametrize("use_cache", [False, True])
+@pytest.mark.parametrize("cloud_type,version_aware", [("file", False)], indirect=True)
+def test_to_pytorch_from_path(cloud_test_catalog, use_cache):
+    from torch.utils.data import IterableDataset
+
+    ctc = cloud_test_catalog
+    q = DatasetQuery(path=ctc.src_uri, catalog=ctc.catalog).filter(C.name.glob("dog*"))
+    results = set()
+    pt_dataset = q.to_pytorch("name", Stream(), cache=use_cache)
+    assert isinstance(pt_dataset, IterableDataset)
+    for name, stream in pt_dataset:
+        with stream:
+            value = stream.read().decode("utf-8")
+        results.add((name, value))
+    assert results == {
+        ("dog1", "woof"),
+        ("dog2", "arf"),
+        ("dog3", "bark"),
+        ("dog4", "ruff"),
+    }
+
+
 @pytest.mark.parametrize("method", ["to_records", "extract"])
 @pytest.mark.parametrize("save", [True, False])
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -3521,7 +3619,64 @@
         DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
     assert str(exc_info.value) == (
         "Missing default columns from final query: id, vtype, dir_type, parent_id, "
         "parent, checksum, etag, version, is_latest, last_modified, size, "
         "owner_name, owner_id, anno, random, location, source"
     )
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_temp_dataset_used_and_removed(cloud_test_catalog, dogs_cats_dataset):
+    catalog = cloud_test_catalog.catalog
+
+    with session(catalog=catalog) as query_session:
+        temp = query_session.DatasetQuery(
+            name=dogs_cats_dataset.name, catalog=catalog
+        ).save()
+        (
+            query_session.DatasetQuery(name=temp.name, catalog=catalog)
+            .filter(C.name.glob("dog*"))
+            .save("dogs")
+        )
+        (
+            query_session.DatasetQuery(name=temp.name, catalog=catalog)
+            .filter(C.name.glob("cat*"))
+            .save("cats")
+        )
+
+    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
+        "dog1",
+        "dog2",
+        "dog3",
+        "dog4",
+    }
+    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
+        "cat1",
+        "cat2",
+    }
+
+    # make sure temp is removed
+    assert (
+        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
+    )
+    # check one more time 2 datasets created out of temp are present: dogs and cats
+    assert "cats" in [d.name for d in catalog.ls_datasets()]
+    assert "dogs" in [d.name for d in catalog.ls_datasets()]
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_temp_dataset_used_outside_session(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+
+    with pytest.raises(RuntimeError) as exc_info:
+        DatasetQuery(name=dogs_dataset.name, catalog=catalog).save()
+
+    assert str(exc_info.value) == "Temporary dataset must be created using session"
```

### Comparing `dvcx-0.73.0/tests/func/test_datasets.py` & `dvcx-0.74.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/func/test_ls.py` & `dvcx-0.74.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/func/test_pull.py` & `dvcx-0.74.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/func/test_pytorch.py` & `dvcx-0.74.0/tests/func/test_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     yield DatasetQuery(uri).add_signals(extract_label).save("fake")
 
     catalog.remove_dataset("fake", version=1)
     catalog.id_generator.cleanup_for_tests()
 
 
 def test_pytorch_dataset(tmp_path, fake_dataset):
-    transform = v2.Resize((64, 64))
+    transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
     pt_dataset = PytorchDataset(
         params=[Image(), "label"],
         name=fake_dataset.name,
         version=fake_dataset.version,
         transform=transform,
     )
     for img, label in pt_dataset:
```

### Comparing `dvcx-0.73.0/tests/func/test_query.py` & `dvcx-0.74.0/tests/func/test_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from itertools import dropwhile
 from textwrap import dedent
 
 import dill
 import pytest
 
-from dvcx.catalog import QUERY_DATASET_NAME_PREFIX
+from dvcx.catalog import QUERY_DATASET_NAME_PREFIX, TEMP_DATASET_NAME_PREFIX
 from dvcx.cli import query
 
 
 @pytest.fixture
 def catalog_info_filepath(cloud_test_catalog_tmpfile, tmp_path):
     catalog = cloud_test_catalog_tmpfile.catalog
 
@@ -75,23 +74,16 @@
 
     filepath = tmp_path / "query_script.py"
     filepath.write_text(query_script)
 
     ds_name = "my-dataset"
     query(catalog, str(filepath), ds_name, columns=["name"])
     captured = capsys.readouterr()
-    assert captured.err == ""
 
-    # drop lines with progress bars or empty lines, until we get to the table
-    header, *rows = list(
-        dropwhile(
-            lambda line: not line or "Listing" in line,
-            captured.out.splitlines(),
-        )
-    )
+    header, *rows = captured.out.splitlines()
     assert header.strip() == "name"
     name_rows = {row.split()[1] for row in rows}
     assert name_rows == {"cat1", "cat2", "description", "dog1", "dog2", "dog3", "dog4"}
 
 
 def test_query(cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath):
     catalog = cloud_test_catalog_tmpfile.catalog
@@ -210,7 +202,92 @@
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
+
+
+def test_query_with_temp_dataset(
+    cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
+):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    src_uri = cloud_test_catalog_tmpfile.src_uri
+
+    query_script = f"""\
+    from dvcx.query import C, DatasetQuery
+
+    # creating temp dataset for optimization
+    temp = DatasetQuery({src_uri!r}, catalog=catalog).save()
+    DatasetQuery(
+        name=temp.name, catalog=catalog
+    ).filter(C.name.glob("cat*")).save("cats")
+    DatasetQuery(
+        name=temp.name, catalog=catalog
+    ).filter(C.name.glob("dog*")).save("dogs")
+    """
+    query_script = setup_catalog(query_script, catalog_info_filepath)
+
+    catalog.query(query_script, save=True)
+
+    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
+        "dog1",
+        "dog2",
+        "dog3",
+        "dog4",
+    }
+    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
+        "cat1",
+        "cat2",
+    }
+
+    # make sure temp is removed
+    assert (
+        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
+    )
+    # check one more time only 2 datasets are present: dogs and cats
+    assert sorted([d.name for d in catalog.ls_datasets()]) == ["cats", "dogs"]
+
+
+def test_query_with_temp_dataset_using_session(
+    cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
+):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    src_uri = cloud_test_catalog_tmpfile.src_uri
+
+    query_script = f"""\
+    from dvcx.query import C, DatasetQuery, session
+
+    with session(catalog=catalog) as session:
+        # creating temp dataset for optimization
+        temp = DatasetQuery({src_uri!r}, catalog=catalog).save()
+        DatasetQuery(name=temp.name, catalog=catalog).filter(
+            C.name.glob("cat*")
+        ).save("cats")
+        DatasetQuery(name=temp.name, catalog=catalog).filter(
+            C.name.glob("dog*")
+        ).save("dogs")
+
+    DatasetQuery(name="dogs", catalog=catalog)
+    """
+    query_script = setup_catalog(query_script, catalog_info_filepath)
+
+    catalog.query(query_script, save=True)
+
+    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
+        "dog1",
+        "dog2",
+        "dog3",
+        "dog4",
+    }
+    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
+        "cat1",
+        "cat2",
+    }
+
+    # make sure temp is removed
+    assert (
+        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
+    )
+    # check one more time only 2 datasets are present: dogs and cats
+    assert sorted([d.name for d in catalog.ls_datasets()]) == ["cats", "dogs"]
```

### Comparing `dvcx-0.73.0/tests/test_cli_e2e.py` & `dvcx-0.74.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.74.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/lib/test_feature.py` & `dvcx-0.74.0/tests/unit/lib/test_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from decimal import Decimal
-from typing import Optional
+from typing import Optional, Union
 
 import pytest
 from pydantic import Field, ValidationError
 
 from dvcx.lib.feature import Feature, ShallowFeature
 from dvcx.sql.types import JSON, Array, Binary, Boolean, DateTime, Int, String
 
@@ -397,7 +397,18 @@
     class MyTest2(Feature):
         b: MyTest1
 
     class MyTest3(Feature):
         c: MyTest2
 
     assert MyTest3.c.b.a.name == "my_test3__c__b__a"
+
+
+def test_list_of_dicts_as_dict():
+    class MyTest1(Feature):
+        val1: Union[dict, list[dict]]
+        val2: Optional[Union[list[dict], dict]]
+
+    schema = Feature._features_to_udf_spec([MyTest1])
+    assert len(schema) == 2
+    assert list(schema.values())[0] == JSON
+    assert list(schema.values())[1] == JSON
```

### Comparing `dvcx-0.73.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.74.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/lib/test_file.py` & `dvcx-0.74.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.74.0/tests/unit/lib/test_webdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     assert len(groups) == 2
 
     (file01, laion01), (file64, laion64) = groups
 
     assert file01.name == "01.jpg"
     assert file01.parent == stream.name
     assert file01.location is not None
-    assert isinstance(file01.location, dict)
-    assert file01.location["parent"] == stream.name
+    assert isinstance(file01.location, list)
+    assert file01.location[0]["parent"] == stream.name
 
     assert file64.name == "64.jpg"
     assert file64.parent == stream.name
 
     assert laion01.txt is None
     assert laion01.json.uid == "5678"
```

### Comparing `dvcx-0.73.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.74.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/sql/test_array.py` & `dvcx-0.74.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/sql/test_conditional.py` & `dvcx-0.74.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/sql/test_path.py` & `dvcx-0.74.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/sql/test_selectable.py` & `dvcx-0.74.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/sql/test_string.py` & `dvcx-0.74.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_asyn.py` & `dvcx-0.74.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_cache.py` & `dvcx-0.74.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_catalog.py` & `dvcx-0.74.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_catalog_formats.py` & `dvcx-0.74.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_catalog_loader.py` & `dvcx-0.74.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_cli_parsing.py` & `dvcx-0.74.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_client.py` & `dvcx-0.74.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_client_s3.py` & `dvcx-0.74.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_data_storage.py` & `dvcx-0.74.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_database_engine.py` & `dvcx-0.74.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_dataset.py` & `dvcx-0.74.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_fileslice.py` & `dvcx-0.74.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_id_generator.py` & `dvcx-0.74.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_listing.py` & `dvcx-0.74.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_metastore.py` & `dvcx-0.74.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_serializer.py` & `dvcx-0.74.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_storage.py` & `dvcx-0.74.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_udf.py` & `dvcx-0.74.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_utils.py` & `dvcx-0.74.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/unit/test_warehouse.py` & `dvcx-0.74.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.73.0/tests/utils.py` & `dvcx-0.74.0/tests/utils.py`

 * *Files identical despite different names*

