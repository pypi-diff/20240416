# Comparing `tmp/pyiceberg-0.6.0rc6.tar.gz` & `tmp/pyiceberg-0.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiceberg-0.6.0rc6.tar", max compression
+gzip compressed data, was "pyiceberg-0.6.1rc1.tar", max compression
```

## Comparing `pyiceberg-0.6.0rc6.tar` & `pyiceberg-0.6.1rc1.tar`

### file list

```diff
@@ -1,148 +1,149 @@
--rw-r--r--   0        0        0    12548 2024-02-14 12:34:51.897390 pyiceberg-0.6.0rc6/LICENSE
--rw-r--r--   0        0        0     2567 2024-02-14 12:34:51.897390 pyiceberg-0.6.0rc6/Makefile
--rw-r--r--   0        0        0      251 2024-02-14 12:34:51.897390 pyiceberg-0.6.0rc6/NOTICE
--rw-r--r--   0        0        0     1218 2024-02-14 12:34:51.897390 pyiceberg-0.6.0rc6/README.md
--rw-r--r--   0        0        0     2196 2024-02-14 12:34:51.897390 pyiceberg-0.6.0rc6/build-module.py
--rw-r--r--   0        0        0       43 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/.rat-excludes
--rw-r--r--   0        0        0     2856 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/Dockerfile
--rwxr-xr-x   0        0        0     2529 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/check-license
--rw-r--r--   0        0        0     1018 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/docker-compose-azurite.yml
--rw-r--r--   0        0        0     1061 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/docker-compose-gcs-server.yml
--rw-r--r--   0        0        0     2851 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/docker-compose-integration.yml
--rw-r--r--   0        0        0     1626 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/docker-compose.yml
--rwxr-xr-x   0        0        0      912 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/entrypoint.sh
--rw-r--r--   0        0        0     1584 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/hive/Dockerfile
--rw-r--r--   0        0        0     1756 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/hive/core-site.xml
--rw-r--r--   0        0        0    11857 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/provision.py
--rwxr-xr-x   0        0        0     1198 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/run-azurite.sh
--rw-r--r--   0        0        0     1218 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/run-gcs-server.sh
--rwxr-xr-x   0        0        0     1194 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/run-minio.sh
--rw-r--r--   0        0        0     1895 2024-02-14 12:34:51.901389 pyiceberg-0.6.0rc6/dev/spark-defaults.conf
--rw-r--r--   0        0        0      808 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/__init__.py
--rw-r--r--   0        0        0     1021 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/__init__.py
--rw-r--r--   0        0        0     1685 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/__init__.py
--rw-r--r--   0        0        0     1621 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/bzip2.py
--rw-r--r--   0        0        0     1115 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/codec.py
--rw-r--r--   0        0        0     1416 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/deflate.py
--rw-r--r--   0        0        0     2702 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/snappy_codec.py
--rw-r--r--   0        0        0     2075 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/zstandard_codec.py
--rw-r--r--   0        0        0     6025 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/decoder.py
--rw-r--r--   0        0        0     1985 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_basic.c
--rw-r--r--   0        0        0     1811 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_fast.pyi
--rw-r--r--   0        0        0     6360 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_fast.pyx
--rw-r--r--   0        0        0     2904 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/encoder.py
--rw-r--r--   0        0        0     9396 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/file.py
--rw-r--r--   0        0        0    16716 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/reader.py
--rw-r--r--   0        0        0    20003 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/resolver.py
--rw-r--r--   0        0        0     6564 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/avro/writer.py
--rw-r--r--   0        0        0    24603 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/__init__.py
--rw-r--r--   0        0        0    31704 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/dynamodb.py
--rw-r--r--   0        0        0    28768 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/glue.py
--rw-r--r--   0        0        0    24302 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/hive.py
--rw-r--r--   0        0        0     3587 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/noop.py
--rw-r--r--   0        0        0    26112 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/rest.py
--rw-r--r--   0        0        0    27905 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/catalog/sql.py
--rw-r--r--   0        0        0      785 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/cli/__init__.py
--rw-r--r--   0        0        0    14432 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/cli/console.py
--rw-r--r--   0        0        0     8772 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/cli/output.py
--rw-r--r--   0        0        0    10197 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/conversions.py
--rw-r--r--   0        0        0     3085 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/exceptions.py
--rw-r--r--   0        0        0    30164 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/expressions/__init__.py
--rw-r--r--   0        0        0    22684 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/expressions/literals.py
--rw-r--r--   0        0        0     7761 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/expressions/parser.py
--rw-r--r--   0        0        0    55617 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/expressions/visitors.py
--rw-r--r--   0        0        0    11628 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/io/__init__.py
--rw-r--r--   0        0        0    12121 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/io/fsspec.py
--rw-r--r--   0        0        0    70976 2024-02-14 12:34:51.905389 pyiceberg-0.6.0rc6/pyiceberg/io/pyarrow.py
--rw-r--r--   0        0        0    36875 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/manifest.py
--rw-r--r--   0        0        0     8250 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/partitioning.py
--rw-r--r--   0        0        0      826 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/py.typed
--rw-r--r--   0        0        0    60722 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/schema.py
--rw-r--r--   0        0        0     4702 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/serializers.py
--rw-r--r--   0        0        0    97344 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/__init__.py
--rw-r--r--   0        0        0    19613 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/metadata.py
--rw-r--r--   0        0        0     6754 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/name_mapping.py
--rw-r--r--   0        0        0     2460 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/refs.py
--rw-r--r--   0        0        0    14702 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/snapshots.py
--rw-r--r--   0        0        0     6892 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/table/sorting.py
--rw-r--r--   0        0        0    27363 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/transforms.py
--rw-r--r--   0        0        0     7322 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/typedef.py
--rw-r--r--   0        0        0    23492 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/types.py
--rw-r--r--   0        0        0      785 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/__init__.py
--rw-r--r--   0        0        0     3243 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/bin_packing.py
--rw-r--r--   0        0        0     1830 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/concurrent.py
--rw-r--r--   0        0        0     6501 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/config.py
--rw-r--r--   0        0        0     7022 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/datetime.py
--rw-r--r--   0        0        0     4348 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/decimal.py
--rw-r--r--   0        0        0     1829 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/deprecated.py
--rw-r--r--   0        0        0     2349 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/lazydict.py
--rw-r--r--   0        0        0     1405 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/parsing.py
--rw-r--r--   0        0        0    23395 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/schema_conversion.py
--rw-r--r--   0        0        0     2141 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/singleton.py
--rw-r--r--   0        0        0     1856 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/pyiceberg/utils/truncate.py
--rw-r--r--   0        0        0    18191 2024-02-14 12:35:03.041373 pyiceberg-0.6.0rc6/pyproject.toml
--rw-r--r--   0        0        0     7525 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_decoder.py
--rw-r--r--   0        0        0     3632 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_encoder.py
--rw-r--r--   0        0        0    12572 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_file.py
--rw-r--r--   0        0        0    15572 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_reader.py
--rw-r--r--   0        0        0    12594 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_resolver.py
--rw-r--r--   0        0        0     5939 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/avro/test_writer.py
--rw-r--r--   0        0        0    11602 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/catalog/integration_test_dynamodb.py
--rw-r--r--   0        0        0    19459 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/catalog/integration_test_glue.py
--rw-r--r--   0        0        0    26382 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/catalog/test_base.py
--rw-r--r--   0        0        0    24772 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/catalog/test_dynamodb.py
--rw-r--r--   0        0        0    29880 2024-02-14 12:34:51.909389 pyiceberg-0.6.0rc6/tests/catalog/test_glue.py
--rw-r--r--   0        0        0    34732 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/catalog/test_hive.py
--rw-r--r--   0        0        0    30557 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/catalog/test_rest.py
--rw-r--r--   0        0        0    30422 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/catalog/test_sql.py
--rw-r--r--   0        0        0    36737 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/cli/test_console.py
--rw-r--r--   0        0        0      799 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/cli/test_output.py
--rw-r--r--   0        0        0    77337 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/conftest.py
--rw-r--r--   0        0        0    45204 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_evaluator.py
--rw-r--r--   0        0        0    44013 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_expressions.py
--rw-r--r--   0        0        0    26683 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_literals.py
--rw-r--r--   0        0        0     7014 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_parser.py
--rw-r--r--   0        0        0    12446 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_projection.py
--rw-r--r--   0        0        0    63987 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/expressions/test_visitors.py
--rw-r--r--   0        0        0    21375 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/integration/test_reads.py
--rw-r--r--   0        0        0     4856 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/integration/test_rest_manifest.py
--rw-r--r--   0        0        0    94266 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/integration/test_rest_schema.py
--rw-r--r--   0        0        0    24146 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/integration/test_writes.py
--rw-r--r--   0        0        0    27032 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/io/test_fsspec.py
--rw-r--r--   0        0        0    11532 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/io/test_io.py
--rw-r--r--   0        0        0    59308 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/io/test_pyarrow.py
--rw-r--r--   0        0        0    27462 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/io/test_pyarrow_stats.py
--rw-r--r--   0        0        0    19085 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/io/test_pyarrow_visitor.py
--rw-r--r--   0        0        0    35889 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_init.py
--rw-r--r--   0        0        0    32498 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_metadata.py
--rw-r--r--   0        0        0     8861 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_name_mapping.py
--rw-r--r--   0        0        0     5474 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_partitioning.py
--rw-r--r--   0        0        0     3282 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_refs.py
--rw-r--r--   0        0        0    10093 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_snapshots.py
--rw-r--r--   0        0        0     4111 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/table/test_sorting.py
--rw-r--r--   0        0        0    22756 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/test_conversions.py
--rw-r--r--   0        0        0    61613 2024-02-14 12:34:51.913390 pyiceberg-0.6.0rc6/tests/test_schema.py
--rw-r--r--   0        0        0    35991 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/test_transforms.py
--rw-r--r--   0        0        0     2567 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/test_typedef.py
--rw-r--r--   0        0        0    18815 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/test_types.py
--rw-r--r--   0        0        0     1113 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/test_version.py
--rw-r--r--   0        0        0     2725 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_bin_packing.py
--rw-r--r--   0        0        0     1720 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_concurrent.py
--rw-r--r--   0        0        0     2930 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_config.py
--rw-r--r--   0        0        0     2551 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1705 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_decimal.py
--rw-r--r--   0        0        0     1354 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_deprecated.py
--rw-r--r--   0        0        0     1198 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_lazydict.py
--rw-r--r--   0        0        0    19047 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_manifest.py
--rw-r--r--   0        0        0    13077 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_schema_conversion.py
--rw-r--r--   0        0        0     1334 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_singleton.py
--rw-r--r--   0        0        0     1319 2024-02-14 12:34:51.917389 pyiceberg-0.6.0rc6/tests/utils/test_truncate.py
--rw-r--r--   0        0        0    74745 2024-02-14 12:34:51.921389 pyiceberg-0.6.0rc6/vendor/fb303/FacebookService.py
--rw-r--r--   0        0        0      853 2024-02-14 12:34:51.921389 pyiceberg-0.6.0rc6/vendor/fb303/__init__.py
--rw-r--r--   0        0        0      943 2024-02-14 12:34:51.921389 pyiceberg-0.6.0rc6/vendor/fb303/constants.py
--rw-r--r--   0        0        0     1549 2024-02-14 12:34:51.921389 pyiceberg-0.6.0rc6/vendor/fb303/ttypes.py
--rw-r--r--   0        0        0  2241478 2024-02-14 12:34:51.925389 pyiceberg-0.6.0rc6/vendor/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0      856 2024-02-14 12:34:51.925389 pyiceberg-0.6.0rc6/vendor/hive_metastore/__init__.py
--rw-r--r--   0        0        0     2401 2024-02-14 12:34:51.925389 pyiceberg-0.6.0rc6/vendor/hive_metastore/constants.py
--rw-r--r--   0        0        0  1354270 2024-02-14 12:34:51.929389 pyiceberg-0.6.0rc6/vendor/hive_metastore/ttypes.py
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 pyiceberg-0.6.0rc6/PKG-INFO
+-rw-r--r--   0        0        0    12548 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/LICENSE
+-rw-r--r--   0        0        0     2567 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/Makefile
+-rw-r--r--   0        0        0      251 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/NOTICE
+-rw-r--r--   0        0        0     1218 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/README.md
+-rw-r--r--   0        0        0     2196 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/build-module.py
+-rw-r--r--   0        0        0       43 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/.rat-excludes
+-rw-r--r--   0        0        0     2856 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/Dockerfile
+-rwxr-xr-x   0        0        0     2529 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/check-license
+-rw-r--r--   0        0        0     1018 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/docker-compose-azurite.yml
+-rw-r--r--   0        0        0     1061 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/docker-compose-gcs-server.yml
+-rw-r--r--   0        0        0     2851 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/docker-compose-integration.yml
+-rw-r--r--   0        0        0     1626 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/docker-compose.yml
+-rwxr-xr-x   0        0        0      912 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/entrypoint.sh
+-rw-r--r--   0        0        0     1584 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/hive/Dockerfile
+-rw-r--r--   0        0        0     1756 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/hive/core-site.xml
+-rw-r--r--   0        0        0    11857 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/provision.py
+-rwxr-xr-x   0        0        0     1198 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/run-azurite.sh
+-rw-r--r--   0        0        0     1218 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/run-gcs-server.sh
+-rwxr-xr-x   0        0        0     1194 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/run-minio.sh
+-rw-r--r--   0        0        0     1895 2024-04-01 15:37:35.811514 pyiceberg-0.6.1rc1/dev/spark-defaults.conf
+-rw-r--r--   0        0        0      808 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/__init__.py
+-rw-r--r--   0        0        0     1685 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/bzip2.py
+-rw-r--r--   0        0        0     1115 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/codec.py
+-rw-r--r--   0        0        0     1416 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/deflate.py
+-rw-r--r--   0        0        0     2702 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/snappy_codec.py
+-rw-r--r--   0        0        0     2075 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/zstandard_codec.py
+-rw-r--r--   0        0        0     6025 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/decoder.py
+-rw-r--r--   0        0        0     1985 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_basic.c
+-rw-r--r--   0        0        0     1811 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_fast.pyi
+-rw-r--r--   0        0        0     6360 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_fast.pyx
+-rw-r--r--   0        0        0     2904 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/encoder.py
+-rw-r--r--   0        0        0     9396 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/file.py
+-rw-r--r--   0        0        0    16716 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/reader.py
+-rw-r--r--   0        0        0    20003 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/resolver.py
+-rw-r--r--   0        0        0     6564 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/avro/writer.py
+-rw-r--r--   0        0        0    24804 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/__init__.py
+-rw-r--r--   0        0        0    31800 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/dynamodb.py
+-rw-r--r--   0        0        0    28799 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/glue.py
+-rw-r--r--   0        0        0    24390 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/hive.py
+-rw-r--r--   0        0        0     3583 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/noop.py
+-rw-r--r--   0        0        0    26345 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/rest.py
+-rw-r--r--   0        0        0    27936 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/catalog/sql.py
+-rw-r--r--   0        0        0      785 2024-04-01 15:37:35.815514 pyiceberg-0.6.1rc1/pyiceberg/cli/__init__.py
+-rw-r--r--   0        0        0    14432 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/cli/console.py
+-rw-r--r--   0        0        0     8772 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/cli/output.py
+-rw-r--r--   0        0        0    10197 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/conversions.py
+-rw-r--r--   0        0        0     3085 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/exceptions.py
+-rw-r--r--   0        0        0    30164 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/expressions/__init__.py
+-rw-r--r--   0        0        0    22684 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/expressions/literals.py
+-rw-r--r--   0        0        0     7761 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/expressions/parser.py
+-rw-r--r--   0        0        0    55613 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/expressions/visitors.py
+-rw-r--r--   0        0        0    11628 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/io/__init__.py
+-rw-r--r--   0        0        0    12121 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/io/fsspec.py
+-rw-r--r--   0        0        0    70985 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/io/pyarrow.py
+-rw-r--r--   0        0        0    36875 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/manifest.py
+-rw-r--r--   0        0        0     8250 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/partitioning.py
+-rw-r--r--   0        0        0      826 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/py.typed
+-rw-r--r--   0        0        0    61024 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/schema.py
+-rw-r--r--   0        0        0     4964 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/serializers.py
+-rw-r--r--   0        0        0   100442 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/__init__.py
+-rw-r--r--   0        0        0    20318 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/metadata.py
+-rw-r--r--   0        0        0     6891 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/name_mapping.py
+-rw-r--r--   0        0        0     2460 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/refs.py
+-rw-r--r--   0        0        0    14702 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/snapshots.py
+-rw-r--r--   0        0        0     6892 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/table/sorting.py
+-rw-r--r--   0        0        0    27363 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/transforms.py
+-rw-r--r--   0        0        0     7322 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/typedef.py
+-rw-r--r--   0        0        0    23492 2024-04-01 15:37:35.819514 pyiceberg-0.6.1rc1/pyiceberg/types.py
+-rw-r--r--   0        0        0      785 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/__init__.py
+-rw-r--r--   0        0        0     3243 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/bin_packing.py
+-rw-r--r--   0        0        0     1552 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/concurrent.py
+-rw-r--r--   0        0        0     7219 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/config.py
+-rw-r--r--   0        0        0     7022 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/datetime.py
+-rw-r--r--   0        0        0     4348 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/decimal.py
+-rw-r--r--   0        0        0     1829 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/deprecated.py
+-rw-r--r--   0        0        0     2349 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/lazydict.py
+-rw-r--r--   0        0        0     1405 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/parsing.py
+-rw-r--r--   0        0        0    23395 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/schema_conversion.py
+-rw-r--r--   0        0        0     2141 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/singleton.py
+-rw-r--r--   0        0        0     1856 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/pyiceberg/utils/truncate.py
+-rw-r--r--   0        0        0    18191 2024-04-01 15:37:45.839657 pyiceberg-0.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7525 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_decoder.py
+-rw-r--r--   0        0        0     3632 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_encoder.py
+-rw-r--r--   0        0        0    12572 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_file.py
+-rw-r--r--   0        0        0    15572 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_reader.py
+-rw-r--r--   0        0        0    12594 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_resolver.py
+-rw-r--r--   0        0        0     5939 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/avro/test_writer.py
+-rw-r--r--   0        0        0    11602 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/integration_test_dynamodb.py
+-rw-r--r--   0        0        0    19459 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/integration_test_glue.py
+-rw-r--r--   0        0        0    26374 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_base.py
+-rw-r--r--   0        0        0    24772 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_dynamodb.py
+-rw-r--r--   0        0        0    29880 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_glue.py
+-rw-r--r--   0        0        0    34732 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_hive.py
+-rw-r--r--   0        0        0    30584 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_rest.py
+-rw-r--r--   0        0        0    31465 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/catalog/test_sql.py
+-rw-r--r--   0        0        0    36737 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/cli/test_console.py
+-rw-r--r--   0        0        0      799 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/cli/test_output.py
+-rw-r--r--   0        0        0    77337 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0    45204 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/expressions/test_evaluator.py
+-rw-r--r--   0        0        0    44013 2024-04-01 15:37:35.823514 pyiceberg-0.6.1rc1/tests/expressions/test_expressions.py
+-rw-r--r--   0        0        0    26683 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/expressions/test_literals.py
+-rw-r--r--   0        0        0     7048 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/expressions/test_parser.py
+-rw-r--r--   0        0        0    12446 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/expressions/test_projection.py
+-rw-r--r--   0        0        0    63987 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/expressions/test_visitors.py
+-rw-r--r--   0        0        0    21345 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/integration/test_reads.py
+-rw-r--r--   0        0        0     4856 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/integration/test_rest_manifest.py
+-rw-r--r--   0        0        0    94266 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/integration/test_rest_schema.py
+-rw-r--r--   0        0        0    24178 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/integration/test_writes.py
+-rw-r--r--   0        0        0    27032 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/io/test_fsspec.py
+-rw-r--r--   0        0        0    11532 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/io/test_io.py
+-rw-r--r--   0        0        0    59346 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/io/test_pyarrow.py
+-rw-r--r--   0        0        0    27462 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/io/test_pyarrow_stats.py
+-rw-r--r--   0        0        0    19085 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/io/test_pyarrow_visitor.py
+-rw-r--r--   0        0        0    40869 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_init.py
+-rw-r--r--   0        0        0    32589 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_metadata.py
+-rw-r--r--   0        0        0     8861 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_name_mapping.py
+-rw-r--r--   0        0        0     5474 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_partitioning.py
+-rw-r--r--   0        0        0     3282 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_refs.py
+-rw-r--r--   0        0        0    10093 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_snapshots.py
+-rw-r--r--   0        0        0     4111 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/table/test_sorting.py
+-rw-r--r--   0        0        0    22756 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_conversions.py
+-rw-r--r--   0        0        0    61584 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     2336 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_serializers.py
+-rw-r--r--   0        0        0    35991 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_transforms.py
+-rw-r--r--   0        0        0     2567 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_typedef.py
+-rw-r--r--   0        0        0    18815 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_types.py
+-rw-r--r--   0        0        0     1113 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/test_version.py
+-rw-r--r--   0        0        0     2725 2024-04-01 15:37:35.827514 pyiceberg-0.6.1rc1/tests/utils/test_bin_packing.py
+-rw-r--r--   0        0        0     1720 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_concurrent.py
+-rw-r--r--   0        0        0     3622 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_config.py
+-rw-r--r--   0        0        0     2551 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1705 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_decimal.py
+-rw-r--r--   0        0        0     1354 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_deprecated.py
+-rw-r--r--   0        0        0     1198 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_lazydict.py
+-rw-r--r--   0        0        0    19020 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_manifest.py
+-rw-r--r--   0        0        0    13077 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_schema_conversion.py
+-rw-r--r--   0        0        0     1334 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_singleton.py
+-rw-r--r--   0        0        0     1319 2024-04-01 15:37:35.831514 pyiceberg-0.6.1rc1/tests/utils/test_truncate.py
+-rw-r--r--   0        0        0    74745 2024-04-01 15:37:35.835514 pyiceberg-0.6.1rc1/vendor/fb303/FacebookService.py
+-rw-r--r--   0        0        0      853 2024-04-01 15:37:35.835514 pyiceberg-0.6.1rc1/vendor/fb303/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-01 15:37:35.835514 pyiceberg-0.6.1rc1/vendor/fb303/constants.py
+-rw-r--r--   0        0        0     1549 2024-04-01 15:37:35.835514 pyiceberg-0.6.1rc1/vendor/fb303/ttypes.py
+-rw-r--r--   0        0        0  2241478 2024-04-01 15:37:35.839514 pyiceberg-0.6.1rc1/vendor/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0      856 2024-04-01 15:37:35.839514 pyiceberg-0.6.1rc1/vendor/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     2401 2024-04-01 15:37:35.839514 pyiceberg-0.6.1rc1/vendor/hive_metastore/constants.py
+-rw-r--r--   0        0        0  1354270 2024-04-01 15:37:35.839514 pyiceberg-0.6.1rc1/vendor/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 pyiceberg-0.6.1rc1/PKG-INFO
```

### Comparing `pyiceberg-0.6.0rc6/LICENSE` & `pyiceberg-0.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/Makefile` & `pyiceberg-0.6.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/README.md` & `pyiceberg-0.6.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/build-module.py` & `pyiceberg-0.6.1rc1/build-module.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/Dockerfile` & `pyiceberg-0.6.1rc1/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/check-license` & `pyiceberg-0.6.1rc1/dev/check-license`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/docker-compose-azurite.yml` & `pyiceberg-0.6.1rc1/dev/docker-compose-azurite.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/docker-compose-gcs-server.yml` & `pyiceberg-0.6.1rc1/dev/docker-compose-gcs-server.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/docker-compose-integration.yml` & `pyiceberg-0.6.1rc1/dev/docker-compose-integration.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/docker-compose.yml` & `pyiceberg-0.6.1rc1/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/entrypoint.sh` & `pyiceberg-0.6.1rc1/dev/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/hive/Dockerfile` & `pyiceberg-0.6.1rc1/dev/hive/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/hive/core-site.xml` & `pyiceberg-0.6.1rc1/dev/hive/core-site.xml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/provision.py` & `pyiceberg-0.6.1rc1/dev/provision.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/run-azurite.sh` & `pyiceberg-0.6.1rc1/dev/run-azurite.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/run-gcs-server.sh` & `pyiceberg-0.6.1rc1/dev/run-gcs-server.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/run-minio.sh` & `pyiceberg-0.6.1rc1/dev/run-minio.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/dev/spark-defaults.conf` & `pyiceberg-0.6.1rc1/dev/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/bzip2.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/bzip2.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/codec.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/deflate.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/deflate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/snappy_codec.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/snappy_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/codecs/zstandard_codec.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/codecs/zstandard_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/decoder.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_basic.c` & `pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_basic.c`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_fast.pyi` & `pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_fast.pyi`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/decoder_fast.pyx` & `pyiceberg-0.6.1rc1/pyiceberg/avro/decoder_fast.pyx`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/encoder.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/encoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/file.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/reader.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/resolver.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/avro/writer.py` & `pyiceberg-0.6.1rc1/pyiceberg/avro/writer.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,16 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
+            CommitStateUnknownException: Failed due to an internal exception on the side of the catalog.
         """
 
     @abstractmethod
     def create_namespace(self, namespace: Union[str, Identifier], properties: Properties = EMPTY_DICT) -> None:
         """Create a namespace in the catalog.
 
         Args:
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/dynamodb.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,15 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
         """
         raise NotImplementedError
 
     def load_table(self, identifier: Union[str, Identifier]) -> Table:
         """
         Load the table's metadata and returns the table instance.
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/glue.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/glue.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,14 @@
     EXTERNAL_TABLE,
     ICEBERG,
     LOCATION,
     METADATA_LOCATION,
     PREVIOUS_METADATA_LOCATION,
     TABLE_TYPE,
     Catalog,
