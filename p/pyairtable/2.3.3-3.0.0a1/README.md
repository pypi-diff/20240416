# Comparing `tmp/pyairtable-2.3.3.tar.gz` & `tmp/pyairtable-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyairtable-2.3.3.tar", last modified: Fri Mar 22 17:52:08 2024, max compression
+gzip compressed data, was "pyairtable-3.0.0a1.tar", last modified: Tue Apr 16 03:47:39 2024, max compression
```

## Comparing `pyairtable-2.3.3.tar` & `pyairtable-3.0.0a1.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.595479 pyairtable-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-22 17:52:04.000000 pyairtable-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 17:52:04.000000 pyairtable-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-22 17:52:08.591479 pyairtable-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-22 17:52:04.000000 pyairtable-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.583479 pyairtable-2.3.3/pyairtable/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.587479 pyairtable-2.3.3/pyairtable/api/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/retrying.py
--rw-r--r--   0 runner    (1001) docker     (127)    23636 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/formulas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.587479 pyairtable-2.3.3/pyairtable/models/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/collaborator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    38575 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.587479 pyairtable-2.3.3/pyairtable/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30354 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/orm/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/orm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyairtable/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.591479 pyairtable-2.3.3/pyairtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-22 17:52:08.000000 pyairtable-2.3.3/pyairtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-22 17:52:08.000000 pyairtable-2.3.3/pyairtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:52:08.000000 pyairtable-2.3.3/pyairtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 17:52:08.000000 pyairtable-2.3.3/pyairtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 17:52:08.000000 pyairtable-2.3.3/pyairtable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-22 17:52:04.000000 pyairtable-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-22 17:52:08.595479 pyairtable-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 17:52:04.000000 pyairtable-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:52:08.591479 pyairtable-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_retrying.py
--rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_api_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_formulas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_models_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_models_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_models_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_models_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21827 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_orm_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_orm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_url_escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-22 17:52:04.000000 pyairtable-2.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.678950 pyairtable-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-16 03:47:39.678950 pyairtable-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.670950 pyairtable-3.0.0a1/pyairtable/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.674950 pyairtable-3.0.0a1/pyairtable/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23474 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34695 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/formulas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.674950 pyairtable-3.0.0a1/pyairtable/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38675 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.674950 pyairtable-3.0.0a1/pyairtable/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52420 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/orm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyairtable/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.678950 pyairtable-3.0.0a1/pyairtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-16 03:47:39.000000 pyairtable-3.0.0a1/pyairtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-16 03:47:39.000000 pyairtable-3.0.0a1/pyairtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:47:39.000000 pyairtable-3.0.0a1/pyairtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 03:47:39.000000 pyairtable-3.0.0a1/pyairtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 03:47:39.000000 pyairtable-3.0.0a1/pyairtable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 03:47:39.682950 pyairtable-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:47:39.678950 pyairtable-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_retrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_api_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_formulas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_models_collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_models_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_models_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_models_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_orm_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_orm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_url_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-16 03:47:35.000000 pyairtable-3.0.0a1/tox.ini
```

### Comparing `pyairtable-2.3.3/LICENSE` & `pyairtable-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/PKG-INFO` & `pyairtable-3.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairtable
-Version: 2.3.3
+Version: 3.0.0a1
 Summary: Python Client for the Airtable API
 Home-page: https://github.com/gtalarico/pyairtable
 Author: Gui Talarico
 License: MIT
 Keywords: airtable,api,client,pyairtable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyairtable-2.3.3/README.md` & `pyairtable-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/api/api.py` & `pyairtable-3.0.0a1/pyairtable/api/api.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/api/base.py` & `pyairtable-3.0.0a1/pyairtable/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                     id='ach00000000000001',
                     are_notifications_enabled=True,
                     cursor_for_next_payload=1,
                     is_hook_enabled=True,
                     last_successful_notification_time=None,
                     notification_url="https://example.com",
                     last_notification_result=None,
-                    expiration_time="2023-07-01T00:00:00.000Z",
+                    expiration_time=datetime.datetime(...),
                     specification: WebhookSpecification(...)
                 )
             ]
         """
         response = self.api.get(self.webhooks_url)
         return [
             Webhook.from_api(data, self.api, context=self)
@@ -260,15 +260,15 @@
             ...             }
             ...         }
             ...     }
             ... )
             CreateWebhookResponse(
                 id='ach00000000000001',
                 mac_secret_base64='c3VwZXIgZHVwZXIgc2VjcmV0',
-                expiration_time='2023-07-01T00:00:00.000Z'
+                expiration_time=datetime.datetime(...)
             )
 
         Raises:
             pydantic.ValidationError: If the dict provided is invalid.
 
         Args:
             notify_url: The URL where Airtable will POST all event notifications.
```

### Comparing `pyairtable-2.3.3/pyairtable/api/enterprise.py` & `pyairtable-3.0.0a1/pyairtable/api/enterprise.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/api/params.py` & `pyairtable-3.0.0a1/pyairtable/api/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     # list records
     "cell_format": "cellFormat",
     "fields": "fields",
     "formula": "filterByFormula",
     "max_records": "maxRecords",
     "offset": "offset",
     "page_size": "pageSize",
-    "return_fields_by_field_id": "returnFieldsByFieldId",
+    "use_field_ids": "returnFieldsByFieldId",
     "sort": "sort",
     "time_zone": "timeZone",
     "user_locale": "userLocale",
     "view": "view",
     # get webhook payloads
     "limit": "limit",
     "cursor": "cursor",
```

### Comparing `pyairtable-2.3.3/pyairtable/api/retrying.py` & `pyairtable-3.0.0a1/pyairtable/api/retrying.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/api/table.py` & `pyairtable-3.0.0a1/pyairtable/api/table.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     RecordId,
     UpdateRecordDict,
     UpsertResultDict,
     WritableFields,
     assert_typed_dict,
     assert_typed_dicts,
 )
+from pyairtable.formulas import Formula, to_formula_str
 from pyairtable.models.schema import FieldSchema, TableSchema, parse_field_schema
 from pyairtable.utils import is_table_id
 
 
 class Table:
     """
     Represents an Airtable table.
@@ -190,15 +191,15 @@
         Args:
             record_id: |arg_record_id|
 
         Keyword Args:
             cell_format: |kwarg_cell_format|
             time_zone: |kwarg_time_zone|
             user_locale: |kwarg_user_locale|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         record = self.api.get(self.record_url(record_id), options=options)
         return assert_typed_dict(RecordDict, record)
 
     def iterate(self, **options: Any) -> Iterator[List[RecordDict]]:
         """
         Iterate through each page of results from `List records <https://airtable.com/developers/web/api/list-records>`_.
@@ -221,16 +222,18 @@
             max_records: |kwarg_max_records|
             fields: |kwarg_fields|
             sort: |kwarg_sort|
             formula: |kwarg_formula|
             cell_format: |kwarg_cell_format|
             user_locale: |kwarg_user_locale|
             time_zone: |kwarg_time_zone|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
+        if isinstance(formula := options.get("formula"), Formula):
+            options["formula"] = to_formula_str(formula)
         for page in self.api.iterate_requests(
             method="get",
             url=self.url,
             fallback=("post", f"{self.url}/listRecords"),
             options=options,
         ):
             yield assert_typed_dicts(RecordDict, page.get("records", []))
@@ -251,15 +254,15 @@
             max_records: |kwarg_max_records|
             fields: |kwarg_fields|
             sort: |kwarg_sort|
             formula: |kwarg_formula|
             cell_format: |kwarg_cell_format|
             user_locale: |kwarg_user_locale|
             time_zone: |kwarg_time_zone|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         return [record for page in self.iterate(**options) for record in page]
 
     def first(self, **options: Any) -> Optional[RecordDict]:
         """
         Retrieve the first matching record.
         Returns ``None`` if no records are returned.
@@ -271,55 +274,55 @@
             view: |kwarg_view|
             fields: |kwarg_fields|
             sort: |kwarg_sort|
             formula: |kwarg_formula|
             cell_format: |kwarg_cell_format|
             user_locale: |kwarg_user_locale|
             time_zone: |kwarg_time_zone|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         options.update(dict(page_size=1, max_records=1))
         for page in self.iterate(**options):
             for record in page:
                 return record
         return None
 
     def create(
         self,
         fields: WritableFields,
         typecast: bool = False,
-        return_fields_by_field_id: bool = False,
+        use_field_ids: bool = False,
     ) -> RecordDict:
         """
         Create a new record
 
         >>> record = {'Name': 'John'}
         >>> table = api.table('base_id', 'table_name')
         >>> table.create(record)
 
         Args:
             fields: Fields to insert. Must be a dict with field names or IDs as keys.
             typecast: |kwarg_typecast|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         created = self.api.post(
             url=self.url,
             json={
                 "fields": fields,
                 "typecast": typecast,
-                "returnFieldsByFieldId": return_fields_by_field_id,
+                "returnFieldsByFieldId": use_field_ids,
             },
         )
         return assert_typed_dict(RecordDict, created)
 
     def batch_create(
         self,
         records: Iterable[WritableFields],
         typecast: bool = False,
-        return_fields_by_field_id: bool = False,
+        use_field_ids: bool = False,
     ) -> List[RecordDict]:
         """
         Create a number of new records in batches.
 
         >>> table.batch_create([{'Name': 'John'}, {'Name': 'Marc'}])
         [
             {
@@ -333,85 +336,85 @@
                 'fields': {'Name': 'Marc'}
             }
         ]
 
         Args:
             records: Iterable of dicts representing records to be created.
             typecast: |kwarg_typecast|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         inserted_records = []
 
         # If we got an iterator, exhaust it and collect it into a list.
         records = list(records)
 
         for chunk in self.api.chunked(records):
             new_records = [{"fields": fields} for fields in chunk]
             response = self.api.post(
                 url=self.url,
                 json={
                     "records": new_records,
                     "typecast": typecast,
-                    "returnFieldsByFieldId": return_fields_by_field_id,
+                    "returnFieldsByFieldId": use_field_ids,
                 },
             )
             inserted_records += assert_typed_dicts(RecordDict, response["records"])
 
         return inserted_records
 
     def update(
         self,
         record_id: RecordId,
         fields: WritableFields,
         replace: bool = False,
         typecast: bool = False,
-        return_fields_by_field_id: bool = False,
+        use_field_ids: bool = False,
     ) -> RecordDict:
         """
         Update a particular record ID with the given fields.
 
         >>> table.update('recwPQIfs4wKPyc9D', {"Age": 21})
         {'id': 'recwPQIfs4wKPyc9D', 'fields': {'First Name': 'John', 'Age': 21}}
         >>> table.update('recwPQIfs4wKPyc9D', {"Age": 22}, replace=True)
         {'id': 'recwPQIfs4wKPyc9D', 'fields': {'Age': 22}}
 
         Args:
             record_id: |arg_record_id|
             fields: Fields to update. Must be a dict with column names or IDs as keys.
             replace: |kwarg_replace|
             typecast: |kwarg_typecast|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
         """
         method = "put" if replace else "patch"
         updated = self.api.request(
             method=method,
             url=self.record_url(record_id),
             json={
                 "fields": fields,
                 "typecast": typecast,
-                "returnFieldsByFieldId": return_fields_by_field_id,
+                "returnFieldsByFieldId": use_field_ids,
             },
         )
         return assert_typed_dict(RecordDict, updated)
 
     def batch_update(
         self,
         records: Iterable[UpdateRecordDict],
         replace: bool = False,
         typecast: bool = False,
-        return_fields_by_field_id: bool = False,
+        use_field_ids: bool = False,
     ) -> List[RecordDict]:
         """
         Update several records in batches.
 
         Args:
             records: Records to update.
             replace: |kwarg_replace|
             typecast: |kwarg_typecast|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
 
         Returns:
             The list of updated records.
         """
         updated_records = []
         method = "put" if replace else "patch"
 
