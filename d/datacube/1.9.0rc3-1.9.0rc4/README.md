# Comparing `tmp/datacube-1.9.0rc3.tar.gz` & `tmp/datacube-1.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacube-1.9.0rc3.tar", last modified: Wed Mar 27 05:42:48 2024, max compression
+gzip compressed data, was "datacube-1.9.0rc4.tar", last modified: Tue Apr 16 07:06:12 2024, max compression
```

## Comparing `datacube-1.9.0rc3.tar` & `datacube-1.9.0rc4.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/
--rw-r--r--   0 odc       (1001) odc        (127)      492 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.coveragerc
--rw-r--r--   0 odc       (1001) odc        (127)      983 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.dockerignore
--rw-r--r--   0 odc       (1001) odc        (127)     4474 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.doctor-rst.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      487 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.editorconfig
--rw-r--r--   0 odc       (1001) odc        (127)      203 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.gitattributes
--rw-r--r--   0 odc       (1001) odc        (127)     1072 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.gitignore
--rw-r--r--   0 odc       (1001) odc        (127)      423 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.mergify.yml
--rw-r--r--   0 odc       (1001) odc        (127)     1201 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      603 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.readthedocs.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      919 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/.yamllint
--rw-r--r--   0 odc       (1001) odc        (127)     1928 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/CONTRIBUTING.md
--rw-r--r--   0 odc       (1001) odc        (127)    11357 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/LICENSE
--rw-r--r--   0 odc       (1001) odc        (127)       70 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/MANIFEST.in
--rw-rw-r--   0 odc       (1001) odc        (127)     5886 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/PKG-INFO
--rw-r--r--   0 odc       (1001) odc        (127)     4436 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/README.rst
--rw-r--r--   0 odc       (1001) odc        (127)      942 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/alembic.ini
--rwxr-xr-x   0 odc       (1001) odc        (127)      980 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/check-code.sh
--rw-r--r--   0 odc       (1001) odc        (127)     3507 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/code-of-conduct.md
--rw-r--r--   0 odc       (1001) odc        (127)      580 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/conda-environment.yml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.613907 datacube-1.9.0rc3/datacube/
--rw-r--r--   0 odc       (1001) odc        (127)     1128 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/datacube/__init__.py
--rw-rw-r--   0 odc       (1001) odc        (127)      163 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube/_version.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.613907 datacube-1.9.0rc3/datacube/api/
--rw-r--r--   0 odc       (1001) odc        (127)      338 2024-03-27 05:33:36.000000 datacube-1.9.0rc3/datacube/api/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    55967 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/api/core.py
--rw-r--r--   0 odc       (1001) odc        (127)    15205 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/api/query.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.613907 datacube-1.9.0rc3/datacube/cfg/
--rw-r--r--   0 odc       (1001) odc        (127)     1135 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    14240 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/api.py
--rw-r--r--   0 odc       (1001) odc        (127)     4993 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/cfg.py
--rw-r--r--   0 odc       (1001) odc        (127)      325 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/exceptions.py
--rw-r--r--   0 odc       (1001) odc        (127)     9916 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/opt.py
--rw-r--r--   0 odc       (1001) odc        (127)     1648 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/cfg/utils.py
--rwxr-xr-x   0 odc       (1001) odc        (127)      328 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/config.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.617907 datacube-1.9.0rc3/datacube/drivers/
--rw-r--r--   0 odc       (1001) odc        (127)      587 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     1065 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/_tools.py
--rw-r--r--   0 odc       (1001) odc        (127)     2946 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/_types.py
--rw-r--r--   0 odc       (1001) odc        (127)     1739 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/datasource.py
--rw-r--r--   0 odc       (1001) odc        (127)     1779 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/driver_cache.py
--rw-r--r--   0 odc       (1001) odc        (127)     1820 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/indexes.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.617907 datacube-1.9.0rc3/datacube/drivers/netcdf/
--rw-r--r--   0 odc       (1001) odc        (127)      432 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/netcdf/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     4864 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/netcdf/_write.py
--rw-r--r--   0 odc       (1001) odc        (127)     2182 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/netcdf/driver.py
--rw-r--r--   0 odc       (1001) odc        (127)    11295 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/netcdf/writer.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.617907 datacube-1.9.0rc3/datacube/drivers/postgis/
--rw-r--r--   0 odc       (1001) odc        (127)      396 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    55202 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_api.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    11290 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_connections.py
--rw-r--r--   0 odc       (1001) odc        (127)    10504 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_core.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    20805 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)    14240 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_schema.py
--rw-r--r--   0 odc       (1001) odc        (127)     9786 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/_spatial.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.617907 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/
--rw-r--r--   0 odc       (1001) odc        (127)       65 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/README
--rw-r--r--   0 odc       (1001) odc        (127)     4772 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/env.py
--rw-r--r--   0 odc       (1001) odc        (127)      811 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/script.py.mako
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.617907 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/versions/
--rw-r--r--   0 odc       (1001) odc        (127)      673 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/alembic/versions/48fb71ece268_initial_revision.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.621907 datacube-1.9.0rc3/datacube/drivers/postgis/samples/
--rw-r--r--   0 odc       (1001) odc        (127)     4023 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-explicit.sql
--rw-r--r--   0 odc       (1001) odc        (127)     2229 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-scalar.sql
--rw-r--r--   0 odc       (1001) odc        (127)     2687 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-view.sql
--rw-r--r--   0 odc       (1001) odc        (127)     4347 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgis/sql.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.621907 datacube-1.9.0rc3/datacube/drivers/postgres/
--rw-r--r--   0 odc       (1001) odc        (127)      400 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    49947 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_api.py
--rwxr-xr-x   0 odc       (1001) odc        (127)     9047 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_connections.py
--rw-r--r--   0 odc       (1001) odc        (127)     9843 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_core.py
--rw-r--r--   0 odc       (1001) odc        (127)     6424 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_dynamic.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    19328 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)     6687 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/_schema.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.621907 datacube-1.9.0rc3/datacube/drivers/postgres/samples/
--rw-r--r--   0 odc       (1001) odc        (127)     4029 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-explicit.sql
--rw-r--r--   0 odc       (1001) odc        (127)     2235 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-scalar.sql
--rw-r--r--   0 odc       (1001) odc        (127)     2692 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-view.sql
--rw-r--r--   0 odc       (1001) odc        (127)     4360 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/postgres/sql.py
--rw-r--r--   0 odc       (1001) odc        (127)     3533 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/readers.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.621907 datacube-1.9.0rc3/datacube/drivers/rio/
--rw-r--r--   0 odc       (1001) odc        (127)      206 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/rio/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     7093 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/rio/_reader.py
--rw-r--r--   0 odc       (1001) odc        (127)     1538 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/drivers/writers.py
--rw-r--r--   0 odc       (1001) odc        (127)     1597 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/helpers.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.625907 datacube-1.9.0rc3/datacube/index/
--rw-r--r--   0 odc       (1001) odc        (127)      597 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     1578 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/_api.py
--rw-r--r--   0 odc       (1001) odc        (127)   101252 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/abstract.py
--rw-r--r--   0 odc       (1001) odc        (127)    10618 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/default-metadata-types.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     8628 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/eo3.py
--rw-r--r--   0 odc       (1001) odc        (127)      500 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/exceptions.py
--rw-r--r--   0 odc       (1001) odc        (127)     2615 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/fields.py
--rw-r--r--   0 odc       (1001) odc        (127)    17590 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/hl.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.625907 datacube-1.9.0rc3/datacube/index/memory/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    38714 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (127)     1876 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)     5382 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (127)     8146 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/_products.py
--rw-r--r--   0 odc       (1001) odc        (127)     2462 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/_users.py
--rw-r--r--   0 odc       (1001) odc        (127)     3930 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/memory/index.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.625907 datacube-1.9.0rc3/datacube/index/null/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (127)     5898 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (127)     1085 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (127)     1299 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/_products.py
--rw-r--r--   0 odc       (1001) odc        (127)      802 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/_users.py
--rw-r--r--   0 odc       (1001) odc        (127)     3531 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/null/index.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.629907 datacube-1.9.0rc3/datacube/index/postgis/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    43517 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (127)     7358 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_lineage.py
--rw-r--r--   0 odc       (1001) odc        (127)     9832 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (127)    15174 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_products.py
--rw-r--r--   0 odc       (1001) odc        (127)     2411 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_transaction.py
--rw-r--r--   0 odc       (1001) odc        (127)     1779 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/_users.py
--rw-r--r--   0 odc       (1001) odc        (127)     2670 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/default-metadata-types.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     9511 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgis/index.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.629907 datacube-1.9.0rc3/datacube/index/postgres/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    42302 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (127)     1469 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_lineage.py
--rw-r--r--   0 odc       (1001) odc        (127)     9777 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (127)    14859 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_products.py
--rw-r--r--   0 odc       (1001) odc        (127)     2408 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_transaction.py
--rw-r--r--   0 odc       (1001) odc        (127)     1845 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/_users.py
--rw-r--r--   0 odc       (1001) odc        (127)     8022 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/index/postgres/index.py
--rw-r--r--   0 odc       (1001) odc        (127)      504 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/migration.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.629907 datacube-1.9.0rc3/datacube/model/
--rw-r--r--   0 odc       (1001) odc        (127)    42688 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)      628 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/_base.py
--rw-r--r--   0 odc       (1001) odc        (127)     3665 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/eo3.py
--rw-r--r--   0 odc       (1001) odc        (127)     6325 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/fields.py
--rw-r--r--   0 odc       (1001) odc        (127)    22567 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/lineage.py
--rw-r--r--   0 odc       (1001) odc        (127)     7132 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/model.py
--rw-r--r--   0 odc       (1001) odc        (127)    25514 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/properties.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.629907 datacube-1.9.0rc3/datacube/model/schema/
--rw-r--r--   0 odc       (1001) odc        (127)     5564 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/schema/dataset-type-schema.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2061 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/schema/metadata-type-schema.yaml
--rw-r--r--   0 odc       (1001) odc        (127)    14149 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/model/utils.py
--rw-r--r--   0 odc       (1001) odc        (127)        0 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/py.typed
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.633907 datacube-1.9.0rc3/datacube/scripts/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)      596 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/cli_app.py
--rw-r--r--   0 odc       (1001) odc        (127)    26833 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/dataset.py
--rw-r--r--   0 odc       (1001) odc        (127)     6010 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/metadata.py
--rw-r--r--   0 odc       (1001) odc        (127)     9017 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/product.py
--rwxr-xr-x   0 odc       (1001) odc        (127)     3736 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/search_tool.py
--rw-r--r--   0 odc       (1001) odc        (127)     6739 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/spindex.py
--rw-r--r--   0 odc       (1001) odc        (127)     4960 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/system.py
--rw-r--r--   0 odc       (1001) odc        (127)     3271 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/scripts/user.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.633907 datacube-1.9.0rc3/datacube/storage/
--rw-r--r--   0 odc       (1001) odc        (127)      594 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     3811 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/_base.py
--rw-r--r--   0 odc       (1001) odc        (127)      224 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/_hdf5.py
--rw-r--r--   0 odc       (1001) odc        (127)     6210 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/_load.py
--rw-r--r--   0 odc       (1001) odc        (127)     7833 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/_read.py
--rw-r--r--   0 odc       (1001) odc        (127)     7555 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/storage/_rio.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.633907 datacube-1.9.0rc3/datacube/testutils/
--rw-r--r--   0 odc       (1001) odc        (127)    14730 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/testutils/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     5273 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/testutils/geom.py
--rw-r--r--   0 odc       (1001) odc        (127)    11937 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/testutils/io.py
--rw-r--r--   0 odc       (1001) odc        (127)     2139 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/testutils/iodriver.py
--rw-r--r--   0 odc       (1001) odc        (127)      797 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/testutils/threads.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.633907 datacube-1.9.0rc3/datacube/ui/
--rw-r--r--   0 odc       (1001) odc        (127)      418 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/ui/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    11817 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/ui/click.py
--rw-r--r--   0 odc       (1001) odc        (127)     4012 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/ui/common.py
--rw-r--r--   0 odc       (1001) odc        (127)     4411 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/ui/expression.py
--rw-r--r--   0 odc       (1001) odc        (127)     8613 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/ui/task_app.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.637907 datacube-1.9.0rc3/datacube/utils/
--rw-r--r--   0 odc       (1001) odc        (127)     1808 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     1328 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/_misc.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.637907 datacube-1.9.0rc3/datacube/utils/aws/
--rw-r--r--   0 odc       (1001) odc        (127)    17300 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/aws/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     6581 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/changes.py
--rw-r--r--   0 odc       (1001) odc        (127)    14807 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/cog.py
--rw-r--r--   0 odc       (1001) odc        (127)    11374 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/dask.py
--rw-r--r--   0 odc       (1001) odc        (127)     3891 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/dates.py
--rw-r--r--   0 odc       (1001) odc        (127)    17351 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/documents.py
--rw-r--r--   0 odc       (1001) odc        (127)     2761 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/generic.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.637907 datacube-1.9.0rc3/datacube/utils/geometry/
--rw-r--r--   0 odc       (1001) odc        (127)     2834 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/geometry/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)    48240 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/geometry/_base.py
--rw-r--r--   0 odc       (1001) odc        (127)     5948 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/geometry/_warp.py
--rw-r--r--   0 odc       (1001) odc        (127)     7757 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/geometry/gbox.py
--rw-r--r--   0 odc       (1001) odc        (127)    18110 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/geometry/tools.py
--rw-r--r--   0 odc       (1001) odc        (127)     2293 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/io.py
--rw-r--r--   0 odc       (1001) odc        (127)     8989 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/masking.py
--rw-r--r--   0 odc       (1001) odc        (127)     5948 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/math.py
--rw-r--r--   0 odc       (1001) odc        (127)     2217 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/py.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.637907 datacube-1.9.0rc3/datacube/utils/rio/
--rw-r--r--   0 odc       (1001) odc        (127)      648 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/rio/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     5105 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/rio/_rio.py
--rw-r--r--   0 odc       (1001) odc        (127)     2336 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/serialise.py
--rw-r--r--   0 odc       (1001) odc        (127)     6894 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/uris.py
--rw-r--r--   0 odc       (1001) odc        (127)     2227 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/utils/xarray_geoextensions.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.641907 datacube-1.9.0rc3/datacube/virtual/
--rw-r--r--   0 odc       (1001) odc        (127)     7775 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     2368 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/catalog.py
--rw-r--r--   0 odc       (1001) odc        (127)     4888 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/expr.py
--rw-r--r--   0 odc       (1001) odc        (127)    41555 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/impl.py
--rw-r--r--   0 odc       (1001) odc        (127)    16795 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/transformations.py
--rw-r--r--   0 odc       (1001) odc        (127)     1634 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/datacube/virtual/utils.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.613907 datacube-1.9.0rc3/datacube.egg-info/
--rw-rw-r--   0 odc       (1001) odc        (127)     5886 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/PKG-INFO
--rw-rw-r--   0 odc       (1001) odc        (127)    14694 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/SOURCES.txt
--rw-rw-r--   0 odc       (1001) odc        (127)        1 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/dependency_links.txt
--rw-rw-r--   0 odc       (1001) odc        (127)      581 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/entry_points.txt
--rw-rw-r--   0 odc       (1001) odc        (127)     1784 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/requires.txt
--rw-rw-r--   0 odc       (1001) odc        (127)        9 2024-03-27 05:42:48.000000 datacube-1.9.0rc3/datacube.egg-info/top_level.txt
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.601906 datacube-1.9.0rc3/examples/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.641907 datacube-1.9.0rc3/examples/io_plugin/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.641907 datacube-1.9.0rc3/examples/io_plugin/dcio_example/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/examples/io_plugin/dcio_example/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     3855 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/examples/io_plugin/dcio_example/pickles.py
--rw-r--r--   0 odc       (1001) odc        (127)     5940 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/examples/io_plugin/dcio_example/xarray_3d.py
--rw-r--r--   0 odc       (1001) odc        (127)      607 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/examples/io_plugin/dcio_example/zeros.py
--rw-r--r--   0 odc       (1001) odc        (127)      747 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/examples/io_plugin/setup.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.645907 datacube-1.9.0rc3/integration_tests/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)      366 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/ancillary-collection.yaml
--rw-r--r--   0 odc       (1001) odc        (127)    39665 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/conftest.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.601906 datacube-1.9.0rc3/integration_tests/data/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.645907 datacube-1.9.0rc3/integration_tests/data/dataset_add/
--rw-r--r--   0 odc       (1001) odc        (127)     3112 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets.yml
--rw-r--r--   0 odc       (1001) odc        (127)     1624 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_bad1.yml
--rw-r--r--   0 odc       (1001) odc        (127)     1010 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_eo3.yml
--rw-r--r--   0 odc       (1001) odc        (127)     1026 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_eo3_updated.yml
--rw-r--r--   0 odc       (1001) odc        (127)      243 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_no_id.yml
--rw-r--r--   0 odc       (1001) odc        (127)        0 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/empty_file.yml
--rw-r--r--   0 odc       (1001) odc        (127)     1664 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/metadata.yml
--rw-r--r--   0 odc       (1001) odc        (127)      820 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/dataset_add/products.yml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.649907 datacube-1.9.0rc3/integration_tests/data/eo3/
--rw-r--r--   0 odc       (1001) odc        (127)     3527 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ard_ls8.odc-product.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     7591 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml
--rw-r--r--   0 odc       (1001) odc        (127)    11664 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/eo3_sentinel_ard.odc-type.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5301 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/final_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     1473 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     3977 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3.odc-product.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5095 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3_final.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5186 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3_interim.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     4793 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     4725 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset2.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5267 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset3.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5261 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset4.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     4793 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset_update.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     5110 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/nrt_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2823 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/s2_africa_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2210 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/s2_africa_product.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     3165 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/wo_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     8572 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     6562 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/data_utils.py
--rw-r--r--   0 odc       (1001) odc        (127)     8099 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/example-ls5-nbar.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2136 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/example-ls5-nbar_302.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2135 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/example-ls5-nbar_505.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2130 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/example-ls5-nbar_606.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     3084 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/extensive-eo-metadata.yaml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.649907 datacube-1.9.0rc3/integration_tests/index/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     1415 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/search_utils.py
--rw-r--r--   0 odc       (1001) odc        (127)    22067 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_config_docs.py
--rw-r--r--   0 odc       (1001) odc        (127)     1741 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_index_cloning.py
--rwxr-xr-x   0 odc       (1001) odc        (127)    24789 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_index_data.py
--rw-r--r--   0 odc       (1001) odc        (127)     7658 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_lineage.py
--rw-r--r--   0 odc       (1001) odc        (127)     2845 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_location.py
--rw-r--r--   0 odc       (1001) odc        (127)    33198 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_memory_index.py
--rw-r--r--   0 odc       (1001) odc        (127)     7729 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_null_index.py
--rw-r--r--   0 odc       (1001) odc        (127)      772 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_pluggable_indexes.py
--rw-r--r--   0 odc       (1001) odc        (127)    10218 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_postgis_index.py
--rw-r--r--   0 odc       (1001) odc        (127)    36049 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_search_eo3.py
--rw-r--r--   0 odc       (1001) odc        (127)    40125 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_search_legacy.py
--rw-r--r--   0 odc       (1001) odc        (127)     4234 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/index/test_update_columns.py
--rw-r--r--   0 odc       (1001) odc        (127)      270 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/integration.conf
--rw-r--r--   0 odc       (1001) odc        (127)    16847 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_3d.py
--rw-r--r--   0 odc       (1001) odc        (127)     9020 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_cli_output.py
--rw-r--r--   0 odc       (1001) odc        (127)     5181 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_cli_spatial_indexes.py
--rw-r--r--   0 odc       (1001) odc        (127)     9572 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_config_tool.py
--rw-r--r--   0 odc       (1001) odc        (127)    23332 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_dataset_add.py
--rw-r--r--   0 odc       (1001) odc        (127)     1427 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_environments.py
--rw-r--r--   0 odc       (1001) odc        (127)     7608 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_index_datasets_search.py
--rw-r--r--   0 odc       (1001) odc        (127)     1731 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/test_model.py
--rw-r--r--   0 odc       (1001) odc        (127)     6680 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/integration_tests/utils.py
--rw-r--r--   0 odc       (1001) odc        (127)      807 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/license-headers.md
--rw-r--r--   0 odc       (1001) odc        (127)      169 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/license-template.txt
--rw-r--r--   0 odc       (1001) odc        (127)       85 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/mypy.ini
--rw-r--r--   0 odc       (1001) odc        (127)     3011 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/odc_search_profile.py
--rw-r--r--   0 odc       (1001) odc        (127)     7160 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/pylintrc
--rw-r--r--   0 odc       (1001) odc        (127)      157 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/pyproject.toml
--rw-r--r--   0 odc       (1001) odc        (127)      161 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/pytest.ini
--rw-r--r--   0 odc       (1001) odc        (127)      235 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/setup.cfg
--rwxr-xr-x   0 odc       (1001) odc        (127)     4766 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/setup.py
--rw-r--r--   0 odc       (1001) odc        (127)      357 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/spellcheck.yaml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.653907 datacube-1.9.0rc3/tests/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/__init__.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.653907 datacube-1.9.0rc3/tests/api/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/api/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     4347 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/api/test_core.py
--rw-r--r--   0 odc       (1001) odc        (127)    13678 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/api/test_masking.py
--rw-r--r--   0 odc       (1001) odc        (127)     8780 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/api/test_query.py
--rw-r--r--   0 odc       (1001) odc        (127)    20421 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/api/test_virtual.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.653907 datacube-1.9.0rc3/tests/cfg/
--rw-r--r--   0 odc       (1001) odc        (127)      736 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/cfg/different_cfg.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      653 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/cfg/simple_cfg.ini
--rw-r--r--   0 odc       (1001) odc        (127)      704 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/cfg/simple_cfg.yaml
--rw-r--r--   0 odc       (1001) odc        (127)    10310 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/conftest.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.657907 datacube-1.9.0rc3/tests/data/
--rw-r--r--   0 odc       (1001) odc        (127)     8099 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ds_eo.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      520 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ds_eo3.yml
--rw-r--r--   0 odc       (1001) odc        (127)      432 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ds_non-geo.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     2516 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/eo3.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      471 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ingest_config.yaml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.605907 datacube-1.9.0rc3/tests/data/lbg/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.657907 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/
--rw-r--r--   0 odc       (1001) odc        (127)     2266 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml
--rw-r--r--   0 odc       (1001) odc        (127)    10819 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.661907 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif
--rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.661907 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/
--rw-r--r--   0 odc       (1001) odc        (127)     4590 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     9115 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.661907 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/
--rw-r--r--   0 odc       (1001) odc        (127)   369213 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.665907 datacube-1.9.0rc3/tests/data/lbg/gedi/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.665907 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/
--rw-r--r--   0 odc       (1001) odc        (127)    39410 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)   195417 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)    39448 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)   195809 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)     2756 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      762 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      756 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/
--rw-r--r--   0 odc       (1001) odc        (127)    46171 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)   327694 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)    46287 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)   328315 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (127)     2756 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      762 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml
--rw-r--r--   0 odc       (1001) odc        (127)      756 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml
--rw-r--r--   0 odc       (1001) odc        (127)     4513 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.605907 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.605907 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/
--rw-r--r--   0 odc       (1001) odc        (127)     1012 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt
--rw-r--r--   0 odc       (1001) odc        (127)     8513 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif
--rw-r--r--   0 odc       (1001) odc        (127)      619 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif
--rw-r--r--   0 odc       (1001) odc        (127)     2055 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt
--rw-r--r--   0 odc       (1001) odc        (127)    20914 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/multi_doc.nc
--rw-r--r--   0 odc       (1001) odc        (127)      201 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/multi_doc.yml
--rw-r--r--   0 odc       (1001) odc        (127)      104 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/multi_doc.yml.gz
--rw-r--r--   0 odc       (1001) odc        (127)     6126 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/no_crs_ds.tif
--rw-r--r--   0 odc       (1001) odc        (127)      109 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/sample.json
--rw-r--r--   0 odc       (1001) odc        (127)   174104 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/sample_tile.nc
--rw-r--r--   0 odc       (1001) odc        (127)    32366 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/sample_tile_151_-29.tif
--rw-r--r--   0 odc       (1001) odc        (127)       84 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/single_doc.yaml
--rw-r--r--   0 odc       (1001) odc        (127)   174104 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/test.nc
--rw-r--r--   0 odc       (1001) odc        (127)   255072 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/test.tif
--rw-r--r--   0 odc       (1001) odc        (127)      170 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/data/zeros_no_geo_int16_7x3.tif
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/drivers/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/drivers/fail_drivers/
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.669907 datacube-1.9.0rc3/tests/drivers/fail_drivers/dc_tests_io/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/drivers/fail_drivers/dc_tests_io/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)      282 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/drivers/fail_drivers/dc_tests_io/dummy.py
--rw-r--r--   0 odc       (1001) odc        (127)      689 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/drivers/fail_drivers/setup.py
--rw-r--r--   0 odc       (1001) odc        (127)      750 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/drivers/test_postgis_utils.py
--rw-r--r--   0 odc       (1001) odc        (127)     6659 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/drivers/test_rio_reader.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/tests/index/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     9639 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_api_index_dataset.py
--rw-r--r--   0 odc       (1001) odc        (127)     3982 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)     1525 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_hl_index.py
--rw-r--r--   0 odc       (1001) odc        (127)     1264 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_postgis_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)     1046 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_query.py
--rw-r--r--   0 odc       (1001) odc        (127)     3077 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/index/test_validate_dataset_type.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/tests/scripts/
--rw-r--r--   0 odc       (1001) odc        (127)      191 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/scripts/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     2078 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/scripts/test_search_tool.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/tests/storage/
--rw-r--r--   0 odc       (1001) odc        (127)     3531 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/storage/test_base.py
--rw-r--r--   0 odc       (1001) odc        (127)    14565 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/storage/test_netcdfwriter.py
--rw-r--r--   0 odc       (1001) odc        (127)    24057 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/storage/test_storage.py
--rw-r--r--   0 odc       (1001) odc        (127)     2346 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/storage/test_storage_load.py
--rw-r--r--   0 odc       (1001) odc        (127)    10391 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/storage/test_storage_read.py
--rw-r--r--   0 odc       (1001) odc        (127)     4353 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_3d.py
--rw-r--r--   0 odc       (1001) odc        (127)    16260 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_cfg.py
--rw-r--r--   0 odc       (1001) odc        (127)     3839 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_driver.py
--rw-r--r--   0 odc       (1001) odc        (127)     1038 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_dynamic_db_passwd.py
--rw-r--r--   0 odc       (1001) odc        (127)    10391 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_eo3.py
--rw-r--r--   0 odc       (1001) odc        (127)    24510 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_ext_lineage.py
--rw-r--r--   0 odc       (1001) odc        (127)    13768 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_load_data.py
--rw-r--r--   0 odc       (1001) odc        (127)     4966 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_metadata_fields.py
--rw-r--r--   0 odc       (1001) odc        (127)    13654 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_model.py
--rw-r--r--   0 odc       (1001) odc        (127)     3472 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_testutils.py
--rw-r--r--   0 odc       (1001) odc        (127)     9030 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_aws.py
--rw-r--r--   0 odc       (1001) odc        (127)     3150 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_changes.py
--rw-r--r--   0 odc       (1001) odc        (127)     6858 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_cog.py
--rw-r--r--   0 odc       (1001) odc        (127)     6045 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_dask.py
--rw-r--r--   0 odc       (1001) odc        (127)     2622 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_dates.py
--rw-r--r--   0 odc       (1001) odc        (127)    22436 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_docs.py
--rw-r--r--   0 odc       (1001) odc        (127)     1463 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_generic.py
--rw-r--r--   0 odc       (1001) odc        (127)    19591 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_other.py
--rw-r--r--   0 odc       (1001) odc        (127)     5752 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_utils_rio.py
--rw-r--r--   0 odc       (1001) odc        (127)     2170 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/test_xarray_extension.py
-drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-03-27 05:42:48.673907 datacube-1.9.0rc3/tests/ui/
--rw-r--r--   0 odc       (1001) odc        (127)      176 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/ui/__init__.py
--rw-r--r--   0 odc       (1001) odc        (127)     3621 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/ui/test_common.py
--rw-r--r--   0 odc       (1001) odc        (127)     5271 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/ui/test_expression_parsing.py
--rw-r--r--   0 odc       (1001) odc        (127)     5753 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/tests/ui/test_task_app.py
--rw-r--r--   0 odc       (1001) odc        (127)     3932 2024-03-27 05:33:37.000000 datacube-1.9.0rc3/wordlist.txt
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/
+-rw-r--r--   0 odc       (1001) odc        (127)      492 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.coveragerc
+-rw-r--r--   0 odc       (1001) odc        (127)      983 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.dockerignore
+-rw-r--r--   0 odc       (1001) odc        (127)     4474 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.doctor-rst.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      487 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.editorconfig
+-rw-r--r--   0 odc       (1001) odc        (127)      203 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.gitattributes
+-rw-r--r--   0 odc       (1001) odc        (127)     1072 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.gitignore
+-rw-r--r--   0 odc       (1001) odc        (127)      423 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.mergify.yml
+-rw-r--r--   0 odc       (1001) odc        (127)     1201 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      603 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.readthedocs.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      919 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/.yamllint
+-rw-r--r--   0 odc       (1001) odc        (127)     1928 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/CONTRIBUTING.md
+-rw-r--r--   0 odc       (1001) odc        (127)    11357 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/LICENSE
+-rw-r--r--   0 odc       (1001) odc        (127)       70 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/MANIFEST.in
+-rw-rw-r--   0 odc       (1001) odc        (127)     5886 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/PKG-INFO
+-rw-r--r--   0 odc       (1001) odc        (127)     4436 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/README.rst
+-rw-r--r--   0 odc       (1001) odc        (127)      942 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/alembic.ini
+-rwxr-xr-x   0 odc       (1001) odc        (127)      980 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/check-code.sh
+-rw-r--r--   0 odc       (1001) odc        (127)     3507 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/code-of-conduct.md
+-rw-r--r--   0 odc       (1001) odc        (127)      580 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/conda-environment.yml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.686363 datacube-1.9.0rc4/datacube/
+-rw-r--r--   0 odc       (1001) odc        (127)     1128 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/__init__.py
+-rw-rw-r--   0 odc       (1001) odc        (127)      163 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube/_version.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.690363 datacube-1.9.0rc4/datacube/api/
+-rw-r--r--   0 odc       (1001) odc        (127)      338 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/api/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    56462 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/api/core.py
+-rw-r--r--   0 odc       (1001) odc        (127)    15205 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/api/query.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.690363 datacube-1.9.0rc4/datacube/cfg/
+-rw-r--r--   0 odc       (1001) odc        (127)     1135 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    14315 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/api.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4993 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/cfg.py
+-rw-r--r--   0 odc       (1001) odc        (127)      325 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/exceptions.py
+-rw-r--r--   0 odc       (1001) odc        (127)    11265 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/opt.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1648 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/cfg/utils.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)      328 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/config.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.690363 datacube-1.9.0rc4/datacube/drivers/
+-rw-r--r--   0 odc       (1001) odc        (127)      587 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1065 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/_tools.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2946 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/_types.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1739 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/datasource.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1779 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/driver_cache.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1820 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/indexes.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.690363 datacube-1.9.0rc4/datacube/drivers/netcdf/
+-rw-r--r--   0 odc       (1001) odc        (127)      432 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/netcdf/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4864 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/netcdf/_write.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2182 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/netcdf/driver.py
+-rw-r--r--   0 odc       (1001) odc        (127)    11295 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/netcdf/writer.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.690363 datacube-1.9.0rc4/datacube/drivers/postgis/
+-rw-r--r--   0 odc       (1001) odc        (127)      396 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    55202 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_api.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    11290 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_connections.py
+-rw-r--r--   0 odc       (1001) odc        (127)    10504 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_core.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    20805 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)    14240 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_schema.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9786 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/_spatial.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/
+-rw-r--r--   0 odc       (1001) odc        (127)       65 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/README
+-rw-r--r--   0 odc       (1001) odc        (127)     4772 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/env.py
+-rw-r--r--   0 odc       (1001) odc        (127)      811 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/script.py.mako
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/versions/
+-rw-r--r--   0 odc       (1001) odc        (127)      673 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/alembic/versions/48fb71ece268_initial_revision.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/postgis/samples/
+-rw-r--r--   0 odc       (1001) odc        (127)     4023 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-explicit.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     2229 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-scalar.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     2687 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-view.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     4347 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgis/sql.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/postgres/
+-rw-r--r--   0 odc       (1001) odc        (127)      400 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    49947 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_api.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)     9047 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_connections.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9843 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_core.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6424 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_dynamic.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    19328 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6687 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/_schema.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/postgres/samples/
+-rw-r--r--   0 odc       (1001) odc        (127)     4029 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-explicit.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     2235 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-scalar.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     2692 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-view.sql
+-rw-r--r--   0 odc       (1001) odc        (127)     4360 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/postgres/sql.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3533 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/readers.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.694363 datacube-1.9.0rc4/datacube/drivers/rio/
+-rw-r--r--   0 odc       (1001) odc        (127)      206 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/rio/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7093 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/rio/_reader.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1538 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/drivers/writers.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1597 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/helpers.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.698363 datacube-1.9.0rc4/datacube/index/
+-rw-r--r--   0 odc       (1001) odc        (127)      597 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1578 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/_api.py
+-rw-r--r--   0 odc       (1001) odc        (127)   101252 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/abstract.py
+-rw-r--r--   0 odc       (1001) odc        (127)    10618 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/default-metadata-types.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     8628 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/eo3.py
+-rw-r--r--   0 odc       (1001) odc        (127)      500 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/exceptions.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2615 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)    17590 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/hl.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.698363 datacube-1.9.0rc4/datacube/index/memory/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    38714 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1876 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5382 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8146 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/_products.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2462 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/_users.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3930 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/memory/index.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.698363 datacube-1.9.0rc4/datacube/index/null/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)     5898 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1085 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1299 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/_products.py
+-rw-r--r--   0 odc       (1001) odc        (127)      802 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/_users.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3531 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/null/index.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.698363 datacube-1.9.0rc4/datacube/index/postgis/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    43517 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7358 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_lineage.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9832 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (127)    15174 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_products.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2411 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_transaction.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1779 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/_users.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2670 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/default-metadata-types.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     9511 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgis/index.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.702363 datacube-1.9.0rc4/datacube/index/postgres/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    42302 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1469 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_lineage.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9777 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (127)    14859 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_products.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2408 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_transaction.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1845 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/_users.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8022 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/index/postgres/index.py
+-rw-r--r--   0 odc       (1001) odc        (127)      504 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/migration.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.702363 datacube-1.9.0rc4/datacube/model/
+-rw-r--r--   0 odc       (1001) odc        (127)    42688 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)      628 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/_base.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3665 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/eo3.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6325 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)    22567 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/lineage.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7132 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/model.py
+-rw-r--r--   0 odc       (1001) odc        (127)    25514 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/properties.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.702363 datacube-1.9.0rc4/datacube/model/schema/
+-rw-r--r--   0 odc       (1001) odc        (127)     5564 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/schema/dataset-type-schema.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2061 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/schema/metadata-type-schema.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)    14149 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/model/utils.py
+-rw-r--r--   0 odc       (1001) odc        (127)        0 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/py.typed
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.706363 datacube-1.9.0rc4/datacube/scripts/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)      596 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/cli_app.py
+-rw-r--r--   0 odc       (1001) odc        (127)    26833 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/dataset.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6010 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/metadata.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9017 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/product.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)     3736 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/search_tool.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6739 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/spindex.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4960 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/system.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3271 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/scripts/user.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.706363 datacube-1.9.0rc4/datacube/storage/
+-rw-r--r--   0 odc       (1001) odc        (127)      594 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3811 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/_base.py
+-rw-r--r--   0 odc       (1001) odc        (127)      224 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/_hdf5.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6253 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/_load.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7833 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/_read.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7555 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/storage/_rio.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.706363 datacube-1.9.0rc4/datacube/testutils/
+-rw-r--r--   0 odc       (1001) odc        (127)    14730 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/testutils/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5273 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/testutils/geom.py
+-rw-r--r--   0 odc       (1001) odc        (127)    11937 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/testutils/io.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2139 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/testutils/iodriver.py
+-rw-r--r--   0 odc       (1001) odc        (127)      797 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/testutils/threads.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.706363 datacube-1.9.0rc4/datacube/ui/
+-rw-r--r--   0 odc       (1001) odc        (127)      418 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/ui/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    11817 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/ui/click.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4012 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/ui/common.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4411 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/ui/expression.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8613 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/ui/task_app.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.710363 datacube-1.9.0rc4/datacube/utils/
+-rw-r--r--   0 odc       (1001) odc        (127)     1808 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1328 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/_misc.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.710363 datacube-1.9.0rc4/datacube/utils/aws/
+-rw-r--r--   0 odc       (1001) odc        (127)    17300 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/aws/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6581 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/changes.py
+-rw-r--r--   0 odc       (1001) odc        (127)    14966 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/cog.py
+-rw-r--r--   0 odc       (1001) odc        (127)    11374 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/dask.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3891 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/dates.py
+-rw-r--r--   0 odc       (1001) odc        (127)    17351 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/documents.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2761 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/generic.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.710363 datacube-1.9.0rc4/datacube/utils/geometry/
+-rw-r--r--   0 odc       (1001) odc        (127)     2834 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/geometry/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)    48240 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/geometry/_base.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5948 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/geometry/_warp.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7757 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/geometry/gbox.py
+-rw-r--r--   0 odc       (1001) odc        (127)    18110 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/geometry/tools.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2293 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/io.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8989 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/masking.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5948 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/math.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2217 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/py.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.710363 datacube-1.9.0rc4/datacube/utils/rio/
+-rw-r--r--   0 odc       (1001) odc        (127)      648 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/rio/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5105 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/rio/_rio.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2336 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/serialise.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6894 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/uris.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2227 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/utils/xarray_geoextensions.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.710363 datacube-1.9.0rc4/datacube/virtual/
+-rw-r--r--   0 odc       (1001) odc        (127)     7775 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2368 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/catalog.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4888 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/expr.py
+-rw-r--r--   0 odc       (1001) odc        (127)    41555 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/impl.py
+-rw-r--r--   0 odc       (1001) odc        (127)    16795 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/transformations.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1634 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/datacube/virtual/utils.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.686363 datacube-1.9.0rc4/datacube.egg-info/
+-rw-rw-r--   0 odc       (1001) odc        (127)     5886 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/PKG-INFO
+-rw-rw-r--   0 odc       (1001) odc        (127)    14694 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/SOURCES.txt
+-rw-rw-r--   0 odc       (1001) odc        (127)        1 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/dependency_links.txt
+-rw-rw-r--   0 odc       (1001) odc        (127)      581 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/entry_points.txt
+-rw-rw-r--   0 odc       (1001) odc        (127)     1784 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/requires.txt
+-rw-rw-r--   0 odc       (1001) odc        (127)        9 2024-04-16 07:06:12.000000 datacube-1.9.0rc4/datacube.egg-info/top_level.txt
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.678363 datacube-1.9.0rc4/examples/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.714363 datacube-1.9.0rc4/examples/io_plugin/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.714363 datacube-1.9.0rc4/examples/io_plugin/dcio_example/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/examples/io_plugin/dcio_example/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3855 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/examples/io_plugin/dcio_example/pickles.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5940 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/examples/io_plugin/dcio_example/xarray_3d.py
+-rw-r--r--   0 odc       (1001) odc        (127)      607 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/examples/io_plugin/dcio_example/zeros.py
+-rw-r--r--   0 odc       (1001) odc        (127)      747 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/examples/io_plugin/setup.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.718363 datacube-1.9.0rc4/integration_tests/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)      366 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/ancillary-collection.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)    39665 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/conftest.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.678363 datacube-1.9.0rc4/integration_tests/data/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.718363 datacube-1.9.0rc4/integration_tests/data/dataset_add/
+-rw-r--r--   0 odc       (1001) odc        (127)     3112 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets.yml
+-rw-r--r--   0 odc       (1001) odc        (127)     1624 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_bad1.yml
+-rw-r--r--   0 odc       (1001) odc        (127)     1010 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_eo3.yml
+-rw-r--r--   0 odc       (1001) odc        (127)     1026 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_eo3_updated.yml
+-rw-r--r--   0 odc       (1001) odc        (127)      243 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_no_id.yml
+-rw-r--r--   0 odc       (1001) odc        (127)        0 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/empty_file.yml
+-rw-r--r--   0 odc       (1001) odc        (127)     1664 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/metadata.yml
+-rw-r--r--   0 odc       (1001) odc        (127)      820 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/dataset_add/products.yml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.722363 datacube-1.9.0rc4/integration_tests/data/eo3/
+-rw-r--r--   0 odc       (1001) odc        (127)     3527 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ard_ls8.odc-product.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     7591 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)    11664 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/eo3_sentinel_ard.odc-type.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5301 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/final_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     1473 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     3977 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3.odc-product.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5095 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3_final.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5186 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3_interim.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     4793 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     4725 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset2.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5267 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset3.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5261 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset4.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     4793 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset_update.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     5110 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/nrt_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2823 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/s2_africa_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2210 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/s2_africa_product.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     3165 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/wo_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     8572 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     6562 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/data_utils.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8099 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/example-ls5-nbar.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2136 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/example-ls5-nbar_302.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2135 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/example-ls5-nbar_505.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2130 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/example-ls5-nbar_606.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     3084 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/extensive-eo-metadata.yaml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.722363 datacube-1.9.0rc4/integration_tests/index/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1415 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/search_utils.py
+-rw-r--r--   0 odc       (1001) odc        (127)    22067 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_config_docs.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1741 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_index_cloning.py
+-rwxr-xr-x   0 odc       (1001) odc        (127)    24789 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_index_data.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7658 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_lineage.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2845 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_location.py
+-rw-r--r--   0 odc       (1001) odc        (127)    33198 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_memory_index.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7729 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_null_index.py
+-rw-r--r--   0 odc       (1001) odc        (127)      772 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_pluggable_indexes.py
+-rw-r--r--   0 odc       (1001) odc        (127)    10218 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_postgis_index.py
+-rw-r--r--   0 odc       (1001) odc        (127)    36049 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_search_eo3.py
+-rw-r--r--   0 odc       (1001) odc        (127)    40125 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_search_legacy.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4234 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/index/test_update_columns.py
+-rw-r--r--   0 odc       (1001) odc        (127)      270 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/integration.conf
+-rw-r--r--   0 odc       (1001) odc        (127)    16847 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_3d.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9020 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_cli_output.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5181 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_cli_spatial_indexes.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9572 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_config_tool.py
+-rw-r--r--   0 odc       (1001) odc        (127)    23332 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_dataset_add.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1427 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_environments.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7608 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_index_datasets_search.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1731 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/test_model.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6680 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/integration_tests/utils.py
+-rw-r--r--   0 odc       (1001) odc        (127)      807 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/license-headers.md
+-rw-r--r--   0 odc       (1001) odc        (127)      169 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/license-template.txt
+-rw-r--r--   0 odc       (1001) odc        (127)       85 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/mypy.ini
+-rw-r--r--   0 odc       (1001) odc        (127)     3011 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/odc_search_profile.py
+-rw-r--r--   0 odc       (1001) odc        (127)     7160 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/pylintrc
+-rw-r--r--   0 odc       (1001) odc        (127)      157 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/pyproject.toml
+-rw-r--r--   0 odc       (1001) odc        (127)      161 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/pytest.ini
+-rw-r--r--   0 odc       (1001) odc        (127)      235 2024-04-16 07:06:12.750363 datacube-1.9.0rc4/setup.cfg
+-rwxr-xr-x   0 odc       (1001) odc        (127)     4766 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/setup.py
+-rw-r--r--   0 odc       (1001) odc        (127)      357 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/spellcheck.yaml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.726363 datacube-1.9.0rc4/tests/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/__init__.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.730363 datacube-1.9.0rc4/tests/api/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/api/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5241 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/api/test_core.py
+-rw-r--r--   0 odc       (1001) odc        (127)    13678 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/api/test_masking.py
+-rw-r--r--   0 odc       (1001) odc        (127)     8780 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/api/test_query.py
+-rw-r--r--   0 odc       (1001) odc        (127)    20421 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/api/test_virtual.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.730363 datacube-1.9.0rc4/tests/cfg/
+-rw-r--r--   0 odc       (1001) odc        (127)      736 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/cfg/different_cfg.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      653 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/cfg/simple_cfg.ini
+-rw-r--r--   0 odc       (1001) odc        (127)      704 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/cfg/simple_cfg.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)    10310 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/conftest.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.734363 datacube-1.9.0rc4/tests/data/
+-rw-r--r--   0 odc       (1001) odc        (127)     8099 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ds_eo.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      520 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ds_eo3.yml
+-rw-r--r--   0 odc       (1001) odc        (127)      432 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ds_non-geo.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     2516 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/eo3.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      471 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ingest_config.yaml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.682363 datacube-1.9.0rc4/tests/data/lbg/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.734363 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/
+-rw-r--r--   0 odc       (1001) odc        (127)     2266 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)    10819 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.738363 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif
+-rw-r--r--   0 odc       (1001) odc        (127)   369231 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.738363 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/
+-rw-r--r--   0 odc       (1001) odc        (127)     4590 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     9115 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.738363 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/
+-rw-r--r--   0 odc       (1001) odc        (127)   369213 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.738363 datacube-1.9.0rc4/tests/data/lbg/gedi/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.738363 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/
+-rw-r--r--   0 odc       (1001) odc        (127)    39410 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)   195417 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)    39448 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)   195809 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)     2756 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      762 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      756 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.742363 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/
+-rw-r--r--   0 odc       (1001) odc        (127)    46171 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)   327694 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)    46287 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)   328315 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (127)     2756 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      762 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)      756 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)     4513 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.682363 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.682363 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.742363 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/
+-rw-r--r--   0 odc       (1001) odc        (127)     1012 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt
+-rw-r--r--   0 odc       (1001) odc        (127)     8513 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.742363 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      619 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif
+-rw-r--r--   0 odc       (1001) odc        (127)     2055 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt
+-rw-r--r--   0 odc       (1001) odc        (127)    20914 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/multi_doc.nc
+-rw-r--r--   0 odc       (1001) odc        (127)      201 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/multi_doc.yml
+-rw-r--r--   0 odc       (1001) odc        (127)      104 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/multi_doc.yml.gz
+-rw-r--r--   0 odc       (1001) odc        (127)     6126 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/no_crs_ds.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      109 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/sample.json
+-rw-r--r--   0 odc       (1001) odc        (127)   174104 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/sample_tile.nc
+-rw-r--r--   0 odc       (1001) odc        (127)    32366 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/sample_tile_151_-29.tif
+-rw-r--r--   0 odc       (1001) odc        (127)       84 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/single_doc.yaml
+-rw-r--r--   0 odc       (1001) odc        (127)   174104 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/test.nc
+-rw-r--r--   0 odc       (1001) odc        (127)   255072 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/test.tif
+-rw-r--r--   0 odc       (1001) odc        (127)      170 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/data/zeros_no_geo_int16_7x3.tif
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/drivers/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/drivers/fail_drivers/
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/drivers/fail_drivers/dc_tests_io/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/drivers/fail_drivers/dc_tests_io/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)      282 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/drivers/fail_drivers/dc_tests_io/dummy.py
+-rw-r--r--   0 odc       (1001) odc        (127)      689 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/drivers/fail_drivers/setup.py
+-rw-r--r--   0 odc       (1001) odc        (127)      750 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/drivers/test_postgis_utils.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6659 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/drivers/test_rio_reader.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/index/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9639 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_api_index_dataset.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3982 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1525 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_hl_index.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1264 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_postgis_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1046 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_query.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3077 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/index/test_validate_dataset_type.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/scripts/
+-rw-r--r--   0 odc       (1001) odc        (127)      191 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/scripts/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2078 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/scripts/test_search_tool.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/storage/
+-rw-r--r--   0 odc       (1001) odc        (127)     3531 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/storage/test_base.py
+-rw-r--r--   0 odc       (1001) odc        (127)    14565 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/storage/test_netcdfwriter.py
+-rw-r--r--   0 odc       (1001) odc        (127)    24057 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/storage/test_storage.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2346 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/storage/test_storage_load.py
+-rw-r--r--   0 odc       (1001) odc        (127)    10834 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/storage/test_storage_read.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4353 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_3d.py
+-rw-r--r--   0 odc       (1001) odc        (127)    16571 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_cfg.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3839 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_driver.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1038 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_dynamic_db_passwd.py
+-rw-r--r--   0 odc       (1001) odc        (127)    10391 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_eo3.py
+-rw-r--r--   0 odc       (1001) odc        (127)    24510 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_ext_lineage.py
+-rw-r--r--   0 odc       (1001) odc        (127)    13768 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_load_data.py
+-rw-r--r--   0 odc       (1001) odc        (127)     4966 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_metadata_fields.py
+-rw-r--r--   0 odc       (1001) odc        (127)    13654 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_model.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3472 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_testutils.py
+-rw-r--r--   0 odc       (1001) odc        (127)     9030 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_aws.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3150 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_changes.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6858 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_cog.py
+-rw-r--r--   0 odc       (1001) odc        (127)     6045 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_dask.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2622 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_dates.py
+-rw-r--r--   0 odc       (1001) odc        (127)    22436 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_docs.py
+-rw-r--r--   0 odc       (1001) odc        (127)     1463 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_generic.py
+-rw-r--r--   0 odc       (1001) odc        (127)    19591 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_other.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5752 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_utils_rio.py
+-rw-r--r--   0 odc       (1001) odc        (127)     2170 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/test_xarray_extension.py
+drwxrwxr-x   0 odc       (1001) odc        (127)        0 2024-04-16 07:06:12.746363 datacube-1.9.0rc4/tests/ui/
+-rw-r--r--   0 odc       (1001) odc        (127)      176 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/ui/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3621 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/ui/test_common.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5271 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/ui/test_expression_parsing.py
+-rw-r--r--   0 odc       (1001) odc        (127)     5753 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/tests/ui/test_task_app.py
+-rw-r--r--   0 odc       (1001) odc        (127)     3932 2024-04-16 06:57:24.000000 datacube-1.9.0rc4/wordlist.txt
```

### Comparing `datacube-1.9.0rc3/.dockerignore` & `datacube-1.9.0rc4/.dockerignore`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/.doctor-rst.yaml` & `datacube-1.9.0rc4/.doctor-rst.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/.gitignore` & `datacube-1.9.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/.pre-commit-config.yaml` & `datacube-1.9.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/.readthedocs.yaml` & `datacube-1.9.0rc4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/.yamllint` & `datacube-1.9.0rc4/.yamllint`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/CONTRIBUTING.md` & `datacube-1.9.0rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/LICENSE` & `datacube-1.9.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/PKG-INFO` & `datacube-1.9.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacube
-Version: 1.9.0rc3
+Version: 1.9.0rc4
 Summary: An analysis environment for satellite and other earth observation data
 Home-page: https://github.com/opendatacube/datacube-core
 Author: Open Data Cube
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
 Platform: UNKNOWN
