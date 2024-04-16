# Comparing `tmp/cythereal-neomodel-3.2.5.tar.gz` & `tmp/cythereal-neomodel-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cythereal-neomodel-3.2.5.tar", last modified: Mon Mar 26 21:24:24 2018, max compression
+gzip compressed data, was "cythereal-neomodel-3.3.2.tar", last modified: Tue Apr 16 16:20:46 2024, max compression
```

## Comparing `cythereal-neomodel-3.2.5.tar` & `cythereal-neomodel-3.3.2.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     3235 2018-03-26 21:20:02.000000 cythereal-neomodel-3.2.5/README.rst
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     7824 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/Changelog
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1099 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/LICENSE
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1297 2018-03-26 21:20:39.000000 cythereal-neomodel-3.2.5/setup.py
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/test/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1047 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_label_drop.py
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/test/test_contrib/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      453 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_contrib/test_semi_structured.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        0 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_contrib/__init__.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4193 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_relationship_models.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     5766 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/test/test_models.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      882 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/conftest.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      470 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_multiprocessing.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1742 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_transactions.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4022 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_relationships.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     7196 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/test/test_match_api.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      895 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_alias.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      887 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_label_install.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      859 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/test/test_exceptions.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1526 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_indexing.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      305 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_issue112.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     2612 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_cardinality.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      961 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_cypher.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     8127 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/test/test_properties.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      733 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_hooks.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        0 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/__init__.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      607 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/test/test_relative_relationships.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     3194 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/test/test_batch.py
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/neomodel/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    15978 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/properties.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      363 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/neomodel/hooks.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     2741 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/neomodel/relationship.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     3436 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/cardinality.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4882 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/exceptions.py
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/neomodel/contrib/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     2261 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/contrib/semi_structured.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       48 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/neomodel/contrib/__init__.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     6873 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/util.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    18629 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/core.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    13851 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/relationship_manager.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      268 2018-02-14 18:48:55.000000 cythereal-neomodel-3.2.5/neomodel/config.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    22825 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/match.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      796 2018-03-23 20:14:04.000000 cythereal-neomodel-3.2.5/neomodel/__init__.py
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      102 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/setup.cfg
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4904 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/PKG-INFO
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/scripts/
--rwxrwxr-x   0 cledoux   (1000) cledoux   (1000)     1004 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/scripts/neomodel_remove_labels
--rwxrwxr-x   0 cledoux   (1000) cledoux   (1000)     1890 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/scripts/neomodel_install_labels
-drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       31 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/requires.txt
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4904 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/PKG-INFO
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        1 2018-03-26 21:20:56.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/zip-safe
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1228 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/SOURCES.txt
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       14 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/top_level.txt
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        1 2018-03-26 21:24:24.000000 cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/dependency_links.txt
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      704 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/AUTHORS.txt
--rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       73 2018-02-14 18:42:14.000000 cythereal-neomodel-3.2.5/MANIFEST.in
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      704 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/AUTHORS.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12753 2019-09-29 08:39:52.000000 cythereal-neomodel-3.3.2/Changelog
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1099 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/LICENSE
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       73 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/MANIFEST.in
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/PKG-INFO
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3968 2024-04-16 16:00:13.000000 cythereal-neomodel-3.3.2/README.rst
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4849 2024-04-16 16:20:46.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/PKG-INFO
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1225 2024-04-16 16:20:46.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 16:20:46.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       34 2024-04-16 16:20:46.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/requires.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        9 2024-04-16 16:20:46.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/top_level.txt
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        1 2024-04-16 16:14:55.000000 cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/zip-safe
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/neomodel/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1085 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/neomodel/__init__.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3590 2024-04-16 15:49:42.000000 cythereal-neomodel-3.3.2/neomodel/cardinality.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      269 2024-04-16 15:40:08.000000 cythereal-neomodel-3.3.2/neomodel/config.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/neomodel/contrib/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       48 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/neomodel/contrib/__init__.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2369 2024-04-16 15:51:07.000000 cythereal-neomodel-3.3.2/neomodel/contrib/semi_structured.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    15083 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/neomodel/contrib/spatial_properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19167 2024-04-16 15:53:25.000000 cythereal-neomodel-3.3.2/neomodel/core.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)       40 2024-04-16 15:53:45.000000 cythereal-neomodel-3.3.2/neomodel/exception.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6938 2024-04-16 15:55:02.000000 cythereal-neomodel-3.3.2/neomodel/exceptions.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      388 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/neomodel/hooks.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    26572 2024-04-16 15:41:52.000000 cythereal-neomodel-3.3.2/neomodel/match.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     7754 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/neomodel/match_q.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    19062 2024-04-16 15:57:04.000000 cythereal-neomodel-3.3.2/neomodel/properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3031 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/neomodel/relationship.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    14580 2024-04-16 15:42:30.000000 cythereal-neomodel-3.3.2/neomodel/relationship_manager.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    11885 2024-04-16 15:48:17.000000 cythereal-neomodel-3.3.2/neomodel/util.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/scripts/
+-rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1890 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/scripts/neomodel_install_labels
+-rwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1004 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/scripts/neomodel_remove_labels
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      112 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/setup.cfg
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1320 2024-04-16 16:03:13.000000 cythereal-neomodel-3.3.2/setup.py
+drwxrwxr-x   0 hubbard-zlee  (1000) hubbard-zlee  (1000)        0 2024-04-16 16:20:46.304323 cythereal-neomodel-3.3.2/test/
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      895 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_alias.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     3194 2024-04-16 16:05:40.000000 cythereal-neomodel-3.3.2/test/test_batch.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     2798 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_cardinality.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      961 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_cypher.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      864 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_exceptions.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      733 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_hooks.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1526 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_indexing.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      305 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_issue112.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    10529 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_issue283.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1047 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_label_drop.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1633 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_label_install.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12062 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_match_api.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     6423 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_models.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      470 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_multiprocessing.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)    12356 2019-09-29 08:36:41.000000 cythereal-neomodel-3.3.2/test/test_properties.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4192 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_relationship_models.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     4878 2019-05-05 21:51:23.000000 cythereal-neomodel-3.3.2/test/test_relationships.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)      607 2019-05-02 13:03:22.000000 cythereal-neomodel-3.3.2/test/test_relative_relationships.py
+-rw-rw-r--   0 hubbard-zlee  (1000) hubbard-zlee  (1000)     1771 2019-05-08 16:01:01.000000 cythereal-neomodel-3.3.2/test/test_transactions.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cythereal-neomodel-3.2.5/README.rst` & `cythereal-neomodel-3.3.2/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
+.. image:: https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png
    :alt: neomodel
 
 NOTE: This is a customized version of neomodel for personal use. Use the
 `official version`_ instead.
 
 An Object Graph Mapper (OGM) for the neo4j_ graph database, built on the awesome neo4j_driver_
 
@@ -10,50 +10,51 @@
 - Powerful query API.
 - Enforce your schema through cardinality restrictions.
 - Full transaction support.
 - Thread safe.
 - pre/post save/delete hooks.
 - Django integration via django_neomodel_
 
-.. _django_neomodel: https://github.com/robinedwards/django-neomodel
-.. _neo4j: https://www.neo4j.org
+.. _django_neomodel: https://github.com/neo4j-contrib/django-neomodel
+.. _neo4j: https://neo4j.com/
 .. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
 .. _official version: https://github.com/neo4j-contrib/neomodel
 
-.. image:: https://secure.travis-ci.org/robinedwards/neomodel.png
-    :target: https://secure.travis-ci.org/robinedwards/neomodel/
+.. image:: https://secure.travis-ci.org/neo4j-contrib/neomodel.png
+    :target: https://secure.travis-ci.org/neo4j-contrib/neomodel/
 
 .. image:: https://readthedocs.org/projects/neomodel/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://neomodel.readthedocs.io/en/latest/?badge=latest
 
+
 Documentation
 =============
 
 Available on readthedocs_.
 
 .. _readthedocs: http://neomodel.readthedocs.org
 
 Requirements
 ============
 
-- Python 2.7, 3.4+
+- Python 2.7 (Up to version 3.3.1), 3.4+
 - neo4j 3.0, 3.1, 3.2, 3.3
 
 Installation
 ============
 
 Install from pypi (recommended)::
 
     $ pip install neomodel
 
 To install from github::
 
-    $ pip install git+git://github.com/robinedwards/neomodel.git@HEAD#egg=neomodel-dev
+    $ pip install git+git://github.com/neo4j-contrib/neomodel.git@HEAD#egg=neomodel-dev
 
 Upgrading 2.x to 3.x
 ====================
 
  * Now utilises neo4j_driver as the backend which uses bolt so neo4j 3 is required
  * Connection now set through config.DATABASE_URL (see getting started docs)
  * The deprecated category() method on StructuredNode has been removed
@@ -61,39 +62,45 @@
  * The streaming=True flag is now irrelevant with bolt and produces a deprecation warning
  * Batch operations must now be wrapped in a transaction in order to be atomic
  * Indexing NodeSets returns a single node now as opposed to a list
 
 Contributing
 ============
 
-Ideas, bugs, tests and pull requests always welcome.
+Ideas, bugs, tests and pull requests always welcome. 
 