@@ -422,43 +425,43 @@
             chunk_records = [{"id": x["id"], "fields": x["fields"]} for x in chunk]
             response = self.api.request(
                 method=method,
                 url=self.url,
                 json={
                     "records": chunk_records,
                     "typecast": typecast,
-                    "returnFieldsByFieldId": return_fields_by_field_id,
+                    "returnFieldsByFieldId": use_field_ids,
                 },
             )
             updated_records += assert_typed_dicts(RecordDict, response["records"])
 
         return updated_records
 
     def batch_upsert(
         self,
         records: Iterable[Dict[str, Any]],
         key_fields: List[FieldName],
         replace: bool = False,
         typecast: bool = False,
-        return_fields_by_field_id: bool = False,
+        use_field_ids: bool = False,
     ) -> UpsertResultDict:
         """
         Update or create records in batches, either using ``id`` (if given) or using a set of
         fields (``key_fields``) to look for matches. For more information on how this operation
         behaves, see Airtable's API documentation for `Update multiple records <https://airtable.com/developers/web/api/update-multiple-records#request-performupsert-fieldstomergeon>`__.
 
         .. versionadded:: 1.5.0
 
         Args:
             records: Records to update.
             key_fields: List of field names that Airtable should use to match
                 records in the input with existing records on the server.
             replace: |kwarg_replace|
             typecast: |kwarg_typecast|
-            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+            use_field_ids: |kwarg_use_field_ids|
 
         Returns:
             Lists of created/updated record IDs, along with the list of all records affected.
         """
         # If we got an iterator, exhaust it and collect it into a list.
         records = list(records)
 