```

### Comparing `datacube-1.9.0rc3/README.rst` & `datacube-1.9.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/alembic.ini` & `datacube-1.9.0rc4/alembic.ini`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/check-code.sh` & `datacube-1.9.0rc4/check-code.sh`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/code-of-conduct.md` & `datacube-1.9.0rc4/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/conda-environment.yml` & `datacube-1.9.0rc4/conda-environment.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/__init__.py` & `datacube-1.9.0rc4/datacube/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/api/core.py` & `datacube-1.9.0rc4/datacube/api/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import xarray
 from dask import array as da
 
 from datacube.cfg import GeneralisedRawCfg, GeneralisedCfg, GeneralisedEnv, ODCConfig
 from datacube.storage import reproject_and_fuse, BandInfo
 from datacube.utils import ignore_exceptions_if
 from odc.geo import CRS, yx_, res_, resyx_, Resolution, XY
+from odc.geo.warp import Resampling
 from odc.geo.xr import xr_coords
 from datacube.utils.dates import normalise_dt
 from odc.geo.geom import intersects, box, bbox_union, Geometry
 from odc.geo.geobox import GeoBox, GeoboxTiles
 from datacube.model import ExtraDimensions, ExtraDimensionSlices, Dataset, Measurement, GridSpec
 from datacube.model.utils import xr_apply
 
