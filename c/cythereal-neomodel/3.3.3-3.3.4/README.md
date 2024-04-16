# Comparing `tmp/cythereal-neomodel-3.3.3.tar.gz` & `tmp/cythereal-neomodel-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cythereal-neomodel-3.3.3.tar", last modified: Tue Apr 16 17:26:52 2024, max compression
+gzip compressed data, was "cythereal-neomodel-3.3.4.tar", last modified: Tue Apr 16 19:35:35 2024, max compression
```

## Comparing `cythereal-neomodel-3.3.3.tar` & `cythereal-neomodel-3.3.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      704 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/AUTHORS.txt
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12753 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/Changelog
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1099 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/LICENSE
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       73 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/MANIFEST.in
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/PKG-INFO
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3968 2024-04-16 17:25:50.000000 cythereal-neomodel-3.3.3/README.rst
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.750124 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 17:26:52.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/PKG-INFO
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1225 2024-04-16 17:26:52.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/SOURCES.txt
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 17:26:52.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/dependency_links.txt
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       34 2024-04-16 17:26:52.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/requires.txt
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        9 2024-04-16 17:26:52.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/top_level.txt
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/zip-safe
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.750124 cythereal-neomodel-3.3.3/neomodel/
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1095 2024-04-16 17:24:24.000000 cythereal-neomodel-3.3.3/neomodel/__init__.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3590 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/cardinality.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      269 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/config.py
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/neomodel/contrib/
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       48 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/neomodel/contrib/__init__.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2369 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/contrib/semi_structured.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    15083 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/contrib/spatial_properties.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19167 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/core.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       40 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/exception.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6938 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/exceptions.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      388 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/hooks.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    26572 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/match.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     7754 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/match_q.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19062 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/properties.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3031 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/relationship.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    14580 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/relationship_manager.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    11885 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/neomodel/util.py
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/scripts/
--rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1890 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/scripts/neomodel_install_labels
--rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1004 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/scripts/neomodel_remove_labels
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      112 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/setup.cfg
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1320 2024-04-16 17:25:58.000000 cythereal-neomodel-3.3.3/setup.py
-drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 17:26:52.754124 cythereal-neomodel-3.3.3/test/
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      895 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/test/test_alias.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3194 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_batch.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2798 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_cardinality.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      961 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_cypher.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      864 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_exceptions.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      733 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_hooks.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1526 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_indexing.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      305 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_issue112.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    10529 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_issue283.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1047 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_label_drop.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1633 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_label_install.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12062 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_match_api.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6423 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_models.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      470 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/test/test_multiprocessing.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12356 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_properties.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4192 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_relationship_models.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4878 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_relationships.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      607 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.3/test/test_relative_relationships.py
--rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1771 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.3/test/test_transactions.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.342656 cythereal-neomodel-3.3.4/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      704 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/AUTHORS.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12753 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/Changelog
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1099 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/LICENSE
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       73 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/MANIFEST.in
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 19:35:35.342656 cythereal-neomodel-3.3.4/PKG-INFO
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3968 2024-04-16 19:34:17.000000 cythereal-neomodel-3.3.4/README.rst
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.338656 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 19:35:35.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/PKG-INFO
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1225 2024-04-16 19:35:35.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 19:35:35.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       34 2024-04-16 19:35:35.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/requires.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        9 2024-04-16 19:35:35.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/top_level.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/zip-safe
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.338656 cythereal-neomodel-3.3.4/neomodel/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1095 2024-04-16 17:24:24.000000 cythereal-neomodel-3.3.4/neomodel/__init__.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3590 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/cardinality.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      269 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/config.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.338656 cythereal-neomodel-3.3.4/neomodel/contrib/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       48 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/neomodel/contrib/__init__.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2369 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/contrib/semi_structured.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    15083 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/contrib/spatial_properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19167 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/core.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       40 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/exception.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6938 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/exceptions.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      388 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/hooks.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    26572 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/match.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     7754 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/match_q.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19062 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3031 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/relationship.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    14580 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/neomodel/relationship_manager.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12033 2024-04-16 19:33:40.000000 cythereal-neomodel-3.3.4/neomodel/util.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.338656 cythereal-neomodel-3.3.4/scripts/
+-rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1890 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/scripts/neomodel_install_labels
+-rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1004 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/scripts/neomodel_remove_labels
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      112 2024-04-16 19:35:35.342656 cythereal-neomodel-3.3.4/setup.cfg
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1320 2024-04-16 19:34:24.000000 cythereal-neomodel-3.3.4/setup.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 19:35:35.342656 cythereal-neomodel-3.3.4/test/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      895 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/test/test_alias.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3194 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_batch.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2798 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_cardinality.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      961 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_cypher.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      864 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_exceptions.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      733 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_hooks.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1526 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_indexing.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      305 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_issue112.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    10529 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_issue283.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1047 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_label_drop.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1633 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_label_install.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12062 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_match_api.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6423 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_models.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      470 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/test/test_multiprocessing.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12356 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4192 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_relationship_models.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4878 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_relationships.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      607 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.4/test/test_relative_relationships.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1771 2024-04-16 17:04:00.000000 cythereal-neomodel-3.3.4/test/test_transactions.py
```

### Comparing `cythereal-neomodel-3.3.3/AUTHORS.txt` & `cythereal-neomodel-3.3.4/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/Changelog` & `cythereal-neomodel-3.3.4/Changelog`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/LICENSE` & `cythereal-neomodel-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/PKG-INFO` & `cythereal-neomodel-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cythereal-neomodel
-Version: 3.3.3
+Version: 3.3.4
 Summary: An object mapper for the neo4j graph database.
 Home-page: http://github.com/neo4j-contrib/neomodel
 Author: Robin Edwards
 Author-email: robin.ge@gmail.com
 License: MIT
 Keywords: graph neo4j ORM OGM
 Platform: UNKNOWN
@@ -88,15 +88,15 @@
  * Indexing NodeSets returns a single node now as opposed to a list
 
 Contributing
 ============
 
 Ideas, bugs, tests and pull requests always welcome. 
 
-As of release `3.3.3` we now have a curated list of issues / development targets for
+As of release `3.3.4` we now have a curated list of issues / development targets for
 `neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
 
 If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
 it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
 contribute towards delivering any of the existing todo items too.
 
 Running the test suite