@@ -487,15 +490,15 @@
             ]
             response = self.api.request(
                 method=method,
                 url=self.url,
                 json={
                     "records": formatted_records,
                     "typecast": typecast,
-                    "returnFieldsByFieldId": return_fields_by_field_id,
+                    "returnFieldsByFieldId": use_field_ids,
                     "performUpsert": {"fieldsToMergeOn": key_fields},
                 },
             )
             result["updatedRecords"].extend(response["updatedRecords"])
             result["createdRecords"].extend(response["createdRecords"])
             result["records"].extend(
                 assert_typed_dicts(RecordDict, response["records"])
@@ -555,15 +558,15 @@
         Usage:
             >>> table = Api.table("appNxslc6jG0XedVM", "tblslc6jG0XedVMNx")
             >>> table.comments("recMNxslc6jG0XedV")
             [
                 Comment(
                     id='comdVMNxslc6jG0Xe',
                     text='Hello, @[usrVMNxslc6jG0Xed]!',
-                    created_time='2023-06-07T17:46:24.435891',
+                    created_time=datetime.datetime(...),
                     last_updated_time=None,
                     mentioned={
                         'usrVMNxslc6jG0Xed': Mentioned(
                             display_name='Alice',
                             email='alice@example.com',
                             id='usrVMNxslc6jG0Xed',
                             type='user'
```

### Comparing `pyairtable-2.3.3/pyairtable/api/types.py` & `pyairtable-3.0.0a1/pyairtable/api/types.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/api/workspace.py` & `pyairtable-3.0.0a1/pyairtable/api/workspace.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/models/__init__.py` & `pyairtable-3.0.0a1/pyairtable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/models/_base.py` & `pyairtable-3.0.0a1/pyairtable/models/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from datetime import datetime
 from functools import partial
 from typing import Any, ClassVar, Dict, Iterable, Mapping, Optional, Set, Type, Union
 
 import inflection
 from typing_extensions import Self as SelfType
 
 from pyairtable._compat import pydantic
-from pyairtable.utils import _append_docstring_text
+from pyairtable.utils import (
+    _append_docstring_text,
+    datetime_from_iso_str,
+    datetime_to_iso_str,
+)
 
 
 class AirtableModel(pydantic.BaseModel):
     """
     Base model for any data structures that will be loaded from the Airtable API.
     """
 
@@ -26,16 +31,24 @@
 
         # We'll assume this in a couple different places
         underscore_attrs_are_private = True
 
     _raw: Any = pydantic.PrivateAttr()
 
     def __init__(self, **data: Any) -> None:
+        self._raw = data.copy()
+        # Convert JSON-serializable input data to the types expected by our model.
+        # For now this only converts ISO 8601 strings to datetime objects.
+        for field_model in self.__fields__.values():
+            for name in {field_model.name, field_model.alias}:
+                if not (value := data.get(name)):
+                    continue
+                if isinstance(value, str) and field_model.type_ is datetime:
+                    data[name] = datetime_from_iso_str(value)
         super().__init__(**data)
-        self._raw = data
 
     @classmethod
     def from_api(
         cls,
         obj: Dict[str, Any],
         api: "pyairtable.api.api.Api",
         *,
@@ -240,14 +253,18 @@
         exclude = set(self.__readonly) if self.__readonly else None
         data = self.dict(
             by_alias=True,
             include=include,
             exclude=exclude,
             exclude_none=(not self.__save_none),
         )
+        # This undoes the finagling we do in __init__, converting datetime back to str.
+        for key in data:
+            if isinstance(value := data.get(key), datetime):
+                data[key] = datetime_to_iso_str(value)
         response = self._api.request(self.__save_http_method, self._url, json=data)
         if self.__reload_after_save:
             self._reload(response)
 
     def __setattr__(self, name: str, value: Any) -> None:
         # Prevents implementers from changing values on readonly or non-writable fields.
         # Mypy can't tell that we are using pydantic v1.
```

### Comparing `pyairtable-2.3.3/pyairtable/models/audit.py` & `pyairtable-3.0.0a1/pyairtable/models/audit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from typing_extensions import TypeAlias
 
 from pyairtable.models._base import AirtableModel, update_forward_refs
 
 
@@ -26,15 +27,15 @@
     Represents a single audit log event.
 
     See `Audit log events <https://airtable.com/developers/web/api/audit-log-events>`__
     for more information on how to interpret this data structure.
     """
 
     id: str
-    timestamp: str
+    timestamp: datetime
     action: str
     actor: "AuditLogActor"
     model_id: str
     model_type: str
     payload: "AuditLogPayload"
     payload_version: str
     context: "AuditLogEvent.Context"
```

### Comparing `pyairtable-2.3.3/pyairtable/models/collaborator.py` & `pyairtable-3.0.0a1/pyairtable/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable/models/comment.py` & `pyairtable-3.0.0a1/pyairtable/models/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import Dict, Optional
 
 from ._base import AirtableModel, CanDeleteModel, CanUpdateModel, update_forward_refs
 from .collaborator import Collaborator
 
 
 class Comment(
@@ -15,15 +16,15 @@
 
     >>> comment = table.add_comment("recMNxslc6jG0XedV", "Hello, @[usrVMNxslc6jG0Xed]!")
     >>> table.comments("recMNxslc6jG0XedV")
     [
         Comment(
             id='comdVMNxslc6jG0Xe',
             text='Hello, @[usrVMNxslc6jG0Xed]!',
-            created_time='2023-06-07T17:46:24.435891',
+            created_time=datetime.datetime(...),
             last_updated_time=None,
             mentioned={
                 'usrVMNxslc6jG0Xed': Mentioned(
                     display_name='Alice',
                     email='alice@example.com',
                     id='usrVMNxslc6jG0Xed',
                     type='user'
@@ -44,15 +45,15 @@
     #: The unique ID of the comment.
     id: str
 
     #: The text of the comment.
     text: str
 
     #: The ISO 8601 timestamp of when the comment was created.
-    created_time: str
+    created_time: datetime
 
     #: The ISO 8601 timestamp of when the comment was last edited.
     last_updated_time: Optional[str]
 
     #: The account which created the comment.
     author: Collaborator
```

### Comparing `pyairtable-2.3.3/pyairtable/models/schema.py` & `pyairtable-3.0.0a1/pyairtable/models/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+from datetime import datetime
 from functools import partial
 from typing import Any, Dict, Iterable, List, Literal, Optional, TypeVar, Union, cast
 
 from typing_extensions import TypeAlias
 
 from pyairtable._compat import pydantic
 from pyairtable.api.types import AddCollaboratorDict
@@ -174,15 +175,15 @@
     individual_collaborators: "BaseCollaborators.IndividualCollaborators" = _F("BaseCollaborators.IndividualCollaborators")  # fmt: skip
     invite_links: "BaseCollaborators.InviteLinks" = _F("BaseCollaborators.InviteLinks")  # fmt: skip
 
     class InterfaceCollaborators(
         _Collaborators,
         url="meta/bases/{base.id}/interfaces/{key}",
     ):
-        created_time: str
+        created_time: datetime
         group_collaborators: List["GroupCollaborator"] = _FL()
         individual_collaborators: List["IndividualCollaborator"] = _FL()
         invite_links: List["InterfaceInviteLink"] = _FL()
 
     class GroupCollaborators(AirtableModel):
         via_base: List["GroupCollaborator"] = _FL(alias="baseCollaborators")
         via_workspace: List["GroupCollaborator"] = _FL(alias="workspaceCollaborators")
@@ -210,15 +211,15 @@
         CanDeleteModel,
         url="meta/bases/{base.id}/shares/{self.share_id}",
         writable=["state"],
         reload_after_save=False,
     ):
         state: str
         created_by_user_id: str
-        created_time: str
+        created_time: datetime
         share_id: str
         type: str
         is_password_protected: bool
         block_installation_id: Optional[str] = None
         restricted_to_email_domains: List[str] = _FL()
         view_id: Optional[str] = None
         effective_email_domain_allow_list: List[str] = _FL()
@@ -344,23 +345,23 @@
     type: str
     name: str
     personal_for_user_id: Optional[str]
     visible_field_ids: Optional[List[str]]
 
 
 class GroupCollaborator(AirtableModel):
-    created_time: str
+    created_time: datetime
     granted_by_user_id: str
     group_id: str
     name: str
     permission_level: str
 
 
 class IndividualCollaborator(AirtableModel):
-    created_time: str
+    created_time: datetime
     granted_by_user_id: str
     user_id: str
     email: str
     permission_level: str
 
 
 class BaseIndividualCollaborator(IndividualCollaborator):
@@ -376,15 +377,15 @@
 class InviteLink(CanDeleteModel, url="{invite_links._url}/{self.id}"):
     """
     Represents an `invite link <https://airtable.com/developers/web/api/model/invite-link>`__.
     """
 
     id: str
     type: str
-    created_time: str
+    created_time: datetime
     invited_email: Optional[str]
     referred_by_user_id: str
     permission_level: str
     restricted_to_email_domains: List[str] = _FL()
 
 
 class BaseInviteLink(
@@ -423,15 +424,15 @@
     Information about groups, users, workspaces, and email domains
     associated with an enterprise account.
 
     See https://airtable.com/developers/web/api/get-enterprise
     """
 
     id: str
-    created_time: str
+    created_time: datetime
     group_ids: List[str]
     user_ids: List[str]
     workspace_ids: List[str]
     email_domains: List["EnterpriseInfo.EmailDomain"]
 
     class EmailDomain(AirtableModel):
         email_domain: str
@@ -443,15 +444,15 @@
     Detailed information about who can access a workspace.
 
     See https://airtable.com/developers/web/api/get-workspace-collaborators
     """
 
     id: str
     name: str
-    created_time: str
+    created_time: datetime
     base_ids: List[str]
     restrictions: "WorkspaceCollaborators.Restrictions" = pydantic.Field(alias="workspaceRestrictions")  # fmt: skip
     group_collaborators: "WorkspaceCollaborators.GroupCollaborators" = _F("WorkspaceCollaborators.GroupCollaborators")  # fmt: skip
     individual_collaborators: "WorkspaceCollaborators.IndividualCollaborators" = _F("WorkspaceCollaborators.IndividualCollaborators")  # fmt: skip
     invite_links: "WorkspaceCollaborators.InviteLinks" = _F("WorkspaceCollaborators.InviteLinks")  # fmt: skip
 
     class Restrictions(
@@ -523,24 +524,24 @@
         """
         Mapping of workspace IDs to collaborations, to make lookups easier.
         """
         return {c.workspace_id: c for c in self.workspace_collaborations}
 
     class BaseCollaboration(AirtableModel):
         base_id: str
-        created_time: str
+        created_time: datetime
         granted_by_user_id: str
         permission_level: str
 
     class InterfaceCollaboration(BaseCollaboration):
         interface_id: str
 
     class WorkspaceCollaboration(AirtableModel):
         workspace_id: str
-        created_time: str
+        created_time: datetime
         granted_by_user_id: str
         permission_level: str
 
 
 class UserInfo(
     CanUpdateModel,
     CanDeleteModel,
@@ -555,16 +556,16 @@
 
     id: str
     name: str
     email: str
     state: str
     is_sso_required: bool
     is_two_factor_auth_enabled: bool
-    last_activity_time: Optional[str]
-    created_time: Optional[str]
+    last_activity_time: Optional[datetime]
+    created_time: Optional[datetime]
     enterprise_user_type: Optional[str]
     invited_to_airtable_by_user_id: Optional[str]
     is_managed: bool = False
     groups: List[NestedId] = _FL()
     collaborations: "Collaborations" = pydantic.Field(default_factory=Collaborations)
 
     def logout(self) -> None:
@@ -577,26 +578,26 @@
 
     See https://airtable.com/developers/web/api/get-user-group
     """
 
     id: str
     name: str
     enterprise_account_id: str
-    created_time: str
-    updated_time: str
+    created_time: datetime
+    updated_time: datetime
     members: List["UserGroup.Member"]
     collaborations: "Collaborations" = pydantic.Field(default_factory=Collaborations)
 
     class Member(AirtableModel):
         user_id: str
         email: str
         first_name: str
         last_name: str
         role: str
-        created_time: str
+        created_time: datetime
 
 
 # The data model is a bit confusing here, but it's designed for maximum reuse.
 # SomethingFieldConfig contains the `type` and `options` values for each field type.
 # _FieldSchemaBase contains the `id`, `name`, and `description` values.
 # SomethingFieldSchema inherits from _FieldSchemaBase and SomethingFieldConfig.
 # FieldConfig is a union of all available *FieldConfig classes.
```

### Comparing `pyairtable-2.3.3/pyairtable/models/webhook.py` & `pyairtable-3.0.0a1/pyairtable/models/webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+from datetime import datetime
 from functools import partial
 from hmac import HMAC
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
 from typing_extensions import Self as SelfType
 
 from pyairtable._compat import pydantic
@@ -26,27 +27,27 @@
     ...         }
     ...     }
     ... }
     >>> base.add_webhook("https://example.com", spec)
     CreateWebhookResponse(
         id='ach00000000000001',
         mac_secret_base64='c3VwZXIgZHVwZXIgc2VjcmV0',
-        expiration_time='2023-07-01T00:00:00.000Z'
+        expiration_time=datetime.datetime(...)
     )
     >>> webhooks = base.webhooks()
     >>> webhooks[0]
     Webhook(
         id='ach00000000000001',
         are_notifications_enabled=True,
         cursor_for_next_payload=1,
         is_hook_enabled=True,
         last_successful_notification_time=None,
         notification_url="https://example.com",
         last_notification_result=None,
-        expiration_time="2023-07-01T00:00:00.000Z",
+        expiration_time=datetime.datetime(...),
         specification: WebhookSpecification(...)
     )
     >>> webhooks[0].disable_notifications()
     >>> webhooks[0].enable_notifications()
     >>> webhooks[0].extend_expiration()
     >>> webhooks[0].delete()
     """
@@ -106,15 +107,15 @@
                 If not provided, will retrieve all remaining payloads.
 
         Usage:
             >>> webhook = Base.webhook("ach00000000000001")
             >>> iter_payloads = webhook.payloads()
             >>> next(iter_payloads)
             WebhookPayload(
-                timestamp="2022-02-01T21:25:05.663Z",
+                timestamp=datetime.datetime(...),
                 base_transaction_number=4,
                 payload_format="v0",
                 action_metadata=ActionMetadata(
                     source="client",
                     source_metadata={
                         "user": {
                             "id": "usr00000000000000",
@@ -200,15 +201,15 @@
 
     See `Webhook notification delivery <https://airtable.com/developers/web/api/webhooks-overview#webhook-notification-delivery>`_
     for more information on how these payloads are structured.
     """
 
     base: _NestedId
     webhook: _NestedId
-    timestamp: str
+    timestamp: datetime
 
     @classmethod
     def from_request(
         cls,
         body: str,
         header: str,
         secret: Union[bytes, str],
@@ -237,15 +238,15 @@
         if header != expected:
             raise ValueError("X-Airtable-Content-MAC header failed validation")
         return cls.parse_raw(body)
 
 
 class WebhookNotificationResult(AirtableModel):
     success: bool
-    completion_timestamp: str
+    completion_timestamp: datetime
     duration_ms: float
     retry_number: int
     will_be_retried: Optional[bool] = None
     error: Optional["WebhookError"] = None
 
 
 class WebhookError(AirtableModel):
@@ -296,24 +297,24 @@
     id: str
 
     #: The base64-encoded MAC secret. This should be saved somewhere upon receipt;
     #: there is no way to retrieve it once this object is discarded.
     mac_secret_base64: str
 
     #: The timestamp when the webhook will expire and be deleted.
-    expiration_time: Optional[str]
+    expiration_time: Optional[datetime]
 
 
 class WebhookPayload(AirtableModel):
     """
     Payload returned by :meth:`Webhook.payloads`. See API docs:
     `Webhooks payload <https://airtable.com/developers/web/api/model/webhooks-payload>`_.
     """
 
-    timestamp: str
+    timestamp: datetime
     base_transaction_number: int
     payload_format: str
     action_metadata: Optional["WebhookPayload.ActionMetadata"]
     changed_tables_by_id: Dict[str, "WebhookPayload.TableChanged"] = FD()
     created_tables_by_id: Dict[str, "WebhookPayload.TableCreated"] = FD()
     destroyed_table_ids: List[str] = FL()
     error: Optional[bool]
@@ -368,15 +369,15 @@
         previous: Optional["WebhookPayload.CellValuesByFieldId"]
         unchanged: Optional["WebhookPayload.CellValuesByFieldId"]
 
     class CellValuesByFieldId(AirtableModel):
         cell_values_by_field_id: Dict[str, Any]
 
     class RecordCreated(AirtableModel):
-        created_time: str
+        created_time: datetime
         cell_values_by_field_id: Dict[str, Any]
 
 
 class WebhookPayloads(AirtableModel):
     cursor: int
     might_have_more: bool
     payloads: List[WebhookPayload]
```

### Comparing `pyairtable-2.3.3/pyairtable/orm/model.py` & `pyairtable-3.0.0a1/pyairtable/orm/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from functools import lru_cache
 from typing import Any, Dict, Iterable, List, Optional
 
 from typing_extensions import Self as SelfType
 
 from pyairtable.api.api import Api
 from pyairtable.api.base import Base
@@ -9,17 +10,18 @@
 from pyairtable.api.types import (
     FieldName,
     RecordDict,
     RecordId,
     UpdateRecordDict,
     WritableFields,
 )
-from pyairtable.formulas import OR, STR_VALUE
+from pyairtable.formulas import EQ, OR, RECORD_ID
 from pyairtable.models import Comment
 from pyairtable.orm.fields import AnyField, Field
+from pyairtable.utils import datetime_from_iso_str, datetime_to_iso_str
 
 
 class Model:
     """
     Supports creating ORM-style classes representing Airtable tables.
     For more details, see :ref:`orm`.
 
@@ -27,14 +29,15 @@
     the following attributes:
 
         * ``api_key`` (required) - API key or personal access token.
         * ``base_id`` (required) - Base ID (not name).
         * ``table_name`` (required) - Table ID or name.
         * ``timeout`` - A tuple indicating a connect and read timeout. Defaults to no timeout.
         * ``typecast`` - |kwarg_typecast| Defaults to ``True``.
+        * ``use_field_ids`` - |kwarg_use_field_ids| Defaults to ``False``.
 
     .. code-block:: python
 
         from pyairtable.orm import Model, fields
 
         class Contact(Model):
             first_name = fields.TextField("First Name")
@@ -65,15 +68,15 @@
 
                 @staticmethod
                 def api_key():
                     return get_secret("AIRTABLE_API_KEY")
     """
 
     id: str = ""
-    created_time: str = ""
+    created_time: Optional[datetime.datetime] = None
     _deleted: bool = False
     _fields: Dict[FieldName, Any]
 
     def __init_subclass__(cls, **kwargs: Any):
         cls._validate_class()
         super().__init_subclass__(**kwargs)
 
@@ -179,14 +182,23 @@
             raise ValueError(
                 "Class {cls} fields clash with existing method: {name}".format(
                     cls=cls.__name__, name=overridden
                 )
             )
 
     @classmethod
+    def _get_meta_request_kwargs(cls) -> Dict[str, Any]:
+        return {
+            "user_locale": None,
+            "cell_format": "json",
+            "time_zone": None,
+            "use_field_ids": cls._get_meta("use_field_ids", default=False),
+        }
+
+    @classmethod
     @lru_cache
     def get_api(cls) -> Api:
         return Api(
             api_key=cls._get_meta("api_key", required=True),
             timeout=cls._get_meta("timeout"),
         )
 
@@ -227,15 +239,15 @@
             record = table.create(fields, typecast=self._typecast())
             did_create = True
         else:
             record = table.update(self.id, fields, typecast=self._typecast())
             did_create = False
 
         self.id = record["id"]
-        self.created_time = record["createdTime"]
+        self.created_time = datetime_from_iso_str(record["createdTime"])
         return did_create
 
     def delete(self) -> bool:
         """
         Delete the record.
 
         Raises:
@@ -251,23 +263,25 @@
 
     @classmethod
     def all(cls, **kwargs: Any) -> List[SelfType]:
         """
         Retrieve all records for this model. For all supported
         keyword arguments, see :meth:`Table.all <pyairtable.Table.all>`.
         """
+        kwargs.update(cls._get_meta_request_kwargs())
         table = cls.get_table()
         return [cls.from_record(record) for record in table.all(**kwargs)]
 
     @classmethod
     def first(cls, **kwargs: Any) -> Optional[SelfType]:
         """
         Retrieve the first record for this model. For all supported
         keyword arguments, see :meth:`Table.first <pyairtable.Table.first>`.
         """
+        kwargs.update(cls._get_meta_request_kwargs())
         table = cls.get_table()
         if record := table.first(**kwargs):
             return cls.from_record(record)
         return None
 
     def to_record(self, only_writable: bool = False) -> RecordDict:
         """
@@ -283,35 +297,40 @@
         """
         map_ = self._field_name_descriptor_map()
         fields = {
             field: None if value is None else map_[field].to_record_value(value)
             for field, value in self._fields.items()
             if not (map_[field].readonly and only_writable)
         }
-        return {"id": self.id, "createdTime": self.created_time, "fields": fields}
+        ct = datetime_to_iso_str(self.created_time) if self.created_time else ""
+        return {"id": self.id, "createdTime": ct, "fields": fields}
 
     @classmethod
     def from_record(cls, record: RecordDict) -> SelfType:
         """
         Create an instance from a record dict.
         """
         name_field_map = cls._field_name_descriptor_map()
         # Convert Column Names into model field names
         field_values = {
             # Use field's to_internal_value to cast into model fields
-            field: name_field_map[field].to_internal_value(value)
+            field: (
+                name_field_map[field].to_internal_value(value)
+                if value is not None
+                else None
+            )
             for (field, value) in record["fields"].items()
             # Silently proceed if Airtable returns fields we don't recognize
-            if field in name_field_map and value is not None
+            if field in name_field_map
         }
         # Since instance(**field_values) will perform validation and fail on
         # any readonly fields, instead we directly set instance._fields.
         instance = cls(id=record["id"])
         instance._fields = field_values
-        instance.created_time = record["createdTime"]
+        instance.created_time = datetime_from_iso_str(record["createdTime"])
         return instance
 
     @classmethod
     def from_id(
         cls,
         record_id: RecordId,
         fetch: bool = True,
@@ -358,22 +377,20 @@
             fetch: If ``True``, records will be fetched and field values will be
                 updated. If ``False``, new instances are created with the provided IDs,
                 but field values are unset.
         """
         record_ids = list(record_ids)
         if not fetch:
             return [cls.from_id(record_id, fetch=False) for record_id in record_ids]
-        formula = OR(
-            *[f"RECORD_ID()={STR_VALUE(record_id)}" for record_id in record_ids]
-        )
-        records = [
-            cls.from_record(record) for record in cls.get_table().all(formula=formula)
-        ]
-        records_by_id = {record.id: record for record in records}
+        # There's no endpoint to query multiple IDs at once, but we can use a formula.
+        formula = OR(EQ(RECORD_ID(), record_id) for record_id in record_ids)
+        record_data = cls.get_table().all(formula=formula)
+        records = [cls.from_record(record) for record in record_data]
         # Ensure we return records in the same order, and raise KeyError if any are missing
+        records_by_id = {record.id: record for record in records}
         return [records_by_id[record_id] for record_id in record_ids]
 
     @classmethod
     def batch_save(cls, models: List[SelfType]) -> None:
         """
         Save a list of model instances to the Airtable API with as few
         network requests as possible. Can accept a mixture of new records
@@ -394,17 +411,17 @@
             for model in update_models
             if (record := model.to_record(only_writable=True))
         ]
 
         table = cls.get_table()
         table.batch_update(update_records, typecast=cls._typecast())
         created_records = table.batch_create(create_records, typecast=cls._typecast())
-        for model, created_record in zip(create_models, created_records):
-            model.id = created_record["id"]
-            model.created_time = created_record["createdTime"]
+        for model, record in zip(create_models, created_records):
+            model.id = record["id"]
+            model.created_time = datetime_from_iso_str(record["createdTime"])
 
     @classmethod
     def batch_delete(cls, models: List[SelfType]) -> None:
         """
         Delete a list of model instances from Airtable.
 
         Raises:
```

### Comparing `pyairtable-2.3.3/pyairtable/testing.py` & `pyairtable-3.0.0a1/pyairtable/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,25 @@
     return type + f"{value:0>14}"[:14]
 
 
 def fake_meta(
     base_id: str = "appFakeTestingApp",
     table_name: str = "tblFakeTestingTbl",
     api_key: str = "patFakePersonalAccessToken",
+    use_field_ids: bool = False,
 ) -> type:
     """
     Generate a ``Meta`` class for inclusion in a ``Model`` subclass.
     """
-    attrs = {"base_id": base_id, "table_name": table_name, "api_key": api_key}
+    attrs = {
+        "base_id": base_id,
+        "table_name": table_name,
+        "api_key": api_key,
+        "use_field_ids": use_field_ids,
+    }
     return type("Meta", (), attrs)
 
 
 def fake_record(
     fields: Optional[Fields] = None,
     id: Optional[str] = None,
     **other_fields: Any,
```

### Comparing `pyairtable-2.3.3/pyairtable/utils.py` & `pyairtable-3.0.0a1/pyairtable/utils.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/pyairtable.egg-info/PKG-INFO` & `pyairtable-3.0.0a1/pyairtable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairtable
-Version: 2.3.3
+Version: 3.0.0a1
 Summary: Python Client for the Airtable API
 Home-page: https://github.com/gtalarico/pyairtable
 Author: Gui Talarico
 License: MIT
 Keywords: airtable,api,client,pyairtable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyairtable-2.3.3/pyairtable.egg-info/SOURCES.txt` & `pyairtable-3.0.0a1/pyairtable.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 pyairtable/__init__.py
 pyairtable/_compat.py
 pyairtable/formulas.py
-pyairtable/metadata.py
 pyairtable/py.typed
 pyairtable/testing.py
 pyairtable/utils.py
 pyairtable.egg-info/PKG-INFO
 pyairtable.egg-info/SOURCES.txt
 pyairtable.egg-info/dependency_links.txt
 pyairtable.egg-info/requires.txt
```

### Comparing `pyairtable-2.3.3/setup.cfg` & `pyairtable-3.0.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_api.py` & `pyairtable-3.0.0a1/tests/test_api_api.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_base.py` & `pyairtable-3.0.0a1/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_enterprise.py` & `pyairtable-3.0.0a1/tests/test_api_enterprise.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_retrying.py` & `pyairtable-3.0.0a1/tests/test_api_retrying.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_table.py` & `pyairtable-3.0.0a1/tests/test_api_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from posixpath import join as urljoin
+from unittest import mock
 
 import pytest
 from requests import Request
 from requests_mock import Mocker
 
 from pyairtable import Api, Base, Table
-from pyairtable.metadata import get_table_schema
+from pyairtable.formulas import AND, EQ, Field
 from pyairtable.models.schema import TableSchema
 from pyairtable.testing import fake_id, fake_record
 from pyairtable.utils import chunked
 
 
 @pytest.fixture()
 def table_schema(sample_json, api, base) -> TableSchema:
@@ -255,14 +256,31 @@
         for page in table.iterate():
             pages.append(page)
 
     for n, response in enumerate(mock_response_list):
         assert seq_equals(pages[n], response["records"])
 
 
+def test_iterate__formula_conversion(table):
+    """
+    Test that .iterate() will convert a Formula to a str.
+    """
+    with mock.patch("pyairtable.Api.iterate_requests") as m:
+        table.all(formula=AND(EQ(Field("Name"), "Alice")))
+
+    m.assert_called_once_with(
+        method="get",
+        url=table.url,
+        fallback=mock.ANY,
+        options={
+            "formula": "AND({Name}='Alice')",
+        },
+    )
+
+
 def test_create(table: Table, mock_response_single):
     with Mocker() as mock:
         post_data = mock_response_single["fields"]
         mock.post(
             table.url,
             status_code=201,
             json=mock_response_single,
@@ -438,34 +456,14 @@
 def test_delete_view(table, mock_schema, requests_mock):
     view = table.schema().view("Grid view")
     m = requests_mock.delete(view._url)
     view.delete()
     assert m.call_count == 1
 
 
-def test_deprecated_get_schema_by_id(base, api, requests_mock, sample_json):
-    """
-    Tests the ability to get a table schema by `id` using the deprecated `pyairtable.metadata.get_table_schema`
-    """
-    mock_create = requests_mock.get(
-        base.meta_url("tables"),
-        json=sample_json("BaseSchema"),
-    )
-
-    # Test fetching schema by id
-    table = api.table(base.id, base.tables()[0].id)
-
-    # Deprecated method for getting table's schema
-    table_schema = get_table_schema(table)
-
-    assert table_schema is not None
-    assert table_schema["id"] == table.id
-    assert mock_create.call_count == 2
-
-
 # Helpers
 
 
 def _chunk(iterable, chunk_size):
     for i in range(0, len(iterable), chunk_size):
         yield iterable[i : i + chunk_size]
```

### Comparing `pyairtable-2.3.3/tests/test_api_types.py` & `pyairtable-3.0.0a1/tests/test_api_types.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_api_workspace.py` & `pyairtable-3.0.0a1/tests/test_api_workspace.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_models.py` & `pyairtable-3.0.0a1/tests/test_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime, timezone
 from typing import List
 
 import pytest
 
 from pyairtable.models._base import (
     AirtableModel,
     CanDeleteModel,
@@ -274,7 +275,27 @@
     with pytest.raises(AttributeError) as exc_info:
         Dummy.from_api(data, api, context={"base": None})
 
     assert exc_info.match(
         r'"\'NoneType\' object has no attribute \'id\'"'
         r", \{'base': None, 'dummy': Dummy\(.*\)\}"
     )
+
+
+def test_datetime_conversion(api, requests_mock):
+    """
+    Test that if an AirtableModel field is specified as a datetime,
+    and the input data is provided as a str, we'll convert to a datetime
+    and back to a str when saving.
+    """
+
+    class Dummy(CanUpdateModel, url="{self.id}", writable=["timestamp"]):
+        id: str
+        timestamp: datetime
+
+    data = {"id": "rec000", "timestamp": "2024-01-08T12:34:56Z"}
+    obj = Dummy.from_api(data, api)
+    assert obj.timestamp == datetime(2024, 1, 8, 12, 34, 56, tzinfo=timezone.utc)
+    m = requests_mock.patch(obj._url, json=data)
+    obj.save()
+    assert m.call_count == 1
+    assert m.request_history[0].json() == {"timestamp": "2024-01-08T12:34:56.000Z"}
```

### Comparing `pyairtable-2.3.3/tests/test_models_collaborator.py` & `pyairtable-3.0.0a1/tests/test_models_collaborator.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_models_comment.py` & `pyairtable-3.0.0a1/tests/test_models_comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 def test_save(comment, requests_mock):
     """
     Test that Comment.save() writes the correct payload to the API
     and that it updates the instance with the values in the API response.
     """
     new_text = "This was changed!"
     mentions = {}
-    modified = dict(comment.dict(by_alias=True), mentioned=mentions, text=new_text)
+    modified = dict(comment._raw, mentioned=mentions, text=new_text)
     m = requests_mock.patch(comment._url, json=modified)
 
     comment.text = "Whatever"
     comment.save()
     assert m.call_count == 1
 
     # Ensure we wrote the changed text to the API...
```

### Comparing `pyairtable-2.3.3/tests/test_models_schema.py` & `pyairtable-3.0.0a1/tests/test_models_schema.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_models_webhook.py` & `pyairtable-3.0.0a1/tests/test_models_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,17 @@
         "hmac-sha256=e26da696a90933647bddc83995c3e1e3bb1c3d8ce1ff61cb7469767d50b2b2d4"
     )
 
     body = json.dumps(notification_json)
     notification = WebhookNotification.from_request(body, header, secret)
     assert notification.base.id == "app00000000000000"
     assert notification.webhook.id == "ach00000000000000"
-    assert notification.timestamp == "2022-02-01T21:25:05.663Z"
+    assert notification.timestamp == datetime.datetime(
+        2022, 2, 1, 21, 25, 5, 663000, tzinfo=datetime.timezone.utc
+    )
 
     with pytest.raises(ValueError):
         WebhookNotification.from_request("[1,2,3]", header, secret)
     with pytest.raises(ValueError):
         WebhookNotification.from_request(body, "bad-header", secret)
     with pytest.raises(ValueError):
         WebhookNotification.from_request(body, header, b"bad-secret")
```

### Comparing `pyairtable-2.3.3/tests/test_orm.py` & `pyairtable-3.0.0a1/tests/test_orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import re
-from datetime import datetime
+from datetime import datetime, timezone
 from operator import itemgetter
 from unittest import mock
 
 import pytest
 from requests_mock import Mocker
 
 from pyairtable import Table
 from pyairtable.orm import Model
 from pyairtable.orm import fields as f
 from pyairtable.testing import fake_meta, fake_record
+from pyairtable.utils import datetime_to_iso_str
+
+NOW = datetime.now().isoformat() + "Z"
 
 
 class Address(Model):
     Meta = fake_meta(table_name="Address")
     street = f.TextField("Street")
-    number = f.TextField("Number")
+    number = f.IntegerField("Number")
 
 
 class Contact(Model):
     Meta = fake_meta(table_name="Contact")
     first_name = f.TextField("First Name")
     last_name = f.TextField("Last Name")
     email = f.EmailField("Email")
@@ -40,60 +43,61 @@
 
     # attribute look up
     assert contact.first_name == "Gui"
     assert not contact.id
 
     # save
     with mock.patch.object(Table, "create") as m_save:
-        m_save.return_value = {"id": "id", "createdTime": "time"}
+        m_save.return_value = {"id": "id", "createdTime": NOW}
         contact.save()
 
     assert m_save.called
     assert contact.id == "id"
+    assert contact.created_time.tzinfo is timezone.utc
 
     # delete
     with mock.patch.object(Table, "delete") as m_delete:
         m_delete.return_value = {"deleted": True}
         contact.delete()
 
     assert m_delete.called
 
     # cannot save a deleted record
     with pytest.raises(RuntimeError):
         contact.save()
 
     record = contact.to_record()
     assert record["id"] == contact.id
-    assert record["createdTime"] == contact.created_time
+    assert record["createdTime"] == datetime_to_iso_str(contact.created_time)
     assert record["fields"]["First Name"] == contact.first_name
 
 
 def test_unsupplied_fields():
     """
     Test that we can create a record without fields.
     """
     a = Address()
     assert a.number is None
-    assert a.street is None
+    assert a.street == ""
 
 
 def test_null_fields():
     """
     Test that we can create a record with null fields.
     """
     a = Address(number=None, street=None)
     assert a.number is None
-    assert a.street is None
+    assert a.street == ""
 
 
 def test_first():
     with mock.patch.object(Table, "first") as m_first:
         m_first.return_value = {
             "id": "recwnBLPIeQJoYVt4",
-            "createdTime": "",
+            "createdTime": NOW,
             "fields": {
                 "First Name": "X",
                 "Created At": "2014-09-05T12:34:56.000Z",
             },
         }
         contact = Contact.first()
 
@@ -109,15 +113,15 @@
 
 
 def test_from_record():
     # Fetch = True
     with mock.patch.object(Table, "get") as m_get:
         m_get.return_value = {
             "id": "recwnBLPIeQJoYVt4",
-            "createdTime": "",
+            "createdTime": NOW,
             "fields": {
                 "First Name": "X",
                 "Birthday": None,
                 "Created At": "2014-09-05T12:34:56.000Z",
             },
         }
         contact = Contact.from_id("recwnBLPIeQJoYVt4")
@@ -138,15 +142,15 @@
     """
     Test that we do not attempt to save readonly fields to the API,
     but we can retrieve readonly fields and set them on instantiation.
     """
 
     record = {
         "id": "recwnBLPIeQJoYVt4",
-        "createdTime": datetime.utcnow().isoformat(),
+        "createdTime": datetime.now(timezone.utc).isoformat(),
         "fields": {
             "Birthday": "1970-01-01",
             "Age": 57,
         },
     }
 
     contact = Contact.from_record(record)
@@ -158,15 +162,15 @@
     # We should not pass 'Age' to the API
     m_update.assert_called_once_with(
         contact.id, {"Birthday": "2000-01-01"}, typecast=True
     )
 
 
 def test_linked_record():
-    record = {"id": "recFake", "createdTime": "", "fields": {"Street": "A"}}
+    record = {"id": "recFake", "createdTime": NOW, "fields": {"Street": "A"}}
     address = Address.from_id("recFake", fetch=False)
 
     # Id Reference
     contact = Contact(address=[address])
     assert contact.address[0].id == address.id
     assert not contact.address[0].street
 
@@ -184,15 +188,15 @@
     Test that we can call Model.save() on a model with a non-lazy linked field,
     whether we've already accessed the field contents or not.
 
     Accessing the linked field converts its internal representation from
     record IDs into instances of the model. This could interfere with save(),
     so this test ensures we don't regress the capability.
     """
-    address_json = fake_record(Number="123", Street="Fake St")
+    address_json = fake_record(Number=123, Street="Fake St")
     address_id = address_json["id"]
     address_url_re = re.escape(Address.get_table().url + "?filterByFormula=")
     contact_json = fake_record(Email="alice@example.com", Link=[address_id])
     contact_id = contact_json["id"]
     contact_url = Contact.get_table().record_url(contact_id)
     contact_url_re = re.escape(Contact.get_table().url + "?filterByFormula=")
     requests_mock.get(re.compile(address_url_re), json={"records": [address_json]})
@@ -242,15 +246,15 @@
     Test that Model methods which fetch data from the Airtable API will
     ignore any fields which are missing from the Model definition.
 
     See https://github.com/gtalarico/pyairtable/issues/190
     """
 
     record = fake_record(
-        Number="123",
+        Number=123,
         Street="Fake St",
         City="Springfield",
         State="IL",
     )
 
     requests_mock.get(
         Address.get_table().url,
@@ -261,57 +265,57 @@
         Address.get_table().record_url(record["id"]),
         status_code=200,
         json=record,
     )
 
     _, get_model_instance = test_case
     instance = get_model_instance(Address, record["id"])
-    assert instance.to_record()["fields"] == {"Number": "123", "Street": "Fake St"}
+    assert instance.to_record()["fields"] == {"Number": 123, "Street": "Fake St"}
 
 
 @mock.patch("pyairtable.Table.batch_create")
 @mock.patch("pyairtable.Table.batch_update")
 def test_batch_save(mock_update, mock_create):
     """
     Test that we can pass multiple unsaved Model instances (or dicts) to batch_save
     and it will create or update them all in as few requests as possible.
     """
-    addr1 = Address(number="123", street="Fake St")
-    addr2 = Address(number="456", street="Fake St")
+    addr1 = Address(number=123, street="Fake St")
+    addr2 = Address(number=456, street="Fake St")
     addr3 = Address.from_record(
         {
             "id": "recExistingRecord",
-            "createdTime": datetime.utcnow().isoformat(),
-            "fields": {"Number": "789", "Street": "Fake St"},
+            "createdTime": datetime.now(timezone.utc).isoformat(),
+            "fields": {"Number": 789, "Street": "Fake St"},
         }
     )
 
     mock_create.return_value = [
-        fake_record(id="abc", Number="123", Street="Fake St"),
-        fake_record(id="def", Number="456", Street="Fake St"),
+        fake_record(id="abc", Number=123, Street="Fake St"),
+        fake_record(id="def", Number=456, Street="Fake St"),
     ]
 
     # Just like model.save(), Model.batch_save() will set IDs on new records.
     Address.batch_save([addr1, addr2, addr3])
     assert addr1.id == "rec00000000000abc"
     assert addr2.id == "rec00000000000def"
     assert addr3.id == "recExistingRecord"
 
     mock_create.assert_called_once_with(
         [
-            {"Number": "123", "Street": "Fake St"},
-            {"Number": "456", "Street": "Fake St"},
+            {"Number": 123, "Street": "Fake St"},
+            {"Number": 456, "Street": "Fake St"},
         ],
         typecast=True,
     )
     mock_update.assert_called_once_with(
         [
             {
                 "id": "recExistingRecord",
-                "fields": {"Number": "789", "Street": "Fake St"},
+                "fields": {"Number": 789, "Street": "Fake St"},
             },
         ],
         typecast=True,
     )
 
 
 @mock.patch("pyairtable.Table.batch_create")
@@ -362,16 +366,16 @@
 @mock.patch("pyairtable.Table.batch_delete")
 def test_batch_delete__unsaved_record(mock_delete):
     """
     Test that we get a ValueError (and make no deletions) if Model.batch_delete
     receives any models which have not been created yet.
     """
     addresses = [
-        Address.from_record(fake_record(Number="1", Street="Fake St")),
-        Address(number="2", street="Fake St"),
+        Address.from_record(fake_record(Number=1, Street="Fake St")),
+        Address(number=2, street="Fake St"),
     ]
     with pytest.raises(ValueError):
         Address.batch_delete(addresses)
 
     assert mock_delete.call_count == 0
```

### Comparing `pyairtable-2.3.3/tests/test_orm_fields.py` & `pyairtable-3.0.0a1/tests/test_orm_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import datetime
 import operator
 import re
+from unittest import mock
 
 import pytest
+from requests_mock import NoMockAddress
 
+from pyairtable.formulas import OR, RECORD_ID
 from pyairtable.orm import fields as f
 from pyairtable.orm.model import Model
 from pyairtable.testing import (
     fake_attachment,
     fake_id,
     fake_meta,
     fake_record,
     fake_user,
 )
+from pyairtable.utils import datetime_to_iso_str
 
 DATE_S = "2023-01-01"
 DATE_V = datetime.date(2023, 1, 1)
 DATETIME_S = "2023-04-12T09:30:00.000Z"
 DATETIME_V = datetime.datetime(2023, 4, 12, 9, 30, 0, tzinfo=datetime.timezone.utc)
 
 
+class Dummy(Model):
+    Meta = fake_meta()
+
+
 def test_field():
     class T:
         name = f.Field("Name")
 
     t = T()
     t.name = "x"
     assert t.name == "x"
@@ -66,25 +74,32 @@
             f.LookupField[dict]("Items", validate_type=False),
             "LookupField('Items', readonly=True, validate_type=False)",
         ),
         (
             f.LinkField("Records", type("TestModel", (Model,), {"Meta": fake_meta()})),
             "LinkField('Records', model=<class 'test_orm_fields.TestModel'>, validate_type=True, readonly=False, lazy=False)",
         ),
+        (
+            f.SingleLinkField(
+                "Records", type("TestModel", (Model,), {"Meta": fake_meta()})
+            ),
+            "SingleLinkField('Records', model=<class 'test_orm_fields.TestModel'>, validate_type=True, readonly=False, lazy=False, raise_if_many=False)",
+        ),
     ],
 )
 def test_repr(instance, expected):
     assert repr(instance) == expected
 
 
 @pytest.mark.parametrize(
     argnames=("field_type", "default_value"),
     argvalues=[
         (f.Field, None),
         (f.CheckboxField, False),
+        (f.TextField, ""),
         (f.LookupField, []),
         (f.AttachmentsField, []),
         (f.MultipleCollaboratorsField, []),
         (f.MultipleSelectField, []),
     ],
 )
 def test_orm_missing_values(field_type, default_value):
@@ -96,52 +111,75 @@
     class T(Model):
         Meta = fake_meta()
         the_field = field_type("Field Name")
 
     t = T()
     assert t.the_field == default_value
 
+    t = T.from_record(fake_record({"Field Name": None}))
+    assert t.the_field == default_value
+
 
 # Mapping from types to a test value for that type.
 TYPE_VALIDATION_TEST_VALUES = {
-    **{t: t() for t in (str, bool, list, dict)},
+    str: "some value",
+    bool: False,
+    list: [],
+    dict: {},
     int: 1,  # cannot use int() because RatingField requires value >= 1
     float: 1.0,  # cannot use float() because RatingField requires value >= 1
     datetime.date: datetime.date.today(),
     datetime.datetime: datetime.datetime.now(),
     datetime.timedelta: datetime.timedelta(seconds=1),
 }
 
 
 @pytest.mark.parametrize(
     "test_case",
     [
         (f.Field, tuple(TYPE_VALIDATION_TEST_VALUES)),
-        (f.TextField, str),
-        (f.IntegerField, int),
-        (f.RichTextField, str),
-        (f.DatetimeField, datetime.datetime),
-        (f.TextField, str),
-        (f.CheckboxField, bool),
+        (f.AttachmentsField, list),
         (f.BarcodeField, dict),
-        (f.NumberField, (int, float)),
-        (f.PhoneNumberField, str),
+        (f.CheckboxField, bool),
+        (f.CollaboratorField, dict),
+        (f.CurrencyField, (int, float)),
+        (f.DateField, (datetime.date, datetime.datetime)),
+        (f.DatetimeField, datetime.datetime),
         (f.DurationField, datetime.timedelta),
-        (f.RatingField, int),
-        (f.UrlField, str),
+        (f.EmailField, str),
+        (f.FloatField, float),
+        (f.IntegerField, int),
+        (f.MultipleCollaboratorsField, list),
         (f.MultipleSelectField, list),
+        (f.NumberField, (int, float)),
         (f.PercentField, (int, float)),
-        (f.DateField, (datetime.date, datetime.datetime)),
-        (f.FloatField, float),
-        (f.CollaboratorField, dict),
+        (f.PhoneNumberField, str),
+        (f.RatingField, int),
+        (f.RichTextField, str),
         (f.SelectField, str),
-        (f.EmailField, str),
-        (f.AttachmentsField, list),
-        (f.MultipleCollaboratorsField, list),
-        (f.CurrencyField, (int, float)),
+        (f.TextField, str),
+        (f.TextField, str),
+        (f.UrlField, str),
+        (f.RequiredBarcodeField, dict),
+        (f.RequiredCollaboratorField, dict),
+        (f.RequiredCurrencyField, (int, float)),
+        (f.RequiredDateField, (datetime.date, datetime.datetime)),
+        (f.RequiredDatetimeField, datetime.datetime),
+        (f.RequiredDurationField, datetime.timedelta),
+        (f.RequiredFloatField, float),
+        (f.RequiredIntegerField, int),
+        (f.RequiredNumberField, (int, float)),
+        (f.RequiredPercentField, (int, float)),
+        (f.RequiredRatingField, int),
+        (f.RequiredSelectField, str),
+        (f.RequiredEmailField, str),
+        (f.RequiredPhoneNumberField, str),
+        (f.RequiredRichTextField, str),
+        (f.RequiredTextField, str),
+        (f.RequiredUrlField, str),
     ],
     ids=operator.itemgetter(0),
 )
 def test_type_validation(test_case):
     """
     Test that attempting to assign the wrong type of value to a field
     will throw TypeError, but the right kind of value will work.
@@ -224,14 +262,17 @@
         (f.ButtonField, {"label": "Click me!"}),
         (f.LookupField, ["any", "values"]),
         (f.CreatedByField, fake_user()),
         (f.LastModifiedByField, fake_user()),
         # If a 3-tuple, we should be able to convert API -> ORM values.
         (f.CreatedTimeField, DATETIME_S, DATETIME_V),
         (f.LastModifiedTimeField, DATETIME_S, DATETIME_V),
+        # We also want to test the not-null versions of these fields
+        (f.RequiredAITextField, {"state": "empty", "isStale": True, "value": None}),
+        (f.RequiredCountField, 1),
     ],
     ids=operator.itemgetter(0),
 )
 def test_readonly_fields(test_case):
     """
     Test that a readonly field cannot be overwritten.
     """
@@ -272,20 +313,39 @@
         (f.AttachmentsField, [fake_attachment(), fake_attachment()]),
         (f.MultipleSelectField, ["any", "values"]),
         (f.MultipleCollaboratorsField, [fake_user(), fake_user()]),
         (f.BarcodeField, {"type": "upce", "text": "084114125538"}),
         (f.PercentField, 0.5),
         (f.PhoneNumberField, "+49 40-349180"),
         (f.RichTextField, "Check out [Airtable](www.airtable.com)"),
+        (f.SelectField, ""),
         (f.SelectField, "any value"),
         (f.UrlField, "www.airtable.com"),
+        (f.RequiredNumberField, 1),
+        (f.RequiredNumberField, 1.5),
+        (f.RequiredIntegerField, 1),
+        (f.RequiredFloatField, 1.5),
+        (f.RequiredRatingField, 1),
+        (f.RequiredCurrencyField, 1.05),
+        (f.RequiredCollaboratorField, {"id": "usrFakeUserId", "email": "x@y.com"}),
+        (f.RequiredBarcodeField, {"type": "upce", "text": "084114125538"}),
+        (f.RequiredPercentField, 0.5),
+        (f.RequiredSelectField, "any value"),
+        (f.RequiredEmailField, "any value"),
+        (f.RequiredPhoneNumberField, "any value"),
+        (f.RequiredRichTextField, "any value"),
+        (f.RequiredTextField, "any value"),
+        (f.RequiredUrlField, "any value"),
         # If a 3-tuple, we should be able to convert API -> ORM values.
         (f.DateField, DATE_S, DATE_V),
-        (f.DurationField, 100.5, datetime.timedelta(seconds=100, microseconds=500000)),
         (f.DatetimeField, DATETIME_S, DATETIME_V),
+        (f.DurationField, 100.5, datetime.timedelta(seconds=100, microseconds=500000)),
+        (f.RequiredDateField, DATE_S, DATE_V),
+        (f.RequiredDatetimeField, DATETIME_S, DATETIME_V),
+        (f.RequiredDurationField, 100, datetime.timedelta(seconds=100)),
     ],
     ids=operator.itemgetter(0),
 )
 def test_writable_fields(test_case):
     """
     Test that the ORM does not modify values that can be persisted as-is.
     """
@@ -309,26 +369,128 @@
     from_init = T(the_field=orm_value)
     assert from_init.the_field == orm_value
 
     existing_obj = T.from_record(fake_record({"Field Name": api_value}))
     assert existing_obj.the_field == orm_value
 
 
+@pytest.mark.parametrize(
+    "field_type",
+    [
+        f.Field,
+        f.AITextField,
+        f.AttachmentsField,
+        f.BarcodeField,
+        f.CheckboxField,
+        f.CollaboratorField,
+        f.CountField,
+        f.CurrencyField,
+        f.DateField,
+        f.DatetimeField,
+        f.DurationField,
+        f.EmailField,
+        f.ExternalSyncSourceField,
+        f.FloatField,
+        f.IntegerField,
+        f.LastModifiedByField,
+        f.LastModifiedTimeField,
+        f.LookupField,
+        f.MultipleCollaboratorsField,
+        f.MultipleSelectField,
+        f.NumberField,
+        f.NumberField,
+        f.PercentField,
+        f.PhoneNumberField,
+        f.RatingField,
+        f.RichTextField,
+        f.SelectField,
+        f.TextField,
+        f.UrlField,
+    ],
+)
+def test_accepts_null(field_type):
+    """
+    Test field types that allow null values from Airtable.
+    """
+
+    class T(Model):
+        Meta = fake_meta()
+        the_field = field_type("Field Name")
+
+    obj = T()
+    assert not obj.the_field
+
+
+@pytest.mark.parametrize(
+    "field_type",
+    [
+        f.AutoNumberField,
+        f.ButtonField,
+        f.CreatedByField,
+        f.CreatedTimeField,
+        f.RequiredAITextField,
+        f.RequiredBarcodeField,
+        f.RequiredCollaboratorField,
+        f.RequiredCountField,
+        f.RequiredCurrencyField,
+        f.RequiredDateField,
+        f.RequiredDatetimeField,
+        f.RequiredDurationField,
+        f.RequiredEmailField,
+        f.RequiredFloatField,
+        f.RequiredIntegerField,
+        f.RequiredNumberField,
+        f.RequiredPercentField,
+        f.RequiredPhoneNumberField,
+        f.RequiredRatingField,
+        f.RequiredRichTextField,
+        f.RequiredSelectField,
+        f.RequiredTextField,
+        f.RequiredUrlField,
+    ],
+)
+def test_rejects_null(field_type):
+    """
+    Test field types that do not allow null values from Airtable.
+    """
+
+    class T(Model):
+        Meta = fake_meta()
+        the_field = field_type("Field Name")
+
+    obj = T()
+    with pytest.raises(f.MissingValue):
+        obj.the_field
+    with pytest.raises(f.MissingValue):
+        obj.the_field = None
+    with pytest.raises(f.MissingValue):
+        T(the_field=None)
+
+
 def test_completeness():
     """
     Ensure that we test conversion of all readonly and writable fields.
     """
-    assert_all_fields_tested_by(test_writable_fields, test_readonly_fields)
+    assert_all_fields_tested_by(
+        test_writable_fields,
+        test_readonly_fields,
+        exclude=(f.LinkField, f.SingleLinkField),
+    )
     assert_all_fields_tested_by(
         test_type_validation,
-        exclude=f.READONLY_FIELDS | {f.LinkField},
+        exclude=f.READONLY_FIELDS | {f.LinkField, f.SingleLinkField},
+    )
+    assert_all_fields_tested_by(
+        test_accepts_null,
+        test_rejects_null,
+        exclude={f.LinkField, f.SingleLinkField},
     )
 
 
-def assert_all_fields_tested_by(*test_fns, exclude=(f.Field, f.LinkField)):
+def assert_all_fields_tested_by(*test_fns, exclude=()):
     """
     Allows meta-tests that fail if any new Field classes appear in pyairtable.orm.fields
     which are not covered by one of a few basic tests. This is intended to help remind
     us as contributors to test our edge cases :)
     """
 
     def extract_fields(obj):
@@ -431,20 +593,21 @@
         items = f._ListField("Items", str)
 
     t = T()
     with pytest.raises(TypeError):
         t.items = "hello!"
 
 
-def test_link_field_must_link_to_model():
+@pytest.mark.parametrize("cls", (f.LinkField, f.SingleLinkField))
+def test_link_field_must_link_to_model(cls):
     """
     Tests that a LinkField cannot link to an arbitrary type.
     """
     with pytest.raises(TypeError):
-        f.LinkField("Field Name", model=dict)
+        cls("Field Name", model=dict)
 
 
 def test_link_field():
     """
     Test basic interactions and type checking for LinkField.
     """
 
@@ -466,18 +629,14 @@
     with pytest.raises(TypeError):
         author.books = [1, 2, 3]
 
     with pytest.raises(TypeError):
         author.books = -1
 
 
-class Dummy(Model):
-    Meta = fake_meta()
-
-
 def test_link_field__linked_model():
     """
     Test the various ways of specifying a linked model for the LinkField.
     """
 
     class HasLinks(Model):
         Meta = fake_meta()
@@ -585,14 +744,162 @@
     assert mock_list.call_count == 2
     assert len(person.friends) == len(friend_ids)
     assert [friend.id for friend in person.friends] == friend_ids
     # Make sure we didn't keep calling the API on every `person.friends`
     assert mock_list.call_count == 2
 
 
+def test_single_link_field():
+    class Author(Model):
+        Meta = fake_meta()
+        name = f.TextField("Name")
+
+    class Book(Model):
+        Meta = fake_meta()
+        author = f.SingleLinkField("Author", Author, lazy=True)
+
+    assert Book.author.linked_model is Author
+
+    book = Book()
+    assert book.author is None
+
+    with pytest.raises(TypeError):
+        book.author = [Author()]
+
+    with pytest.raises(TypeError):
+        book.author = []
+
+    alice = Author.from_record(fake_record(Name="Alice"))
+    book.author = alice
+
+    with mock.patch("pyairtable.Table.get", return_value=alice.to_record()) as m:
+        book.author.fetch()
+        m.assert_called_once_with(alice.id)
+
+    assert book.author.id == alice.id
+    assert book.author.name == "Alice"
+
+    book.author = (bob := Author(name="Bob"))
+    assert not book.author.exists()
+    assert book.author.name == "Bob"
+
+    with mock.patch("pyairtable.Table.create", return_value=fake_record()) as m:
+        book.author.save()
+        m.assert_called_once_with({"Name": "Bob"}, typecast=True)
+
+    with mock.patch("pyairtable.Table.create", return_value=fake_record()) as m:
+        book.save()
+        m.assert_called_once_with({"Author": [bob.id]}, typecast=True)
+
+    with mock.patch("pyairtable.Table.update", return_value=book.to_record()) as m:
+        book.author = None
+        book.save()
+        m.assert_called_once_with(book.id, {"Author": None}, typecast=True)
+
+
+def test_single_link_field__multiple_values():
+    """
+    Test the behavior of SingleLinkField when the Airtable API
+    returns multiple values.
+    """
+
+    class Author(Model):
+        Meta = fake_meta()
+        name = f.TextField("Name")
+
+    class Book(Model):
+        Meta = fake_meta()
+        author = f.SingleLinkField("Author", Author)
+
+    records = [fake_record(Name=f"Author {n+1}") for n in range(3)]
+    a1, a2, a3 = [r["id"] for r in records]
+
+    # if Airtable sends back multiple IDs, we'll only retrieve the first one.
+    book = Book.from_record(fake_record(Author=[a1, a2, a3]))
+    with mock.patch("pyairtable.Table.all", return_value=records) as m:
+        book.author
+        m.assert_called_once_with(formula=OR(RECORD_ID().eq(records[0]["id"])))
+
+    assert book.author.id == a1
+    assert book.author.name == "Author 1"
+    assert book._fields["Author"][1:] == [a2, a3]  # not converted to models
+
+    # if book.author.__set__ not called, the entire list will be sent back to the API
+    with mock.patch("pyairtable.Table.update", return_value=book.to_record()) as m:
+        book.save()
+        m.assert_called_once_with(book.id, {"Author": [a1, a2, a3]}, typecast=True)
+
+    # if we modify the field value, it will drop items 2-N
+    book.author = Author.from_record(fake_record())
+    with mock.patch("pyairtable.Table.update", return_value=book.to_record()) as m:
+        book.save()
+        m.assert_called_once_with(book.id, {"Author": [book.author.id]}, typecast=True)
+
+
+def test_single_link_field__raise_if_many():
+    """
+    Test that passing raise_if_many=True to SingleLinkField will cause an exception
+    to be raised if (1) the field receives multiple values and (2) is accessed.
+    """
+
+    class Author(Model):
+        Meta = fake_meta()
+        name = f.TextField("Name")
+
+    class Book(Model):
+        Meta = fake_meta()
+        author = f.SingleLinkField("Author", Author, raise_if_many=True)
+
+    book = Book.from_record(fake_record(Author=[fake_id(), fake_id()]))
+    with pytest.raises(f.MultipleValues):
+        book.author
+
+
+@pytest.mark.parametrize("field_type", (f.LinkField, f.SingleLinkField))
+def test_link_field__populate(field_type, requests_mock):
+    """
+    Test that implementers can use Model.link_field.populate(instance) to control
+    whether loading happens lazy or non-lazy at runtime.
+    """
+
+    class Linked(Model):
+        Meta = fake_meta()
+        name = f.TextField("Name")
+
+    class T(Model):
+        Meta = fake_meta()
+        link = field_type("Link", Linked)
+
+    links = [fake_record(id=n, Name=f"link{n}") for n in range(1, 4)]
+    link_ids = [link["id"] for link in links]
+    obj = T.from_record(fake_record(Link=link_ids[:]))
+    assert obj._fields.get("Link") == link_ids
+    assert obj._fields.get("Link") is not link_ids
+
+    # calling the record directly will attempt network traffic
+    with pytest.raises(NoMockAddress):
+        obj.link
+
+    # on a non-lazy field, we can still call .populate() to load it lazily
+    T.link.populate(obj, lazy=True)
+
+    if field_type is f.SingleLinkField:
+        assert isinstance(obj.link, Linked)
+        assert obj.link.id == links[0]["id"]
+        assert obj.link.name == ""
+    else:
+        assert isinstance(obj.link[0], Linked)
+        assert link_ids == [link.id for link in obj.link]
+        assert all(link.name == "" for link in obj.link)
+
+    # calling .populate() on the wrong model raises an exception
+    with pytest.raises(RuntimeError):
+        T.link.populate(Linked())
+
+
 def test_lookup_field():
     class T:
         items = f.LookupField("Items")
 
     lookup_from_airtable = ["Item 1", "Item 2", "Item 3"]
     rv_list = T.items.to_internal_value(lookup_from_airtable)
     rv_json = T.items.to_record_value(rv_list)
@@ -646,15 +953,15 @@
         dt = f.DatetimeField("dt")
 
     obj = M.from_record(fake_record(dt="2024-02-29T12:34:56Z"))
 
     def patch_callback(request, context):
         return {
             "id": obj.id,
-            "createdTime": obj.created_time,
+            "createdTime": datetime_to_iso_str(obj.created_time),
             "fields": request.json()["fields"],
         }
 
     m = requests_mock.patch(M.get_table().record_url(obj.id), json=patch_callback)
 
     # Test that we parse the "Z" into UTC correctly
     assert obj.dt.date() == datetime.date(2024, 2, 29)
@@ -675,7 +982,33 @@
 
     # Test that a timezone-unaware datetime is passed as-is to Airtable.
     # This behavior will vary depending on how the field is configured.
     # See https://airtable.com/developers/web/api/field-model#dateandtime
     obj.dt = datetime.datetime(2024, 3, 1, 11, 22, 33)
     obj.save()
     assert m.last_request.json()["fields"]["dt"] == "2024-03-01T11:22:33.000"
+
+
+@pytest.mark.parametrize(
+    "fields,expected",
+    [
+        ({}, None),
+        ({"Field": None}, None),
+        ({"Field": ""}, ""),
+        ({"Field": "xyz"}, "xyz"),
+    ],
+)
+def test_select_field(fields, expected):
+    """
+    Test that select field distinguishes between empty string and None.
+    """
+
+    class T(Model):
+        Meta = fake_meta()
+        the_field = f.SelectField("Field")
+
+    obj = T.from_record(fake_record(**fields))
+    assert obj.the_field == expected
+
+    with mock.patch("pyairtable.Table.update", return_value=obj.to_record()) as m:
+        obj.save()
+        m.assert_called_once_with(obj.id, fields, typecast=True)
```

### Comparing `pyairtable-2.3.3/tests/test_orm_model.py` & `pyairtable-3.0.0a1/tests/test_orm_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import partial
 from unittest import mock
 
 import pytest
+from requests_mock import Mocker
 
 from pyairtable.orm import Model
 from pyairtable.orm import fields as f
 from pyairtable.testing import fake_id, fake_meta, fake_record
 
 
 @pytest.fixture(autouse=True)
@@ -86,14 +87,20 @@
 
 class FakeModel(Model):
     Meta = fake_meta()
     one = f.TextField("one")
     two = f.TextField("two")
 
 
+class FakeModelByIds(Model):
+    Meta = fake_meta(use_field_ids=True, table_name="Apartments")
+    Name = f.TextField("fld1VnoyuotSTyxW1")
+    Age = f.NumberField("fld2VnoyuotSTy4g6")
+
+
 def test_repr():
     record = fake_record()
     assert repr(FakeModel.from_record(record)) == f"<FakeModel id='{record['id']}'>"
     assert repr(FakeModel()) == "<unsaved FakeModel>"
 
 
 def test_delete():
@@ -158,41 +165,110 @@
     fake_contact = fake_record(Name="Alice")
     mock_get.return_value = fake_contact
     contact = Contact.from_id(fake_contact["id"])
     assert contact.id == fake_contact["id"]
     assert contact.name == "Alice"
 
 
-@mock.patch("pyairtable.Table.all")
-def test_from_ids(mock_all):
+@mock.patch("pyairtable.Api.iterate_requests")
+def test_from_ids(mock_api):
     fake_records = [fake_record() for _ in range(10)]
-    mock_all.return_value = fake_records
+    mock_api.return_value = [{"records": fake_records}]
 
     fake_ids = [record["id"] for record in fake_records]
     contacts = FakeModel.from_ids(fake_ids)
-    mock_all.assert_called_once()
+    mock_api.assert_called_once_with(
+        method="get",
+        url=FakeModel.get_table().url,
+        fallback=("post", FakeModel.get_table().url + "/listRecords"),
+        options={
+            "formula": "OR(%s)" % ", ".join(f"RECORD_ID()='{id}'" for id in fake_ids)
+        },
+    )
     assert len(contacts) == len(fake_records)
     assert {c.id for c in contacts} == {r["id"] for r in fake_records}
 
+
+@mock.patch("pyairtable.Table.all")
+def test_from_ids__invalid_id(mock_all):
     # Should raise KeyError because of the invalid ID
-    mock_all.reset_mock()
     with pytest.raises(KeyError):
-        FakeModel.from_ids(fake_ids + ["recDefinitelyNotValid"])
+        FakeModel.from_ids(["recDefinitelyNotValid"])
     mock_all.assert_called_once()
 
 
 @mock.patch("pyairtable.Table.all")
 def test_from_ids__no_fetch(mock_all):
     fake_ids = [fake_id() for _ in range(10)]
     contacts = FakeModel.from_ids(fake_ids, fetch=False)
     assert mock_all.call_count == 0
     assert len(contacts) == 10
     assert set(contact.id for contact in contacts) == set(fake_ids)
 
 
+@pytest.mark.parametrize(
+    "methodname,returns",
+    (
+        ("all", [fake_record(), fake_record(), fake_record()]),
+        ("first", fake_record()),
+    ),
+)
+def test_passthrough(methodname, returns):
+    """
+    Test that .all() and .first() pass through whatever they get.
+    """
+    with mock.patch(
+        f"pyairtable.Table.{methodname}", return_value=returns
+    ) as mock_endpoint:
+        method = getattr(FakeModel, methodname)
+        method(a=1, b=2, c=3)
+    mock_endpoint.assert_called_once_with(
+        a=1,
+        b=2,
+        c=3,
+        use_field_ids=getattr(FakeModel.Meta, "use_field_ids", False),
+        user_locale=None,
+        time_zone=None,
+        cell_format="json",
+    )
+
+
+@pytest.fixture
+def fake_records_by_id():
+    return {
+        "records": [
+            fake_record(fld1VnoyuotSTyxW1="Alice", fld2VnoyuotSTy4g6=25),
+            fake_record(Name="Jack", Age=30),
+        ]
+    }
+
+
+def test_get_fields_by_id(fake_records_by_id):
+    """
+    Test that we can get fields by their field ID.
+    """
+    with Mocker() as mock:
+        mock.get(
+            f"{FakeModelByIds.get_table().url}?&returnFieldsByFieldId=1&cellFormat=json",
+            json=fake_records_by_id,
+            complete_qs=True,
+            status_code=200,
+        )
+        fake_models = FakeModelByIds.all()
+
+    assert fake_models[0].Name == "Alice"
+    assert fake_models[0].Age == 25
+
+    assert fake_models[1].Name != "Jack"
+    assert fake_models[1].Age != 30
+
+    with pytest.raises(KeyError):
+        _ = getattr(fake_models[1], fake_records_by_id[0]["Age"])
+
+
 def test_dynamic_model_meta():
     """
     Test that we can provide callables in our Meta class to provide
     the access token, base ID, and table name at runtime. Also ensure
     that callable Meta attributes don't get called until they're needed.
     """
     data = {
```

### Comparing `pyairtable-2.3.3/tests/test_params.py` & `pyairtable-3.0.0a1/tests/test_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def test_params_integration(table, mock_records, mock_response_iterator):
     params = {
         "max_records": 1,
         "view": "View",
         "sort": ["Name"],
         "fields": ["Name", "Age"],
-        "return_fields_by_field_id": True,
+        "use_field_ids": True,
     }
     with Mocker() as m:
         url_params = (
             "maxRecords=1"
             "&sort%5B0%5D%5Bdirection%5D=asc"
             "&sort%5B0%5D%5Bfield%5D=Name"
             "&view=View"
@@ -96,17 +96,17 @@
         ["user_locale", "en-US", "?userLocale=en-US"],
         [
             "time_zone",
             "America/Chicago",
             "?timeZone=America%2FChicago",
             # '?timeZone=America/Chicago'
         ],
-        ["return_fields_by_field_id", True, "?returnFieldsByFieldId=1"],
-        ["return_fields_by_field_id", 1, "?returnFieldsByFieldId=1"],
-        ["return_fields_by_field_id", False, "?returnFieldsByFieldId=0"],
+        ["use_field_ids", True, "?returnFieldsByFieldId=1"],
+        ["use_field_ids", 1, "?returnFieldsByFieldId=1"],
+        ["use_field_ids", False, "?returnFieldsByFieldId=0"],
         # TODO
         # [
         #     {"sort": [("Name", "desc"), ("Phone", "asc")]},
         #     # "?sort[0][direction]=desc&sort[0][field]=Name&sort[1][direction]=asc&sort[1][field]=Phone"
         #     "?sort%5B0%5D%5Bdirection%5D=desc&sort%5B0%5D%5Bfield%5D=Name&sort%5B1%5D%5Bdirection%5D=asc&sort%5B1%5D%5Bfield%5D=Phone",
         # ],
     ],
@@ -159,17 +159,17 @@
                 "sort": [
                     {"field": "Name", "direction": "asc"},
                     {"field": "Phone", "direction": "desc"},
                 ]
             },
         ],
         ["cell_format", "string", {"cellFormat": "string"}],
-        ["return_fields_by_field_id", True, {"returnFieldsByFieldId": True}],
-        ["return_fields_by_field_id", 1, {"returnFieldsByFieldId": True}],
-        ["return_fields_by_field_id", False, {"returnFieldsByFieldId": False}],
+        ["use_field_ids", True, {"returnFieldsByFieldId": True}],
+        ["use_field_ids", 1, {"returnFieldsByFieldId": True}],
+        ["use_field_ids", False, {"returnFieldsByFieldId": False}],
         # userLocale and timeZone are not supported via POST, so they return "spare params"
         ["user_locale", "en-US", ({}, {"userLocale": "en-US"})],
         ["time_zone", "America/Chicago", ({}, {"timeZone": "America/Chicago"})],
     ],
 )
 def test_convert_options_to_json(option, value, expected):
     if isinstance(expected, dict):
```

### Comparing `pyairtable-2.3.3/tests/test_request_errors.py` & `pyairtable-3.0.0a1/tests/test_request_errors.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_testing.py` & `pyairtable-3.0.0a1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_typing.py` & `pyairtable-3.0.0a1/tests/test_typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -67,29 +67,31 @@
     )
 
     # Test type annotations for the ORM
     class Actor(orm.Model):
         name = orm.fields.TextField("Name")
         logins = orm.fields.MultipleCollaboratorsField("Logins")
 
-    assert_type(Actor().name, Optional[str])
+    assert_type(Actor().name, str)
     assert_type(Actor().logins, List[T.CollaboratorDict])
 
     class Movie(orm.Model):
         name = orm.fields.TextField("Name")
         rating = orm.fields.RatingField("Star Rating")
         prequels = orm.fields.LinkField["Movie"]("Prequels", "path.to.Movie")
         actors = orm.fields.LinkField("Actors", Actor)
+        prequel = orm.fields.SingleLinkField["Movie"]("Prequels", orm.fields.LinkSelf)
 
     movie = Movie()
-    assert_type(movie.name, Optional[str])
+    assert_type(movie.name, str)
     assert_type(movie.rating, Optional[int])
     assert_type(movie.actors, List[Actor])
     assert_type(movie.prequels, List[Movie])
-    assert_type(movie.actors[0].name, Optional[str])
+    assert_type(movie.prequel, Optional[Movie])
+    assert_type(movie.actors[0].name, str)
 
     class EveryField(orm.Model):
         aitext = orm.fields.AITextField("AI Generated Text")
         attachments = orm.fields.AttachmentsField("Attachments")
         autonumber = orm.fields.AutoNumberField("Autonumber")
         barcode = orm.fields.BarcodeField("Barcode")
         button = orm.fields.ButtonField("Open URL")
@@ -112,37 +114,73 @@
         number = orm.fields.NumberField("Number")
         percent = orm.fields.PercentField("Percent")
         phone = orm.fields.PhoneNumberField("Phone")
         rating = orm.fields.RatingField("Stars")
         rich_text = orm.fields.RichTextField("Notes")
         select = orm.fields.SelectField("Status")
         url = orm.fields.UrlField("URL")
+        required_aitext = orm.fields.RequiredAITextField("AI Generated Text")
+        required_barcode = orm.fields.RequiredBarcodeField("Barcode")
+        required_collaborator = orm.fields.RequiredCollaboratorField("Assignee")
+        required_count = orm.fields.RequiredCountField("Count")
+        required_currency = orm.fields.RequiredCurrencyField("Dollars")
+        required_date = orm.fields.RequiredDateField("Date")
+        required_datetime = orm.fields.RequiredDatetimeField("DateTime")
+        required_duration = orm.fields.RequiredDurationField("Duration (h:mm)")
+        required_email = orm.fields.RequiredEmailField("Email")
+        required_float = orm.fields.RequiredFloatField("Decimal 1")
+        required_integer = orm.fields.RequiredIntegerField("Integer")
+        required_number = orm.fields.RequiredNumberField("Number")
+        required_percent = orm.fields.RequiredPercentField("Percent")
+        required_phone = orm.fields.RequiredPhoneNumberField("Phone")
+        required_rating = orm.fields.RequiredRatingField("Stars")
+        required_rich_text = orm.fields.RequiredRichTextField("Notes")
+        required_select = orm.fields.RequiredSelectField("Status")
+        required_url = orm.fields.RequiredUrlField("URL")
 
     record = EveryField()
     assert_type(record.aitext, Optional[T.AITextDict])
     assert_type(record.attachments, List[T.AttachmentDict])
-    assert_type(record.autonumber, Optional[int])
+    assert_type(record.autonumber, int)
     assert_type(record.barcode, Optional[T.BarcodeDict])
-    assert_type(record.button, Optional[T.ButtonDict])
-    assert_type(record.checkbox, Optional[bool])
+    assert_type(record.button, T.ButtonDict)
+    assert_type(record.checkbox, bool)
     assert_type(record.collaborator, Optional[T.CollaboratorDict])
     assert_type(record.count, Optional[int])
-    assert_type(record.created_by, Optional[T.CollaboratorDict])
-    assert_type(record.created, Optional[datetime.datetime])
+    assert_type(record.created_by, T.CollaboratorDict)
+    assert_type(record.created, datetime.datetime)
     assert_type(record.currency, Optional[Union[int, float]])
     assert_type(record.date, Optional[datetime.date])
     assert_type(record.datetime, Optional[datetime.datetime])
     assert_type(record.duration, Optional[datetime.timedelta])
-    assert_type(record.email, Optional[str])
+    assert_type(record.email, str)
     assert_type(record.float, Optional[float])
     assert_type(record.integer, Optional[int])
     assert_type(record.last_modified_by, Optional[T.CollaboratorDict])
     assert_type(record.last_modified, Optional[datetime.datetime])
     assert_type(record.multi_user, List[T.CollaboratorDict])
     assert_type(record.multi_select, List[str])
     assert_type(record.number, Optional[Union[int, float]])
     assert_type(record.percent, Optional[Union[int, float]])
-    assert_type(record.phone, Optional[str])
+    assert_type(record.phone, str)
     assert_type(record.rating, Optional[int])
-    assert_type(record.rich_text, Optional[str])
+    assert_type(record.rich_text, str)
     assert_type(record.select, Optional[str])
-    assert_type(record.url, Optional[str])
+    assert_type(record.url, str)
+    assert_type(record.required_aitext, T.AITextDict)
+    assert_type(record.required_barcode, T.BarcodeDict)
+    assert_type(record.required_collaborator, T.CollaboratorDict)
+    assert_type(record.required_count, int)
+    assert_type(record.required_currency, Union[int, float])
+    assert_type(record.required_date, datetime.date)
+    assert_type(record.required_datetime, datetime.datetime)
+    assert_type(record.required_duration, datetime.timedelta)
+    assert_type(record.required_email, str)
+    assert_type(record.required_float, float)
+    assert_type(record.required_integer, int)
+    assert_type(record.required_number, Union[int, float])
+    assert_type(record.required_percent, Union[int, float])
+    assert_type(record.required_phone, str)
+    assert_type(record.required_rating, int)
+    assert_type(record.required_rich_text, str)
+    assert_type(record.required_select, str)
+    assert_type(record.required_url, str)
```

### Comparing `pyairtable-2.3.3/tests/test_url_escape.py` & `pyairtable-3.0.0a1/tests/test_url_escape.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tests/test_utils.py` & `pyairtable-3.0.0a1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.3.3/tox.ini` & `pyairtable-3.0.0a1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tox]
 envlist =
     pre-commit
     mypy
     py3{8,9,10,11,12}{,-pydantic1,-requestsmin}
+    integration
     coverage
 
 [gh-actions]
 python =
-    3.8: py38, coverage
-    3.9: py39
-    3.10: py310
-    3.11: py311
-    3.12: py312
+    3.8: py38, mypy
+    3.9: py39, mypy
+    3.10: py310, mypy
+    3.11: py311, mypy
+    3.12: coverage, mypy
 
 [testenv:pre-commit]
 deps = pre-commit
 commands = pre-commit run --all-files
 
 [testenv:mypy]
 deps = -r requirements-dev.txt
@@ -23,20 +24,25 @@
 
 [testenv]
 passenv =
     AIRTABLE_API_KEY
     AIRTABLE_ENTERPRISE_ID
 addopts = -v
 testpaths = tests
-commands = python -m pytest {posargs}
+commands =
+    python -m pytest {posargs:-m 'not integration'}
 deps =
     -r requirements-test.txt
     requestsmin: requests==2.22.0  # Keep in sync with setup.cfg
     pydantic1: pydantic<2  # Lots of projects still use 1.x
 
+[testenv:integration]
+commands =
+    python -m pytest -m integration
+
 [testenv:coverage]
 passenv = COVERAGE_FORMAT
 commands =
     python -m pytest -m 'not integration' --cov=pyairtable --cov-report={env:COVERAGE_FORMAT:html}
 
 [testenv:docs]
 basepython = python3.8
```