-    Identifier,
-    Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     CommitFailedException,
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchIcebergTableError,
@@ -63,15 +61,15 @@
 from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema, SchemaVisitor, visit
 from pyiceberg.serializers import FromInputFile
 from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table, update_table_metadata
 from pyiceberg.table.metadata import TableMetadata, new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
-from pyiceberg.typedef import EMPTY_DICT
+from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DecimalType,
     DoubleType,
     FixedType,
@@ -400,15 +398,15 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
-            CommitFailedException: If the commit failed.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
         """
         identifier_tuple = self.identifier_to_tuple_without_catalog(
             tuple(table_request.identifier.namespace.root + [table_request.identifier.name])
         )
         database_name, table_name = self.identifier_to_database_and_table(identifier_tuple)
 
         current_glue_table = self._get_glue_table(database_name=database_name, table_name=table_name)
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/hive.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,14 @@
 from pyiceberg.catalog import (
     EXTERNAL_TABLE,
     ICEBERG,
     LOCATION,
     METADATA_LOCATION,
     TABLE_TYPE,
     Catalog,
-    Identifier,
-    Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     CommitFailedException,
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchIcebergTableError,
@@ -75,15 +73,15 @@
 from pyiceberg.io import FileIO, load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema, SchemaVisitor, visit
 from pyiceberg.serializers import FromInputFile
 from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table, TableProperties, update_table_metadata
 from pyiceberg.table.metadata import new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
-from pyiceberg.typedef import EMPTY_DICT
+from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DecimalType,
     DoubleType,
     FixedType,
@@ -356,14 +354,15 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
         """
         identifier_tuple = self.identifier_to_tuple_without_catalog(
             tuple(table_request.identifier.namespace.root + [table_request.identifier.name])
         )
         current_table = self.load_table(identifier_tuple)
         database_name, table_name = self.identifier_to_database_and_table(identifier_tuple, NoSuchTableError)
         base_metadata = current_table.metadata
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/noop.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/noop.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 from pyiceberg.catalog import Catalog, PropertiesUpdateSummary
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema
 from pyiceberg.table import (
     CommitTableRequest,
     CommitTableResponse,
-    SortOrder,
     Table,
 )