```

### Comparing `cythereal-neomodel-3.3.3/README.rst` & `cythereal-neomodel-3.3.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
  * Indexing NodeSets returns a single node now as opposed to a list
 
 Contributing
 ============
 
 Ideas, bugs, tests and pull requests always welcome. 
 
-As of release `3.3.3` we now have a curated list of issues / development targets for
+As of release `3.3.4` we now have a curated list of issues / development targets for
 `neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
 
 If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
 it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
 contribute towards delivering any of the existing todo items too.
 
 Running the test suite
```

### Comparing `cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/PKG-INFO` & `cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cythereal-neomodel
-Version: 3.3.3
+Version: 3.3.4
 Summary: An object mapper for the neo4j graph database.
 Home-page: http://github.com/neo4j-contrib/neomodel
 Author: Robin Edwards
 Author-email: robin.ge@gmail.com
 License: MIT
 Keywords: graph neo4j ORM OGM
 Platform: UNKNOWN
@@ -88,15 +88,15 @@
  * Indexing NodeSets returns a single node now as opposed to a list
 
 Contributing
 ============
 
 Ideas, bugs, tests and pull requests always welcome. 
 
-As of release `3.3.3` we now have a curated list of issues / development targets for
+As of release `3.3.4` we now have a curated list of issues / development targets for
 `neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
 
 If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
 it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
 contribute towards delivering any of the existing todo items too.
 
 Running the test suite
```