@@ -240,15 +241,15 @@
 
     #: pylint: disable=too-many-arguments, too-many-locals
     def load(self,
              product: str | None = None,
              measurements: str | list[str] | None = None,
              output_crs: Any = None,
              resolution: int | float | tuple[int | float, int | float] | Resolution | None = None,
-             resampling: str | dict[str, str] | None = None,
+             resampling: Resampling | dict[str, Resampling] | None = None,
              align: XY[float] | Iterable[float] | None = None,
              skip_broken_datasets: bool = False,
              dask_chunks: dict[str, str | int] | None = None,
              like: GeoBox | xarray.Dataset | xarray.DataArray | None = None,
              fuse_func: FuserFunction | Mapping[str, FuserFunction | None] | None = None,
              datasets: Sequence[Dataset] | None = None,
              dataset_predicate: Callable[[Dataset], bool] | None = None,
@@ -874,15 +875,15 @@
                 return data
 
         return data
 
     @staticmethod
     def load_data(sources: xarray.DataArray, geobox: GeoBox,
                   measurements: Mapping[str, Measurement] | list[Measurement],
-                  resampling: str | dict[str, str] | None = None,
+                  resampling: Resampling | dict[str, Resampling] | None = None,
                   fuse_func: FuserFunction | Mapping[str, FuserFunction | None] | None = None,
                   dask_chunks: dict[str, str | int] | None = None,
                   skip_broken_datasets: bool = False,
                   progress_cbk: ProgressFunction | None = None,
                   extra_dims: ExtraDimensions | None = None,
                   patch_url: Callable[[str], str] | None = None,
                   **extra) -> xarray.Dataset:
@@ -965,28 +966,28 @@
         return self
 
     def __exit__(self, type_, value, traceback):
         self.close()
 
 
 def per_band_load_data_settings(measurements: list[Measurement] | Mapping[str, Measurement],
-                                resampling: str | Mapping[str, str] | None = None,
+                                resampling: Resampling | Mapping[str, Resampling] | None = None,
                                 fuse_func: FuserFunction | Mapping[str, FuserFunction | None] | None = None
                                 ) -> list[Measurement]:
     def with_resampling(m, resampling, default=None):
         m = m.copy()
         m['resampling_method'] = resampling.get(m.name, default)
         return m
 
     def with_fuser(m, fuser, default=None):
         m = m.copy()
         m['fuser'] = fuser.get(m.name, default)
         return m
 
-    if isinstance(resampling, str):
+    if resampling is not None and not isinstance(resampling, dict):
         resampling = {'*': resampling}
 
     if fuse_func is None or callable(fuse_func):
         fuse_func = {'*': fuse_func}
 
     if isinstance(measurements, dict):
         measurements = list(measurements.values())
@@ -1014,16 +1015,20 @@
     """ Configure output geobox from user provided output specs. """
 
     if like is not None:
         assert output_crs is None, "'like' and 'output_crs' are not supported together"
         assert resolution is None, "'like' and 'resolution' are not supported together"
         assert align is None, "'like' and 'align' are not supported together"
         if isinstance(like, GeoBox):
+            # Is already a GeoBox
             return like
-
+        if like.__class__.__name__ == "GeoBox" and like.__class__.__module__ == 'datacube.utils.geometry._base':
+            # Is a legacy GeoBox: convert to odc.geo.geobox.GeoBox (check class without importing deprecated class)
+            return GeoBox(shape=(like.height, like.width), affine=like.affine, crs=like.crs)
+        # Is an Xarray object
         return like.odc.geobox
 
     if load_hints:
         if output_crs is None:
             output_crs = load_hints.get('output_crs', None)
 
         if resolution is None:
```

### Comparing `datacube-1.9.0rc3/datacube/api/query.py` & `datacube-1.9.0rc4/datacube/api/query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/cfg/__init__.py` & `datacube-1.9.0rc4/datacube/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/cfg/api.py` & `datacube-1.9.0rc4/datacube/cfg/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,17 @@
             elif "default" in self.known_environments:
                 item = "default"
             elif "datacube" in self.known_environments:
                 warnings.warn("Defaulting to the 'datacube' environment - "
                               "this fallback behaviour is deprecated and may change in a future release.")
                 item = "datacube"
             else:
-                raise ConfigException("No environment specified and no default environment could be identified.")
+                # No explicitly defined (known) environments - assume default and hope there's config
+                # available in environment variables.
+                item = "default"
         if item not in self.known_environments:
             self.known_environments[item] = ODCEnvironment(self, item, {}, True)
         return self.known_environments[item]
 
 
 class ODCEnvironment:
     """
```

### Comparing `datacube-1.9.0rc3/datacube/cfg/cfg.py` & `datacube-1.9.0rc4/datacube/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/cfg/opt.py` & `datacube-1.9.0rc4/datacube/cfg/opt.py`

 * *Files 14% similar despite different names*

```diff
@@ -203,26 +203,58 @@
         if components.scheme != "postgresql":
             raise ConfigException("Database URL is not a postgresql connection URL")
         # Don't bother splitting up the url, we'd just have to put it back together again later
         return value
 
     def handle_dependent_options(self, value: Any) -> None:
         if value is None:
-            for handler in (
-                    ODCOptionHandler("db_username", self.env, legacy_env_aliases=['DB_USERNAME'],
-                                     default=_DEFAULT_DB_USER),
-                    ODCOptionHandler("db_password", self.env, legacy_env_aliases=['DB_PASSWORD']),
-                    ODCOptionHandler("db_hostname", self.env, legacy_env_aliases=['DB_HOSTNAME'],
-                                     default=_DEFAULT_HOSTNAME),
-                    IntOptionHandler("db_port", self.env, default=5432, legacy_env_aliases=['DB_PORT'],
-                                     minval=1, maxval=49151),
-                    ODCOptionHandler("db_database", self.env, legacy_env_aliases=['DB_DATABASE'],
-                                     default=_DEFAULT_DATABASE),
-            ):
-                self.env._option_handlers.append(handler)
+            handlers: tuple[ODCOptionHandler, ...] = (
+                ODCOptionHandler("db_username", self.env, legacy_env_aliases=['DB_USERNAME'],
+                                 default=_DEFAULT_DB_USER),
+                ODCOptionHandler("db_password", self.env, legacy_env_aliases=['DB_PASSWORD']),
+                ODCOptionHandler("db_hostname", self.env, legacy_env_aliases=['DB_HOSTNAME'],
+                                 default=_DEFAULT_HOSTNAME),
+                IntOptionHandler("db_port", self.env, default=5432, legacy_env_aliases=['DB_PORT'],
+                                 minval=1, maxval=49151),
+                ODCOptionHandler("db_database", self.env, legacy_env_aliases=['DB_DATABASE'],
+                                 default=_DEFAULT_DATABASE),
+            )
+        else:
+            # These pseudo-handlers extract the equivalent config from the url returned by this handler.
+            handlers = (
+                PostgresURLPartHandler(self, "username", "db_username", self.env),
+                PostgresURLPartHandler(self, "password", "db_password", self.env),
+                PostgresURLPartHandler(self, "hostname", "db_hostname", self.env),
+                PostgresURLPartHandler(self, "port", "db_port", self.env),
+                PostgresURLPartHandler(self, "path", "db_database", self.env),
+            )
+
+        for handler in handlers:
+            self.env._option_handlers.append(handler)
+
+
+class PostgresURLPartHandler(ODCOptionHandler):
+    def __init__(self, urlhandler: PostgresURLOptionHandler, urlpart: str, name: str, env: "ODCEnvironment"):
+        self.urlhandler = urlhandler
+        self.urlpart = urlpart
+        super().__init__(name, env)
+
+    def validate_and_normalise(self, value: Any) -> Any:
+        url = self.env._normalised[self.urlhandler.name]
+        purl = urlparse(url)
+        part = getattr(purl, self.urlpart)
+        if self.urlpart == "path" and part.startswith('/'):
+            # Remove leading slash
+            return str(part)[1:]
+        else:
+            return part
+
+    def get_val_from_environment(self) -> str | None:
+        # Never read from environment - take from URL, wherever it came from
+        return None
 
 
 def config_options_for_psql_driver(env: "ODCEnvironment"):
     """
        Config options for shared use by postgres-based index drivers
        (i.e. postgres and postgis drivers)
     """
```

### Comparing `datacube-1.9.0rc3/datacube/cfg/utils.py` & `datacube-1.9.0rc4/datacube/cfg/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/__init__.py` & `datacube-1.9.0rc4/datacube/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/_tools.py` & `datacube-1.9.0rc4/datacube/drivers/_tools.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/_types.py` & `datacube-1.9.0rc4/datacube/drivers/_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/datasource.py` & `datacube-1.9.0rc4/datacube/drivers/datasource.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/driver_cache.py` & `datacube-1.9.0rc4/datacube/drivers/driver_cache.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/indexes.py` & `datacube-1.9.0rc4/datacube/drivers/indexes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/netcdf/_write.py` & `datacube-1.9.0rc4/datacube/drivers/netcdf/_write.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/netcdf/driver.py` & `datacube-1.9.0rc4/datacube/drivers/netcdf/driver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/netcdf/writer.py` & `datacube-1.9.0rc4/datacube/drivers/netcdf/writer.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_api.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_connections.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_connections.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_core.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_core.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_fields.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_schema.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_schema.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/_spatial.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/_spatial.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/alembic/env.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/alembic/env.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/alembic/script.py.mako` & `datacube-1.9.0rc4/datacube/drivers/postgis/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/alembic/versions/48fb71ece268_initial_revision.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/alembic/versions/48fb71ece268_initial_revision.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-explicit.sql` & `datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-explicit.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-scalar.sql` & `datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-scalar.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/samples/range-tests-view.sql` & `datacube-1.9.0rc4/datacube/drivers/postgis/samples/range-tests-view.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgis/sql.py` & `datacube-1.9.0rc4/datacube/drivers/postgis/sql.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_api.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_connections.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_connections.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_core.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_core.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_dynamic.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_dynamic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_fields.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/_schema.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/_schema.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-explicit.sql` & `datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-explicit.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-scalar.sql` & `datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-scalar.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/samples/range-tests-view.sql` & `datacube-1.9.0rc4/datacube/drivers/postgres/samples/range-tests-view.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/postgres/sql.py` & `datacube-1.9.0rc4/datacube/drivers/postgres/sql.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/readers.py` & `datacube-1.9.0rc4/datacube/drivers/readers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/rio/_reader.py` & `datacube-1.9.0rc4/datacube/drivers/rio/_reader.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/drivers/writers.py` & `datacube-1.9.0rc4/datacube/drivers/writers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/helpers.py` & `datacube-1.9.0rc4/datacube/helpers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/__init__.py` & `datacube-1.9.0rc4/datacube/index/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/_api.py` & `datacube-1.9.0rc4/datacube/index/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/abstract.py` & `datacube-1.9.0rc4/datacube/index/abstract.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/default-metadata-types.yaml` & `datacube-1.9.0rc4/datacube/index/default-metadata-types.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/eo3.py` & `datacube-1.9.0rc4/datacube/index/eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/fields.py` & `datacube-1.9.0rc4/datacube/index/fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/hl.py` & `datacube-1.9.0rc4/datacube/index/hl.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/_datasets.py` & `datacube-1.9.0rc4/datacube/index/memory/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/_fields.py` & `datacube-1.9.0rc4/datacube/index/memory/_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/_metadata_types.py` & `datacube-1.9.0rc4/datacube/index/memory/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/_products.py` & `datacube-1.9.0rc4/datacube/index/memory/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/_users.py` & `datacube-1.9.0rc4/datacube/index/memory/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/memory/index.py` & `datacube-1.9.0rc4/datacube/index/memory/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/null/_datasets.py` & `datacube-1.9.0rc4/datacube/index/null/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/null/_metadata_types.py` & `datacube-1.9.0rc4/datacube/index/null/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/null/_products.py` & `datacube-1.9.0rc4/datacube/index/null/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/null/_users.py` & `datacube-1.9.0rc4/datacube/index/null/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/null/index.py` & `datacube-1.9.0rc4/datacube/index/null/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_datasets.py` & `datacube-1.9.0rc4/datacube/index/postgis/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_lineage.py` & `datacube-1.9.0rc4/datacube/index/postgis/_lineage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_metadata_types.py` & `datacube-1.9.0rc4/datacube/index/postgis/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_products.py` & `datacube-1.9.0rc4/datacube/index/postgis/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_transaction.py` & `datacube-1.9.0rc4/datacube/index/postgis/_transaction.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/_users.py` & `datacube-1.9.0rc4/datacube/index/postgis/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/default-metadata-types.yaml` & `datacube-1.9.0rc4/datacube/index/postgis/default-metadata-types.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgis/index.py` & `datacube-1.9.0rc4/datacube/index/postgis/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_datasets.py` & `datacube-1.9.0rc4/datacube/index/postgres/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_lineage.py` & `datacube-1.9.0rc4/datacube/index/postgres/_lineage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_metadata_types.py` & `datacube-1.9.0rc4/datacube/index/postgres/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_products.py` & `datacube-1.9.0rc4/datacube/index/postgres/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_transaction.py` & `datacube-1.9.0rc4/datacube/index/postgres/_transaction.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/_users.py` & `datacube-1.9.0rc4/datacube/index/postgres/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/index/postgres/index.py` & `datacube-1.9.0rc4/datacube/index/postgres/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/__init__.py` & `datacube-1.9.0rc4/datacube/model/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/_base.py` & `datacube-1.9.0rc4/datacube/model/_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/eo3.py` & `datacube-1.9.0rc4/datacube/model/eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/fields.py` & `datacube-1.9.0rc4/datacube/model/fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/lineage.py` & `datacube-1.9.0rc4/datacube/model/lineage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/model.py` & `datacube-1.9.0rc4/datacube/model/model.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/properties.py` & `datacube-1.9.0rc4/datacube/model/properties.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/schema/dataset-type-schema.yaml` & `datacube-1.9.0rc4/datacube/model/schema/dataset-type-schema.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/schema/metadata-type-schema.yaml` & `datacube-1.9.0rc4/datacube/model/schema/metadata-type-schema.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/model/utils.py` & `datacube-1.9.0rc4/datacube/model/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/cli_app.py` & `datacube-1.9.0rc4/datacube/scripts/cli_app.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/dataset.py` & `datacube-1.9.0rc4/datacube/scripts/dataset.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/metadata.py` & `datacube-1.9.0rc4/datacube/scripts/metadata.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/product.py` & `datacube-1.9.0rc4/datacube/scripts/product.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/search_tool.py` & `datacube-1.9.0rc4/datacube/scripts/search_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/spindex.py` & `datacube-1.9.0rc4/datacube/scripts/spindex.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/system.py` & `datacube-1.9.0rc4/datacube/scripts/system.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/scripts/user.py` & `datacube-1.9.0rc4/datacube/scripts/user.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/storage/__init__.py` & `datacube-1.9.0rc4/datacube/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/storage/_base.py` & `datacube-1.9.0rc4/datacube/storage/_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/storage/_load.py` & `datacube-1.9.0rc4/datacube/storage/_load.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 
 from datacube.utils import ignore_exceptions_if
 from datacube.utils.math import invalid_mask
 from odc.geo.geobox import GeoBox
 from odc.geo.roi import roi_is_empty
 from odc.geo.xr import xr_coords
+from odc.geo.warp import Resampling
 from datacube.model import Measurement
 from datacube.drivers._types import ReaderDriver
 from ..drivers.datasource import DataSource
 from ._base import BandInfo
 
 _LOG = logging.getLogger(__name__)
 
@@ -43,15 +44,15 @@
     np.copyto(dst, src, where=invalid_mask(dst, dst_nodata))
 
 
 def reproject_and_fuse(datasources: List[DataSource],
                        destination: np.ndarray,
                        dst_geobox: GeoBox,
                        dst_nodata: Optional[Union[int, float]],
-                       resampling: str = 'nearest',
+                       resampling: Resampling = 'nearest',
                        fuse_func: Optional[FuserFunction] = None,
                        skip_broken_datasets: bool = False,
                        progress_cbk: Optional[ProgressFunction] = None,
                        extra_dim_index: Optional[int] = None):
     """
     Reproject and fuse `sources` into a 2D numpy array `destination`.
```

### Comparing `datacube-1.9.0rc3/datacube/storage/_read.py` & `datacube-1.9.0rc4/datacube/storage/_read.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/storage/_rio.py` & `datacube-1.9.0rc4/datacube/storage/_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/testutils/__init__.py` & `datacube-1.9.0rc4/datacube/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/testutils/geom.py` & `datacube-1.9.0rc4/datacube/testutils/geom.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/testutils/io.py` & `datacube-1.9.0rc4/datacube/testutils/io.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/testutils/iodriver.py` & `datacube-1.9.0rc4/datacube/testutils/iodriver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/testutils/threads.py` & `datacube-1.9.0rc4/datacube/testutils/threads.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/ui/click.py` & `datacube-1.9.0rc4/datacube/ui/click.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/ui/common.py` & `datacube-1.9.0rc4/datacube/ui/common.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/ui/expression.py` & `datacube-1.9.0rc4/datacube/ui/expression.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/ui/task_app.py` & `datacube-1.9.0rc4/datacube/ui/task_app.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/__init__.py` & `datacube-1.9.0rc4/datacube/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/_misc.py` & `datacube-1.9.0rc4/datacube/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/aws/__init__.py` & `datacube-1.9.0rc4/datacube/utils/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/changes.py` & `datacube-1.9.0rc4/datacube/utils/changes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/cog.py` & `datacube-1.9.0rc4/datacube/utils/cog.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Union, Optional, List, Any, Dict
 
 from datacube.migration import ODC2DeprecationWarning
 
 from .io import check_write_path
 from odc.geo.geobox import GeoBox
 from odc.geo.math import align_up
+from odc.geo.warp import Resampling, resampling_s2rio
 
 from deprecat import deprecat
 
 __all__ = ("write_cog", "to_cog")
 
 
 def _adjust_blocksize(block, dim):
@@ -34,15 +35,15 @@
 def _write_cog(
     pix: np.ndarray,
     geobox: GeoBox,
     fname: Union[Path, str],
     nodata: Optional[float] = None,
     overwrite: bool = False,
     blocksize: Optional[int] = None,
-    overview_resampling: Optional[str] = None,
+    overview_resampling: Optional[Resampling] = None,
     overview_levels: Optional[List[int]] = None,
     ovr_blocksize: Optional[int] = None,
     use_windowed_writes: bool = False,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
     **extra_rio_opts
 ) -> Union[Path, bytes]:
     """Write geo-registered ndarray to a GeoTiff file or RAM.
@@ -114,15 +115,18 @@
             overview_levels = [2 ** i for i in range(1, 6)]
 
     if fname != ":mem:":
         path = check_write_path(
             fname, overwrite
         )  # aborts if overwrite=False and file exists already
 
-    resampling = rasterio.enums.Resampling[overview_resampling]
+    if isinstance(overview_resampling, str):
+        resampling = resampling_s2rio(overview_resampling)
+    else:
+        resampling = overview_resampling
 
     if (blocksize % 16) != 0:
         warnings.warn("Block size must be a multiple of 16, will be adjusted")
 
     rio_opts = dict(
         width=w,
         height=h,
@@ -215,15 +219,15 @@
 @deprecat(reason='This method has been moved to odc-geo.', version='1.9.0', category=ODC2DeprecationWarning)
 def write_cog(
     geo_im: xr.DataArray,
     fname: Union[str, Path],
     overwrite: bool = False,
     blocksize: Optional[int] = None,
     ovr_blocksize: Optional[int] = None,
-    overview_resampling: Optional[str] = None,
+    overview_resampling: Optional[Resampling] = None,
     overview_levels: Optional[List[int]] = None,
     use_windowed_writes: bool = False,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
     **extra_rio_opts
 ) -> Union[Path, bytes, Delayed]:
     """
     Save ``xarray.DataArray`` to a file in Cloud Optimized GeoTiff format.
```

### Comparing `datacube-1.9.0rc3/datacube/utils/dask.py` & `datacube-1.9.0rc4/datacube/utils/dask.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/dates.py` & `datacube-1.9.0rc4/datacube/utils/dates.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/documents.py` & `datacube-1.9.0rc4/datacube/utils/documents.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/generic.py` & `datacube-1.9.0rc4/datacube/utils/generic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/geometry/__init__.py` & `datacube-1.9.0rc4/datacube/utils/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/geometry/_base.py` & `datacube-1.9.0rc4/datacube/utils/geometry/_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/geometry/_warp.py` & `datacube-1.9.0rc4/datacube/utils/geometry/_warp.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/geometry/gbox.py` & `datacube-1.9.0rc4/datacube/utils/geometry/gbox.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/geometry/tools.py` & `datacube-1.9.0rc4/datacube/utils/geometry/tools.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/io.py` & `datacube-1.9.0rc4/datacube/utils/io.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/masking.py` & `datacube-1.9.0rc4/datacube/utils/masking.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/math.py` & `datacube-1.9.0rc4/datacube/utils/math.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/py.py` & `datacube-1.9.0rc4/datacube/utils/py.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/rio/__init__.py` & `datacube-1.9.0rc4/datacube/utils/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/rio/_rio.py` & `datacube-1.9.0rc4/datacube/utils/rio/_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/serialise.py` & `datacube-1.9.0rc4/datacube/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/uris.py` & `datacube-1.9.0rc4/datacube/utils/uris.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/utils/xarray_geoextensions.py` & `datacube-1.9.0rc4/datacube/utils/xarray_geoextensions.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/__init__.py` & `datacube-1.9.0rc4/datacube/virtual/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/catalog.py` & `datacube-1.9.0rc4/datacube/virtual/catalog.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/expr.py` & `datacube-1.9.0rc4/datacube/virtual/expr.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/impl.py` & `datacube-1.9.0rc4/datacube/virtual/impl.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/transformations.py` & `datacube-1.9.0rc4/datacube/virtual/transformations.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube/virtual/utils.py` & `datacube-1.9.0rc4/datacube/virtual/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube.egg-info/PKG-INFO` & `datacube-1.9.0rc4/datacube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacube
-Version: 1.9.0rc3
+Version: 1.9.0rc4
 Summary: An analysis environment for satellite and other earth observation data
 Home-page: https://github.com/opendatacube/datacube-core
 Author: Open Data Cube
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
 Platform: UNKNOWN
```

### Comparing `datacube-1.9.0rc3/datacube.egg-info/SOURCES.txt` & `datacube-1.9.0rc4/datacube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube.egg-info/entry_points.txt` & `datacube-1.9.0rc4/datacube.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/datacube.egg-info/requires.txt` & `datacube-1.9.0rc4/datacube.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/examples/io_plugin/dcio_example/pickles.py` & `datacube-1.9.0rc4/examples/io_plugin/dcio_example/pickles.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/examples/io_plugin/dcio_example/xarray_3d.py` & `datacube-1.9.0rc4/examples/io_plugin/dcio_example/xarray_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/examples/io_plugin/dcio_example/zeros.py` & `datacube-1.9.0rc4/examples/io_plugin/dcio_example/zeros.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/examples/io_plugin/setup.py` & `datacube-1.9.0rc4/examples/io_plugin/setup.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/conftest.py` & `datacube-1.9.0rc4/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_bad1.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_bad1.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_eo3.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_eo3.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/datasets_eo3_updated.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/datasets_eo3_updated.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/metadata.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/metadata.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/dataset_add/products.yml` & `datacube-1.9.0rc4/integration_tests/data/dataset_add/products.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ard_ls8.odc-product.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ard_ls8.odc-product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/eo3_sentinel_ard.odc-type.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/eo3_sentinel_ard.odc-type.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/final_dataset.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/final_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3.odc-product.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3.odc-product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3_final.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3_final.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ga_s2am_ard_3_interim.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ga_s2am_ard_3_interim.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset2.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset2.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset3.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset3.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset4.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset4.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/ls8_dataset_update.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/ls8_dataset_update.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/nrt_dataset.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/nrt_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/s2_africa_dataset.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/s2_africa_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/s2_africa_product.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/s2_africa_product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/wo_dataset.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/wo_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml` & `datacube-1.9.0rc4/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/data_utils.py` & `datacube-1.9.0rc4/integration_tests/data_utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/example-ls5-nbar.yaml` & `datacube-1.9.0rc4/integration_tests/example-ls5-nbar.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/example-ls5-nbar_302.yaml` & `datacube-1.9.0rc4/integration_tests/example-ls5-nbar_302.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/example-ls5-nbar_505.yaml` & `datacube-1.9.0rc4/integration_tests/example-ls5-nbar_505.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/example-ls5-nbar_606.yaml` & `datacube-1.9.0rc4/integration_tests/example-ls5-nbar_606.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/extensive-eo-metadata.yaml` & `datacube-1.9.0rc4/integration_tests/extensive-eo-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/search_utils.py` & `datacube-1.9.0rc4/integration_tests/index/search_utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_config_docs.py` & `datacube-1.9.0rc4/integration_tests/index/test_config_docs.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_index_cloning.py` & `datacube-1.9.0rc4/integration_tests/index/test_index_cloning.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_index_data.py` & `datacube-1.9.0rc4/integration_tests/index/test_index_data.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_lineage.py` & `datacube-1.9.0rc4/integration_tests/index/test_lineage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_location.py` & `datacube-1.9.0rc4/integration_tests/index/test_location.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_memory_index.py` & `datacube-1.9.0rc4/integration_tests/index/test_memory_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_null_index.py` & `datacube-1.9.0rc4/integration_tests/index/test_null_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_pluggable_indexes.py` & `datacube-1.9.0rc4/integration_tests/index/test_pluggable_indexes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_postgis_index.py` & `datacube-1.9.0rc4/integration_tests/index/test_postgis_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_search_eo3.py` & `datacube-1.9.0rc4/integration_tests/index/test_search_eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_search_legacy.py` & `datacube-1.9.0rc4/integration_tests/index/test_search_legacy.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/index/test_update_columns.py` & `datacube-1.9.0rc4/integration_tests/index/test_update_columns.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_3d.py` & `datacube-1.9.0rc4/integration_tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_cli_output.py` & `datacube-1.9.0rc4/integration_tests/test_cli_output.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_cli_spatial_indexes.py` & `datacube-1.9.0rc4/integration_tests/test_cli_spatial_indexes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_config_tool.py` & `datacube-1.9.0rc4/integration_tests/test_config_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_dataset_add.py` & `datacube-1.9.0rc4/integration_tests/test_dataset_add.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_environments.py` & `datacube-1.9.0rc4/integration_tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_index_datasets_search.py` & `datacube-1.9.0rc4/integration_tests/test_index_datasets_search.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/test_model.py` & `datacube-1.9.0rc4/integration_tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/integration_tests/utils.py` & `datacube-1.9.0rc4/integration_tests/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/license-headers.md` & `datacube-1.9.0rc4/license-headers.md`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/odc_search_profile.py` & `datacube-1.9.0rc4/odc_search_profile.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/pylintrc` & `datacube-1.9.0rc4/pylintrc`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/setup.py` & `datacube-1.9.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/api/test_core.py` & `datacube-1.9.0rc4/tests/api/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import datetime
 from uuid import UUID
 from types import SimpleNamespace
 import pytest
 
 from datacube.api.query import GroupBy
-from datacube.api.core import _calculate_chunk_sizes
+from datacube.api.core import _calculate_chunk_sizes, output_geobox
 from datacube import Datacube
 from datacube.testutils.geom import AlbersGS
 from datacube.testutils import mk_sample_dataset
 
 
 def test_grouping_datasets():
     def group_func(d):
@@ -118,7 +118,35 @@
 
 def test_index_validation():
     index = MagicMock()
     with pytest.raises(ValueError) as e:
         dc = Datacube(index=index, config=["/a/path", "/a/nother/path"], env="prod", app="this_is_me", raw_config="{}")
     estr = str(e.value)
     assert "config,raw_config,app,env" in estr
+
+
+def test_output_geobox():
+    from odc.geo.geobox import GeoBox as ODCGeoGeoBox, CRS as ODCGeoCRS
+    from datacube.utils.geometry import GeoBox as LegacyGeoGeoBox, CRS as LegacyCRS
+    from odc.geo.xr import xr_zeros
+
+    odc_gbox = ODCGeoGeoBox.from_bbox(
+        (-2_000_000, -5_000_000, 2_250_000, -1_000_000),
+        "epsg:3577",
+        resolution=1000
+    )
+    legacy_gbox = LegacyGeoGeoBox(width=odc_gbox.width, height=odc_gbox.height,
+                                  affine=odc_gbox.affine,
+                                  crs=LegacyCRS(str(odc_gbox.crs)))
+
+    assert legacy_gbox != odc_gbox
+
+    xra = xr_zeros(odc_gbox, chunks=(1000, 1000))
+
+    assert xra.odc.geobox == odc_gbox
+
+    gbox = output_geobox(like=xra)
+    assert gbox == odc_gbox
+
+    gbox = output_geobox(like=legacy_gbox)
+    assert gbox == odc_gbox
+    assert isinstance(gbox.crs, ODCGeoCRS)
```

### Comparing `datacube-1.9.0rc3/tests/api/test_masking.py` & `datacube-1.9.0rc4/tests/api/test_masking.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/api/test_query.py` & `datacube-1.9.0rc4/tests/api/test_query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/api/test_virtual.py` & `datacube-1.9.0rc4/tests/api/test_virtual.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/cfg/different_cfg.yaml` & `datacube-1.9.0rc4/tests/cfg/different_cfg.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/cfg/simple_cfg.ini` & `datacube-1.9.0rc4/tests/cfg/simple_cfg.ini`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/cfg/simple_cfg.yaml` & `datacube-1.9.0rc4/tests/cfg/simple_cfg.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/conftest.py` & `datacube-1.9.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ds_eo.yaml` & `datacube-1.9.0rc4/tests/data/ds_eo.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ds_eo3.yml` & `datacube-1.9.0rc4/tests/data/ds_eo3.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/eo3.yaml` & `datacube-1.9.0rc4/tests/data/eo3.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif` & `datacube-1.9.0rc4/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml` & `datacube-1.9.0rc4/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt` & `datacube-1.9.0rc4/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/multi_doc.nc` & `datacube-1.9.0rc4/tests/data/multi_doc.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/no_crs_ds.tif` & `datacube-1.9.0rc4/tests/data/no_crs_ds.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/sample_tile.nc` & `datacube-1.9.0rc4/tests/data/sample_tile.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/sample_tile_151_-29.tif` & `datacube-1.9.0rc4/tests/data/sample_tile_151_-29.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/test.nc` & `datacube-1.9.0rc4/tests/data/test.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/data/test.tif` & `datacube-1.9.0rc4/tests/data/test.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/drivers/fail_drivers/setup.py` & `datacube-1.9.0rc4/tests/drivers/fail_drivers/setup.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/drivers/test_postgis_utils.py` & `datacube-1.9.0rc4/tests/drivers/test_postgis_utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/drivers/test_rio_reader.py` & `datacube-1.9.0rc4/tests/drivers/test_rio_reader.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_api_index_dataset.py` & `datacube-1.9.0rc4/tests/index/test_api_index_dataset.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_fields.py` & `datacube-1.9.0rc4/tests/index/test_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_hl_index.py` & `datacube-1.9.0rc4/tests/index/test_hl_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_postgis_fields.py` & `datacube-1.9.0rc4/tests/index/test_postgis_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_query.py` & `datacube-1.9.0rc4/tests/index/test_query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/index/test_validate_dataset_type.py` & `datacube-1.9.0rc4/tests/index/test_validate_dataset_type.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/scripts/test_search_tool.py` & `datacube-1.9.0rc4/tests/scripts/test_search_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/storage/test_base.py` & `datacube-1.9.0rc4/tests/storage/test_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/storage/test_netcdfwriter.py` & `datacube-1.9.0rc4/tests/storage/test_netcdfwriter.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/storage/test_storage.py` & `datacube-1.9.0rc4/tests/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/storage/test_storage_load.py` & `datacube-1.9.0rc4/tests/storage/test_storage_load.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/storage/test_storage_read.py` & `datacube-1.9.0rc4/tests/storage/test_storage_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This file is part of the Open Data Cube, see https://opendatacube.org for more information
 #
 # Copyright (c) 2015-2024 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
 import numpy as np
 
+import pytest
+from rasterio.enums import Resampling
+
 from datacube.storage._read import (
     read_time_slice,
     read_time_slice_v2,
     pick_read_scale,
     rdr_geobox)
 
 from datacube.testutils.io import RasterFileDataSource
@@ -23,34 +26,40 @@
 
 from datacube.testutils.geom import (
     epsg3857,
     AlbersGS,
 )
 
 
+nearest_resampling_parametrize = pytest.mark.parametrize(
+    "nearest_resampling", ['nearest', Resampling.nearest, Resampling.nearest.value]
+)
+
+
 def test_pick_read_scale():
     assert pick_read_scale(0.7) == 1
     assert pick_read_scale(1.3) == 1
     assert pick_read_scale(2.3) == 2
     assert pick_read_scale(1.99999) == 2
 
 
-def test_read_paste(tmpdir):
+@nearest_resampling_parametrize
+def test_read_paste(nearest_resampling, tmpdir):
     from datacube.testutils import mk_test_image
     from datacube.testutils.io import write_gtiff
     from pathlib import Path
 
     pp = Path(str(tmpdir))
 
     xx = mk_test_image(128, 64, nodata=None)
     assert (xx != -999).all()
 
     mm = write_gtiff(pp/'tst-read-paste-128x64-int16.tif', xx, nodata=None)
 
-    def _read(geobox, resampling='nearest',
+    def _read(geobox, resampling=nearest_resampling,
               fallback_nodata=-999,
               dst_nodata=-999,
               check_paste=False):
         with RasterFileDataSource(mm.path, 1, nodata=fallback_nodata).open() as rdr:
             if check_paste:
                 # check that we are using paste
                 rr = compute_reproject_roi(rdr_geobox(rdr), geobox)
@@ -108,15 +117,16 @@
 
     # scaling paste
     yy, roi = _read(gbx.zoom_out(mm.geobox, 2), check_paste=True)
     assert roi == np.s_[0:32, 0:64]
     np.testing.assert_array_equal(xx[1::2, 1::2], yy)
 
 
-def test_read_with_reproject(tmpdir):
+@nearest_resampling_parametrize
+def test_read_with_reproject(nearest_resampling, tmpdir):
     from datacube.testutils import mk_test_image
     from datacube.testutils.io import write_gtiff
     from pathlib import Path
 
     pp = Path(str(tmpdir))
 
     xx = mk_test_image(128, 64, nodata=None)
@@ -127,15 +137,15 @@
                      crs=str(tile.crs),
                      resolution=tile.resolution.xy,
                      offset=tile.transform*(0, 0),
                      nodata=-999)
     assert mm.geobox == tile
 
     def _read(geobox,
-              resampling='nearest',
+              resampling=nearest_resampling,
               fallback_nodata=None,
               dst_nodata=-999):
         with RasterFileDataSource(mm.path, 1, nodata=fallback_nodata).open() as rdr:
             yy = np.full(geobox.shape, dst_nodata, dtype=rdr.dtype)
             roi = read_time_slice(rdr, yy, geobox, resampling, dst_nodata)
             return yy, roi
 
@@ -167,28 +177,29 @@
     geobox = gbx.zoom_out(geobox, 4)
     yy, roi = _read(geobox, resampling='average')
     nvalid = (yy != -999).sum()
     nempty = (yy == -999).sum()
     assert nvalid > nempty
 
 
-def test_read_paste_v2(tmpdir):
+@nearest_resampling_parametrize
+def test_read_paste_v2(nearest_resampling, tmpdir):
     from datacube.testutils import mk_test_image
     from datacube.testutils.io import write_gtiff
     from datacube.testutils.iodriver import open_reader
     from pathlib import Path
 
     pp = Path(str(tmpdir))
 
     xx = mk_test_image(128, 64, nodata=None)
     assert (xx != -999).all()
 
     mm = write_gtiff(pp/'tst-read-paste-128x64-int16.tif', xx, nodata=None)
 
-    def _read(geobox, resampling='nearest',
+    def _read(geobox, resampling=nearest_resampling,
               fallback_nodata=-999,
               dst_nodata=-999,
               check_paste=False):
 
         rdr = open_reader(mm.path,
                           nodata=fallback_nodata)
         if check_paste:
@@ -252,27 +263,28 @@
 
     # scaling paste
     yy, roi = _read(gbx.zoom_out(mm.geobox, 2), check_paste=True)
     assert roi == np.s_[0:32, 0:64]
     np.testing.assert_array_equal(xx[1::2, 1::2], yy)
 
 
-def test_read_with_reproject_v2(tmpdir):
+@nearest_resampling_parametrize
+def test_read_with_reproject_v2(nearest_resampling, tmpdir):
     from datacube.testutils import mk_test_image
     from datacube.testutils.io import write_gtiff
     from datacube.testutils.iodriver import open_reader
     from pathlib import Path
 
     pp = Path(str(tmpdir))
 
     xx = mk_test_image(128, 64, nodata=None)
     assert (xx != -999).all()
     tile = AlbersGS.tile_geobox((17, -40))[:64, :128]
 
-    def _read(geobox, resampling='nearest',
+    def _read(geobox, resampling=nearest_resampling,
               fallback_nodata=-999,
               dst_nodata=-999):
 
         rdr = open_reader(mm.path,
                           nodata=fallback_nodata)
 
         yy = np.full(geobox.shape, dst_nodata, dtype=rdr.dtype)
```

### Comparing `datacube-1.9.0rc3/tests/test_3d.py` & `datacube-1.9.0rc4/tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_cfg.py` & `datacube-1.9.0rc4/tests/test_cfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,16 +209,17 @@
 
 def test_single_env(single_env_config):
     from datacube.cfg import ODCConfig
     cfg = ODCConfig(text=single_env_config)
 
     assert cfg['experimental'].index_driver == "postgis"
     assert cfg['experimental'].db_url == "postgresql://foo:bar@server.subdomain.domain/mytestdb"
+    assert cfg['experimental'].db_username == "foo"
     with pytest.raises(AttributeError):
-        assert cfg['experimental'].db_username
+        assert cfg['experimental'].not_an_option
     assert cfg['experimental']['db_iam_authentication']
     assert cfg['experimental'].db_iam_timeout == 600
     assert cfg['experimental']['db_connection_timeout'] == 60
 
 
 def assert_simple_aliases(cfg):
     assert cfg['default']._name == 'legacy'
@@ -253,16 +254,17 @@
     assert cfg['default']['index_driver'] == 'default'
     assert cfg['default'].db_username == 'foo'
     assert not cfg['default']['db_iam_authentication']
     with pytest.raises(KeyError):
         assert cfg['default']["db_iam_timeout"]
 
     assert cfg['exp2'].db_url == "postgresql://foo:bar@server.subdomain.domain/mytestdb"
+    assert cfg['exp2'].db_username == "foo"
     with pytest.raises(AttributeError):
-        assert cfg['exp2'].db_username
+        assert cfg['exp2'].not_an_option
     assert cfg['exp2']['db_iam_authentication']
     assert cfg['exp2'].db_iam_timeout == 300
     assert cfg['exp2']['db_connection_timeout'] == 60
 
 
 def test_options(simple_config):
     from datacube.cfg import ODCConfig
@@ -280,16 +282,15 @@
 def test_noenv_overrides_in_text(simple_config, monkeypatch):
     monkeypatch.setenv("ODC_LEGACY_DB_USERNAME", "bar")
     monkeypatch.setenv("ODC_EXPERIMENTAL_DB_USERNAME", "bar")
     from datacube.cfg import ODCConfig
     cfg = ODCConfig(text=simple_config)
 
     assert cfg["legacy"].db_username != 'bar'
-    with pytest.raises(AttributeError):
-        cfg["experimental"].db_username
+    assert cfg["experimental"].db_username != "bar"
 
 
 @pytest.fixture
 def path_to_yaml_config():
     import os.path
     return os.path.join(os.path.dirname(__file__), "cfg", "simple_cfg.yaml")
 
@@ -385,16 +386,15 @@
     from datacube.cfg import ODCConfig
     cfg = ODCConfig(paths=path_to_yaml_config)
     assert cfg["legacy"].db_username == 'bar'
     assert cfg["legacy"].db_iam_authentication
     assert cfg["experimental"].db_iam_authentication
     assert cfg["exp2"].db_iam_authentication
     assert cfg["exp2"].db_connection_timeout == 20
-    with pytest.raises(AttributeError):
-        assert cfg["experimental"].db_username == 'bar'
+    assert cfg["experimental"].db_username != 'bar'
 
 
 def test_intopt_validation():
     from datacube.cfg import ODCConfig, ConfigException
     cfg = ODCConfig(text="""
 env1:
     db_hostname: localhost
@@ -463,14 +463,20 @@
     assert psql_url_from_config(
         cfg["experimental"]
     ) == "postgresql://foo:bar@server.subdomain.domain/mytestdb"
     with pytest.raises(AttributeError):
         psql_url_from_config(
             cfg["memory"]
         )
+    assert cfg["exp2"].db_url == "postgresql://foo:bar@server.subdomain.domain/mytestdb"
+    assert cfg["exp2"].db_username == "foo"
+    assert cfg["exp2"].db_password == "bar"
+    assert cfg["exp2"].db_hostname == "server.subdomain.domain"
+    assert not cfg["exp2"].db_port
+    assert cfg["exp2"].db_database == "mytestdb"
 
     cfg = ODCConfig(raw_dict={
         "foo": {
             "db_hostname": "remotehost.local",
             "db_username": "penelope",
             "db_database": "mydb",
             "db_port": 5544,
@@ -521,15 +527,15 @@
         '{"default":{"alias": "foo"},"foo":{"index_driver":"postgis","db_url":"postgresql:///mydb"}}'
     )
     cfg = ODCConfig()
     assert cfg[None]._name == 'foo'
 
 
 def test_default_environment(simple_config, monkeypatch):
-    from datacube.cfg import ODCConfig, ConfigException
+    from datacube.cfg import ODCConfig
     cfg = ODCConfig(text=simple_config)
     assert cfg[None]._name == 'legacy'
     monkeypatch.setenv('ODC_ENVIRONMENT', 'exp2')
     assert cfg[None]._name == 'exp2'
     monkeypatch.setenv('ODC_ENVIRONMENT', '')
     monkeypatch.setenv('DATACUBE_ENVIRONMENT', 'postgis')
     assert cfg[None]._name == 'experimental'
@@ -538,9 +544,8 @@
     })
     monkeypatch.setenv('DATACUBE_ENVIRONMENT', '')
     assert cfg[None]._name == 'datacube'
     cfg = ODCConfig(raw_dict={
         'weirdname': {"index_driver": "memory"},
         'stupidenv': {"index_driver": "null"},
     })
-    with pytest.raises(ConfigException):
-        cfg[None]._name
+    assert cfg[None]._name == "default"
```

### Comparing `datacube-1.9.0rc3/tests/test_driver.py` & `datacube-1.9.0rc4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_dynamic_db_passwd.py` & `datacube-1.9.0rc4/tests/test_dynamic_db_passwd.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_eo3.py` & `datacube-1.9.0rc4/tests/test_eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_ext_lineage.py` & `datacube-1.9.0rc4/tests/test_ext_lineage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_load_data.py` & `datacube-1.9.0rc4/tests/test_load_data.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_metadata_fields.py` & `datacube-1.9.0rc4/tests/test_metadata_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_model.py` & `datacube-1.9.0rc4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_testutils.py` & `datacube-1.9.0rc4/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_aws.py` & `datacube-1.9.0rc4/tests/test_utils_aws.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_changes.py` & `datacube-1.9.0rc4/tests/test_utils_changes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_cog.py` & `datacube-1.9.0rc4/tests/test_utils_cog.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_dask.py` & `datacube-1.9.0rc4/tests/test_utils_dask.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_dates.py` & `datacube-1.9.0rc4/tests/test_utils_dates.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_docs.py` & `datacube-1.9.0rc4/tests/test_utils_docs.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_generic.py` & `datacube-1.9.0rc4/tests/test_utils_generic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_other.py` & `datacube-1.9.0rc4/tests/test_utils_other.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_utils_rio.py` & `datacube-1.9.0rc4/tests/test_utils_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/test_xarray_extension.py` & `datacube-1.9.0rc4/tests/test_xarray_extension.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/ui/test_common.py` & `datacube-1.9.0rc4/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/ui/test_expression_parsing.py` & `datacube-1.9.0rc4/tests/ui/test_expression_parsing.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/tests/ui/test_task_app.py` & `datacube-1.9.0rc4/tests/ui/test_task_app.py`

 * *Files identical despite different names*

### Comparing `datacube-1.9.0rc3/wordlist.txt` & `datacube-1.9.0rc4/wordlist.txt`

 * *Files identical despite different names*