-from pyiceberg.table.sorting import UNSORTED_SORT_ORDER
+from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 
 if TYPE_CHECKING:
     import pyarrow as pa
 
 
 class NoopCatalog(Catalog):
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/rest.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec, assign_fresh_partition_spec_ids
 from pyiceberg.schema import Schema, assign_fresh_schema_ids
 from pyiceberg.table import (
     CommitTableRequest,
     CommitTableResponse,
     Table,
     TableIdentifier,
-    TableMetadata,
 )
+from pyiceberg.table.metadata import TableMetadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder, assign_fresh_sort_order_ids
 from pyiceberg.typedef import EMPTY_DICT, UTF8, IcebergBaseModel
 
 if TYPE_CHECKING:
     import pyarrow as pa
 
 ICEBERG_REST_SPEC_VERSION = "0.14.1"
@@ -564,14 +564,16 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
+            CommitStateUnknownException: Failed due to an internal exception on the side of the catalog.
         """
         response = self._session.post(
             self.url(Endpoints.update_table, prefixed=True, **self._split_identifier_for_path(table_request.identifier)),
             data=table_request.model_dump_json().encode(UTF8),
         )
         try:
             response.raise_for_status()
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/catalog/sql.py` & `pyiceberg-0.6.1rc1/pyiceberg/catalog/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     Session,
     mapped_column,
 )
 
 from pyiceberg.catalog import (
     METADATA_LOCATION,
     Catalog,
-    Identifier,
-    Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     CommitFailedException,
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchNamespaceError,
@@ -60,15 +58,15 @@
 from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import UNPARTITIONED_PARTITION_SPEC, PartitionSpec
 from pyiceberg.schema import Schema
 from pyiceberg.serializers import FromInputFile
 from pyiceberg.table import CommitTableRequest, CommitTableResponse, Table, update_table_metadata
 from pyiceberg.table.metadata import new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
-from pyiceberg.typedef import EMPTY_DICT
+from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 
 if TYPE_CHECKING:
     import pyarrow as pa
 
 
 class SqlCatalogBaseTable(MappedAsDataclass, DeclarativeBase):
     pass
@@ -369,15 +367,15 @@
             table_request (CommitTableRequest): The table requests to be carried out.
 
         Returns:
             CommitTableResponse: The updated metadata.
 
         Raises:
             NoSuchTableError: If a table with the given identifier does not exist.
-            CommitFailedException: If the commit failed.
+            CommitFailedException: Requirement not met, or a conflict with a concurrent commit.
         """
         identifier_tuple = self.identifier_to_tuple_without_catalog(
             tuple(table_request.identifier.namespace.root + [table_request.identifier.name])
         )
         current_table = self.load_table(identifier_tuple)
         database_name, table_name = self.identifier_to_database_and_table(identifier_tuple, NoSuchTableError)
         base_metadata = current_table.metadata
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/cli/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/cli/console.py` & `pyiceberg-0.6.1rc1/pyiceberg/cli/console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/cli/output.py` & `pyiceberg-0.6.1rc1/pyiceberg/cli/output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/conversions.py` & `pyiceberg-0.6.1rc1/pyiceberg/conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/exceptions.py` & `pyiceberg-0.6.1rc1/pyiceberg/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/expressions/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/expressions/literals.py` & `pyiceberg-0.6.1rc1/pyiceberg/expressions/literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/expressions/parser.py` & `pyiceberg-0.6.1rc1/pyiceberg/expressions/parser.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/expressions/visitors.py` & `pyiceberg-0.6.1rc1/pyiceberg/expressions/visitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,24 +50,23 @@
     BoundNotNull,
     BoundNotStartsWith,
     BoundPredicate,
     BoundSetPredicate,
     BoundStartsWith,
     BoundTerm,
     BoundUnaryPredicate,
-    L,
     Not,
     Or,
     UnboundPredicate,
 )
 from pyiceberg.expressions.literals import Literal
 from pyiceberg.manifest import DataFile, ManifestFile, PartitionFieldSummary
 from pyiceberg.partitioning import PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.typedef import EMPTY_DICT, StructProtocol