-Running the test suite
-----------------------
+As of release `3.3.2` we now have a curated list of issues / development targets for
+`neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
 
-Make sure you have a fresh virtualenv and `nose` installed::
+If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
+it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
+contribute towards delivering any of the existing todo items too.
 
-    $ pip install nose
+Running the test suite
+----------------------
 
-Also a Neo4j database version 3 or higher to run the tests on. (it will wipe this database for each test run)::
+Make sure you have a Neo4j database version 3 or higher to run the tests on.::
 
     $ export NEO4J_BOLT_URL=bolt://neo4j:neo4j@localhost:7687 # (the default)
 
 Setup a virtual environment, install neomodel for development and run the test suite::
 
     $ virtualenv venv
     $ source venv/bin/activate
     $ python setup.py develop
-    $ nosetests -s
+    $ pytest
 
-If your running a neo4j database for the first time the test suite will set the password to 'test'.
+If you are running a neo4j database for the first time the test suite will set the password to 'test'.
+If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
+`--resetdb` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if
+you happen to not have restarted your Neo4j server to point to a (usually named) `debug.db` database.
 
 If you have ``docker-compose`` installed, you can run the test suite against all supported Python
 interpreters and neo4j versions::
 
     # in the project's root folder:
     $ ./tests-with-docker-compose.sh
 
 
 .. image:: https://badges.gitter.im/Join%20Chat.svg
-   :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-   :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+   :alt: Join the chat at https://gitter.im/neo4j-contrib/neomodel
+   :target: https://gitter.im/neo4j-contrib/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `cythereal-neomodel-3.2.5/LICENSE` & `cythereal-neomodel-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/setup.py` & `cythereal-neomodel-3.3.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 
 from setuptools import setup, find_packages
 
 setup(
     name='cythereal-neomodel',
-    version='3.2.5',
+    version='3.3.2',
     description='An object mapper for the neo4j graph database.',
     long_description=open('README.rst').read(),
     author='Robin Edwards',
     author_email='robin.ge@gmail.com',
     zip_safe=True,
-    url='http://github.com/robinedwards/neomodel',
+    url='http://github.com/neo4j-contrib/neomodel',
     license='MIT',
-    packages=find_packages(exclude=('tests',)),
+    packages=find_packages(exclude=('test', 'test.*')),
     keywords='graph neo4j ORM OGM',
     scripts=['scripts/neomodel_install_labels', 'scripts/neomodel_remove_labels'],
     setup_requires=['pytest-runner'] if any(x in ('pytest', 'test') for x in sys.argv) else [],
-    tests_require=['pytest'],
-    install_requires=['neo4j-driver==1.5.3', 'pytz>=2016'],
+    tests_require=['pytest', 'shapely'],
+    install_requires=['neo4j-driver==1.7.2', 'pytz>=2016.10'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `cythereal-neomodel-3.2.5/test/test_label_drop.py` & `cythereal-neomodel-3.3.2/test/test_label_drop.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_relationship_models.py` & `cythereal-neomodel-3.3.2/test/test_relationship_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pytest import raises
 import pytz
 
 from neomodel import (StructuredNode, StructuredRel, Relationship, RelationshipTo,
                       StringProperty, DateTimeProperty, DeflateError)
 
-
 HOOKS_CALLED = {
     'pre_save': 0,
     'post_save': 0
 }
 
 
 class FriendRel(StructuredRel):
```

### Comparing `cythereal-neomodel-3.2.5/test/test_models.py` & `cythereal-neomodel-3.3.2/test/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,30 @@
     rob = User.nodes.get_or_none(email='robin@test.com')
     assert rob.email == 'robin@test.com'
 
     n = User.nodes.get_or_none(email='robin@nothere.com')
     assert n is None
 
 
+def test_first_and_first_or_none():
+    u = User(email='matt@test.com', age=24)
+    assert u.save()
+    u2 = User(email='tbrady@test.com', age=40)
+    assert u2.save()
+    tbrady = User.nodes.order_by('-age').first()
+    assert tbrady.email == 'tbrady@test.com'
+    assert tbrady.age == 40
+
+    tbrady = User.nodes.order_by('-age').first_or_none()
+    assert tbrady.email == 'tbrady@test.com'
+
+    n = User.nodes.first_or_none(email='matt@nothere.com')
+    assert n is None
+
+
 def test_save_to_model():
     u = User(email='jim@test.com', age=3)
     assert u.save()
     assert u.id > 0
     assert u.email == 'jim@test.com'
     assert u.age == 3
 
@@ -158,14 +174,24 @@
 
     assert c.age == 16
 
     c.refresh()
     assert c.age == 20
     assert c.my_custom_prop == 'value'
 
+    c = Customer2.inflate(c.id)
+    c.age = 30
+    c.refresh()
+
+    assert c.age == 20
+
+    c = Customer2.inflate(999)
+    with raises(Customer2.DoesNotExist):
+        c.refresh()
+
 
 def test_setting_value_to_none():
     c = Customer2(email='alice@bob.com', age=42).save()
     assert c.age is not None
 
     c.age = None
     c.save()
```

### Comparing `cythereal-neomodel-3.2.5/test/test_transactions.py` & `cythereal-neomodel-3.3.2/test/test_transactions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from neo4j.addressing import AddressError
+from neobolt.addressing import AddressError
 from pytest import raises
 
 from neomodel import db, StructuredNode, StringProperty, UniqueProperty
 
 
-class Person(StructuredNode):
+class APerson(StructuredNode):
     name = StringProperty(unique_index=True)
 
 
 def test_rollback_and_commit_transaction():
-    for p in Person.nodes:
+    for p in APerson.nodes:
         p.delete()
 
-    Person(name='Roger').save()
+    APerson(name='Roger').save()
 
     db.begin()
-    Person(name='Terry S').save()
+    APerson(name='Terry S').save()
     db.rollback()
 
-    assert len(Person.nodes) == 1
+    assert len(APerson.nodes) == 1
 
     db.begin()
-    Person(name='Terry S').save()
+    APerson(name='Terry S').save()
     db.commit()
 
-    assert len(Person.nodes) == 2
+    assert len(APerson.nodes) == 2
 
 
 @db.transaction
 def in_a_tx(*names):
     for n in names:
-        Person(name=n).save()
+        APerson(name=n).save()
 
 
 def test_transaction_decorator():
-    for p in Person.nodes:
+    for p in APerson.nodes:
         p.delete()
 
     # should work
     in_a_tx('Roger')
     assert True
 
     # should bail but raise correct error
     with raises(UniqueProperty):
         in_a_tx('Jim', 'Roger')
 
-    assert 'Jim' not in [p.name for p in Person.nodes]
+    assert 'Jim' not in [p.name for p in APerson.nodes]
 
 
 def test_transaction_as_a_context():
     with db.transaction:
-        Person(name='Tim').save()
+        APerson(name='Tim').save()
 
-    assert Person.nodes.filter(name='Tim')
+    assert APerson.nodes.filter(name='Tim')
 
     with raises(UniqueProperty):
         with db.transaction:
-            Person(name='Tim').save()
+            APerson(name='Tim').save()
 
 
 def test_query_inside_transaction():
-    for p in Person.nodes:
+    for p in APerson.nodes:
         p.delete()
 
     with db.transaction:
-        Person(name='Alice').save()
-        Person(name='Bob').save()
+        APerson(name='Alice').save()
+        APerson(name='Bob').save()
 
-        assert len([p.name for p in Person.nodes]) == 2
+        assert len([p.name for p in APerson.nodes]) == 2
 
 
 def test_set_connection_works():
-    assert Person(name='New guy').save()
+    assert APerson(name='New guy').save()
     from socket import gaierror
 
     old_url = db.url
     with raises(AddressError):
-        db.set_connection('bolt://user:password@nowhere:7687')
+        db.set_connection('bolt://user:password@6.6.6.6.6.6.6.6:7687')
     db.set_connection(old_url)
     # set connection back
-    assert Person(name='New guy2').save()
+    assert APerson(name='New guy2').save()
```

### Comparing `cythereal-neomodel-3.2.5/test/test_relationships.py` & `cythereal-neomodel-3.3.2/test/test_relationships.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from pytest import raises
 
 from neomodel import (StructuredNode, RelationshipTo, RelationshipFrom, Relationship,
                       StringProperty, IntegerProperty, StructuredRel, One)
 
 
-class Person(StructuredNode):
+class PersonWithRels(StructuredNode):
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True)
     is_from = RelationshipTo('Country', 'IS_FROM')
-    knows = Relationship(u'Person', 'KNOWS')  # use unicode to check issue
+    knows = Relationship(u'PersonWithRels', 'KNOWS')  # use unicode to check issue
 
     @property
     def special_name(self):
         return self.name
 
     def special_power(self):
         return "I have no powers"
 
 
 class Country(StructuredNode):
     code = StringProperty(unique_index=True)
-    inhabitant = RelationshipFrom(Person, 'IS_FROM')
-    president = RelationshipTo(Person, 'PRESIDENT', cardinality=One)
+    inhabitant = RelationshipFrom(PersonWithRels, 'IS_FROM')
+    president = RelationshipTo(PersonWithRels, 'PRESIDENT', cardinality=One)
 
 
-class SuperHero(Person):
+class SuperHero(PersonWithRels):
     power = StringProperty(index=True)
 
     def special_power(self):
         return "I have powers"
 
 
 def test_actions_on_deleted_node():
-    u = Person(name='Jim2', age=3).save()
+    u = PersonWithRels(name='Jim2', age=3).save()
     u.delete()
     with raises(ValueError):
         u.is_from.connect(None)
 
     with raises(ValueError):
         u.is_from.get()
 
     with raises(ValueError):
         u.save()
 
 
 def test_bidirectional_relationships():
-    u = Person(name='Jim', age=3).save()
+    u = PersonWithRels(name='Jim', age=3).save()
     assert u
 
     de = Country(code='DE').save()
     assert de
 
     assert len(u.is_from) == 0
     assert not u.is_from
@@ -70,16 +70,16 @@
     assert s.name == 'Jim'
 
     u.is_from.disconnect(b)
     assert not u.is_from.is_connected(b)
 
 
 def test_either_direction_connect():
-    rey = Person(name='Rey', age=3).save()
-    sakis = Person(name='Sakis', age=3).save()
+    rey = PersonWithRels(name='Rey', age=3).save()
+    sakis = PersonWithRels(name='Sakis', age=3).save()
 
     rey.knows.connect(sakis)
     assert rey.knows.is_connected(sakis)
     assert sakis.knows.is_connected(rey)
     sakis.knows.connect(rey)
 
     result, meta = sakis.cypher("""MATCH (us), (them)
@@ -92,15 +92,15 @@
     assert isinstance(rel, StructuredRel)
 
     rels = rey.knows.all_relationships(sakis)
     assert isinstance(rels[0], StructuredRel)
 
 
 def test_search_and_filter_and_exclude():
-    fred = Person(name='Fred', age=13).save()
+    fred = PersonWithRels(name='Fred', age=13).save()
     zz = Country(code='ZZ').save()
     zx = Country(code='ZX').save()
     zt = Country(code='ZY').save()
     fred.is_from.connect(zz)
     fred.is_from.connect(zx)
     fred.is_from.connect(zt)
     result = fred.is_from.search(code='ZX')
@@ -110,26 +110,26 @@
     assert result[0].code == 'ZX'
 
     result = fred.is_from.exclude(code='ZZ').exclude(code='ZY')
     assert result[0].code == 'ZX' and len(result) == 1
 
 
 def test_custom_methods():
-    u = Person(name='Joe90', age=13).save()
+    u = PersonWithRels(name='Joe90', age=13).save()
     assert u.special_power() == "I have no powers"
     u = SuperHero(name='Joe91', age=13, power='xxx').save()
     assert u.special_power() == "I have powers"
     assert u.special_name == 'Joe91'
 
 
 def test_valid_reconnection():
-    p = Person(name='ElPresidente', age=93).save()
+    p = PersonWithRels(name='ElPresidente', age=93).save()
     assert p
 
-    pp = Person(name='TheAdversary', age=33).save()
+    pp = PersonWithRels(name='TheAdversary', age=33).save()
     assert pp
 
     c = Country(code='CU').save()
     assert c
 
     c.president.connect(p)
     assert c.president.is_connected(p)
@@ -139,16 +139,42 @@
     assert c.president.is_connected(pp)
 
     # reelection time
     c.president.reconnect(pp, pp)
     assert c.president.is_connected(pp)
 
 
+def test_valid_replace():
+    brady = PersonWithRels(name='Tom Brady', age=40).save()
+    assert brady
+
+    gronk = PersonWithRels(name='Rob Gronkowski', age=28).save()
+    assert gronk
+
+    colbert = PersonWithRels(name='Stephen Colbert', age=53).save()
+    assert colbert
+
+    hanks = PersonWithRels(name='Tom Hanks', age=61).save()
+    assert hanks
+
+    brady.knows.connect(gronk)
+    brady.knows.connect(colbert)
+    assert len(brady.knows) == 2
+    assert brady.knows.is_connected(gronk)
+    assert brady.knows.is_connected(colbert)
+
+    brady.knows.replace(hanks)
+    assert len(brady.knows) == 1
+    assert brady.knows.is_connected(hanks)
+    assert not brady.knows.is_connected(gronk)
+    assert not brady.knows.is_connected(colbert)
+
+
 def test_props_relationship():
-    u = Person(name='Mar', age=20).save()
+    u = PersonWithRels(name='Mar', age=20).save()
     assert u
 
     c = Country(code='AT').save()
     assert c
 
     c2 = Country(code='LA').save()
     assert c2
```

### Comparing `cythereal-neomodel-3.2.5/test/test_match_api.py` & `cythereal-neomodel-3.3.2/test/test_match_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
 
 from pytest import raises
 
-from neomodel import (StructuredNode, StringProperty, IntegerProperty, RelationshipFrom,
-                      RelationshipTo, StructuredRel, DateTimeProperty)
-from neomodel.match import NodeSet, QueryBuilder
+from neomodel import (
+    INCOMING, DateTimeProperty, IntegerProperty, RelationshipFrom, RelationshipTo,
+    StringProperty, StructuredNode, StructuredRel, Q
+)
+from neomodel.match import NodeSet, QueryBuilder, Traversal
 from neomodel.exceptions import MultipleNodesReturned
 
 
 class SupplierRel(StructuredRel):
     since = DateTimeProperty(default=datetime.now)
     courier = StringProperty()
 
@@ -19,14 +21,15 @@
     coffees = RelationshipTo('Coffee', 'COFFEE SUPPLIERS')  # Space to check for escaping
 
 
 class Coffee(StructuredNode):
     name = StringProperty(unique_index=True)
     price = IntegerProperty()
     suppliers = RelationshipFrom(Supplier, 'COFFEE SUPPLIERS', model=SupplierRel)
+    id_ = IntegerProperty()
 
 
 def test_filter_exclude_via_labels():
     Coffee(name='Java', price=99).save()
 
     node_set = NodeSet(Coffee)
     qb = QueryBuilder(node_set).build_ast()
@@ -214,18 +217,18 @@
 
 
 def test_extra_filters():
 
     for c in Coffee.nodes:
         c.delete()
 
-    c1 = Coffee(name="Icelands finest", price=5).save()
-    c2 = Coffee(name="Britains finest", price=10).save()
-    c3 = Coffee(name="Japans finest", price=35).save()
-    c4 = Coffee(name="US extra-fine", price=None).save()
+    c1 = Coffee(name="Icelands finest", price=5, id_=1).save()
+    c2 = Coffee(name="Britains finest", price=10, id_=2).save()
+    c3 = Coffee(name="Japans finest", price=35, id_=3).save()
+    c4 = Coffee(name="US extra-fine", price=None, id_=4).save()
 
     coffees_5_10 = Coffee.nodes.filter(price__in=[10, 5]).all()
     assert len(coffees_5_10) == 2, "unexpected number of results"
     assert c1 in coffees_5_10, "doesnt contain 5 price coffee"
     assert c2 in coffees_5_10, "doesnt contain 10 price coffee"
 
     finest_coffees = Coffee.nodes.filter(name__iendswith=' Finest').all()
@@ -233,7 +236,128 @@
     assert c1 in finest_coffees, "doesnt contain 1st finest coffee"
     assert c2 in finest_coffees, "doesnt contain 2nd finest coffee"
     assert c3 in finest_coffees, "doesnt contain 3rd finest coffee"
 
     unpriced_coffees = Coffee.nodes.filter(price__isnull=True).all()
     assert len(unpriced_coffees) == 1, "unexpected number of results"
     assert c4 in unpriced_coffees, "doesnt contain unpriced coffee"
+
+    coffees_with_id_gte_3 = Coffee.nodes.filter(id___gte=3).all()
+    assert len(coffees_with_id_gte_3) == 2, "unexpected number of results"
+    assert c3 in coffees_with_id_gte_3
+    assert c4 in coffees_with_id_gte_3
+
+
+def test_traversal_definition_keys_are_valid():
+    muckefuck = Coffee(name='Mukkefuck', price=1)
+
+    with raises(ValueError):
+        Traversal(
+            muckefuck, 'a_name', {
+                'node_class': Supplier, 'direction': INCOMING,
+                'relationship_type': 'KNOWS', 'model': None
+            }
+        )
+
+    Traversal(
+        muckefuck, 'a_name', {
+            'node_class': Supplier, 'direction': INCOMING,
+            'relation_type': 'KNOWS', 'model': None
+        }
+    )
+
+
+def test_empty_filters():
+    """Test this case:
+        ```
+            SomeModel.nodes.filter().filter(Q(arg1=val1)).all()
+            SomeModel.nodes.exclude().exclude(Q(arg1=val1)).all()
+            SomeModel.nodes.filter().filter(arg1=val1).all()
+       ```
+       In django_rest_framework filter uses such as lazy function and
+       ``get_queryset`` function in ``GenericAPIView`` should returns
+       ``NodeSet`` object.
+    """
+
+    for c in Coffee.nodes:
+        c.delete()
+
+    c1 = Coffee(name="Super", price=5, id_=1).save()
+    c2 = Coffee(name="Puper", price=10, id_=2).save()
+
+    empty_filter = Coffee.nodes.filter()
+
+    all_coffees = empty_filter.all()
+    assert len(all_coffees) == 2, "unexpected number of results"
+
+    filter_empty_filter = empty_filter.filter(price=5)
+    assert len(filter_empty_filter.all()) == 1, "unexpected number of results"
+    assert c1 in filter_empty_filter.all(), "doesnt contain c1 in ``filter_empty_filter``"
+
+    filter_q_empty_filter = empty_filter.filter(Q(price=5))
+    assert len(filter_empty_filter.all()) == 1, "unexpected number of results"
+    assert c1 in filter_empty_filter.all(), "doesnt contain c1 in ``filter_empty_filter``"
+
+
+def test_q_filters():
+
+    for c in Coffee.nodes:
+        c.delete()
+
+    c1 = Coffee(name="Icelands finest", price=5, id_=1).save()
+    c2 = Coffee(name="Britains finest", price=10, id_=2).save()
+    c3 = Coffee(name="Japans finest", price=35, id_=3).save()
+    c4 = Coffee(name="US extra-fine", price=None, id_=4).save()
+    c5 = Coffee(name="Latte", price=35, id_=5).save()
+    c6 = Coffee(name="Cappuccino", price=35, id_=6).save()
+
+    coffees_5_10 = Coffee.nodes.filter(Q(price=10) | Q(price=5)).all()
+    assert len(coffees_5_10) == 2, "unexpected number of results"
+    assert c1 in coffees_5_10, "doesnt contain 5 price coffee"
+    assert c2 in coffees_5_10, "doesnt contain 10 price coffee"
+
+    coffees_5_6 = Coffee.nodes.filter(Q(name="Latte") | Q(name="Cappuccino")).filter(price=35).all()
+    assert len(coffees_5_6) == 2, "unexpected number of results"
+    assert c5 in coffees_5_6, "doesnt contain 5 coffee"
+    assert c6 in coffees_5_6, "doesnt contain 6 coffee"
+
+    coffees_5_6 = Coffee.nodes.filter(price=35).filter(Q(name="Latte") | Q(name="Cappuccino")).all()
+    assert len(coffees_5_6) == 2, "unexpected number of results"
+    assert c5 in coffees_5_6, "doesnt contain 5 coffee"
+    assert c6 in coffees_5_6, "doesnt contain 6 coffee"
+
+    finest_coffees = Coffee.nodes.filter(name__iendswith=' Finest').all()
+    assert len(finest_coffees) == 3, "unexpected number of results"
+    assert c1 in finest_coffees, "doesnt contain 1st finest coffee"
+    assert c2 in finest_coffees, "doesnt contain 2nd finest coffee"
+    assert c3 in finest_coffees, "doesnt contain 3rd finest coffee"
+
+    unpriced_coffees = Coffee.nodes.filter(Q(price__isnull=True)).all()
+    assert len(unpriced_coffees) == 1, "unexpected number of results"
+    assert c4 in unpriced_coffees, "doesnt contain unpriced coffee"
+
+    coffees_with_id_gte_3 = Coffee.nodes.filter(Q(id___gte=3)).all()
+    assert len(coffees_with_id_gte_3) == 4, "unexpected number of results"
+    assert c3 in coffees_with_id_gte_3
+    assert c4 in coffees_with_id_gte_3
+    assert c5 in coffees_with_id_gte_3
+    assert c6 in coffees_with_id_gte_3
+
+    coffees_5_not_japans = Coffee.nodes.filter(Q(price__gt=5) & ~Q(name="Japans finest")).all()
+    assert c3 not in coffees_5_not_japans
+
+
+def test_traversal_filter_left_hand_statement():
+    nescafe = Coffee(name='Nescafe2', price=99).save()
+    nescafe_gold = Coffee(name='Nescafe gold', price=11).save()
+
+    tesco = Supplier(name='Sainsburys', delivery_cost=3).save()
+    biedronka = Supplier(name='Biedronka', delivery_cost=5).save()
+    lidl = Supplier(name='Lidl', delivery_cost=3).save()
+
+    nescafe.suppliers.connect(tesco)
+    nescafe_gold.suppliers.connect(biedronka)
+    nescafe_gold.suppliers.connect(lidl)
+
+    lidl_supplier = NodeSet(Coffee.nodes.filter(price=11).suppliers).filter(delivery_cost=3).all()
+
+    assert lidl in lidl_supplier
```

### Comparing `cythereal-neomodel-3.2.5/test/test_alias.py` & `cythereal-neomodel-3.3.2/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_label_install.py` & `cythereal-neomodel-3.3.2/test/test_label_install.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from neomodel import config, StructuredNode, StringProperty, install_all_labels, install_labels
+from six import StringIO
+import pytest
+from neo4j.exceptions import DatabaseError
+from neomodel import (
+    config, StructuredNode, StringProperty, install_all_labels, install_labels,
+    UniqueIdProperty)
 from neomodel.core import db
 
 
 config.AUTO_INSTALL_LABELS = False
 
 
 class NoConstraintsSetup(StructuredNode):
@@ -29,7 +34,22 @@
 def test_install_all():
     install_labels(AbstractNode)
     # run install all labels
     install_all_labels()
     assert True
     # remove constraint for above test
     db.cypher_query("DROP CONSTRAINT on (n:NoConstraintsSetup) ASSERT n.name IS UNIQUE")
+
+
+def test_install_labels_db_property():
+    class SomeNode(StructuredNode):
+        id_ = UniqueIdProperty(db_property='id')
+    stdout = StringIO()
+    install_labels(SomeNode, quiet=False, stdout=stdout)
+    assert 'id' in stdout.getvalue()
+    # make sure that the id_ constraint doesn't exist
+    with pytest.raises(DatabaseError) as exc_info:
+        db.cypher_query(
+            'DROP CONSTRAINT on (n:SomeNode) ASSERT n.id_ IS UNIQUE')
+    assert 'No such constraint' in exc_info.exconly()
+    # make sure the id constraint exists and can be removed
+    db.cypher_query('DROP CONSTRAINT on (n:SomeNode) ASSERT n.id IS UNIQUE')
```

### Comparing `cythereal-neomodel-3.2.5/test/test_exceptions.py` & `cythereal-neomodel-3.3.2/test/test_exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import pickle
 
 from neomodel import StructuredNode, StringProperty, DoesNotExist
 
 
-class Person(StructuredNode):
+class EPerson(StructuredNode):
     name = StringProperty(unique_index=True)
 
 
 def test_object_does_not_exist():
     try:
-        Person.nodes.get(name="johnny")
-    except Person.DoesNotExist as e:
+        EPerson.nodes.get(name="johnny")
+    except EPerson.DoesNotExist as e:
         pickle_instance = pickle.dumps(e)
         assert pickle_instance
         assert pickle.loads(pickle_instance)
         assert isinstance(pickle.loads(pickle_instance), DoesNotExist)
     else:
         assert False, "Person.DoesNotExist not raised."
 
 
 def test_pickle_does_not_exist():
     try:
-        raise Person.DoesNotExist("My Test Message")
-    except Person.DoesNotExist as e:
+        raise EPerson.DoesNotExist("My Test Message")
+    except EPerson.DoesNotExist as e:
         pickle_instance = pickle.dumps(e)
         assert pickle_instance
         assert pickle.loads(pickle_instance)
         assert isinstance(pickle.loads(pickle_instance), DoesNotExist)
```

### Comparing `cythereal-neomodel-3.2.5/test/test_indexing.py` & `cythereal-neomodel-3.3.2/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_cardinality.py` & `cythereal-neomodel-3.3.2/test/test_cardinality.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     assert len(m.dryers.all()) == 1
     assert m.dryers.single().version == 1
 
     m.dryers.disconnect(h)
     assert m.dryers.all() == []
     assert m.dryers.single() is None
 
+    h2 = HairDryer(version=2).save()
+    m.dryers.connect(h)
+    m.dryers.connect(h2)
+    m.dryers.disconnect_all()
+    assert m.dryers.all() == []
+    assert m.dryers.single() is None
+
 
 def test_cardinality_zero_or_one():
     m = Monkey(name='bob').save()
     assert m.driver.all() == []
     assert m.driver.single() is None
     h = ScrewDriver(version=1).save()
```

### Comparing `cythereal-neomodel-3.2.5/test/test_cypher.py` & `cythereal-neomodel-3.3.2/test/test_cypher.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_hooks.py` & `cythereal-neomodel-3.3.2/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_relative_relationships.py` & `cythereal-neomodel-3.3.2/test/test_relative_relationships.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/test/test_batch.py` & `cythereal-neomodel-3.3.2/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/neomodel/properties.py` & `cythereal-neomodel-3.3.2/neomodel/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,107 +1,113 @@
-from .exceptions import InflateError, DeflateError, RequiredProperty
-from . import config
-
-from datetime import datetime, date
-from uuid import uuid4
-import re
-import types
-import pytz
+import functools
 import json
 import sys
-import functools
+import types
+import re
+import uuid
+import warnings
+from datetime import date, datetime
+
+import pytz
+
+from neomodel import config
+from neomodel.exceptions import InflateError, DeflateError, RequiredProperty
 
 
 if sys.version_info >= (3, 0):
-    unicode = lambda x: str(x)
+    unicode = str
 
 
 def display_for(key):
     def display_choice(self):
-        return getattr(self.__class__, key).choice_map[getattr(self, key)]
+        return getattr(self.__class__, key).choices[getattr(self, key)]
     return display_choice
 
 
 class PropertyManager(object):
-    # Common methods for handling properties on node and relationship objects
-
-    def __init__(self, *args, **kwargs):
+    """
+    Common methods for handling properties on node and relationship objects.
+    """
 
+    def __init__(self, **kwargs):
         properties = getattr(self, "__all_properties__", None)
         if properties is None:
-            properties = self.defined_properties(rels=False, aliases=False).items()
-        for key, val in properties:
-            # handle default values
-            if key not in kwargs or kwargs[key] is None:
-                if hasattr(val, 'has_default') and val.has_default:
-                    setattr(self, key, val.default_value())
+            properties = \
+                self.defined_properties(rels=False, aliases=False).items()
+        for name, property in properties:
+            if kwargs.get(name) is None:
+                if getattr(property, 'has_default', False):
+                    setattr(self, name, property.default_value())
                 else:
-                    setattr(self, key, None)
+                    setattr(self, name, None)
             else:
-                setattr(self, key, kwargs[key])
+                setattr(self, name, kwargs[name])
 
-            if hasattr(val, 'choices') and getattr(val, 'choices'):
-                setattr(self, 'get_{}_display'.format(key),
-                        types.MethodType(display_for(key), self))
+            if getattr(property, 'choices', None):
+                setattr(self, 'get_{0}_display'.format(name),
+                        types.MethodType(display_for(name), self))
 
-            if key in kwargs:
-                del kwargs[key]
+            if name in kwargs:
+                del kwargs[name]
 
         aliases = getattr(self, "__all_aliases__", None)
         if aliases is None:
-            aliases = self.defined_properties(rels=False, properties=False).items()
-        # aliases next so they don't have their alias over written
-        for key, val in aliases:
-            if key in kwargs:
-                setattr(self, key, kwargs[key])
-                del kwargs[key]
-
-        # undefined properties last (for magic @prop.setters etc)
-        for key, val in kwargs.items():
-            setattr(self, key, val)
+            aliases = self.defined_properties(
+                aliases=True, rels=False, properties=False).items()
+        for name, property in aliases:
+            if name in kwargs:
+                setattr(self, name, kwargs[name])
+                del kwargs[name]
+
+        # undefined properties (for magic @prop.setters etc)
+        for name, property in kwargs.items():
+            setattr(self, name, property)
 
     @property
     def __properties__(self):
         from .relationship_manager import RelationshipManager
-        props = {}
-        for key, value in self.__dict__.items():
-            if not (key.startswith('_')
-                    or isinstance(value,
-                        (types.MethodType, RelationshipManager, AliasProperty,))):
-                props[key] = value
-        return props
+
+        return dict((name, value) for name, value in vars(self).items()
+                    if not name.startswith('_')
+                    and not callable(value)
+                    and not isinstance(value,
+                                       (RelationshipManager, AliasProperty,))
+                    )
 
     @classmethod
-    def deflate(cls, obj_props, obj=None, skip_empty=False):
+    def deflate(cls, properties, obj=None, skip_empty=False):
         # deflate dict ready to be stored
         deflated = {}
-        for key, prop in cls.defined_properties(aliases=False, rels=False).items():
-            # map property name to correct database property
-            db_property = prop.db_property or key
-            if key in obj_props and obj_props[key] is not None:
-                deflated[db_property] = prop.deflate(obj_props[key], obj)
-            elif prop.has_default:
-                deflated[db_property] = prop.deflate(prop.default_value(), obj)
-            elif prop.required or prop.unique_index:
-                raise RequiredProperty(key, cls)
-            elif skip_empty is not True:
+        for name, property \
+                in cls.defined_properties(aliases=False, rels=False).items():
+            db_property = property.db_property or name
+            if properties.get(name) is not None:
+                deflated[db_property] = property.deflate(properties[name], obj)
+            elif property.has_default:
+                deflated[db_property] = property.deflate(
+                    property.default_value(), obj
+                )
+            elif property.required:
+                raise RequiredProperty(name, cls)
+            elif not skip_empty:
                 deflated[db_property] = None
         return deflated
 
     @classmethod
     def defined_properties(cls, aliases=True, properties=True, rels=True):
         from .relationship_manager import RelationshipDefinition
         props = {}
-        for scls in reversed(cls.mro()):
-            for key, prop in scls.__dict__.items():
-                if ((aliases and isinstance(prop, AliasProperty))
-                        or (properties and hasattr(prop, '__class__') and issubclass(prop.__class__, Property)
-                            and not isinstance(prop, AliasProperty))
-                        or (rels and isinstance(prop, RelationshipDefinition))):
-                    props[key] = prop
+        for baseclass in reversed(cls.__mro__):
+            props.update(dict(
+                (name, property) for name, property in vars(baseclass).items()
+                if (aliases and isinstance(property, AliasProperty))
+                or (properties and isinstance(property, Property)
+                    and not isinstance(property, AliasProperty))
+                or (rels and isinstance(property, RelationshipDefinition))
+            ))
         return props
 
 
 def validator(fn):
     fn_name = fn.func_name if hasattr(fn, 'func_name') else fn.__name__
     if fn_name == 'inflate':
         exc_class = InflateError
@@ -184,38 +190,59 @@
             raise Exception("No default value specified")
 
     @property
     def is_indexed(self):
         return self.unique_index or self.index
 
 
-class NormalProperty(Property):
+class NormalizedProperty(Property):
     """
-    Base class for Normalized properties
-
-    Those that use the same normalization method to inflate or deflate.
+    Base class for normalized properties. These use the same normalization
+    method to in- or deflating.
     """
 
     @validator
     def inflate(self, value):
         return self.normalize(value)
 
     @validator
     def deflate(self, value):
         return self.normalize(value)
 
     def default_value(self):
-        default = super(NormalProperty, self).default_value()
+        default = super(NormalizedProperty, self).default_value()
         return self.normalize(default)
 
     def normalize(self, value):
         raise NotImplementedError('Specialize normalize method')
 
 
-class RegexProperty(NormalProperty):
+# TODO remove this with the next major release
+def _warn_NormalProperty_renamed():
+    warnings.warn(
+        'The class NormalProperty was renamed to NormalizedProperty. '
+        'Use that one as base class. The former will be removed in the next '
+        'major release.', DeprecationWarning)
+
+
+if sys.version_info >= (3, 6):
+    class NormalProperty(NormalizedProperty):
+
+        def __init_subclass__(cls, **kwargs):
+            _warn_NormalProperty_renamed()
+else:
+    class NormalProperty(NormalizedProperty):
+
+        def __init__(self, *args, **kwargs):
+            _warn_NormalProperty_renamed()
+            super(NormalProperty, self).__init__(*args, **kwargs)
+##
+
+
+class RegexProperty(NormalizedProperty):
     """
     Validates a property against a regular expression.
 
     If sub-classing set:
 
         expression = r'[^@]+@[^@]+\.[^@]+'
     """
@@ -251,50 +278,64 @@
     """
     Store email addresses
     """
     form_field_class = 'EmailField'
     expression = r'[^@]+@[^@]+\.[^@]+'
 
 
-class StringProperty(Property):
+class StringProperty(NormalizedProperty):
     """
-    Store strings
-    """
-    def __init__(self, choices=None, **kwargs):
-        """
-        :param choices: tuple of tuple pairs.
-        :type: tuple
-        :param kwargs:
-        """
-        super(StringProperty, self).__init__(**kwargs)
-        self.choices = choices
-
-        if self.choices:
-            if not isinstance(self.choices, tuple):
-                raise ValueError("Choices must be a tuple of tuples")
-
-            self.choice_map = dict(self.choices)
-            self.form_field_class = 'TypedChoiceField'
+    Stores a unicode string
 
-    @validator
-    def inflate(self, value):
-        if self.choices and value not in self.choice_map:
-            raise ValueError("Invalid choice {}".format(value))
+    :param choices: A mapping of valid strings to label strings that are used
+                    to display information in an application. If the default
+                    value ``None`` is used, any string is valid.
+    :type choices: Any type that can be used to initiate a :class:`dict`.
+    :param max_length: The maximum non-zero length that this attribute can be
+    :type max_length: int
+    """
+
+    def __init__(self, choices=None, max_length=None, **kwargs):
+        if max_length is not None:
+            if choices is not None:
+                raise ValueError("The arguments `choices` and `max_length` are mutually exclusive.")
+            if max_length<1:
+                raise ValueError("`max_length` cannot be zero or take negative values.")
 
-        return unicode(value)
+        super(StringProperty, self).__init__(**kwargs)
 
-    @validator
-    def deflate(self, value):
-        if self.choices and value not in self.choice_map:
-            raise ValueError("Invalid choice {}".format(value))
+        self.max_length = max_length
+        if choices is None:
+            self.choices = None
+        else:
+            try:
+                self.choices = dict(choices)
+            except Exception:
+                raise ValueError("The choices argument must be convertable to a dictionary.")
+            # Python 3:
+            # except Exception as e:
+            #     raise ValueError("The choices argument must be convertable to "
+            #                      "a dictionary.") from e
+            self.form_field_class = 'TypedChoiceField'
 
+    def normalize(self, value):
+        # One thing to note here is that the following two checks can remain uncoupled
+        # as long as it is guaranteed (by the constructor) that `choices` and `max_length`
+        # are mutually exclusive. If that check in the constructor ever has to be removed, 
+        # these two validation checks here will have to be coupled so that having set 
+        # `choices` overrides having set the `max_length`.
+        if self.choices is not None and value not in self.choices:
+            raise ValueError("Invalid choice: {}".format(value))
+        if self.max_length is not None and len(value) > self.max_length:
+            raise ValueError("Property max length exceeded. Expected {}, got {} == len('{}')".format(
+                             self.max_length, len(value), value))
         return unicode(value)
 
     def default_value(self):
-        return unicode(super(StringProperty, self).default_value())
+        return self.normalize(super(StringProperty, self).default_value())
 
 
 class IntegerProperty(Property):
     """
     Stores an Integer value
     """
     form_field_class = 'IntegerField'
@@ -330,15 +371,15 @@
                 raise TypeError('Expecting neomodel Property')
 
             if isinstance(base_property, ArrayProperty):
                 raise TypeError('Cannot have nested ArrayProperty')
 
             for ilegal_attr in ['default', 'index', 'unique_index', 'required']:
                 if getattr(base_property, ilegal_attr, None):
-                    raise ValueError('ArrayProperty base_property cannot have "{}" set'.format(ilegal_attr))
+                    raise ValueError('ArrayProperty base_property cannot have "{0}" set'.format(ilegal_attr))
 
         self.base_property = base_property
 
         super(ArrayProperty, self).__init__(**kwargs)
 
     @validator
     def inflate(self, value):
@@ -407,14 +448,47 @@
     @validator
     def deflate(self, value):
         if not isinstance(value, date):
             msg = 'datetime.date object expected, got {0}'.format(repr(value))
             raise ValueError(msg)
         return value.isoformat()
 
+class DateTimeFormatProperty(Property):
+    """
+    Store a datetime by custome format
+    :param default_now: If ``True``, the creation time (Local) will be used as default.
+                        Defaults to ``False``.
+    :param format:      Date format string, default is %Y-%m-%d
+
+    :type default_now:  :class:`bool`
+    :type format:       :class:`str`
+    """
+    form_field_class = 'DateTimeFormatField'
+
+    def __init__(self, default_now=False, format="%Y-%m-%d", **kwargs):
+        if default_now:
+            if 'default' in kwargs:
+                raise ValueError('too many defaults')
+            kwargs['default'] = lambda: datetime.now()
+
+        self.format = format
+        super(DateTimeFormatProperty, self).__init__(**kwargs)
+
+    @validator
+    def inflate(self, value):
+        return datetime.strptime(unicode(value), self.format)
+
+    @validator
+    def deflate(self, value):
+        if not isinstance(value, datetime):
+            raise ValueError('datetime object expected, got {0}.'.format(type(value)))
+        return datetime.strftime(value, self.format)
+
+
+
 
 class DateTimeProperty(Property):
     """ A property representing a :class:`datetime.datetime` object as
         unix epoch.
 
         :param default_now: If ``True``, the creation time (UTC) will be used as default.
                             Defaults to ``False``.
@@ -443,27 +517,28 @@
     def deflate(self, value):
         if not isinstance(value, datetime):
             raise ValueError('datetime object expected, got {0}.'.format(type(value)))
         if value.tzinfo:
             value = value.astimezone(pytz.utc)
             epoch_date = datetime(1970, 1, 1, tzinfo=pytz.utc)
         elif config.FORCE_TIMEZONE:
-            raise ValueError("Error deflating {}: No timezone provided.".format(value))
+            raise ValueError("Error deflating {0}: No timezone provided.".format(value))
         else:
             # No timezone specified on datetime object.. assuming UTC
             epoch_date = datetime(1970, 1, 1)
         return float((value - epoch_date).total_seconds())
 
 
 class JSONProperty(Property):
     """
     Store a data structure as a JSON string.
 
     The structure will be inflated when a node is retrieved.
     """
+
     def __init__(self, *args, **kwargs):
         super(JSONProperty, self).__init__(*args, **kwargs)
 
     @validator
     def inflate(self, value):
         return json.loads(value)
 
@@ -472,14 +547,15 @@
         return json.dumps(value)
 
 
 class AliasProperty(property, Property):
     """
     Alias another existing property
     """
+
     def __init__(self, to=None):
         """
         Create new alias
 
         :param to: name of property aliasing
         :type: str
         """
@@ -505,21 +581,22 @@
         return getattr(self.owner, self.aliased_to()).unique_index
 
 
 class UniqueIdProperty(Property):
     """
     A unique identifier, a randomly generated uid (uuid4) with a unique index
     """
+
     def __init__(self, **kwargs):
         for item in ['required', 'unique_index', 'index', 'default']:
             if item in kwargs:
-                raise ValueError('{} argument ignored by {}'.format(item, self.__class__.__name__))
+                raise ValueError('{0} argument ignored by {1}'.format(item, self.__class__.__name__))
 
         kwargs['unique_index'] = True
-        kwargs['default'] = lambda: uuid4().hex
+        kwargs['default'] = lambda: uuid.uuid4().hex
         super(UniqueIdProperty, self).__init__(**kwargs)
 
     @validator
     def inflate(self, value):
         return unicode(value)
 
     @validator
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/relationship.py` & `cythereal-neomodel-3.3.2/neomodel/relationship.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         Save the relationship
 
         :return: self
         """
         props = self.deflate(self.__properties__)
         query = "MATCH ()-[r]->() WHERE id(r)={self} "
         for key in props:
-            query += " SET r.{} = {{{}}}".format(key, key)
+            query += " SET r.{0} = {{{1}}}".format(key, key)
         props['self'] = self.id
 
         db.cypher_query(query, props)
 
         return self
 
     @deprecated('This method will be removed in neomodel 4')
@@ -54,29 +54,29 @@
 
     def start_node(self):
         """
         Get start node
 
         :return: StructuredNode
         """
-        node = self._start_node_class()
-        node.id = self._start_node_id
-        node.refresh()
-        return node
-
+        return db.cypher_query("MATCH (aNode) "
+                               "WHERE id(aNode)={nodeid} "
+                               "RETURN aNode".format(nodeid=self._start_node_id),
+                               resolve_objects = True)[0][0][0]
+      
     def end_node(self):
         """
         Get end node
 
         :return: StructuredNode
         """
-        node = self._end_node_class()
-        node.id = self._end_node_id
-        node.refresh()
-        return node
+        return db.cypher_query("MATCH (aNode) "
+                               "WHERE id(aNode)={nodeid} "
+                               "RETURN aNode".format(nodeid=self._end_node_id),
+                               resolve_objects = True)[0][0][0]
 
     @classmethod
     def inflate(cls, rel):
         """
         Inflate a neo4j_driver relationship object to a neomodel object
         :param rel:
         :return: StructuredRel
@@ -86,11 +86,11 @@
             if key in rel:
                 props[key] = prop.inflate(rel[key], obj=rel)
             elif prop.has_default:
                 props[key] = prop.default_value()
             else:
                 props[key] = None
         srel = cls(**props)
-        srel._start_node_id = rel.start
-        srel._end_node_id = rel.end
+        srel._start_node_id = rel.start_node.id
+        srel._end_node_id = rel.end_node.id
         srel.id = rel.id
         return srel
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/cardinality.py` & `cythereal-neomodel-3.3.2/neomodel/cardinality.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         return [self.single()]
 
     def disconnect(self, node):
         raise AttemptedCardinalityViolation(
             "Cardinality one, cannot disconnect use reconnect."
         )
 
+    def disconnect_all(self):
+        raise AttemptedCardinalityViolation(
+            "Cardinality one, cannot disconnect_all use reconnect."
+        )
+
     def connect(self, node, properties=None):
         """
         Connect a node
 
         :param node:
         :param properties: relationship properties
         :return: True / rel instance
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/contrib/semi_structured.py` & `cythereal-neomodel-3.3.2/neomodel/contrib/semi_structured.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from neomodel.core import StructuredNode
 from neomodel.exceptions import InflateConflict, DeflateConflict
+from neomodel.util import _get_node_properties
 
 
 class SemiStructuredNode(StructuredNode):
     """
     A base class allowing properties to be stored on a node that aren't
     specified in its definition. Conflicting properties are signaled with the
     :class:`DeflateConflict` exception::
@@ -29,26 +30,27 @@
         # support lazy loading
         if isinstance(node, int):
             snode = cls()
             snode.id = node
         else:
             props = {}
             for key, prop in cls.__all_properties__:
-                if key in node.properties:
-                    props[key] = prop.inflate(node.properties[key], node)
+                node_properties = _get_node_properties(node)
+                if key in node_properties:
+                    props[key] = prop.inflate(node_properties[key], node)
                 elif prop.has_default:
                     props[key] = prop.default_value()
                 else:
                     props[key] = None
             # handle properties not defined on the class
-            for free_key in (x for x in node.properties if x not in props):
+            for free_key in (x for x in node_properties if x not in props):
                 if hasattr(cls, free_key):
                     raise InflateConflict(cls, free_key,
-                                          node.properties[free_key], node.id)
-                props[free_key] = node.properties[free_key]
+                                          node_properties[free_key], node.id)
+                props[free_key] = node_properties[free_key]
 
             snode = cls(**props)
             snode.id = node.id
 
         return snode
 
     @classmethod
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/core.py` & `cythereal-neomodel-3.3.2/neomodel/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __future__ import print_function
-import warnings
-import sys
 import re
+import sys
+import warnings
 
-from .exceptions import DoesNotExist
-from .properties import Property, PropertyManager
-from .hooks import hooks
-from .util import Database, classproperty, _UnsavedNode
-from . import config
+from neomodel import config
+from neomodel.exceptions import DoesNotExist, ClassAlreadyDefined
+from neomodel.hooks import hooks
+from neomodel.properties import Property, PropertyManager
+from neomodel.util import Database, classproperty, _UnsavedNode, _get_node_properties
 
 db = Database()
 
 
 def drop_constraints(quiet=True, stdout=None):
     """
     Discover and drop all constraints.
@@ -21,15 +20,15 @@
     """
 
     results, meta = db.cypher_query("CALL db.constraints()")
     pattern = re.compile(':(.*) \).*\.(\w*)')
     for constraint in results:
         db.cypher_query('DROP ' + constraint[0])
         match = pattern.search(constraint[0])
-        stdout.write(''' - Droping unique constraint and index on label {} with property {}.\n'''.format(
+        stdout.write(''' - Droping unique constraint and index on label {0} with property {1}.\n'''.format(
             match.group(1), match.group(2)))
     stdout.write("\n")
 
 
 def drop_indexes(quiet=True, stdout=None):
     """
     Discover and drop all indexes.
@@ -39,15 +38,15 @@
     """
 
     results, meta = db.cypher_query("CALL db.indexes()")
     pattern = re.compile(':(.*)\((.*)\)')
     for index in results:
         db.cypher_query('DROP ' + index[0])
         match = pattern.search(index[0])
-        stdout.write(' - Dropping index on label {} with property {}.\n'.format(
+        stdout.write(' - Dropping index on label {0} with property {1}.\n'.format(
             match.group(1), match.group(2)))
     stdout.write("\n")
 
 
 def remove_all_labels(stdout=None):
     """
     Calls functions for dropping constraints and indexes.
@@ -76,307 +75,215 @@
     :param stdout: stdout stream
     :type: bool
     :return: None
     """
 
     if not hasattr(cls, '__label__'):
         if not quiet:
-            stdout.write(' ! Skipping class {}.{} is abstract\n'.format(cls.__module__, cls.__name__))
+            stdout.write(' ! Skipping class {0}.{1} is abstract\n'.format(cls.__module__, cls.__name__))
         return
 
-    for key, prop in cls.defined_properties(aliases=False, rels=False).items():
-        if prop.index:
+    for name, property in cls.defined_properties(aliases=False, rels=False).items():
+        db_property = property.db_property or name
+        if property.index:
             if not quiet:
-                stdout.write(' + Creating index {} on label {} for class {}.{}\n'.format(
-                    key, cls.__label__, cls.__module__, cls.__name__))
+                stdout.write(' + Creating index {0} on label {1} for class {2}.{3}\n'.format(
+                    name, cls.__label__, cls.__module__, cls.__name__))
 
-            db.cypher_query("CREATE INDEX on :{}({}); ".format(
-                cls.__label__, key))
+            db.cypher_query("CREATE INDEX on :{0}({1}); ".format(
+                cls.__label__, db_property))
 
-        elif prop.unique_index:
+        elif property.unique_index:
             if not quiet:
-                stdout.write(' + Creating unique constraint for {} on label {} for class {}.{}\n'.format(
-                    key, cls.__label__, cls.__module__, cls.__name__))
+                stdout.write(' + Creating unique constraint for {0} on label {1} for class {2}.{3}\n'.format(
+                    name, cls.__label__, cls.__module__, cls.__name__))
 
             db.cypher_query("CREATE CONSTRAINT "
-                            "on (n:{}) ASSERT n.{} IS UNIQUE; ".format(
-                cls.__label__, key))
+                            "on (n:{0}) ASSERT n.{1} IS UNIQUE; ".format(
+                cls.__label__, db_property))
 
 
 def install_all_labels(stdout=None):
     """
     Discover all subclasses of StructuredNode in your application and execute install_labels on each.
     Note: code most be loaded (imported) in order for a class to be discovered.
 
     :param stdout: output stream
     :return: None
     """
 
     if not stdout:
         stdout = sys.stdout
 
-    def subsub(kls):  # recursively return all subclasses
-        return kls.__subclasses__() + [g for s in kls.__subclasses__() for g in subsub(s)]
+    def subsub(cls):  # recursively return all subclasses
+        return cls.__subclasses__() + [g for s in cls.__subclasses__() for g in subsub(s)]
 
     stdout.write("Setting up indexes and constraints...\n\n")
 
     i = 0
     for cls in subsub(StructuredNode):
-        stdout.write('Found {}.{}\n'.format(cls.__module__, cls.__name__))
+        stdout.write('Found {0}.{1}\n'.format(cls.__module__, cls.__name__))
         install_labels(cls, quiet=False, stdout=stdout)
         i += 1
 
     if i:
         stdout.write('\n')
 
-    stdout.write('Finished {} classes.\n'.format(i))
+    stdout.write('Finished {0} classes.\n'.format(i))
 
 
 class NodeMeta(type):
-    def __new__(mcs, name, bases, dct):
-        dct.update({'DoesNotExist': type('DoesNotExist', (DoesNotExist,), {})})
-        inst = super(NodeMeta, mcs).__new__(mcs, name, bases, dct)
+    def __new__(mcs, name, bases, namespace):
+        namespace['DoesNotExist'] = \
+            type(name + 'DoesNotExist', (DoesNotExist,), {})
+        cls = super(NodeMeta, mcs).__new__(mcs, name, bases, namespace)
         # needed by Python < 3.5 for unpickling DoesNotExist objects:
-        inst.DoesNotExist._model_class = inst
+        cls.DoesNotExist._model_class = cls
 
-        if hasattr(inst, '__abstract_node__'):
-            delattr(inst, '__abstract_node__')
+        if hasattr(cls, '__abstract_node__'):
+            delattr(cls, '__abstract_node__')
         else:
-            for key, value in dct.items():
-                if key == 'deleted':
-                    raise ValueError("Class property called 'deleted' conflicts with neomodel internals")
-
-                # If not a class (django-neomodel Meta)
-                if hasattr(value, '__class__') and issubclass(value.__class__, Property):
-                    value.name = key
-                    value.owner = inst
-                    # support for 'magic' properties
-                    if hasattr(value, 'setup') and hasattr(
-                            value.setup, '__call__'):
-                        value.setup()
-
-            # cache the names of all required and unique_index properties
-            all_required = set(name for name, p in inst.defined_properties(aliases=False, rels=False).items()
-                               if p.required or p.unique_index)
-            inst.__required_properties__ = tuple(all_required)
-            # cache all definitions
-            inst.__all_properties__ = tuple(inst.defined_properties(aliases=False, rels=False).items())
-            inst.__all_aliases__ = tuple(inst.defined_properties(properties=False, rels=False).items())
-            inst.__all_relationships__ = tuple(inst.defined_properties(aliases=False, properties=False).items())
+            if 'deleted' in namespace:
+                raise ValueError("Class property called 'deleted' conflicts "
+                                 "with neomodel internals.")
+            for key, value in ((x, y) for x, y in namespace.items()
+                               if isinstance(y, Property)):
+                value.name, value.owner = key, cls
+                if hasattr(value, 'setup') and callable(value.setup):
+                    value.setup()
+
+            # cache various groups of properies
+            cls.__required_properties__ = tuple(
+                name for name, property
+                in cls.defined_properties(aliases=False, rels=False).items()
+                if property.required or property.unique_index
+            )
+            cls.__all_properties__ = tuple(
+                cls.defined_properties(aliases=False, rels=False).items()
+            )
+            cls.__all_aliases__ = tuple(
+                cls.defined_properties(properties=False, rels=False).items()
+            )
+            cls.__all_relationships__ = tuple(
+                cls.defined_properties(aliases=False, properties=False).items()
+            )
 
-            if '__label__' in dct:
-                inst.__label__ = dct['__label__']
-            else:
-                inst.__label__ = inst.__name__
+            cls.__label__ = namespace.get('__label__', name)
 
             if config.AUTO_INSTALL_LABELS:
-                install_labels(inst)
+                install_labels(cls)
 
-        return inst
+            label_set = frozenset(cls.inherited_labels())
+            if label_set not in db._NODE_CLASS_REGISTRY:
+                db._NODE_CLASS_REGISTRY[label_set] = cls
+            else:
+                raise ClassAlreadyDefined(cls, db._NODE_CLASS_REGISTRY)
+
+        return cls
 
 
 NodeBase = NodeMeta('NodeBase', (PropertyManager,), {'__abstract_node__': True})
 
 
 class StructuredNode(NodeBase):
     """
     Base class for all node definitions to inherit from.
 
     If you want to create your own abstract classes set:
         __abstract_node__ = True
     """
 
-    __abstract_node__ = True
-    __required_properties__ = ()
-    __all_properties__ = ()
-    __all_aliases__ = ()
-    __all_relationships__ = ()
-
-    @classproperty
-    def nodes(cls):
-        """
-        Returns a NodeSet object representing all nodes of the classes label
-        :return: NodeSet
-        :rtype: NodeSet
-        """
-        from .match import NodeSet
+    # static properties
 
-        return NodeSet(cls)
-
-    @property
-    def _id(self, val):
-        warnings.warn('the _id property is deprecated please use .id',
-                      category=DeprecationWarning, stacklevel=1)
-        if val:
-            self.id = val
+    __abstract_node__ = True
 
-        return self.id
+    # magic methods
 
     def __init__(self, *args, **kwargs):
         if 'deleted' in kwargs:
             raise ValueError("deleted property is reserved for neomodel")
 
         for key, val in self.__all_relationships__:
             self.__dict__[key] = val.build_manager(self, key)
 
         super(StructuredNode, self).__init__(*args, **kwargs)
 
-    def __str__(self):
-        return repr(self.__properties__)
-
-    def __repr__(self):
-        return '<{}: {}>'.format(self.__class__.__name__, self)
-
     def __eq__(self, other):
         if not isinstance(other, (StructuredNode,)):
             return False
         if hasattr(self, 'id') and hasattr(other, 'id'):
             return self.id == other.id
         return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
-    def labels(self):
-        """
-        Returns list of labels tied to the node from neo4j.
-
-        :return: list of labels
-        :rtype: list
-        """
-        self._pre_action_check('labels')
-        return self.cypher("MATCH (n) WHERE id(n)={self} "
-                           "RETURN labels(n)")[0][0][0]
-
-    def cypher(self, query, params=None):
-        """
-        Execute a cypher query with the param 'self' pre-populated with the nodes neo4j id.
-
-        :param query: cypher query string
-        :type: string
-        :param params: query parameters
-        :type: dict
-        :return: list containing query results
-        :rtype: list
-        """
-        self._pre_action_check('cypher')
-        params = params or {}
-        params.update({'self': self.id})
-        return db.cypher_query(query, params)
-
-    @classmethod
-    def inherited_labels(cls):
-        """
-        Return list of labels from nodes class hierarchy.
+    def __repr__(self):
+        return '<{0}: {1}>'.format(self.__class__.__name__, self)
 
-        :return: list
-        """
-        return [scls.__label__ for scls in cls.mro()
-                if hasattr(scls, '__label__') and not hasattr(
-                scls, '__abstract_node__')]
+    def __str__(self):
+        return repr(self.__properties__)
 
-    @classmethod
-    def category(cls):
-        raise NotImplementedError("Category was deprecated and has now been removed, "
-            "the functionality is now achieved using the {}.nodes attribute".format(cls.__name__))
+    # dynamic properties
 
-    @hooks
-    def save(self):
+    @classproperty
+    def nodes(cls):
         """
-        Save the node to neo4j or raise an exception
-
-        :return: the node instance
+        Returns a NodeSet object representing all nodes of the classes label
+        :return: NodeSet
+        :rtype: NodeSet
         """
+        from .match import NodeSet
+        return NodeSet(cls)
 
-        # create or update instance node
-        if hasattr(self, 'id'):
-            # update
-            params = self.deflate(self.__properties__, self)
-            query = "MATCH (n) WHERE id(n)={self} \n"
-            query += "\n".join(["SET n.{} = {{{}}}".format(key, key) + "\n"
-                                for key in params.keys()])
-            for label in self.inherited_labels():
-                query += "SET n:`{}`\n".format(label)
-            self.cypher(query, params)
-        elif hasattr(self, 'deleted') and self.deleted:
-            raise ValueError("{}.save() attempted on deleted node".format(
-                self.__class__.__name__))
-        else:  # create
-            self.id = self.create(self.__properties__)[0].id
-        return self
-
-    def _pre_action_check(self, action):
-        if hasattr(self, 'deleted') and self.deleted:
-            raise ValueError("{}.{}() attempted on deleted node".format(
-                self.__class__.__name__, action))
-        if not hasattr(self, 'id'):
-            raise ValueError("{}.{}() attempted on unsaved node".format(
-                self.__class__.__name__, action))
-
-    @hooks
-    def delete(self):
-        """
-        Delete a node and it's relationships
+    @property
+    def _id(self, val):
+        warnings.warn('the _id property is deprecated please use .id',
+                      category=DeprecationWarning, stacklevel=1)
+        if val:
+            self.id = val
 
-        :return: True
-        """
-        self._pre_action_check('delete')
-        self.cypher("MATCH (self) WHERE id(self)={self} "
-                    "OPTIONAL MATCH (self)-[r]-()"
-                    " DELETE r, self")
-        del self.__dict__['id']
-        self.deleted = True
-        return True
+        return self.id
 
-    def refresh(self):
-        """
-        Reload the node from neo4j
-        """
-        self._pre_action_check('refresh')
-        if hasattr(self, 'id'):
-            node = self.inflate(self.cypher("MATCH (n) WHERE id(n)={self}"
-                                            " RETURN n")[0][0][0])
-            for key, val in node.__properties__.items():
-                setattr(self, key, val)
-        else:
-            raise ValueError("Can't refresh unsaved node")
+    # methods
 
     @classmethod
     def _build_merge_query(cls, merge_params, update_existing=False, lazy=False, relationship=None):
         """
         Get a tuple of a CYPHER query and a params dict for the specified MERGE query.
 
         :param merge_params: The target node match parameters, each node must have a "create" key and optional "update".
         :type merge_params: list of dict
         :param update_existing: True to update properties of existing nodes, default False to keep existing values.
         :type update_existing: bool
         :rtype: tuple
         """
         query_params = dict(merge_params=merge_params)
-        n_merge = "n:{} {{{}}}".format(':'.join(cls.inherited_labels()),
-                                         ", ".join("{0}: params.create.{0}".format(p) for p in cls.__required_properties__))
+        n_merge = "n:{0} {{{1}}}".format(
+            ":".join(cls.inherited_labels()),
+            ", ".join("{0}: params.create.{0}".format(getattr(cls, p).db_property or p) for p in cls.__required_properties__))
         if relationship is None:
             # create "simple" unwind query
-            query = "UNWIND {{merge_params}} as params\n MERGE ({})\n ".format(n_merge)
+            query = "UNWIND {{merge_params}} as params\n MERGE ({0})\n ".format(n_merge)
         else:
             # validate relationship
             if not isinstance(relationship.source, StructuredNode):
-                raise ValueError("relationship source [%s] is not a StructuredNode" % repr(relationship.source))
+                raise ValueError("relationship source [{0}] is not a StructuredNode".format(repr(relationship.source)))
             relation_type = relationship.definition.get('relation_type')
             if not relation_type:
                 raise ValueError('No relation_type is specified on provided relationship')
 
-            from .match import OUTGOING, _rel_helper
+            from .match import _rel_helper
 
             query_params["source_id"] = relationship.source.id
-            query = "MATCH (source:{}) WHERE ID(source) = {{source_id}}\n ".format(relationship.source.__label__)
+            query = "MATCH (source:{0}) WHERE ID(source) = {{source_id}}\n ".format(relationship.source.__label__)
             query += "WITH source\n UNWIND {merge_params} as params \n "
             query += "MERGE "
-            query += _rel_helper(rhs='source', lhs=n_merge, ident=None,
-                                 relation_type=relation_type, direction=OUTGOING)
+            query += _rel_helper(lhs='source', rhs=n_merge, ident=None,
+                                 relation_type=relation_type, direction=relationship.definition['direction'])
 
         query += "ON CREATE SET n = params.create\n "
         # if update_existing, write properties on match as well
         if update_existing is True:
             query += "ON MATCH SET n += params.update\n"
 
         # close query
@@ -384,14 +291,19 @@
             query += "RETURN id(n)"
         else:
             query += "RETURN n"
 
         return query, query_params
 
     @classmethod
+    def category(cls):
+        raise NotImplementedError("Category was deprecated and has now been removed, "
+            "the functionality is now achieved using the {0}.nodes attribute".format(cls.__name__))
+
+    @classmethod
     def create(cls, *props, **kwargs):
         """
         Call to CREATE with parameters map. A new instance will be created and saved.
 
         :param props: dict of properties to create the nodes.
         :type props: tuple
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
@@ -401,15 +313,15 @@
 
         if 'streaming' in kwargs:
             warnings.warn('streaming is not supported by bolt, please remove the kwarg',
                           category=DeprecationWarning, stacklevel=1)
 
         lazy = kwargs.get('lazy', False)
         # create mapped query
-        query = "CREATE (n:{} {{create_params}})".format(':'.join(cls.inherited_labels()))
+        query = "CREATE (n:{0} {{create_params}})".format(':'.join(cls.inherited_labels()))
 
         # close query
         if lazy:
             query += " RETURN id(n)"
         else:
             query += " RETURN n"
 
@@ -423,67 +335,99 @@
         if not lazy and hasattr(cls, 'post_create'):
             for node in nodes:
                 node.post_create()
 
         return nodes
 
     @classmethod
-    def get_or_create(cls, *props, **kwargs):
+    def create_or_update(cls, *props, **kwargs):
         """
         Call to MERGE with parameters map. A new instance will be created and saved if does not already exists,
-        this is an atomic operation.
-        Parameters must contain all required properties, any non required properties with defaults will be generated.
+        this is an atomic operation. If an instance already exists all optional properties specified will be updated.
 
-        Note that the post_create hook isn't called after get_or_create
+        Note that the post_create hook isn't called after create_or_update
 
-        :param props: dict of properties to get or create the entities with.
+        :param props: List of dict arguments to get or create the entities with.
         :type props: tuple
         :param relationship: Optional, relationship to get/create on when new entity is created.
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :rtype: list
         """
         lazy = kwargs.get('lazy', False)
         relationship = kwargs.get('relationship')
 
-        # build merge query
-        get_or_create_params = [{"create": cls.deflate(p, skip_empty=True)} for p in props]
-        query, params = cls._build_merge_query(get_or_create_params, relationship=relationship, lazy=lazy)
+        # build merge query, make sure to update only explicitly specified properties
+        create_or_update_params = []
+        for specified, deflated in [(p, cls.deflate(p, skip_empty=True)) for p in props]:
+            create_or_update_params.append({"create": deflated,
+                                            "update": dict((k, v) for k, v in deflated.items() if k in specified)})
+        query, params = cls._build_merge_query(create_or_update_params, update_existing=True, relationship=relationship,
+                                               lazy=lazy)
 
         if 'streaming' in kwargs:
             warnings.warn('streaming is not supported by bolt, please remove the kwarg',
                           category=DeprecationWarning, stacklevel=1)
 
         # fetch and build instance for each result
         results = db.cypher_query(query, params)
         return [cls.inflate(r[0]) for r in results[0]]
 
+    def cypher(self, query, params=None):
+        """
+        Execute a cypher query with the param 'self' pre-populated with the nodes neo4j id.
+
+        :param query: cypher query string
+        :type: string
+        :param params: query parameters
+        :type: dict
+        :return: list containing query results
+        :rtype: list
+        """
+        self._pre_action_check('cypher')
+        params = params or {}
+        params.update({'self': self.id})
+        return db.cypher_query(query, params)
+
+    @hooks
+    def delete(self):
+        """
+        Delete a node and it's relationships
+
+        :return: True
+        """
+        self._pre_action_check('delete')
+        self.cypher("MATCH (self) WHERE id(self)={self} "
+                    "OPTIONAL MATCH (self)-[r]-()"
+                    " DELETE r, self")
+        delattr(self, 'id')
+        self.deleted = True
+        return True
+
     @classmethod
-    def create_or_update(cls, *props, **kwargs):
+    def get_or_create(cls, *props, **kwargs):
         """
-        Call to MERGE with parameters map. A new instance will be created and saved if does not already exists,
-        this is an atomic operation. If an instance already exists all optional properties specified will be updated.
+        Call to MERGE with parameters map. A new instance will be created and saved if does not already exist,
+        this is an atomic operation.
+        Parameters must contain all required properties, any non required properties with defaults will be generated.
 
         Note that the post_create hook isn't called after get_or_create
 
-        :param props: List of dict arguments to get or create the entities with.
+        :param props: Arguments to get_or_create as tuple of dict with property names and values to get or create
+                      the entities with.
         :type props: tuple
         :param relationship: Optional, relationship to get/create on when new entity is created.
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :rtype: list
         """
         lazy = kwargs.get('lazy', False)
         relationship = kwargs.get('relationship')
 
-        # build merge query, make sure to update only explicitly specified properties
-        create_or_update_params = []
-        for specified, deflated in [(p, cls.deflate(p, skip_empty=True)) for p in props]:
-            create_or_update_params.append({"create": deflated,
-                                            "update": dict((k, v) for k, v in deflated.items() if k in specified)})
-        query, params = cls._build_merge_query(create_or_update_params, update_existing=True, relationship=relationship,
-                                               lazy=lazy)
+        # build merge query
+        get_or_create_params = [{"create": cls.deflate(p, skip_empty=True)} for p in props]
+        query, params = cls._build_merge_query(get_or_create_params, relationship=relationship, lazy=lazy)
 
         if 'streaming' in kwargs:
             warnings.warn('streaming is not supported by bolt, please remove the kwarg',
                           category=DeprecationWarning, stacklevel=1)
 
         # fetch and build instance for each result
         results = db.cypher_query(query, params)
@@ -497,23 +441,95 @@
         :return: node object
         """
         # support lazy loading
         if isinstance(node, int):
             snode = cls()
             snode.id = node
         else:
+            node_properties = _get_node_properties(node)
             props = {}
             for key, prop in cls.__all_properties__:
                 # map property name from database to object property
                 db_property = prop.db_property or key
 
-                if db_property in node.properties:
-                    props[key] = prop.inflate(node.properties[db_property], node)
+                if db_property in node_properties:
+                    props[key] = prop.inflate(node_properties[db_property], node)
                 elif prop.has_default:
                     props[key] = prop.default_value()
                 else:
                     props[key] = None
 
             snode = cls(**props)
             snode.id = node.id
 
         return snode
+
+    @classmethod
+    def inherited_labels(cls):
+        """
+        Return list of labels from nodes class hierarchy.
+
+        :return: list
+        """
+        return [scls.__label__ for scls in cls.mro()
+                if hasattr(scls, '__label__') and not hasattr(
+                scls, '__abstract_node__')]
+
+    def labels(self):
+        """
+        Returns list of labels tied to the node from neo4j.
+
+        :return: list of labels
+        :rtype: list
+        """
+        self._pre_action_check('labels')
+        return self.cypher("MATCH (n) WHERE id(n)={self} "
+                           "RETURN labels(n)")[0][0][0]
+
+    def _pre_action_check(self, action):
+        if hasattr(self, 'deleted') and self.deleted:
+            raise ValueError("{0}.{1}() attempted on deleted node".format(
+                self.__class__.__name__, action))
+        if not hasattr(self, 'id'):
+            raise ValueError("{0}.{1}() attempted on unsaved node".format(
+                self.__class__.__name__, action))
+
+    def refresh(self):
+        """
+        Reload the node from neo4j
+        """
+        self._pre_action_check('refresh')
+        if hasattr(self, 'id'):
+            request = self.cypher("MATCH (n) WHERE id(n)={self}"
+                                            " RETURN n")[0]
+            if not request or not request[0]:
+                raise self.__class__.DoesNotExist("Can't refresh non existent node")
+            node = self.inflate(request[0][0])
+            for key, val in node.__properties__.items():
+                setattr(self, key, val)
+        else:
+            raise ValueError("Can't refresh unsaved node")
+
+    @hooks
+    def save(self):
+        """
+        Save the node to neo4j or raise an exception
+
+        :return: the node instance
+        """
+
+        # create or update instance node
+        if hasattr(self, 'id'):
+            # update
+            params = self.deflate(self.__properties__, self)
+            query = "MATCH (n) WHERE id(n)={self} \n"
+            query += "\n".join(["SET n.{0} = {{{1}}}".format(key, key) + "\n"
+                                for key in params.keys()])
+            for label in self.inherited_labels():
+                query += "SET n:`{0}`\n".format(label)
+            self.cypher(query, params)
+        elif hasattr(self, 'deleted') and self.deleted:
+            raise ValueError("{0}.save() attempted on deleted node".format(
+                self.__class__.__name__))
+        else:  # create
+            self.id = self.create(self.__properties__)[0].id
+        return self
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/relationship_manager.py` & `cythereal-neomodel-3.3.2/neomodel/relationship_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import functools
 from importlib import import_module
 from .exceptions import NotConnected
-from .util import deprecated
+from .util import deprecated, _get_node_properties
 from .match import OUTGOING, INCOMING, EITHER, _rel_helper, Traversal, NodeSet
 from .relationship import StructuredRel
 
 
 # basestring python 3.x fallback
 try:
     basestring
@@ -46,15 +46,15 @@
 
         return "{0} in {1} direction of type {2} on node ({3}) of class '{4}'".format(
             self.description, direction,
             self.definition['relation_type'], self.source.id, self.source_class.__name__)
 
     def _check_node(self, obj):
         """check for valid node i.e correct class and is saved"""
-        if not isinstance(obj, self.definition['node_class']):
+        if not issubclass(type(obj), self.definition['node_class']):
             raise ValueError("Expected node of class " + self.definition['node_class'].__name__)
         if not hasattr(obj, 'id'):
             raise ValueError("Can't perform operation on unsaved node " + repr(obj))
 
     @check_source
     def connect(self, node, properties=None):
         """
@@ -104,14 +104,27 @@
 
         if hasattr(rel_instance, 'post_save'):
             rel_instance.post_save()
 
         return rel_instance
 
     @check_source
+    def replace(self, node, properties=None):
+        """
+        Disconnect all existing nodes and connect the supplied node
+
+        :param node:
+        :param properties: for the new relationship
+        :type: dict
+        :return:
+        """
+        self.disconnect_all()
+        self.connect(node, properties)
+
+    @check_source
     def relationship(self, node):
         """
         Retrieve the relationship object for this first relationship between self and node.
 
         :param node:
         :return: StructuredRel
         """
@@ -173,28 +186,29 @@
         old_rel = _rel_helper(lhs='us', rhs='old', ident='r', **self.definition)
 
         # get list of properties on the existing rel
         result, meta = self.source.cypher(
             "MATCH (us), (old) WHERE id(us)={self} and id(old)={old} "
             "MATCH " + old_rel + " RETURN r", {'old': old_node.id})
         if result:
-            existing_properties = result[0][0].properties.keys()
+            node_properties = _get_node_properties(result[0][0])
+            existing_properties = node_properties.keys()
         else:
             raise NotConnected('reconnect', self.source, old_node)
 
         # remove old relationship and create new one
         new_rel = _rel_helper(lhs='us', rhs='new', ident='r2', **self.definition)
         q = "MATCH (us), (old), (new) " \
             "WHERE id(us)={self} and id(old)={old} and id(new)={new} " \
             "MATCH " + old_rel
         q += " CREATE UNIQUE" + new_rel
 
         # copy over properties if we have
         for p in existing_properties:
-            q += " SET r2.{} = r.{}".format(p, p)
+            q += " SET r2.{0} = r.{1}".format(p, p)
         q += " WITH r DELETE r"
 
         self.source.cypher(q, {'old': old_node.id, 'new': new_node.id})
 
     @check_source
     def disconnect(self, node):
         """
@@ -205,14 +219,26 @@
         """
         rel = _rel_helper(lhs='a', rhs='b', ident='r', **self.definition)
         q = "MATCH (a), (b) WHERE id(a)={self} and id(b)={them} " \
             "MATCH " + rel + " DELETE r"
         self.source.cypher(q, {'them': node.id})
 
     @check_source
+    def disconnect_all(self):
+        """
+        Disconnect all nodes
+
+        :return:
+        """
+        rhs = 'b:' + self.definition['node_class'].__label__
+        rel = _rel_helper(lhs='a', rhs=rhs, ident='r', **self.definition)
+        q = 'MATCH (a) WHERE id(a)={self} MATCH ' + rel + ' DELETE r'
+        self.source.cypher(q)
+
+    @check_source
     def _new_traversal(self):
         return Traversal(self.source, self.name, self.definition)
 
     # The methods below simply proxy the match engine.
     def get(self, **kwargs):
         """
         Retrieve a related node with the matching node properties.
@@ -350,15 +376,15 @@
                 # __name__ is the namespace of the parent module for __init__.py files,
                 # and the namespace of the current module for other .py files,
                 # therefore there's a need to define the namespace differently for
                 # these two cases in order for . in relative imports to work correctly
                 # (i.e. to mean the same thing for both cases).
                 # For example in the comments below, namespace == myapp, always
                 if not hasattr(self, 'module_file'):
-                    raise ImportError("Couldn't lookup '{}'".format(name))
+                    raise ImportError("Couldn't lookup '{0}'".format(name))
 
                 if '__init__.py' in self.module_file:
                     # e.g. myapp/__init__.py -[__name__]-> myapp
                     namespace = self.module_name
                 else:
                     # e.g. myapp/models.py -[__name__]-> myapp.models
                     namespace = self.module_name.rpartition('.')[0]
@@ -383,15 +409,14 @@
     """
     description = "zero or more relationships"
 
 
 def _relate(cls_name, direction, rel_type, cardinality=None, model=None):
     if not isinstance(cls_name, (basestring, object)):
         raise ValueError('Expected class name or class got ' + repr(cls_name))
-    from .relationship import StructuredRel # TODO
 
     if model and not issubclass(model, (StructuredRel,)):
         raise ValueError('model must be a StructuredRel')
     return RelationshipDefinition(rel_type, cls_name, direction, cardinality, model)
 
 
 def RelationshipTo(cls_name, rel_type, cardinality=ZeroOrMore, model=None):
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/match.py` & `cythereal-neomodel-3.3.2/neomodel/match.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .core import StructuredNode, db
 from .properties import AliasProperty
 from .exceptions import MultipleNodesReturned
+from .match_q import Q, QBase
 import inspect
 import re
 OUTGOING, INCOMING, EITHER = 1, -1, 0
 
+
 # basestring python 3.x fallback
 try:
     basestring
 except NameError:
     basestring = str
 
 
@@ -40,25 +42,25 @@
     else:
         stmt = '-{0}-'
 
     rel_props = ''
 
     if relation_properties:
         rel_props = ' {{{0}}}'.format(', '.join(
-            ['{}: {}'.format(key, value) for key, value in relation_properties.items()]))
+            ['{0}: {1}'.format(key, value) for key, value in relation_properties.items()]))
 
     # direct, relation_type=None is unspecified, relation_type
     if relation_type is None:
         stmt = stmt.format('')
     # all("*" wildcard) relation_type
     elif relation_type == '*':
         stmt = stmt.format('[*]')
     else:
         # explicit relation_type