### Comparing `cythereal-neomodel-3.3.3/cythereal_neomodel.egg-info/SOURCES.txt` & `cythereal-neomodel-3.3.4/cythereal_neomodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/__init__.py` & `cythereal-neomodel-3.3.4/neomodel/__init__.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/cardinality.py` & `cythereal-neomodel-3.3.4/neomodel/cardinality.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/contrib/semi_structured.py` & `cythereal-neomodel-3.3.4/neomodel/contrib/semi_structured.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/contrib/spatial_properties.py` & `cythereal-neomodel-3.3.4/neomodel/contrib/spatial_properties.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/core.py` & `cythereal-neomodel-3.3.4/neomodel/core.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/exceptions.py` & `cythereal-neomodel-3.3.4/neomodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/match.py` & `cythereal-neomodel-3.3.4/neomodel/match.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/match_q.py` & `cythereal-neomodel-3.3.4/neomodel/match_q.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/properties.py` & `cythereal-neomodel-3.3.4/neomodel/properties.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/relationship.py` & `cythereal-neomodel-3.3.4/neomodel/relationship.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/relationship_manager.py` & `cythereal-neomodel-3.3.4/neomodel/relationship_manager.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/neomodel/util.py` & `cythereal-neomodel-3.3.4/neomodel/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -241,24 +241,26 @@
                     raise exc_info[1]
         except SessionError:
             if retry_on_session_expire:
                 self.set_connection(self.url)
                 return self.cypher_query(query=query,
                                          params=params,
                                          handle_unique=handle_unique,
-                                         retry_on_session_expire=False)
+                                         retry_on_session_expire=False,
+                                         resolve_objects=resolve_objects)
             raise
         except (TimeoutError,ServiceUnavailable) as err:
             # If there is a ServiceUnavailable Error or a Timeout, go ahead and retry.
             if retry_failed_connection <= config.MAX_CONNECTION_RETRY:
                 self.set_connection(self.url)
                 return self.cypher_query(query=query,
                                          params=params,
                                          handle_unique=handle_unique,
                                          retry_on_session_expire=False,
+                                         resolve_objects=resolve_objects,
                                          retry_failed_connection=retry_failed_connection+1)
             raise
 
         if os.environ.get('NEOMODEL_CYPHER_DEBUG', False):
             logger.debug("query: " + query + "\nparams: " + repr(params) + "\ntook: {:.2g}s\n".format(end - start))
 
         return results, meta
```

### Comparing `cythereal-neomodel-3.3.3/scripts/neomodel_install_labels` & `cythereal-neomodel-3.3.4/scripts/neomodel_install_labels`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/scripts/neomodel_remove_labels` & `cythereal-neomodel-3.3.4/scripts/neomodel_remove_labels`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/setup.py` & `cythereal-neomodel-3.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from setuptools import setup, find_packages
 
 setup(
     name='cythereal-neomodel',
-    version='3.3.3',
+    version='3.3.4',
     description='An object mapper for the neo4j graph database.',
     long_description=open('README.rst').read(),
     author='Robin Edwards',
     author_email='robin.ge@gmail.com',
     zip_safe=True,
     url='http://github.com/neo4j-contrib/neomodel',
     license='MIT',
```

### Comparing `cythereal-neomodel-3.3.3/test/test_alias.py` & `cythereal-neomodel-3.3.4/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_batch.py` & `cythereal-neomodel-3.3.4/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_cardinality.py` & `cythereal-neomodel-3.3.4/test/test_cardinality.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_cypher.py` & `cythereal-neomodel-3.3.4/test/test_cypher.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_exceptions.py` & `cythereal-neomodel-3.3.4/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_hooks.py` & `cythereal-neomodel-3.3.4/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_indexing.py` & `cythereal-neomodel-3.3.4/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_issue283.py` & `cythereal-neomodel-3.3.4/test/test_issue283.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_label_drop.py` & `cythereal-neomodel-3.3.4/test/test_label_drop.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_label_install.py` & `cythereal-neomodel-3.3.4/test/test_label_install.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_match_api.py` & `cythereal-neomodel-3.3.4/test/test_match_api.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_models.py` & `cythereal-neomodel-3.3.4/test/test_models.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_properties.py` & `cythereal-neomodel-3.3.4/test/test_properties.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_relationship_models.py` & `cythereal-neomodel-3.3.4/test/test_relationship_models.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_relationships.py` & `cythereal-neomodel-3.3.4/test/test_relationships.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_relative_relationships.py` & `cythereal-neomodel-3.3.4/test/test_relative_relationships.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.3.3/test/test_transactions.py` & `cythereal-neomodel-3.3.4/test/test_transactions.py`

 * *Files identical despite different names*