+from pyiceberg.typedef import EMPTY_DICT, L, StructProtocol
 from pyiceberg.types import (
     DoubleType,
     FloatType,
     IcebergType,
     PrimitiveType,
     StructType,
     TimestampType,
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/io/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/io/fsspec.py` & `pyiceberg-0.6.1rc1/pyiceberg/io/fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/io/pyarrow.py` & `pyiceberg-0.6.1rc1/pyiceberg/io/pyarrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
 from pyiceberg.avro.resolver import ResolveError
 from pyiceberg.conversions import to_bytes
 from pyiceberg.expressions import (
     AlwaysTrue,
     BooleanExpression,
     BoundTerm,
-    Literal,
 )
+from pyiceberg.expressions.literals import Literal
 from pyiceberg.expressions.visitors import (
     BoundBooleanExpressionVisitor,
     bind,
     extract_field_ids,
     translate_column_names,
 )
 from pyiceberg.expressions.visitors import visit as boolean_expression_visit
@@ -651,14 +651,18 @@
     else:
         raise ValueError(
             "Parquet file does not have field-ids and the Iceberg table does not have 'schema.name-mapping.default' defined"
         )
     return visit_pyarrow(schema, visitor)
 
 
+def _pyarrow_to_schema_without_ids(schema: pa.Schema) -> Schema:
+    return visit_pyarrow(schema, _ConvertToIcebergWithoutIDs())
+
+
 @singledispatch
 def visit_pyarrow(obj: Union[pa.DataType, pa.Schema], visitor: PyArrowSchemaVisitor[T]) -> T:
     """Apply a pyarrow schema visitor to any point within a schema.
 
     The function traverses the schema in post-order fashion.
 
     Args:
@@ -934,21 +938,17 @@
     fs: FileSystem,
     task: FileScanTask,
     bound_row_filter: BooleanExpression,
     projected_schema: Schema,
     projected_field_ids: Set[int],
     positional_deletes: Optional[List[ChunkedArray]],
     case_sensitive: bool,
-    row_counts: List[int],
     limit: Optional[int] = None,
     name_mapping: Optional[NameMapping] = None,
 ) -> Optional[pa.Table]:
-    if limit and sum(row_counts) >= limit:
-        return None
-
     _, _, path = PyArrowFileIO.parse_location(task.file.file_path)
     arrow_format = ds.ParquetFileFormat(pre_buffer=True, buffer_size=(ONE_MEGABYTE * 8))
     with fs.open_input_file(path) as fin:
         fragment = arrow_format.make_fragment(fin)
         physical_schema = fragment.physical_schema
         schema_raw = None
         if metadata := physical_schema.metadata:
@@ -1003,19 +1003,14 @@
                 arrow_table = fragment_scanner.head(limit)
             else:
                 arrow_table = fragment_scanner.to_table()
 
         if len(arrow_table) < 1:
             return None
 
-        if limit is not None and sum(row_counts) >= limit:
-            return None
-
-        row_counts.append(len(arrow_table))
-
         return to_requested_schema(projected_schema, file_project_schema, arrow_table)
 
 
 def _read_all_delete_files(fs: FileSystem, tasks: Iterable[FileScanTask]) -> Dict[str, List[ChunkedArray]]:
     deletes_per_file: Dict[str, List[ChunkedArray]] = {}
     unique_deletes = set(itertools.chain.from_iterable([task.delete_files for task in tasks]))
     if len(unique_deletes) > 0:
@@ -1073,42 +1068,41 @@
 
     bound_row_filter = bind(table.schema(), row_filter, case_sensitive=case_sensitive)
 
     projected_field_ids = {
         id for id in projected_schema.field_ids if not isinstance(projected_schema.find_type(id), (MapType, ListType))
     }.union(extract_field_ids(bound_row_filter))
 
-    row_counts: List[int] = []
     deletes_per_file = _read_all_delete_files(fs, tasks)
     executor = ExecutorFactory.get_or_create()
     futures = [
         executor.submit(
             _task_to_table,
             fs,
             task,
             bound_row_filter,
             projected_schema,
             projected_field_ids,
             deletes_per_file.get(task.file.file_path),
             case_sensitive,
-            row_counts,
             limit,
             table.name_mapping(),
         )
         for task in tasks
     ]
-
+    total_row_count = 0
     # for consistent ordering, we need to maintain future order
     futures_index = {f: i for i, f in enumerate(futures)}
     completed_futures: SortedList[Future[pa.Table]] = SortedList(iterable=[], key=lambda f: futures_index[f])
     for future in concurrent.futures.as_completed(futures):
         completed_futures.add(future)
-
+        if table_result := future.result():
+            total_row_count += len(table_result)
         # stop early if limit is satisfied
-        if limit is not None and sum(row_counts) >= limit:
+        if limit is not None and total_row_count >= limit:
             break
 
     # by now, we've either completed all tasks or satisfied the limit
     if limit is not None:
         _ = [f.cancel() for f in futures if not f.done()]
 
     tables = [f.result() for f in completed_futures if f.result()]
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/manifest.py` & `pyiceberg-0.6.1rc1/pyiceberg/manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/partitioning.py` & `pyiceberg-0.6.1rc1/pyiceberg/partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/py.typed` & `pyiceberg-0.6.1rc1/pyiceberg/py.typed`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/schema.py` & `pyiceberg-0.6.1rc1/pyiceberg/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from __future__ import annotations
 
 import itertools
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from functools import cached_property, partial, singledispatch
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Literal,
     Optional,
@@ -58,14 +59,19 @@
     StructType,
     TimestampType,
     TimestamptzType,
     TimeType,
     UUIDType,
 )
 
+if TYPE_CHECKING:
+    from pyiceberg.table.name_mapping import (
+        NameMapping,
+    )
+
 T = TypeVar("T")
 P = TypeVar("P")
 
 INITIAL_SCHEMA_ID = 0
 
 
 class Schema(IcebergBaseModel):
@@ -217,14 +223,20 @@
             raise ValueError(f"Could not find field with name or id {name_or_id}, case_sensitive={case_sensitive}")
         return field.field_type
 
     @property
     def highest_field_id(self) -> int:
         return max(self._lazy_id_to_name.keys(), default=0)
 
+    @cached_property
+    def name_mapping(self) -> NameMapping:
+        from pyiceberg.table.name_mapping import create_mapping_from_schema
+
+        return create_mapping_from_schema(self)
+
     def find_column_name(self, column_id: int) -> Optional[str]:
         """Find a column name given a column ID.
 
         Args:
             column_id (int): The ID of the column.
 
         Returns:
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/serializers.py` & `pyiceberg-0.6.1rc1/pyiceberg/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import gzip
 from abc import ABC, abstractmethod
 from typing import Callable
 
 from pyiceberg.io import InputFile, InputStream, OutputFile
 from pyiceberg.table.metadata import TableMetadata, TableMetadataUtil
 from pyiceberg.typedef import UTF8
+from pyiceberg.utils.config import Config
 
 GZIP = "gzip"
 
 
 class Compressor(ABC):
     @staticmethod
     def get_compressor(location: str) -> Compressor:
@@ -123,10 +124,13 @@
         """Write a TableMetadata instance to an output file.
 
         Args:
             output_file (OutputFile): A custom implementation of the iceberg.io.file.OutputFile abstract base class.
             overwrite (bool): Where to overwrite the file if it already exists. Defaults to `False`.
         """
         with output_file.create(overwrite=overwrite) as output_stream:
-            json_bytes = metadata.model_dump_json().encode(UTF8)
+            # We need to serialize None values, in order to dump `None` current-snapshot-id as `-1`
+            exclude_none = False if Config().get_bool("legacy-current-snapshot-id") else True
+
+            json_bytes = metadata.model_dump_json(exclude_none=exclude_none).encode(UTF8)
             json_bytes = Compressor.get_compressor(output_file.location).bytes_compressor()(json_bytes)
             output_stream.write(json_bytes)
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,27 @@
     Optional,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
-from pydantic import Field, SerializeAsAny
+from pydantic import Field
 from sortedcontainers import SortedList
 from typing_extensions import Annotated
 
+import pyiceberg.expressions.parser as parser
+import pyiceberg.expressions.visitors as visitors
 from pyiceberg.exceptions import CommitFailedException, ResolveError, ValidationError
 from pyiceberg.expressions import (
     AlwaysTrue,
     And,
     BooleanExpression,
     EqualTo,
-    parser,
-    visitors,
 )
-from pyiceberg.expressions.visitors import _InclusiveMetricsEvaluator, inclusive_projection
 from pyiceberg.io import FileIO, load_file_io
 from pyiceberg.manifest import (
     POSITIONAL_DELETE_SCHEMA,
     DataFile,
     DataFileContent,
     ManifestContent,
     ManifestEntry,
@@ -129,14 +128,57 @@
 
 ALWAYS_TRUE = AlwaysTrue()
 TABLE_ROOT_ID = -1
 
 _JAVA_LONG_MAX = 9223372036854775807
 
 
+def _check_schema_compatible(table_schema: Schema, other_schema: "pa.Schema") -> None:
+    """
+    Check if the `table_schema` is compatible with `other_schema`.
+
+    Two schemas are considered compatible when they are equal in terms of the Iceberg Schema type.
+
+    Raises:
+        ValueError: If the schemas are not compatible.
+    """
+    from pyiceberg.io.pyarrow import _pyarrow_to_schema_without_ids, pyarrow_to_schema
+
+    name_mapping = table_schema.name_mapping
+    try:
+        task_schema = pyarrow_to_schema(other_schema, name_mapping=name_mapping)
+    except ValueError as e:
+        other_schema = _pyarrow_to_schema_without_ids(other_schema)
+        additional_names = set(other_schema.column_names) - set(table_schema.column_names)
+        raise ValueError(
+            f"PyArrow table contains more columns: {', '.join(sorted(additional_names))}. Update the schema first (hint, use union_by_name)."
+        ) from e
+
+    if table_schema.as_struct() != task_schema.as_struct():
+        from rich.console import Console
+        from rich.table import Table as RichTable
+
+        console = Console(record=True)
+
+        rich_table = RichTable(show_header=True, header_style="bold")
+        rich_table.add_column("")
+        rich_table.add_column("Table field")
+        rich_table.add_column("Dataframe field")
+
+        for lhs in table_schema.fields:
+            try:
+                rhs = task_schema.find_field(lhs.field_id)
+                rich_table.add_row("✅" if lhs == rhs else "❌", str(lhs), str(rhs))
+            except ValueError:
+                rich_table.add_row("❌", str(lhs), "Missing")
+
+        console.print(rich_table)
+        raise ValueError(f"Mismatch in fields:\n{console.export_text()}")
+
+
 class TableProperties:
     PARQUET_ROW_GROUP_SIZE_BYTES = "write.parquet.row-group-size-bytes"
     PARQUET_ROW_GROUP_SIZE_BYTES_DEFAULT = 128 * 1024 * 1024  # 128 MB
 
     PARQUET_ROW_GROUP_LIMIT = "write.parquet.row-group-limit"
     PARQUET_ROW_GROUP_LIMIT_DEFAULT = 128 * 1024 * 1024  # 128 MB
 
@@ -364,137 +406,138 @@
                 requirements=self._requirements,
             )
             return self._table
         else:
             return self._table
 
 
-class TableUpdateAction(Enum):
-    upgrade_format_version = "upgrade-format-version"
-    add_schema = "add-schema"
-    set_current_schema = "set-current-schema"
-    add_spec = "add-spec"
-    set_default_spec = "set-default-spec"
-    add_sort_order = "add-sort-order"
-    set_default_sort_order = "set-default-sort-order"
-    add_snapshot = "add-snapshot"
-    set_snapshot_ref = "set-snapshot-ref"
-    remove_snapshots = "remove-snapshots"
-    remove_snapshot_ref = "remove-snapshot-ref"
-    set_location = "set-location"
-    set_properties = "set-properties"
-    remove_properties = "remove-properties"
-
-
-class TableUpdate(IcebergBaseModel):
-    action: TableUpdateAction
-
-
-class UpgradeFormatVersionUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.upgrade_format_version
+class UpgradeFormatVersionUpdate(IcebergBaseModel):
+    action: Literal['upgrade-format-version'] = Field(default="upgrade-format-version")
     format_version: int = Field(alias="format-version")
 
 
-class AddSchemaUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.add_schema
+class AddSchemaUpdate(IcebergBaseModel):
+    action: Literal['add-schema'] = Field(default="add-schema")
     schema_: Schema = Field(alias="schema")
     # This field is required: https://github.com/apache/iceberg/pull/7445
     last_column_id: int = Field(alias="last-column-id")
 
 
-class SetCurrentSchemaUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_current_schema
+class SetCurrentSchemaUpdate(IcebergBaseModel):
+    action: Literal['set-current-schema'] = Field(default="set-current-schema")
     schema_id: int = Field(
         alias="schema-id", description="Schema ID to set as current, or -1 to set last added schema", default=-1
     )
 
 
-class AddPartitionSpecUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.add_spec
+class AddPartitionSpecUpdate(IcebergBaseModel):
+    action: Literal['add-spec'] = Field(default="add-spec")
     spec: PartitionSpec
 
 
-class SetDefaultSpecUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_default_spec
+class SetDefaultSpecUpdate(IcebergBaseModel):
+    action: Literal['set-default-spec'] = Field(default="set-default-spec")
     spec_id: int = Field(
         alias="spec-id", description="Partition spec ID to set as the default, or -1 to set last added spec", default=-1
     )
 
 
-class AddSortOrderUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.add_sort_order
+class AddSortOrderUpdate(IcebergBaseModel):
+    action: Literal['add-sort-order'] = Field(default="add-sort-order")
     sort_order: SortOrder = Field(alias="sort-order")
 
 
-class SetDefaultSortOrderUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_default_sort_order
+class SetDefaultSortOrderUpdate(IcebergBaseModel):
+    action: Literal['set-default-sort-order'] = Field(default="set-default-sort-order")
     sort_order_id: int = Field(
         alias="sort-order-id", description="Sort order ID to set as the default, or -1 to set last added sort order", default=-1
     )
 
 
-class AddSnapshotUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.add_snapshot
+class AddSnapshotUpdate(IcebergBaseModel):
+    action: Literal['add-snapshot'] = Field(default="add-snapshot")
     snapshot: Snapshot
 
 
-class SetSnapshotRefUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_snapshot_ref
+class SetSnapshotRefUpdate(IcebergBaseModel):
+    action: Literal['set-snapshot-ref'] = Field(default="set-snapshot-ref")
     ref_name: str = Field(alias="ref-name")
     type: Literal["tag", "branch"]
     snapshot_id: int = Field(alias="snapshot-id")
     max_ref_age_ms: Annotated[Optional[int], Field(alias="max-ref-age-ms", default=None)]
     max_snapshot_age_ms: Annotated[Optional[int], Field(alias="max-snapshot-age-ms", default=None)]
     min_snapshots_to_keep: Annotated[Optional[int], Field(alias="min-snapshots-to-keep", default=None)]
 
 
-class RemoveSnapshotsUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.remove_snapshots
+class RemoveSnapshotsUpdate(IcebergBaseModel):
+    action: Literal['remove-snapshots'] = Field(default="remove-snapshots")
     snapshot_ids: List[int] = Field(alias="snapshot-ids")
 
 
-class RemoveSnapshotRefUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.remove_snapshot_ref
+class RemoveSnapshotRefUpdate(IcebergBaseModel):
+    action: Literal['remove-snapshot-ref'] = Field(default="remove-snapshot-ref")
     ref_name: str = Field(alias="ref-name")
 
 
-class SetLocationUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_location
+class SetLocationUpdate(IcebergBaseModel):
+    action: Literal['set-location'] = Field(default="set-location")
     location: str
 
 
-class SetPropertiesUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.set_properties
+class SetPropertiesUpdate(IcebergBaseModel):
+    action: Literal['set-properties'] = Field(default="set-properties")
     updates: Dict[str, str]
 
 
-class RemovePropertiesUpdate(TableUpdate):
-    action: TableUpdateAction = TableUpdateAction.remove_properties
+class RemovePropertiesUpdate(IcebergBaseModel):
+    action: Literal['remove-properties'] = Field(default="remove-properties")
     removals: List[str]
 
 
+TableUpdate = Annotated[
+    Union[
+        UpgradeFormatVersionUpdate,
+        AddSchemaUpdate,
+        SetCurrentSchemaUpdate,
+        AddPartitionSpecUpdate,
+        SetDefaultSpecUpdate,
+        AddSortOrderUpdate,
+        SetDefaultSortOrderUpdate,
+        AddSnapshotUpdate,
+        SetSnapshotRefUpdate,
+        RemoveSnapshotsUpdate,
+        RemoveSnapshotRefUpdate,
+        SetLocationUpdate,
+        SetPropertiesUpdate,
+        RemovePropertiesUpdate,
+    ],
+    Field(discriminator='action'),
+]
+
+
 class _TableMetadataUpdateContext:
     _updates: List[TableUpdate]
 
     def __init__(self) -> None:
         self._updates = []
 
     def add_update(self, update: TableUpdate) -> None:
         self._updates.append(update)
 
     def is_added_snapshot(self, snapshot_id: int) -> bool:
         return any(
-            update.snapshot.snapshot_id == snapshot_id
-            for update in self._updates
-            if update.action == TableUpdateAction.add_snapshot
+            update.snapshot.snapshot_id == snapshot_id for update in self._updates if isinstance(update, AddSnapshotUpdate)
         )
 
     def is_added_schema(self, schema_id: int) -> bool:
+        return any(update.schema_.schema_id == schema_id for update in self._updates if isinstance(update, AddSchemaUpdate))
+
+    def is_added_sort_order(self, sort_order_id: int) -> bool:
         return any(
-            update.schema_.schema_id == schema_id for update in self._updates if update.action == TableUpdateAction.add_schema
+            update.sort_order.order_id == sort_order_id for update in self._updates if isinstance(update, AddSortOrderUpdate)
         )
 
 
 @singledispatch
 def _apply_table_update(update: TableUpdate, base_metadata: TableMetadata, context: _TableMetadataUpdateContext) -> TableMetadata:
     """Apply a table update to the table metadata.
 
@@ -670,15 +713,15 @@
 
     for update in updates:
         new_metadata = _apply_table_update(update, new_metadata, context)
 
     return new_metadata.model_copy(deep=True)
 
 
-class TableRequirement(IcebergBaseModel):
+class ValidatableTableRequirement(IcebergBaseModel):
     type: str
 
     @abstractmethod
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         """Validate the requirement against the base metadata.
 
         Args:
@@ -686,38 +729,38 @@
 
         Raises:
             CommitFailedException: When the requirement is not met.
         """
         ...
 
 
-class AssertCreate(TableRequirement):
+class AssertCreate(ValidatableTableRequirement):
     """The table must not already exist; used for create transactions."""
 
     type: Literal["assert-create"] = Field(default="assert-create")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is not None:
             raise CommitFailedException("Table already exists")
 
 
-class AssertTableUUID(TableRequirement):
+class AssertTableUUID(ValidatableTableRequirement):
     """The table UUID must match the requirement's `uuid`."""
 
     type: Literal["assert-table-uuid"] = Field(default="assert-table-uuid")
     uuid: uuid.UUID
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif self.uuid != base_metadata.table_uuid:
             raise CommitFailedException(f"Table UUID does not match: {self.uuid} != {base_metadata.table_uuid}")
 
 
-class AssertRefSnapshotId(TableRequirement):
+class AssertRefSnapshotId(ValidatableTableRequirement):
     """The table branch or tag identified by the requirement's `ref` must reference the requirement's `snapshot-id`.
 
     if `snapshot-id` is `null` or missing, the ref must not already exist.
     """
 
     type: Literal["assert-ref-snapshot-id"] = Field(default="assert-ref-snapshot-id")
     ref: str = Field(...)
@@ -734,89 +777,106 @@
                 raise CommitFailedException(
                     f"Requirement failed: {ref_type} {self.ref} has changed: expected id {self.snapshot_id}, found {snapshot_ref.snapshot_id}"
                 )
         elif self.snapshot_id is not None:
             raise CommitFailedException(f"Requirement failed: branch or tag {self.ref} is missing, expected {self.snapshot_id}")
 
 
-class AssertLastAssignedFieldId(TableRequirement):
+class AssertLastAssignedFieldId(ValidatableTableRequirement):
     """The table's last assigned column id must match the requirement's `last-assigned-field-id`."""
 
     type: Literal["assert-last-assigned-field-id"] = Field(default="assert-last-assigned-field-id")
     last_assigned_field_id: int = Field(..., alias="last-assigned-field-id")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif base_metadata.last_column_id != self.last_assigned_field_id:
             raise CommitFailedException(
                 f"Requirement failed: last assigned field id has changed: expected {self.last_assigned_field_id}, found {base_metadata.last_column_id}"
             )
 
 
-class AssertCurrentSchemaId(TableRequirement):
+class AssertCurrentSchemaId(ValidatableTableRequirement):
     """The table's current schema id must match the requirement's `current-schema-id`."""
 
     type: Literal["assert-current-schema-id"] = Field(default="assert-current-schema-id")
     current_schema_id: int = Field(..., alias="current-schema-id")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif self.current_schema_id != base_metadata.current_schema_id:
             raise CommitFailedException(
                 f"Requirement failed: current schema id has changed: expected {self.current_schema_id}, found {base_metadata.current_schema_id}"
             )
 
 
-class AssertLastAssignedPartitionId(TableRequirement):
+class AssertLastAssignedPartitionId(ValidatableTableRequirement):
     """The table's last assigned partition id must match the requirement's `last-assigned-partition-id`."""
 
     type: Literal["assert-last-assigned-partition-id"] = Field(default="assert-last-assigned-partition-id")
     last_assigned_partition_id: int = Field(..., alias="last-assigned-partition-id")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif base_metadata.last_partition_id != self.last_assigned_partition_id:
             raise CommitFailedException(
                 f"Requirement failed: last assigned partition id has changed: expected {self.last_assigned_partition_id}, found {base_metadata.last_partition_id}"
             )
 
 
-class AssertDefaultSpecId(TableRequirement):
+class AssertDefaultSpecId(ValidatableTableRequirement):
     """The table's default spec id must match the requirement's `default-spec-id`."""
 
     type: Literal["assert-default-spec-id"] = Field(default="assert-default-spec-id")
     default_spec_id: int = Field(..., alias="default-spec-id")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif self.default_spec_id != base_metadata.default_spec_id:
             raise CommitFailedException(
                 f"Requirement failed: default spec id has changed: expected {self.default_spec_id}, found {base_metadata.default_spec_id}"
             )
 
 
-class AssertDefaultSortOrderId(TableRequirement):
+class AssertDefaultSortOrderId(ValidatableTableRequirement):
     """The table's default sort order id must match the requirement's `default-sort-order-id`."""
 
     type: Literal["assert-default-sort-order-id"] = Field(default="assert-default-sort-order-id")
     default_sort_order_id: int = Field(..., alias="default-sort-order-id")
 
     def validate(self, base_metadata: Optional[TableMetadata]) -> None:
         if base_metadata is None:
             raise CommitFailedException("Requirement failed: current table metadata is missing")
         elif self.default_sort_order_id != base_metadata.default_sort_order_id:
             raise CommitFailedException(
                 f"Requirement failed: default sort order id has changed: expected {self.default_sort_order_id}, found {base_metadata.default_sort_order_id}"
             )
 
 
+TableRequirement = Annotated[
+    Union[
+        AssertCreate,
+        AssertTableUUID,
+        AssertRefSnapshotId,
+        AssertLastAssignedFieldId,
+        AssertCurrentSchemaId,
+        AssertLastAssignedPartitionId,
+        AssertDefaultSpecId,
+        AssertDefaultSortOrderId,
+    ],
+    Field(discriminator='type'),
+]
+
+UpdatesAndRequirements = Tuple[Tuple[TableUpdate, ...], Tuple[TableRequirement, ...]]
+
+
 class Namespace(IcebergRootModel[List[str]]):
     """Reference to one or more levels of a namespace."""
 
     root: List[str] = Field(
         ...,
         description='Reference to one or more levels of a namespace',
     )
@@ -827,16 +887,16 @@
 
     namespace: Namespace
     name: str
 
 
 class CommitTableRequest(IcebergBaseModel):
     identifier: TableIdentifier = Field()
-    requirements: Tuple[SerializeAsAny[TableRequirement], ...] = Field(default_factory=tuple)
-    updates: Tuple[SerializeAsAny[TableUpdate], ...] = Field(default_factory=tuple)
+    requirements: Tuple[TableRequirement, ...] = Field(default_factory=tuple)
+    updates: Tuple[TableUpdate, ...] = Field(default_factory=tuple)
 
 
 class CommitTableResponse(IcebergBaseModel):
     metadata: TableMetadata
     metadata_location: str = Field(alias="metadata-location")
 
 
@@ -988,14 +1048,22 @@
 
         if not isinstance(df, pa.Table):
             raise ValueError(f"Expected PyArrow table, got: {df}")
 
         if len(self.spec().fields) > 0:
             raise ValueError("Cannot write to partitioned tables")
 
+        from pyiceberg.io.pyarrow import schema_to_pyarrow
+
+        _check_schema_compatible(self.schema(), other_schema=df.schema)
+        # cast if the two schemas are compatible but not equal
+        table_arrow_schema = schema_to_pyarrow(self.schema())
+        if table_arrow_schema != df.schema:
+            df = df.cast(table_arrow_schema)
+
         merge = _MergingSnapshotProducer(operation=Operation.APPEND, table=self)
 
         # skip writing data files if the dataframe is empty
         if df.shape[0] > 0:
             data_files = _dataframe_to_data_files(self, df=df)
             for data_file in data_files:
                 merge.append_data_file(data_file)
@@ -1021,14 +1089,22 @@
 
         if overwrite_filter != AlwaysTrue():
             raise NotImplementedError("Cannot overwrite a subset of a table")
 
         if len(self.spec().fields) > 0:
             raise ValueError("Cannot write to partitioned tables")
 
+        from pyiceberg.io.pyarrow import schema_to_pyarrow
+
+        _check_schema_compatible(self.schema(), other_schema=df.schema)
+        # cast if the two schemas are compatible but not equal
+        table_arrow_schema = schema_to_pyarrow(self.schema())
+        if table_arrow_schema != df.schema:
+            df = df.cast(table_arrow_schema)
+
         merge = _MergingSnapshotProducer(
             operation=Operation.OVERWRITE if self.current_snapshot() is not None else Operation.APPEND,
             table=self,
         )
 
         # skip writing data files if the dataframe is empty
         if df.shape[0] > 0:
@@ -1271,15 +1347,17 @@
 
     Returns:
         A set of files that are relevant for the data file.
     """
     relevant_entries = positional_delete_entries[positional_delete_entries.bisect_right(data_entry) :]
 
     if len(relevant_entries) > 0:
-        evaluator = _InclusiveMetricsEvaluator(POSITIONAL_DELETE_SCHEMA, EqualTo("file_path", data_entry.data_file.file_path))
+        evaluator = visitors._InclusiveMetricsEvaluator(
+            POSITIONAL_DELETE_SCHEMA, EqualTo("file_path", data_entry.data_file.file_path)
+        )
         return {
             positional_delete_entry.data_file
             for positional_delete_entry in relevant_entries
             if evaluator.eval(positional_delete_entry.data_file)
         }
     else:
         return set()
@@ -1295,15 +1373,15 @@
         snapshot_id: Optional[int] = None,
         options: Properties = EMPTY_DICT,
         limit: Optional[int] = None,
     ):
         super().__init__(table, row_filter, selected_fields, case_sensitive, snapshot_id, options, limit)
 
     def _build_partition_projection(self, spec_id: int) -> BooleanExpression:
-        project = inclusive_projection(self.table.schema(), self.table.specs()[spec_id])
+        project = visitors.inclusive_projection(self.table.schema(), self.table.specs()[spec_id])
         return project(self.row_filter)
 
     @cached_property
     def partition_filters(self) -> KeyDefaultDict[int, BooleanExpression]:
         return KeyDefaultDict(self._build_partition_projection)
 
     def _build_manifest_evaluator(self, spec_id: int) -> Callable[[ManifestFile], bool]:
@@ -1362,15 +1440,15 @@
             if manifest_evaluators[manifest_file.partition_spec_id](manifest_file)
         ]
 
         # step 2: filter the data files in each manifest
         # this filter depends on the partition spec used to write the manifest file
 
         partition_evaluators: Dict[int, Callable[[DataFile], bool]] = KeyDefaultDict(self._build_partition_evaluator)
-        metrics_evaluator = _InclusiveMetricsEvaluator(
+        metrics_evaluator = visitors._InclusiveMetricsEvaluator(
             self.table.schema(), self.row_filter, self.case_sensitive, self.options.get("include_empty_files") == "true"
         ).eval
 
         min_data_sequence_number = _min_data_file_sequence_number(manifests)
 
         data_entries: List[ManifestEntry] = []
         positional_delete_entries = SortedList(key=lambda entry: entry.data_sequence_number or INITIAL_SEQUENCE_NUMBER)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/metadata.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Dict,
     List,
     Literal,
     Optional,
     Union,
 )
 
-from pydantic import Field, model_validator
+from pydantic import Field, field_serializer, model_validator
 from pydantic import ValidationError as PydanticValidationError
 from typing_extensions import Annotated
 
 from pyiceberg.exceptions import ValidationError
 from pyiceberg.partitioning import PARTITION_FIELD_ID_START, PartitionSpec, assign_fresh_partition_spec_ids
 from pyiceberg.schema import Schema, assign_fresh_schema_ids
 from pyiceberg.table.refs import MAIN_BRANCH, SnapshotRef, SnapshotRefType
@@ -45,14 +45,15 @@
 )
 from pyiceberg.typedef import (
     EMPTY_DICT,
     IcebergBaseModel,
     IcebergRootModel,
     Properties,
 )
+from pyiceberg.utils.config import Config
 from pyiceberg.utils.datetime import datetime_to_millis
 
 CURRENT_SNAPSHOT_ID = "current-snapshot-id"
 CURRENT_SCHEMA_ID = "current-schema-id"
 SCHEMAS = "schemas"
 DEFAULT_SPEC_ID = "default-spec-id"
 PARTITION_SPEC = "partition-spec"
@@ -222,14 +223,20 @@
         """Get the snapshot by snapshot_id."""
         return next((snapshot for snapshot in self.snapshots if snapshot.snapshot_id == snapshot_id), None)
 
     def schema_by_id(self, schema_id: int) -> Optional[Schema]:
         """Get the schema by schema_id."""
         return next((schema for schema in self.schemas if schema.schema_id == schema_id), None)
 
+    @field_serializer('current_snapshot_id')
+    def serialize_current_snapshot_id(self, current_snapshot_id: Optional[int]) -> Optional[int]:
+        if current_snapshot_id is None and Config().get_bool("legacy-current-snapshot-id"):
+            return -1
+        return current_snapshot_id
+
 
 class TableMetadataV1(TableMetadataCommonFields, IcebergBaseModel):
     """Represents version 1 of the Table Metadata.
 
     More information about the specification:
     https://iceberg.apache.org/spec/#version-1-analytic-data-tables
     """
@@ -302,14 +309,19 @@
         """
         if not data.get(PARTITION_SPECS):
             if data.get(PARTITION_SPEC) is not None:
                 # Promote the spec from partition-spec to partition-specs
                 fields = data[PARTITION_SPEC]
                 data[PARTITION_SPECS] = [{SPEC_ID: INITIAL_SPEC_ID, FIELDS: fields}]
                 data[DEFAULT_SPEC_ID] = INITIAL_SPEC_ID
+            elif data.get("partition_spec") is not None:
+                # Promote the spec from partition_spec to partition-specs
+                fields = data["partition_spec"]
+                data[PARTITION_SPECS] = [{SPEC_ID: INITIAL_SPEC_ID, FIELDS: fields}]
+                data[DEFAULT_SPEC_ID] = INITIAL_SPEC_ID
             else:
                 data[PARTITION_SPECS] = [{"field-id": 0, "fields": ()}]
 
         data[LAST_PARTITION_ID] = max(
             [field.get(FIELD_ID) for spec in data[PARTITION_SPECS] for field in spec[FIELDS]], default=PARTITION_FIELD_ID_START
         )
 
@@ -324,15 +336,15 @@
 
         Args:
             data: The raw data after validation, meaning that the aliases are applied.
 
         Returns:
             The TableMetadata with the sort_orders set, if not provided.
         """
-        if not data.get(SORT_ORDERS):
+        if not data.get(SORT_ORDERS) and not data.get("sort_orders"):
             data[SORT_ORDERS] = [UNSORTED_SORT_ORDER]
         return data
 
     def to_v2(self) -> TableMetadataV2:
         metadata = copy(self.model_dump())
         metadata["format-version"] = 2
         return TableMetadataV2.model_validate(metadata)
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/name_mapping.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/name_mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import ChainMap
 from functools import cached_property, singledispatch
-from typing import Any, Dict, Generic, List, TypeVar, Union
+from typing import Any, Dict, Generic, Iterator, List, TypeVar, Union
 
 from pydantic import Field, conlist, field_validator, model_serializer
 
 from pyiceberg.schema import Schema, SchemaVisitor, visit
 from pyiceberg.typedef import IcebergBaseModel, IcebergRootModel
 from pyiceberg.types import ListType, MapType, NestedField, PrimitiveType, StructType
 
@@ -81,14 +81,18 @@
         except KeyError as e:
             raise ValueError(f"Could not find field with name: {name}") from e
 
     def __len__(self) -> int:
         """Return the number of mappings."""
         return len(self.root)
 
+    def __iter__(self) -> Iterator[MappedField]:
+        """Iterate over the mapped fields."""
+        return iter(self.root)
+
     def __str__(self) -> str:
         """Convert the name-mapping into a nicely formatted string."""
         if len(self.root) == 0:
             return "[]"
         else:
             return "[\n  " + "\n  ".join([str(e) for e in self.root]) + "\n]"
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/refs.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/snapshots.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/table/sorting.py` & `pyiceberg-0.6.1rc1/pyiceberg/table/sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/transforms.py` & `pyiceberg-0.6.1rc1/pyiceberg/transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/typedef.py` & `pyiceberg-0.6.1rc1/pyiceberg/typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/types.py` & `pyiceberg-0.6.1rc1/pyiceberg/types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/__init__.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/bin_packing.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/concurrent.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/concurrent.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,17 +33,8 @@
             ExecutorFactory._instance = ThreadPoolExecutor(max_workers=max_workers)
 
         return ExecutorFactory._instance
 
     @staticmethod
     def max_workers() -> Optional[int]:
         """Return the max number of workers configured."""
-        config = Config()
-        val = config.config.get("max-workers")
-
-        if val is None:
-            return None
-
-        try:
-            return int(val)  # type: ignore
-        except ValueError as err:
-            raise ValueError(f"Max workers should be an integer or left unset. Current value: {val}") from err
+        return Config().get_int("max-workers")
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/config.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 import logging
 import os
+from distutils.util import strtobool
 from typing import List, Optional
 
 import strictyaml
 
 from pyiceberg.typedef import UTF8, FrozenDict, RecursiveDict
 
 PYICEBERG = "pyiceberg_"
@@ -150,7 +151,23 @@
             if not isinstance(catalogs, dict):
                 raise ValueError(f"Catalog configurations needs to be an object: {catalog_name}")
             if catalog_name_lower in catalogs:
                 catalog_conf = catalogs[catalog_name_lower]
                 assert isinstance(catalog_conf, dict), f"Configuration path catalogs.{catalog_name_lower} needs to be an object"
                 return catalog_conf
         return None
+
+    def get_int(self, key: str) -> Optional[int]:
+        if (val := self.config.get(key)) is not None:
+            try:
+                return int(val)  # type: ignore
+            except ValueError as err:
+                raise ValueError(f"{key} should be an integer or left unset. Current value: {val}") from err
+        return None
+
+    def get_bool(self, key: str) -> Optional[bool]:
+        if (val := self.config.get(key)) is not None:
+            try:
+                return strtobool(val)  # type: ignore
+            except ValueError as err:
+                raise ValueError(f"{key} should be a boolean or left unset. Current value: {val}") from err
+        return None
```

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/datetime.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/decimal.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/decimal.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/deprecated.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/lazydict.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/lazydict.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/parsing.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/schema_conversion.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/singleton.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyiceberg/utils/truncate.py` & `pyiceberg-0.6.1rc1/pyiceberg/utils/truncate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/pyproject.toml` & `pyiceberg-0.6.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.poetry]
 name = "pyiceberg"
-version = "0.6.0rc6"
+version = "0.6.1rc1"
 readme = "README.md"
 homepage = "https://py.iceberg.apache.org/"
 repository = "https://github.com/apache/iceberg-python"
 description = "Apache Iceberg is an open table format for huge analytic datasets"
 authors = ["Apache Software Foundation <dev@iceberg.apache.org>"]
 license = "Apache License 2.0"
 classifiers = [
```

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_decoder.py` & `pyiceberg-0.6.1rc1/tests/avro/test_decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_encoder.py` & `pyiceberg-0.6.1rc1/tests/avro/test_encoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_file.py` & `pyiceberg-0.6.1rc1/tests/avro/test_file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_reader.py` & `pyiceberg-0.6.1rc1/tests/avro/test_reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_resolver.py` & `pyiceberg-0.6.1rc1/tests/avro/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/avro/test_writer.py` & `pyiceberg-0.6.1rc1/tests/avro/test_writer.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/integration_test_dynamodb.py` & `pyiceberg-0.6.1rc1/tests/catalog/integration_test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/integration_test_glue.py` & `pyiceberg-0.6.1rc1/tests/catalog/integration_test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_base.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
 import pyarrow as pa
 import pytest
 from pytest_lazyfixture import lazy_fixture
 
 from pyiceberg.catalog import (
     Catalog,
-    Identifier,
-    Properties,
     PropertiesUpdateSummary,
 )
 from pyiceberg.exceptions import (
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchNamespaceError,
     NoSuchTableError,
@@ -52,15 +50,15 @@
     SetCurrentSchemaUpdate,
     Table,
     TableIdentifier,
 )
 from pyiceberg.table.metadata import TableMetadata, TableMetadataV1, new_table_metadata
 from pyiceberg.table.sorting import UNSORTED_SORT_ORDER, SortOrder
 from pyiceberg.transforms import IdentityTransform
-from pyiceberg.typedef import EMPTY_DICT
+from pyiceberg.typedef import EMPTY_DICT, Identifier, Properties
 from pyiceberg.types import IntegerType, LongType, NestedField
 
 
 class InMemoryCatalog(Catalog):
     """An in-memory catalog implementation for testing purposes."""
 
     __tables: Dict[Identifier, Table]
```

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_dynamodb.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_glue.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_hive.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_hive.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_rest.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 from typing import Any, Dict, cast
 from unittest import mock
 
 import pytest
 from requests_mock import Mocker
 
 import pyiceberg
-from pyiceberg.catalog import PropertiesUpdateSummary, Table, load_catalog
+from pyiceberg.catalog import PropertiesUpdateSummary, load_catalog
 from pyiceberg.catalog.rest import AUTH_URL, RestCatalog
 from pyiceberg.exceptions import (
     NamespaceAlreadyExistsError,
     NoSuchNamespaceError,
     NoSuchTableError,
     OAuthError,
     TableAlreadyExistsError,
 )
 from pyiceberg.io import load_file_io
 from pyiceberg.partitioning import PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
+from pyiceberg.table import Table
 from pyiceberg.table.metadata import TableMetadataV1
 from pyiceberg.table.sorting import SortField, SortOrder
 from pyiceberg.transforms import IdentityTransform, TruncateTransform
 from pyiceberg.typedef import RecursiveDict
 from pyiceberg.utils.config import Config
 
 TEST_URI = "https://iceberg-test-catalog/"
```

### Comparing `pyiceberg-0.6.0rc6/tests/catalog/test_sql.py` & `pyiceberg-0.6.1rc1/tests/catalog/test_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from typing import Generator, List
 
 import pyarrow as pa
 import pytest
 from pytest_lazyfixture import lazy_fixture
 from sqlalchemy.exc import ArgumentError, IntegrityError
 
-from pyiceberg.catalog import Identifier
 from pyiceberg.catalog.sql import SqlCatalog
 from pyiceberg.exceptions import (
     CommitFailedException,
     NamespaceAlreadyExistsError,
     NamespaceNotEmptyError,
     NoSuchNamespaceError,
     NoSuchPropertyException,
@@ -43,14 +42,15 @@
 from pyiceberg.table.sorting import (
     NullOrder,
     SortDirection,
     SortField,
     SortOrder,
 )
 from pyiceberg.transforms import IdentityTransform
+from pyiceberg.typedef import Identifier
 from pyiceberg.types import IntegerType
 
 
 @pytest.fixture(name="random_identifier")
 def fixture_random_identifier(warehouse: Path, database_name: str, table_name: str) -> Identifier:
     os.makedirs(f"{warehouse}/{database_name}.db/{table_name}/metadata/", exist_ok=True)
     return database_name, table_name
@@ -192,14 +192,44 @@
 
 
 @pytest.mark.parametrize(
     'catalog',
     [
         lazy_fixture('catalog_memory'),
         lazy_fixture('catalog_sqlite'),
+    ],
+)
+def test_write_pyarrow_schema(catalog: SqlCatalog, random_identifier: Identifier) -> None:
+    import pyarrow as pa
+
+    pyarrow_table = pa.Table.from_arrays(
+        [
+            pa.array([None, "A", "B", "C"]),  # 'foo' column
+            pa.array([1, 2, 3, 4]),  # 'bar' column
+            pa.array([True, None, False, True]),  # 'baz' column
+            pa.array([None, "A", "B", "C"]),  # 'large' column
+        ],
+        schema=pa.schema([
+            pa.field('foo', pa.string(), nullable=True),
+            pa.field('bar', pa.int32(), nullable=False),
+            pa.field('baz', pa.bool_(), nullable=True),
+            pa.field('large', pa.large_string(), nullable=True),
+        ]),
+    )
+    database_name, _table_name = random_identifier
+    catalog.create_namespace(database_name)
+    table = catalog.create_table(random_identifier, pyarrow_table.schema)
+    table.overwrite(pyarrow_table)
+
+
+@pytest.mark.parametrize(
+    'catalog',
+    [
+        lazy_fixture('catalog_memory'),
+        lazy_fixture('catalog_sqlite'),
     ],
 )
 def test_create_table_custom_sort_order(catalog: SqlCatalog, table_schema_nested: Schema, random_identifier: Identifier) -> None:
     database_name, _table_name = random_identifier
     catalog.create_namespace(database_name)
     order = SortOrder(SortField(source_id=2, transform=IdentityTransform(), null_order=NullOrder.NULLS_FIRST))
     table = catalog.create_table(random_identifier, table_schema_nested, sort_order=order)
```

### Comparing `pyiceberg-0.6.0rc6/tests/cli/test_console.py` & `pyiceberg-0.6.1rc1/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/cli/test_output.py` & `pyiceberg-0.6.1rc1/tests/cli/test_output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/conftest.py` & `pyiceberg-0.6.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_evaluator.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_expressions.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_literals.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_parser.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 import pytest
 from pyparsing import ParseException
 
+import pyiceberg.expressions.parser as parser
 from pyiceberg.expressions import (
     AlwaysFalse,
     AlwaysTrue,
     And,
     EqualTo,
     GreaterThan,
     GreaterThanOrEqual,
@@ -33,15 +34,14 @@
     NotEqualTo,
     NotIn,
     NotNaN,
     NotNull,
     NotStartsWith,
     Or,
     StartsWith,
-    parser,
 )
 
 
 def test_true() -> None:
     assert AlwaysTrue() == parser.parse("true")
```

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_projection.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_projection.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/expressions/test_visitors.py` & `pyiceberg-0.6.1rc1/tests/expressions/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/integration/test_reads.py` & `pyiceberg-0.6.1rc1/tests/integration/test_reads.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,14 @@
 
 @pytest.mark.integration
 @pytest.mark.parametrize('catalog', [pytest.lazy_fixture('catalog_hive'), pytest.lazy_fixture('catalog_rest')])
 @pytest.mark.skip(reason="Fixing issues with NaN's: https://github.com/apache/arrow/issues/34162")
 def test_ray_not_nan_count(catalog: Catalog) -> None:
     table_test_null_nan_rewritten = catalog.load_table("default.test_null_nan_rewritten")
     ray_dataset = table_test_null_nan_rewritten.scan(row_filter=NotNaN("col_numeric"), selected_fields=("idx",)).to_ray()
-    print(ray_dataset.take())
     assert ray_dataset.count() == 2
 
 
 @pytest.mark.integration
 @pytest.mark.parametrize('catalog', [pytest.lazy_fixture('catalog_hive'), pytest.lazy_fixture('catalog_rest')])
 def test_ray_all_types(catalog: Catalog) -> None:
     table_test_all_types = catalog.load_table("default.test_all_types")
```

### Comparing `pyiceberg-0.6.0rc6/tests/integration/test_rest_manifest.py` & `pyiceberg-0.6.1rc1/tests/integration/test_rest_manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/integration/test_rest_schema.py` & `pyiceberg-0.6.1rc1/tests/integration/test_rest_schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/integration/test_writes.py` & `pyiceberg-0.6.1rc1/tests/integration/test_writes.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 import pyarrow.parquet as pq
 import pytest
 import pytz
 from pyarrow.fs import S3FileSystem
 from pyspark.sql import SparkSession
 from pytest_mock.plugin import MockerFixture
 
-from pyiceberg.catalog import Catalog, Properties, Table, load_catalog
+from pyiceberg.catalog import Catalog, load_catalog
 from pyiceberg.catalog.sql import SqlCatalog
 from pyiceberg.exceptions import NamespaceAlreadyExistsError, NoSuchTableError
 from pyiceberg.schema import Schema
+from pyiceberg.table import Table
+from pyiceberg.typedef import Properties
 from pyiceberg.types import (
     BinaryType,
     BooleanType,
     DateType,
     DoubleType,
     FixedType,
     FloatType,
@@ -475,15 +477,14 @@
     mocker: MockerFixture,
     spark: SparkSession,
     session_catalog: Catalog,
     arrow_table_with_null: pa.Table,
     properties: Dict[str, Any],
     expected_kwargs: Dict[str, Any],
 ) -> None:
-    print(type(mocker))
     identifier = "default.test_write_parquet_other_properties"
 
     # The properties we test cannot be checked on the resulting Parquet file, so we spy on the ParquetWriter call instead
     ParquetWriter = mocker.spy(pq, "ParquetWriter")
     _create_table(session_catalog, identifier, properties, [arrow_table_with_null])
 
     call_kwargs = ParquetWriter.call_args[1]
```

### Comparing `pyiceberg-0.6.0rc6/tests/io/test_fsspec.py` & `pyiceberg-0.6.1rc1/tests/io/test_fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/io/test_io.py` & `pyiceberg-0.6.1rc1/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/io/test_pyarrow.py` & `pyiceberg-0.6.1rc1/tests/io/test_pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     BoundNotNull,
     BoundNotStartsWith,
     BoundReference,
     BoundStartsWith,
     GreaterThan,
     Not,
     Or,
-    literal,
 )
+from pyiceberg.expressions.literals import literal
 from pyiceberg.io import InputStream, OutputStream, load_file_io
 from pyiceberg.io.pyarrow import (
     ICEBERG_SCHEMA,
     PyArrowFile,
     PyArrowFileIO,
     StatsAggregator,
     _ConvertToArrowSchema,
```

### Comparing `pyiceberg-0.6.0rc6/tests/io/test_pyarrow_stats.py` & `pyiceberg-0.6.1rc1/tests/io/test_pyarrow_stats.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/io/test_pyarrow_visitor.py` & `pyiceberg-0.6.1rc1/tests/io/test_pyarrow_visitor.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_init.py` & `pyiceberg-0.6.1rc1/tests/table/test_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # specific language governing permissions and limitations
 # under the License.
 # pylint:disable=redefined-outer-name
 import uuid
 from copy import copy
 from typing import Dict
 
+import pyarrow as pa
 import pytest
 from sortedcontainers import SortedList
 
 from pyiceberg.catalog.noop import NoopCatalog
 from pyiceberg.exceptions import CommitFailedException
 from pyiceberg.expressions import (
     AlwaysTrue,
@@ -49,25 +50,26 @@
     AssertLastAssignedFieldId,
     AssertLastAssignedPartitionId,
     AssertRefSnapshotId,
     AssertTableUUID,
     RemovePropertiesUpdate,
     SetPropertiesUpdate,
     SetSnapshotRefUpdate,
-    SnapshotRef,
     StaticTable,
     Table,
     UpdateSchema,
     _apply_table_update,
+    _check_schema_compatible,
     _generate_snapshot_id,
     _match_deletes_to_data_file,
     _TableMetadataUpdateContext,
     update_table_metadata,
 )
 from pyiceberg.table.metadata import INITIAL_SEQUENCE_NUMBER, TableMetadataUtil, TableMetadataV2
+from pyiceberg.table.refs import SnapshotRef
 from pyiceberg.table.snapshots import (
     Operation,
     Snapshot,
     SnapshotLogEntry,
     Summary,
 )
 from pyiceberg.table.sorting import (
@@ -978,7 +980,97 @@
         t.scan(snapshot_id=234).projection()
 
     # Invalid snapshot
     with pytest.raises(ValueError) as exc_info:
         _ = t.scan(snapshot_id=-1).projection()
 
     assert "Snapshot not found: -1" in str(exc_info.value)
+
+
+def test_schema_mismatch_type(table_schema_simple: Schema) -> None:
+    other_schema = pa.schema((
+        pa.field("foo", pa.string(), nullable=True),
+        pa.field("bar", pa.decimal128(18, 6), nullable=False),
+        pa.field("baz", pa.bool_(), nullable=True),
+    ))
+
+    expected = r"""Mismatch in fields:
+┏━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃    ┃ Table field              ┃ Dataframe field                 ┃
+┡━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ ✅ │ 1: foo: optional string  │ 1: foo: optional string         │
+│ ❌ │ 2: bar: required int     │ 2: bar: required decimal\(18, 6\) │
+│ ✅ │ 3: baz: optional boolean │ 3: baz: optional boolean        │
+└────┴──────────────────────────┴─────────────────────────────────┘
+"""
+
+    with pytest.raises(ValueError, match=expected):
+        _check_schema_compatible(table_schema_simple, other_schema)
+
+
+def test_schema_mismatch_nullability(table_schema_simple: Schema) -> None:
+    other_schema = pa.schema((
+        pa.field("foo", pa.string(), nullable=True),
+        pa.field("bar", pa.int32(), nullable=True),
+        pa.field("baz", pa.bool_(), nullable=True),
+    ))
+
+    expected = """Mismatch in fields:
+┏━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃    ┃ Table field              ┃ Dataframe field          ┃
+┡━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ ✅ │ 1: foo: optional string  │ 1: foo: optional string  │
+│ ❌ │ 2: bar: required int     │ 2: bar: optional int     │
+│ ✅ │ 3: baz: optional boolean │ 3: baz: optional boolean │
+└────┴──────────────────────────┴──────────────────────────┘
+"""
+
+    with pytest.raises(ValueError, match=expected):
+        _check_schema_compatible(table_schema_simple, other_schema)
+
+
+def test_schema_mismatch_missing_field(table_schema_simple: Schema) -> None:
+    other_schema = pa.schema((
+        pa.field("foo", pa.string(), nullable=True),
+        pa.field("baz", pa.bool_(), nullable=True),
+    ))
+
+    expected = """Mismatch in fields:
+┏━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃    ┃ Table field              ┃ Dataframe field          ┃
+┡━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ ✅ │ 1: foo: optional string  │ 1: foo: optional string  │
+│ ❌ │ 2: bar: required int     │ Missing                  │
+│ ✅ │ 3: baz: optional boolean │ 3: baz: optional boolean │
+└────┴──────────────────────────┴──────────────────────────┘
+"""
+
+    with pytest.raises(ValueError, match=expected):
+        _check_schema_compatible(table_schema_simple, other_schema)
+
+
+def test_schema_mismatch_additional_field(table_schema_simple: Schema) -> None:
+    other_schema = pa.schema((
+        pa.field("foo", pa.string(), nullable=True),
+        pa.field("bar", pa.int32(), nullable=True),
+        pa.field("baz", pa.bool_(), nullable=True),
+        pa.field("new_field", pa.date32(), nullable=True),
+    ))
+
+    expected = r"PyArrow table contains more columns: new_field. Update the schema first \(hint, use union_by_name\)."
+
+    with pytest.raises(ValueError, match=expected):
+        _check_schema_compatible(table_schema_simple, other_schema)
+
+
+def test_schema_downcast(table_schema_simple: Schema) -> None:
+    # large_string type is compatible with string type
+    other_schema = pa.schema((
+        pa.field("foo", pa.large_string(), nullable=True),
+        pa.field("bar", pa.int32(), nullable=False),
+        pa.field("baz", pa.bool_(), nullable=True),
+    ))
+
+    try:
+        _check_schema_compatible(table_schema_simple, other_schema)
+    except Exception:
+        pytest.fail("Unexpected Exception raised when calling `_check_schema`")
```

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_metadata.py` & `pyiceberg-0.6.1rc1/tests/table/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,22 @@
 
 import pytest
 
 from pyiceberg.exceptions import ValidationError
 from pyiceberg.partitioning import PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
 from pyiceberg.serializers import FromByteStream
-from pyiceberg.table import SortOrder
 from pyiceberg.table.metadata import (
     TableMetadataUtil,
     TableMetadataV1,
     TableMetadataV2,
     new_table_metadata,
 )
 from pyiceberg.table.refs import SnapshotRef, SnapshotRefType
-from pyiceberg.table.sorting import NullOrder, SortDirection, SortField
+from pyiceberg.table.sorting import NullOrder, SortDirection, SortField, SortOrder
 from pyiceberg.transforms import IdentityTransform
 from pyiceberg.typedef import UTF8
 from pyiceberg.types import (
     BooleanType,
     FloatType,
     IntegerType,
     ListType,
@@ -231,14 +230,19 @@
         NestedField(field_id=3, name="baz", field_type=BooleanType(), required=False),
         schema_id=0,
         identifier_field_ids=[2],
     )
 
     expected_spec = PartitionSpec(PartitionField(source_id=2, field_id=1000, transform=IdentityTransform(), name="bar"))
 
+    expected_sort_order = SortOrder(
+        SortField(source_id=1, transform=IdentityTransform(), direction=SortDirection.ASC, null_order=NullOrder.NULLS_LAST),
+        order_id=1,
+    )
+
     expected = TableMetadataV1(
         location="s3://some_v1_location/",
         table_uuid=actual.table_uuid,
         last_updated_ms=actual.last_updated_ms,
         last_column_id=3,
         schemas=[expected_schema],
         schema_=expected_schema,
@@ -248,28 +252,24 @@
         default_spec_id=0,
         last_partition_id=1000,
         properties={},
         current_snapshot_id=None,
         snapshots=[],
         snapshot_log=[],
         metadata_log=[],
-        sort_orders=[
-            SortOrder(
-                SortField(
-                    source_id=1, transform=IdentityTransform(), direction=SortDirection.ASC, null_order=NullOrder.NULLS_LAST
-                ),
-                order_id=1,
-            )
-        ],
+        sort_orders=[expected_sort_order],
         default_sort_order_id=1,
         refs={},
         format_version=1,
     )
 
     assert actual.model_dump() == expected.model_dump()
+    assert actual.schemas == [expected_schema]
+    assert actual.partition_specs == [expected_spec]
+    assert actual.sort_orders == [expected_sort_order]
 
 
 def test_invalid_format_version(example_table_metadata_v1: Dict[str, Any]) -> None:
     """Test the exception when trying to load an unknown version"""
 
     example_table_metadata_v22 = copy(example_table_metadata_v1)
     example_table_metadata_v22["format-version"] = -1
```

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_name_mapping.py` & `pyiceberg-0.6.1rc1/tests/table/test_name_mapping.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_partitioning.py` & `pyiceberg-0.6.1rc1/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_refs.py` & `pyiceberg-0.6.1rc1/tests/table/test_refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_snapshots.py` & `pyiceberg-0.6.1rc1/tests/table/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/table/test_sorting.py` & `pyiceberg-0.6.1rc1/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/test_conversions.py` & `pyiceberg-0.6.1rc1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/test_schema.py` & `pyiceberg-0.6.1rc1/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Any, Dict, List
 
 import pyarrow as pa
 import pytest
 
 from pyiceberg import schema
 from pyiceberg.exceptions import ResolveError, ValidationError
-from pyiceberg.expressions import Accessor
 from pyiceberg.schema import (
+    Accessor,
     Schema,
     build_position_accessors,
     promote,
     prune_columns,
     sanitize_column_names,
 )
 from pyiceberg.table import UpdateSchema
```

### Comparing `pyiceberg-0.6.0rc6/tests/test_transforms.py` & `pyiceberg-0.6.1rc1/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/test_typedef.py` & `pyiceberg-0.6.1rc1/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/test_types.py` & `pyiceberg-0.6.1rc1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/test_version.py` & `pyiceberg-0.6.1rc1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_bin_packing.py` & `pyiceberg-0.6.1rc1/tests/utils/test_bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_concurrent.py` & `pyiceberg-0.6.1rc1/tests/utils/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_config.py` & `pyiceberg-0.6.1rc1/tests/utils/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,7 +72,24 @@
 
 
 def test_merge_config() -> None:
     lhs: RecursiveDict = {"common_key": "abc123"}
     rhs: RecursiveDict = {"common_key": "xyz789"}
     result = merge_config(lhs, rhs)
     assert result["common_key"] == rhs["common_key"]
+
+
+def test_from_configuration_files_get_typed_value(tmp_path_factory: pytest.TempPathFactory) -> None:
+    config_path = str(tmp_path_factory.mktemp("config"))
+    with open(f"{config_path}/.pyiceberg.yaml", "w", encoding=UTF8) as file:
+        yaml_str = as_document({"max-workers": "4", "legacy-current-snapshot-id": "True"}).as_yaml()
+        file.write(yaml_str)
+
+    os.environ["PYICEBERG_HOME"] = config_path
+    with pytest.raises(ValueError):
+        Config().get_bool("max-workers")
+
+    with pytest.raises(ValueError):
+        Config().get_int("legacy-current-snapshot-id")
+
+    assert Config().get_bool("legacy-current-snapshot-id")
+    assert Config().get_int("max-workers") == 4
```

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_datetime.py` & `pyiceberg-0.6.1rc1/tests/utils/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_decimal.py` & `pyiceberg-0.6.1rc1/tests/utils/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_deprecated.py` & `pyiceberg-0.6.1rc1/tests/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_lazydict.py` & `pyiceberg-0.6.1rc1/tests/utils/test_lazydict.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_manifest.py` & `pyiceberg-0.6.1rc1/tests/utils/test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     PartitionFieldSummary,
     read_manifest_list,
     write_manifest,
     write_manifest_list,
 )
 from pyiceberg.partitioning import PartitionField, PartitionSpec
 from pyiceberg.schema import Schema
-from pyiceberg.table import Snapshot
-from pyiceberg.table.snapshots import Operation, Summary
+from pyiceberg.table.snapshots import Operation, Snapshot, Summary
 from pyiceberg.transforms import IdentityTransform
 from pyiceberg.typedef import Record
 from pyiceberg.types import IntegerType, NestedField
 
 
 def _verify_metadata_with_fastavro(avro_file: str, expected_metadata: Dict[str, str]) -> None:
     with open(avro_file, "rb") as f:
```

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_schema_conversion.py` & `pyiceberg-0.6.1rc1/tests/utils/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_singleton.py` & `pyiceberg-0.6.1rc1/tests/utils/test_singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/tests/utils/test_truncate.py` & `pyiceberg-0.6.1rc1/tests/utils/test_truncate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/fb303/FacebookService.py` & `pyiceberg-0.6.1rc1/vendor/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/fb303/__init__.py` & `pyiceberg-0.6.1rc1/vendor/fb303/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/fb303/constants.py` & `pyiceberg-0.6.1rc1/vendor/fb303/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/fb303/ttypes.py` & `pyiceberg-0.6.1rc1/vendor/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/hive_metastore/ThriftHiveMetastore.py` & `pyiceberg-0.6.1rc1/vendor/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/hive_metastore/__init__.py` & `pyiceberg-0.6.1rc1/vendor/hive_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/hive_metastore/constants.py` & `pyiceberg-0.6.1rc1/vendor/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/vendor/hive_metastore/ttypes.py` & `pyiceberg-0.6.1rc1/vendor/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.0rc6/PKG-INFO` & `pyiceberg-0.6.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiceberg
-Version: 0.6.0rc6
+Version: 0.6.1rc1
 Summary: Apache Iceberg is an open table format for huge analytic datasets
 Home-page: https://py.iceberg.apache.org/
 License: Apache-2.0
 Author: Apache Software Foundation
 Author-email: dev@iceberg.apache.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