-        stmt = stmt.format('[%s:`%s`%s]' % (ident if ident else '', relation_type, rel_props))
+        stmt = stmt.format('[{0}:`{1}`{2}]'.format(ident if ident else '', relation_type, rel_props))
 
     return "({0}){1}({2})".format(lhs, stmt, rhs)
 
 
 # special operators
 _SPECIAL_OPERATOR_IN = 'IN'
 _SPECIAL_OPERATOR_INSENSITIVE = '(?i)'
@@ -111,61 +113,61 @@
     For a StructuredNode class install Traversal objects for each
     relationship definition on a NodeSet instance
     """
     rels = cls.defined_properties(rels=True, aliases=False, properties=False)
 
     for key, value in rels.items():
         if hasattr(node_set, key):
-            raise ValueError("Can't install traversal '{}' exists on NodeSet".format(key))
+            raise ValueError("Can't install traversal '{0}' exists on NodeSet".format(key))
 
         rel = getattr(cls, key)
         rel._lookup_node_class()
 
-        traversal = Traversal(source=node_set, key=key, definition=rel.definition)
+        traversal = Traversal(source=node_set, name=key, definition=rel.definition)
         setattr(node_set, key, traversal)
 
 
 def process_filter_args(cls, kwargs):
     """
     loop through properties in filter parameters check they match class definition
     deflate them and convert into something easy to generate cypher from
     """
 
     output = {}
 
     for key, value in kwargs.items():
         if '__' in key:
-            prop, operator = key.split('__')
+            prop, operator = key.rsplit('__')
             operator = OPERATOR_TABLE[operator]
         else:
             prop = key
             operator = '='
 
         if prop not in cls.defined_properties(rels=False):
-            raise ValueError("No such property {} on {}".format(prop, cls.__name__))
+            raise ValueError("No such property {0} on {1}".format(prop, cls.__name__))
 
         property_obj = getattr(cls, prop)
         if isinstance(property_obj, AliasProperty):
             prop = property_obj.aliased_to()
             deflated_value = getattr(cls, prop).deflate(value)
         else:
             # handle special operators
             if operator == _SPECIAL_OPERATOR_IN:
                 if not isinstance(value, tuple) and not isinstance(value, list):
-                    raise ValueError('Value must be a tuple or list for IN operation {}={}'.format(key, value))
+                    raise ValueError('Value must be a tuple or list for IN operation {0}={1}'.format(key, value))
                 deflated_value = [property_obj.deflate(v) for v in value]
             elif operator == _SPECIAL_OPERATOR_ISNULL:
                 if not isinstance(value, bool):
-                    raise ValueError('Value must be a bool for isnull operation on {}'.format(key))
+                    raise ValueError('Value must be a bool for isnull operation on {0}'.format(key))
                 operator = 'IS NULL' if value else 'IS NOT NULL'
                 deflated_value = None
             elif operator in _REGEX_OPERATOR_TABLE.values():
                 deflated_value = property_obj.deflate(value)
                 if not isinstance(deflated_value, basestring):
-                    raise ValueError('Must be a string value for {}'.format(key))
+                    raise ValueError('Must be a string value for {0}'.format(key))
                 if operator in _STRING_REGEX_OPERATOR_TABLE.values():
                     deflated_value = re.escape(deflated_value)
                 deflated_value = operator.format(deflated_value)
                 operator = _SPECIAL_OPERATOR_REGEX
             else:
                 deflated_value = property_obj.deflate(value)
 
@@ -183,15 +185,15 @@
     """
     rel_definitions = cls.defined_properties(properties=False, rels=True, aliases=False)
 
     match, dont_match = {}, {}
 
     for key, value in kwargs.items():
         if key not in rel_definitions:
-            raise ValueError("No such relation {} defined on a {}".format(key, cls.__name__))
+            raise ValueError("No such relation {0} defined on a {1}".format(key, cls.__name__))
 
         rhs_ident = key
 
         rel_definitions[key]._lookup_node_class()
 
         if value is True:
             match[rhs_ident] = rel_definitions[key].definition
@@ -233,33 +235,33 @@
                 ident = self.build_source(source.source)
 
             self.build_additional_match(ident, source)
 
             if hasattr(source, '_order_by'):
                 self.build_order_by(ident, source)
 
-            if source.filters:
-                self.build_where_stmt(ident, source.filters)
+            if source.filters or source.q_filters:
+                self.build_where_stmt(ident, source.filters, source.q_filters, source_class=source.source_class)
 
             return ident
         elif isinstance(source, StructuredNode):
             return self.build_node(source)
         else:
             raise ValueError("Unknown source type " + repr(source))
 
     def create_ident(self):
         self._ident_count += 1
         return 'r' + str(self._ident_count)
 
     def build_order_by(self, ident, source):
         if '?' in source._order_by:
-            self._ast['with'] = '{}, rand() as r'.format(ident)
+            self._ast['with'] = '{0}, rand() as r'.format(ident)
             self._ast['order_by'] = 'r'
         else:
-            self._ast['order_by'] = ['{}.{}'.format(ident, p)
+            self._ast['order_by'] = ['{0}.{1}'.format(ident, p)
                                      for p in source._order_by]
 
     def build_traversal(self, traversal):
         """
         traverse a relationship from a node to a set of nodes
         """
         # build source
@@ -281,29 +283,29 @@
         return traversal.name
 
     def build_node(self, node):
         ident = node.__class__.__name__.lower()
         place_holder = self._register_place_holder(ident)
 
         # Hack to emulate START to lookup a node by id
-        _node_lookup = 'MATCH ({}) WHERE id({})={{{}}} WITH {}'.format(ident, ident, place_holder, ident)
+        _node_lookup = 'MATCH ({0}) WHERE id({1})={{{2}}} WITH {3}'.format(ident, ident, place_holder, ident)
         self._ast['lookup'] = _node_lookup
 
         self._query_params[place_holder] = node.id
 
         self._ast['return'] = ident
         self._ast['result_class'] = node.__class__
         return ident
 
     def build_label(self, ident, cls):
         """
         match nodes by a label
         """
         ident_w_label = ident + ':' + cls.__label__
-        self._ast['match'].append('({})'.format(ident_w_label))
+        self._ast['match'].append('({0})'.format(ident_w_label))
         self._ast['return'] = ident
         self._ast['result_class'] = cls
         return ident
 
     def build_additional_match(self, ident, node_set):
         """
             handle additional matches supplied by 'has()' calls
@@ -329,48 +331,79 @@
     def _register_place_holder(self, key):
         if key in self._place_holder_registry:
             self._place_holder_registry[key] += 1
         else:
             self._place_holder_registry[key] = 1
         return key + '_' + str(self._place_holder_registry[key])
 
-    def build_where_stmt(self, ident, filters):
+    def _parse_q_filters(self, ident, q, source_class):
+        target = []
+        for child in q.children:
+            if isinstance(child, QBase):
+                q_childs = self._parse_q_filters(ident, child, source_class)
+                if child.connector == Q.OR:
+                    q_childs = "(" + q_childs + ")"
+                target.append(q_childs)
+            else:
+                kwargs = {child[0]: child[1]}
+                filters = process_filter_args(source_class, kwargs)
+                for prop, op_and_val in filters.items():
+                    op, val = op_and_val
+                    if op in _UNARY_OPERATORS:
+                        # unary operators do not have a parameter
+                        statement = '{0}.{1} {2}'.format(ident, prop, op)
+                    else:
+                        place_holder = self._register_place_holder(ident + '_' + prop)
+                        statement = '{0}.{1} {2} {{{3}}}'.format(ident, prop, op, place_holder)
+                        self._query_params[place_holder] = val
+                    target.append(statement)
+        ret = ' {0} '.format(q.connector).join(target)
+        if q.negated:
+            ret = 'NOT ({0})'.format(ret)
+        return ret
+
+    def build_where_stmt(self, ident, filters, q_filters=None, source_class=None):
         """
         construct a where statement from some filters
         """
-        stmts = []
-        for row in filters:
-            negate = False
-
-            # pre-process NOT cases as they are nested dicts
-            if '__NOT__' in row and len(row) == 1:
-                negate = True
-                row = row['__NOT__']
-
-            for prop, op_and_val in row.items():
-                op, val = op_and_val
-                if op in _UNARY_OPERATORS:
-                    # unary operators do not have a parameter
-                    statement = '{} {}.{} {}'.format('NOT' if negate else '', ident, prop, op)
-                else:
-                    place_holder = self._register_place_holder(ident + '_' + prop)
-                    statement = '{} {}.{} {} {{{}}}'.format('NOT' if negate else '', ident, prop, op, place_holder)
-                    self._query_params[place_holder] = val
-                stmts.append(statement)
+        if q_filters is not None:
+            stmts = self._parse_q_filters(ident, q_filters, source_class)
+            if stmts:
+                self._ast['where'].append(stmts)
+        else:
+            stmts = []
+            for row in filters:
+                negate = False
+
+                # pre-process NOT cases as they are nested dicts
+                if '__NOT__' in row and len(row) == 1:
+                    negate = True
+                    row = row['__NOT__']
+
+                for prop, op_and_val in row.items():
+                    op, val = op_and_val
+                    if op in _UNARY_OPERATORS:
+                        # unary operators do not have a parameter
+                        statement = '{0} {1}.{2} {3}'.format('NOT' if negate else '', ident, prop, op)
+                    else:
+                        place_holder = self._register_place_holder(ident + '_' + prop)
+                        statement = '{0} {1}.{2} {3} {{{4}}}'.format('NOT' if negate else '', ident, prop, op, place_holder)
+                        self._query_params[place_holder] = val
+                    stmts.append(statement)
 
-        self._ast['where'].append(' AND '.join(stmts))
+            self._ast['where'].append(' AND '.join(stmts))
 
     def build_query(self):
         query = ''
 
         if 'lookup' in self._ast:
             query += self._ast['lookup']
 
         query += ' MATCH '
-        query += ', '.join(['({})'.format(i) for i in self._ast['match']])
+        query += ', '.join(['({0})'.format(i) for i in self._ast['match']])
 
         if 'where' in self._ast and self._ast['where']:
             query += ' WHERE '
             query += ' AND '.join(self._ast['where'])
 
         if 'with' in self._ast and self._ast['with']:
             query += ' WITH '
@@ -387,52 +420,60 @@
 
         if 'limit' in self._ast:
             query += ' LIMIT {0:d}'.format(self._ast['limit'])
 
         return query
 
     def _count(self):
-        self._ast['return'] = 'count({})'.format(self._ast['return'])
+        self._ast['return'] = 'count({0})'.format(self._ast['return'])
         # drop order_by, results in an invalid query
         self._ast.pop('order_by', None)
         query = self.build_query()
         results, _ = db.cypher_query(query, self._query_params)
         return int(results[0][0])
 
     def _contains(self, node_id):
         # inject id = into ast
         ident = self._ast['return']
         place_holder = self._register_place_holder(ident + '_contains')
-        self._ast['where'].append('id({}) = {{{}}}'.format(ident, place_holder))
+        self._ast['where'].append('id({0}) = {{{1}}}'.format(ident, place_holder))
         self._query_params[place_holder] = node_id
-        return self._count() == 1
+        return self._count() >= 1
 
-    def _execute(self):
+    def _execute(self, lazy=False):
+        if lazy:
+            # inject id = into ast
+            self._ast['return'] = 'id({})'.format(self._ast['return'])
         query = self.build_query()
-        results, _ = db.cypher_query(query, self._query_params)
+        results, _ = db.cypher_query(query, self._query_params, resolve_objects=True)            
+        # The following is not as elegant as it could be but had to be copied from the 
+        # version prior to cypher_query with the resolve_objects capability.
+        # It seems that certain calls are only supposed to be focusing to the first 
+        # result item returned (?)
         if results:
-            return [self._ast['result_class'].inflate(n[0]) for n in results]
+            return [n[0] for n in results]
         return []
-
-
+        
+        
 class BaseSet(object):
     """
     Base class for all node sets.
 
     Contains common python magic methods, __len__, __contains__ etc
     """
     query_cls = QueryBuilder
 
-    def all(self):
+    def all(self, lazy=False):
         """
         Return all nodes belonging to the set
+        :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :return: list of nodes
         :rtype: list
         """
-        return self.query_cls(self).build_ast()._execute()
+        return self.query_cls(self).build_ast()._execute(lazy)
 
     def __iter__(self):
         return (i for i in self.query_cls(self).build_ast()._execute())
 
     def __len__(self):
         return self.query_cls(self).build_ast()._count()
 
@@ -484,31 +525,34 @@
         else:
             raise ValueError("Bad source for nodeset " + repr(source))
 
         # setup Traversal objects using relationship definitions
         install_traversals(self.source_class, self)
 
         self.filters = []
+        self.q_filters = Q()
 
         # used by has()
         self.must_match = {}
         self.dont_match = {}
 
-    def get(self, **kwargs):
+    def _get(self, limit=None, lazy=False, **kwargs):
+        self.filter(**kwargs)
+        if limit:
+            self.limit = limit
+        return self.query_cls(self).build_ast()._execute(lazy)
+
+    def get(self, lazy=False, **kwargs):
         """
         Retrieve one node from the set matching supplied parameters
-
+        :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :param kwargs: same syntax as `filter()`
         :return: node
         """
-        output = process_filter_args(self.source_class, kwargs)
-        if output:
-            self.filters.append(output)
-        self.limit = 2
-        result = self.query_cls(self).build_ast()._execute()
+        result = self._get(limit=2, lazy=lazy, **kwargs)
         if len(result) > 1:
             raise MultipleNodesReturned(repr(kwargs))
         elif not result:
             raise self.source_class.DoesNotExist(repr(kwargs))
         else:
             return result[0]
 
@@ -520,15 +564,40 @@
         :return: node or none
         """
         try:
             return self.get(**kwargs)
         except self.source_class.DoesNotExist:
             pass
 
-    def filter(self, **kwargs):
+    def first(self, **kwargs):
+        """
+        Retrieve the first node from the set matching supplied parameters
+
+        :param kwargs: same syntax as `filter()`
+        :return: node
+        """
+        result = result = self._get(limit=1, **kwargs)
+        if result:
+            return result[0]
+        else:
+            raise self.source_class.DoesNotExist(repr(kwargs))
+
+    def first_or_none(self, **kwargs):
+        """
+        Retrieve the first node from the set matching supplied parameters or return none
+
+        :param kwargs: same syntax as `filter()`
+        :return: node or none
+        """
+        try:
+            return self.first(**kwargs)
+        except self.source_class.DoesNotExist:
+            pass
+
+    def filter(self, *args, **kwargs):
         """
         Apply filters to the existing nodes in the set.
 
         :param kwargs: filter parameters
 
             Filters mimic Django's syntax with the double '__' to separate field and operators.
 
@@ -551,30 +620,27 @@
              * 'startswith': string starts with
              * 'istartswith': case insensitive string starts with
              * 'endswith': string ends with
              * 'iendswith': case insensitive string ends with
 
         :return: self
         """
-
-        output = process_filter_args(self.source_class, kwargs)
-        if output:
-            self.filters.append(output)
+        if args or kwargs:
+            self.q_filters = Q(self.q_filters & Q(*args, **kwargs))
         return self
 
-    def exclude(self, **kwargs):
+    def exclude(self, *args, **kwargs):
         """
         Exclude nodes from the NodeSet via filters.
 
         :param kwargs: filter parameters see syntax for the filter method
         :return: self
         """
-        output = process_filter_args(self.source_class, kwargs)
-        if output:
-            self.filters.append({'__NOT__': output})
+        if args or kwargs:
+            self.q_filters = Q(self.q_filters & ~Q(*args, **kwargs))
         return self
 
     def has(self, **kwargs):
         must_match, dont_match = process_has_args(self.source_class, kwargs)
         self.must_match.update(must_match)
         self.dont_match.update(dont_match)
         return self
@@ -597,65 +663,83 @@
                 if prop.startswith('-'):
                     prop = prop[1:]
                     desc = True
                 else:
                     desc = False
 
                 if prop not in self.source_class.defined_properties(rels=False):
-                    raise ValueError("No such property {} on {}".format(
+                    raise ValueError("No such property {0} on {1}".format(
                         prop, self.source_class.__name__))
 
                 property_obj = getattr(self.source_class, prop)
                 if isinstance(property_obj, AliasProperty):
                     prop = property_obj.aliased_to()
 
                 self._order_by.append(prop + (' DESC' if desc else ''))
 
         return self
 
 
 class Traversal(BaseSet):
     """
-    Models a traversal from a node to another, inherits from BaseSet
+    Models a traversal from a node to another.
+
+    :param source: Starting of the traversal.
+    :type source: A :class:`~neomodel.core.StructuredNode` subclass, an
+                  instance of such, a :class:`~neomodel.match.NodeSet` instance
+                  or a :class:`~neomodel.match.Traversal` instance.
+    :param name: A name for the traversal.
+    :type name: :class:`str`
+    :param definition: A relationship definition that most certainly deserves
+                       a documentation here.
+    :type defintion: :class:`dict`
     """
 
-    def __init__(self, source, key, definition):
+    def __init__(self, source, name, definition):
         """
         Create a traversal
-        :param source: start of traversal could be any of: StructuredNode instance, StucturedNode class, NodeSet
-        :param key:
-        :param definition: relationship definition
+
         """
         self.source = source
 
         if isinstance(source, Traversal):
             self.source_class = source.target_class
         elif inspect.isclass(source) and issubclass(source, StructuredNode):
             self.source_class = source
         elif isinstance(source, StructuredNode):
             self.source_class = source.__class__
         elif isinstance(source, NodeSet):
             self.source_class = source.source_class
         else:
-            raise ValueError("Bad source for traversal: {}".format(repr(source)))
+            raise TypeError("Bad source for traversal: "
+                            "{0}".format(type(source)))
+
+        invalid_keys = (
+                set(definition) - {'direction', 'model', 'node_class', 'relation_type'}
+        )
+        if invalid_keys:
+            raise ValueError(
+                'Unallowed keys in Traversal definition: {invalid_keys}'
+                .format(invalid_keys=invalid_keys)
+            )
 
         self.definition = definition
         self.target_class = definition['node_class']
-        self.name = key
+        self.name = name
         self.filters = []
 
     def match(self, **kwargs):
         """
         Traverse relationships with properties matching the given parameters.
 
             e.g: `.match(price__lt=10)`
 
         :param kwargs: see `NodeSet.filter()` for syntax
         :return: self
         """
         if kwargs:
-            if 'model' not in self.definition or self.definition['model'] is None:
+            if 'model' not in self.definition or self.definition.get('model') is None:
                 raise ValueError("match() with filter only available on relationships with a model")
             output = process_filter_args(self.definition['model'], kwargs)
             if output:
                 self.filters.append(output)
         return self
```

### Comparing `cythereal-neomodel-3.2.5/neomodel/__init__.py` & `cythereal-neomodel-3.3.2/neomodel/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # pep8: noqa
+import pkg_resources
 from .core import *
 from neomodel.exceptions import *
 from .util import clear_neo4j_database, change_neo4j_password
-from .relationship_manager import (NotConnected, OUTGOING, INCOMING, EITHER,
-        RelationshipTo, RelationshipFrom, Relationship, RelationshipManager, RelationshipDefinition)
+from neomodel.match import EITHER, INCOMING, OUTGOING, NodeSet, Traversal
+from neomodel.match_q import Q  # noqa
+from neomodel.relationship_manager import (
+    NotConnected, RelationshipTo, RelationshipFrom, Relationship,
+    RelationshipManager, RelationshipDefinition
+)
 from .relationship import StructuredRel
 from .cardinality import (ZeroOrMore, OneOrMore, ZeroOrOne, One)
 from .properties import (StringProperty, IntegerProperty, AliasProperty,
-        FloatProperty, BooleanProperty, DateTimeProperty, DateProperty,
-        NormalProperty, RegexProperty, EmailProperty,
-        JSONProperty, ArrayProperty, UniqueIdProperty)
+                         FloatProperty, BooleanProperty, 
+                         DateTimeFormatProperty, DateTimeProperty,
+                         DateProperty, NormalizedProperty, RegexProperty,
+                         EmailProperty, JSONProperty, ArrayProperty,
+                         UniqueIdProperty)
 
 __author__ = 'Robin Edwards'
 __email__ = 'robin.ge@gmail.com'
 __license__ = 'MIT'
 __package__ = 'neomodel'
-__version__ = '3.2.4'
+__version__ = pkg_resources.get_distribution('neomodel').version
```

### Comparing `cythereal-neomodel-3.2.5/PKG-INFO` & `cythereal-neomodel-3.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,132 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cythereal-neomodel
-Version: 3.2.5
+Version: 3.3.2
 Summary: An object mapper for the neo4j graph database.
-Home-page: http://github.com/robinedwards/neomodel
+Home-page: http://github.com/neo4j-contrib/neomodel
 Author: Robin Edwards
 Author-email: robin.ge@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: .. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
-           :alt: neomodel
-        
-        NOTE: This is a customized version of neomodel for personal use. Use the
-        `official version`_ instead.
-        
-        An Object Graph Mapper (OGM) for the neo4j_ graph database, built on the awesome neo4j_driver_
-        
-        - Familiar Django model style definitions.
-        - Powerful query API.
-        - Enforce your schema through cardinality restrictions.
-        - Full transaction support.
-        - Thread safe.
-        - pre/post save/delete hooks.
-        - Django integration via django_neomodel_
-        
-        .. _django_neomodel: https://github.com/robinedwards/django-neomodel
-        .. _neo4j: https://www.neo4j.org
-        .. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
-        .. _official version: https://github.com/neo4j-contrib/neomodel
-        
-        .. image:: https://secure.travis-ci.org/robinedwards/neomodel.png
-            :target: https://secure.travis-ci.org/robinedwards/neomodel/
-        
-        .. image:: https://readthedocs.org/projects/neomodel/badge/?version=latest
-            :alt: Documentation Status
-            :scale: 100%
-            :target: https://neomodel.readthedocs.io/en/latest/?badge=latest
-        
-        Documentation
-        =============
-        
-        Available on readthedocs_.
-        
-        .. _readthedocs: http://neomodel.readthedocs.org
-        
-        Requirements
-        ============
-        
-        - Python 2.7, 3.4+
-        - neo4j 3.0, 3.1, 3.2, 3.3
-        
-        Installation
-        ============
-        
-        Install from pypi (recommended)::
-        
-            $ pip install neomodel
-        
-        To install from github::
-        
-            $ pip install git+git://github.com/robinedwards/neomodel.git@HEAD#egg=neomodel-dev
-        
-        Upgrading 2.x to 3.x
-        ====================
-        
-         * Now utilises neo4j_driver as the backend which uses bolt so neo4j 3 is required
-         * Connection now set through config.DATABASE_URL (see getting started docs)
-         * The deprecated category() method on StructuredNode has been removed
-         * The deprecated index property on StructuredNode has been removed
-         * The streaming=True flag is now irrelevant with bolt and produces a deprecation warning
-         * Batch operations must now be wrapped in a transaction in order to be atomic
-         * Indexing NodeSets returns a single node now as opposed to a list
-        
-        Contributing
-        ============
-        
-        Ideas, bugs, tests and pull requests always welcome.
-        
-        Running the test suite
-        ----------------------
-        
-        Make sure you have a fresh virtualenv and `nose` installed::
-        
-            $ pip install nose
-        
-        Also a Neo4j database version 3 or higher to run the tests on. (it will wipe this database for each test run)::
-        
-            $ export NEO4J_BOLT_URL=bolt://neo4j:neo4j@localhost:7687 # (the default)
-        
-        Setup a virtual environment, install neomodel for development and run the test suite::
-        
-            $ virtualenv venv
-            $ source venv/bin/activate
-            $ python setup.py develop
-            $ nosetests -s
-        
-        If your running a neo4j database for the first time the test suite will set the password to 'test'.
-        
-        If you have ``docker-compose`` installed, you can run the test suite against all supported Python
-        interpreters and neo4j versions::
-        
-            # in the project's root folder:
-            $ ./tests-with-docker-compose.sh
-        
-        
-        .. image:: https://badges.gitter.im/Join%20Chat.svg
-           :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-           :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
 Keywords: graph neo4j ORM OGM
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
+License-File: LICENSE
+License-File: AUTHORS.txt
+
+.. image:: https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png
+   :alt: neomodel
+
+NOTE: This is a customized version of neomodel for personal use. Use the
+`official version`_ instead.
+
+An Object Graph Mapper (OGM) for the neo4j_ graph database, built on the awesome neo4j_driver_
+
+- Familiar Django model style definitions.
+- Powerful query API.
+- Enforce your schema through cardinality restrictions.
+- Full transaction support.
+- Thread safe.
+- pre/post save/delete hooks.
+- Django integration via django_neomodel_
+
+.. _django_neomodel: https://github.com/neo4j-contrib/django-neomodel
+.. _neo4j: https://neo4j.com/
+.. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
+.. _official version: https://github.com/neo4j-contrib/neomodel
+
+.. image:: https://secure.travis-ci.org/neo4j-contrib/neomodel.png
+    :target: https://secure.travis-ci.org/neo4j-contrib/neomodel/
+
+.. image:: https://readthedocs.org/projects/neomodel/badge/?version=latest
+    :alt: Documentation Status
+    :scale: 100%
+    :target: https://neomodel.readthedocs.io/en/latest/?badge=latest
+
+
+Documentation
+=============
+
+Available on readthedocs_.
+
+.. _readthedocs: http://neomodel.readthedocs.org
+
+Requirements
+============
+
+- Python 2.7 (Up to version 3.3.1), 3.4+
+- neo4j 3.0, 3.1, 3.2, 3.3
+
+Installation
+============
+
+Install from pypi (recommended)::
+
+    $ pip install neomodel
+
+To install from github::
+
+    $ pip install git+git://github.com/neo4j-contrib/neomodel.git@HEAD#egg=neomodel-dev
+
+Upgrading 2.x to 3.x
+====================
+
+ * Now utilises neo4j_driver as the backend which uses bolt so neo4j 3 is required
+ * Connection now set through config.DATABASE_URL (see getting started docs)
+ * The deprecated category() method on StructuredNode has been removed
+ * The deprecated index property on StructuredNode has been removed
+ * The streaming=True flag is now irrelevant with bolt and produces a deprecation warning
+ * Batch operations must now be wrapped in a transaction in order to be atomic
+ * Indexing NodeSets returns a single node now as opposed to a list
+
+Contributing
+============
+
+Ideas, bugs, tests and pull requests always welcome. 
+
+As of release `3.3.2` we now have a curated list of issues / development targets for
+`neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
+
+If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
+it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
+contribute towards delivering any of the existing todo items too.
+
+Running the test suite
+----------------------
+
+Make sure you have a Neo4j database version 3 or higher to run the tests on.::
+
+    $ export NEO4J_BOLT_URL=bolt://neo4j:neo4j@localhost:7687 # (the default)
+
+Setup a virtual environment, install neomodel for development and run the test suite::
+
+    $ virtualenv venv
+    $ source venv/bin/activate
+    $ python setup.py develop
+    $ pytest
+
+If you are running a neo4j database for the first time the test suite will set the password to 'test'.
+If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
+`--resetdb` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if
+you happen to not have restarted your Neo4j server to point to a (usually named) `debug.db` database.
+
+If you have ``docker-compose`` installed, you can run the test suite against all supported Python
+interpreters and neo4j versions::
+
+    # in the project's root folder:
+    $ ./tests-with-docker-compose.sh
+
+
+.. image:: https://badges.gitter.im/Join%20Chat.svg
+   :alt: Join the chat at https://gitter.im/neo4j-contrib/neomodel
+   :target: https://gitter.im/neo4j-contrib/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
+
```

### Comparing `cythereal-neomodel-3.2.5/scripts/neomodel_remove_labels` & `cythereal-neomodel-3.3.2/scripts/neomodel_remove_labels`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/scripts/neomodel_install_labels` & `cythereal-neomodel-3.3.2/scripts/neomodel_install_labels`

 * *Files identical despite different names*

### Comparing `cythereal-neomodel-3.2.5/cythereal_neomodel.egg-info/PKG-INFO` & `cythereal-neomodel-3.3.2/cythereal_neomodel.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,132 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cythereal-neomodel
-Version: 3.2.5
+Version: 3.3.2
 Summary: An object mapper for the neo4j graph database.
-Home-page: http://github.com/robinedwards/neomodel
+Home-page: http://github.com/neo4j-contrib/neomodel
 Author: Robin Edwards
 Author-email: robin.ge@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: .. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
-           :alt: neomodel
-        
-        NOTE: This is a customized version of neomodel for personal use. Use the
-        `official version`_ instead.
-        
-        An Object Graph Mapper (OGM) for the neo4j_ graph database, built on the awesome neo4j_driver_
-        
-        - Familiar Django model style definitions.
-        - Powerful query API.
-        - Enforce your schema through cardinality restrictions.
-        - Full transaction support.
-        - Thread safe.
-        - pre/post save/delete hooks.
-        - Django integration via django_neomodel_
-        
-        .. _django_neomodel: https://github.com/robinedwards/django-neomodel
-        .. _neo4j: https://www.neo4j.org
-        .. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
-        .. _official version: https://github.com/neo4j-contrib/neomodel
-        
-        .. image:: https://secure.travis-ci.org/robinedwards/neomodel.png
-            :target: https://secure.travis-ci.org/robinedwards/neomodel/
-        
-        .. image:: https://readthedocs.org/projects/neomodel/badge/?version=latest
-            :alt: Documentation Status
-            :scale: 100%
-            :target: https://neomodel.readthedocs.io/en/latest/?badge=latest
-        
-        Documentation
-        =============
-        
-        Available on readthedocs_.
-        
-        .. _readthedocs: http://neomodel.readthedocs.org
-        
-        Requirements
-        ============
-        
-        - Python 2.7, 3.4+
-        - neo4j 3.0, 3.1, 3.2, 3.3
-        
-        Installation
-        ============
-        
-        Install from pypi (recommended)::
-        
-            $ pip install neomodel
-        
-        To install from github::
-        
-            $ pip install git+git://github.com/robinedwards/neomodel.git@HEAD#egg=neomodel-dev
-        
-        Upgrading 2.x to 3.x
-        ====================
-        
-         * Now utilises neo4j_driver as the backend which uses bolt so neo4j 3 is required
-         * Connection now set through config.DATABASE_URL (see getting started docs)
-         * The deprecated category() method on StructuredNode has been removed
-         * The deprecated index property on StructuredNode has been removed
-         * The streaming=True flag is now irrelevant with bolt and produces a deprecation warning
-         * Batch operations must now be wrapped in a transaction in order to be atomic
-         * Indexing NodeSets returns a single node now as opposed to a list
-        
-        Contributing
-        ============
-        
-        Ideas, bugs, tests and pull requests always welcome.
-        
-        Running the test suite
-        ----------------------
-        
-        Make sure you have a fresh virtualenv and `nose` installed::
-        
-            $ pip install nose
-        
-        Also a Neo4j database version 3 or higher to run the tests on. (it will wipe this database for each test run)::
-        
-            $ export NEO4J_BOLT_URL=bolt://neo4j:neo4j@localhost:7687 # (the default)
-        
-        Setup a virtual environment, install neomodel for development and run the test suite::
-        
-            $ virtualenv venv
-            $ source venv/bin/activate
-            $ python setup.py develop
-            $ nosetests -s
-        
-        If your running a neo4j database for the first time the test suite will set the password to 'test'.
-        
-        If you have ``docker-compose`` installed, you can run the test suite against all supported Python
-        interpreters and neo4j versions::
-        
-            # in the project's root folder:
-            $ ./tests-with-docker-compose.sh
-        
-        
-        .. image:: https://badges.gitter.im/Join%20Chat.svg
-           :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-           :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
 Keywords: graph neo4j ORM OGM
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
+License-File: LICENSE
+License-File: AUTHORS.txt
+
+.. image:: https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png
+   :alt: neomodel
+
+NOTE: This is a customized version of neomodel for personal use. Use the
+`official version`_ instead.
+
+An Object Graph Mapper (OGM) for the neo4j_ graph database, built on the awesome neo4j_driver_
+
+- Familiar Django model style definitions.
+- Powerful query API.
+- Enforce your schema through cardinality restrictions.
+- Full transaction support.
+- Thread safe.
+- pre/post save/delete hooks.
+- Django integration via django_neomodel_
+
+.. _django_neomodel: https://github.com/neo4j-contrib/django-neomodel
+.. _neo4j: https://neo4j.com/
+.. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
+.. _official version: https://github.com/neo4j-contrib/neomodel
+
+.. image:: https://secure.travis-ci.org/neo4j-contrib/neomodel.png
+    :target: https://secure.travis-ci.org/neo4j-contrib/neomodel/
+
+.. image:: https://readthedocs.org/projects/neomodel/badge/?version=latest
+    :alt: Documentation Status
+    :scale: 100%
+    :target: https://neomodel.readthedocs.io/en/latest/?badge=latest
+
+
+Documentation
+=============
+
+Available on readthedocs_.
+
+.. _readthedocs: http://neomodel.readthedocs.org
+
+Requirements
+============
+
+- Python 2.7 (Up to version 3.3.1), 3.4+
+- neo4j 3.0, 3.1, 3.2, 3.3
+
+Installation
+============
+
+Install from pypi (recommended)::
+
+    $ pip install neomodel
+
+To install from github::
+
+    $ pip install git+git://github.com/neo4j-contrib/neomodel.git@HEAD#egg=neomodel-dev
+
+Upgrading 2.x to 3.x
+====================
+
+ * Now utilises neo4j_driver as the backend which uses bolt so neo4j 3 is required
+ * Connection now set through config.DATABASE_URL (see getting started docs)
+ * The deprecated category() method on StructuredNode has been removed
+ * The deprecated index property on StructuredNode has been removed
+ * The streaming=True flag is now irrelevant with bolt and produces a deprecation warning
+ * Batch operations must now be wrapped in a transaction in order to be atomic
+ * Indexing NodeSets returns a single node now as opposed to a list
+
+Contributing
+============
+
+Ideas, bugs, tests and pull requests always welcome. 
+
+As of release `3.3.2` we now have a curated list of issues / development targets for
+`neomodel` available on `the Wiki <https://github.com/neo4j-contrib/neomodel/wiki/TODOs-&-Enhancements>`_.
+
+If you are interested in developing `neomodel` further, pick a subject from the list and open a Pull Request (PR) for 
+it. If you are adding a feature that is not captured in that list yet, consider if the work for it could also 
+contribute towards delivering any of the existing todo items too.
+
+Running the test suite
+----------------------
+
+Make sure you have a Neo4j database version 3 or higher to run the tests on.::
+
+    $ export NEO4J_BOLT_URL=bolt://neo4j:neo4j@localhost:7687 # (the default)
+
+Setup a virtual environment, install neomodel for development and run the test suite::
+
+    $ virtualenv venv
+    $ source venv/bin/activate
+    $ python setup.py develop
+    $ pytest
+
+If you are running a neo4j database for the first time the test suite will set the password to 'test'.
+If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
+`--resetdb` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if
+you happen to not have restarted your Neo4j server to point to a (usually named) `debug.db` database.
+
+If you have ``docker-compose`` installed, you can run the test suite against all supported Python
+interpreters and neo4j versions::
+
+    # in the project's root folder:
+    $ ./tests-with-docker-compose.sh
+
+
+.. image:: https://badges.gitter.im/Join%20Chat.svg
+   :alt: Join the chat at https://gitter.im/neo4j-contrib/neomodel
+   :target: https://gitter.im/neo4j-contrib/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
+
```

### Comparing `cythereal-neomodel-3.2.5/AUTHORS.txt` & `cythereal-neomodel-3.3.2/AUTHORS.txt`

 * *Files identical despite different names*

