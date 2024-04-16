# Comparing `tmp/dsms_sdk-1.4.0rc0.tar.gz` & `tmp/dsms_sdk-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.4.0rc0.tar", last modified: Fri Apr 12 08:33:16 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc1.tar", last modified: Tue Apr 16 07:17:11 2024, max compression
```

## Comparing `dsms_sdk-1.4.0rc0.tar` & `dsms_sdk-1.4.0rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.895386 dsms_sdk-1.4.0rc0/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/user_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16663 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.445315 dsms_sdk-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-16 07:17:11.445315 dsms_sdk-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.433315 dsms_sdk-1.4.0rc1/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.437315 dsms_sdk-1.4.0rc1/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.437315 dsms_sdk-1.4.0rc1/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.437315 dsms_sdk-1.4.0rc1/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/properties/user_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.441315 dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.445315 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-16 07:17:11.000000 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 07:17:11.000000 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:17:11.000000 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-16 07:17:11.000000 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 07:17:11.000000 dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-16 07:17:11.445315 dsms_sdk-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:11.445315 dsms_sdk-1.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-16 07:17:07.000000 dsms_sdk-1.4.0rc1/tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc0/LICENSE` & `dsms_sdk-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/PKG-INFO` & `dsms_sdk-1.4.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc0
+Version: 1.4.0rc1
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc0/README.md` & `dsms_sdk-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc1/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc1/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/core/configuration.py` & `dsms_sdk-1.4.0rc1/dsms/core/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,41 @@
         ..., description="Url of the DSMS instance to connect."
     )
     request_timeout: int = Field(
         30,
         description="Timeout in seconds until the request to the DSMS is timed out.",
     )
 
+    ssl_verify: bool = Field(
+        True,
+        description="Whether the SSL of the DSMS shall be verified during connection.",
+    )
+
     username: Optional[SecretStr] = Field(
         None,
         description="User name for connecting to the DSMS instance",
     )
     password: Optional[SecretStr] = Field(
         None,
         description="Password for connecting to the DSMS instance",
     )
     token: Optional[SecretStr] = Field(
         None,
         description="JWT bearer token for connecting to the DSMS instance",
     )
-    ssl_verify: bool = Field(
+
+    ping_dsms: bool = Field(
+        True, description="Check whether the host is a DSMS instance or not."
+    )
+
+    individual_slugs: bool = Field(
         True,
-        description="Whether the SSL of the DSMS shall be verified during connection.",
+        description="""When set to `True`, the slugs of the KItems will receive the
+        first few characters of the KItem-id, when the slug is derived automatically
+        from the KItem-name.""",
     )
 
     encoding: str = Field(
         "utf-8",
         description="General encoding to be used for reading/writing serializations.",
     )
 
@@ -87,14 +99,15 @@
     @field_validator("token")
     def validate_auth(cls, val, info: ValidationInfo):
         """Validate the provided authentication/authorization secrets."""
         username = info.data.get("username")
         passwd = info.data.get("password")
         host_url = info.data.get("host_url")
         timeout = info.data.get("request_timeout")
+        verify = info.data.get("ssl_verify")
         if username and passwd and val:
             raise ValueError(
                 "Either `username` and `password` or `token` must be provided. Not both."
             )
         if username and not passwd:
             raise ValueError("`username` provided, but `password` not.")
         if not username and passwd:
@@ -107,14 +120,15 @@
         if not val and username and passwd:
             url = urllib.parse.urljoin(str(host_url), "api/users/token")
             authorization = f"Basic {username.get_secret_value()}:{passwd.get_secret_value()}"
             response = requests.get(
                 url,
                 headers={"Authorization": authorization},
                 timeout=timeout,
+                verify=verify,
             )
             if not response.ok:
                 raise RuntimeError(
                     f"Something went wrong fetching the access token: {response.text}"
                 )
             val = response.json().get("token")
         if isinstance(val, str):
```

### Comparing `dsms_sdk-1.4.0rc0/dsms/core/context.py` & `dsms_sdk-1.4.0rc1/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc1/dsms/core/dsms.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,19 +202,20 @@
 def verify_connection(dsms: DSMS) -> None:
     """Check if DSMS is valid."""
     if not isinstance(dsms, DSMS):
         raise TypeError(
             f"""The passed object for the dsms-connection
                 is not of type {DSMS}."""
         )
-    try:
-        response = _ping_dsms()
-        if not response.ok:
+    if dsms.config.ping_dsms:
+        try:
+            response = _ping_dsms()
+            if not response.ok:
+                raise ConnectionError(
+                    f"""Host with `{dsms.config.host_url}`
+                    gave a response with status code `{response.status_code}`"""
+                )
+        except Exception as excep:
             raise ConnectionError(
-                f"""Host with `{dsms.config.host_url}`
-                gave a response with status code `{response.status_code}`"""
-            )
-    except Exception as excep:
-        raise ConnectionError(
-            f"Invalid DSMS instance: `{dsms.config.host_url}`"
-        ) from excep
+                f"Invalid DSMS instance: `{dsms.config.host_url}`"
+            ) from excep
     return dsms
```

### Comparing `dsms_sdk-1.4.0rc0/dsms/core/utils.py` & `dsms_sdk-1.4.0rc1/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/kitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,26 +374,27 @@
 
         return value
 
     @field_validator("slug")
     @classmethod
     def validate_slug(cls, value: str, info: ValidationInfo) -> str:
         """Validate slug"""
+        from dsms import Context
+
         ktype_id = info.data["ktype_id"]
         name = info.data.get("name")
         kitem_id = info.data.get("id")
         if not value:
             value = _slugify(name)
-        slugified = _slugify(value)
-        if len(slugified) < 4:
-            raise ValueError("Slug length must have a minimum length of 4.")
-        if value != slugified:
-            raise ValueError(
-                f"`{value}` is not a valid slug. A valid variation would be `{slugified}`"
-            )
+            if Context.dsms.config.individual_slugs:
+                value += f"-{str(kitem_id).split('-', maxsplit=1)[0]}"
+            if len(value) < 4:
+                raise ValueError(
+                    "Slug length must have a minimum length of 4."
+                )
         if not _kitem_exists(kitem_id) and not _slug_is_available(
             ktype_id.value, value
         ):
             raise ValueError(f"Slug for `{value}` is already taken.")
         return value
 
     @field_validator("summary")
@@ -495,9 +496,9 @@
 
         return Context
 
     @property
     def url(cls) -> str:
         """URL of the KItem"""
         return urljoin(
-            cls.context.dsms.config.host_url, f"{cls.ktype_id}/{cls.slug}"
+            str(cls.context.dsms.config.host_url), f"{cls.ktype_id}/{cls.slug}"
         )
```

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/ktype.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/affiliations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/annotations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """App KProperty"""
 
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, List, Optional
 
 from pydantic import BaseModel, Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
 
 if TYPE_CHECKING:
     from typing import Callable
@@ -13,15 +13,15 @@
 class AdditionalProperties(BaseModel):
     """Additional properties of"""
 
     triggerUponUpload: bool = Field(
         False,
         description="Whether the app should be triggered when a file is uploaded",
     )
-    triggerUponUploadFileExtensions: Optional[list[str]] = Field(
+    triggerUponUploadFileExtensions: Optional[List[str]] = Field(
         None,
         description="File extensions for which the upload shall be triggered.",
     )
 
 
 class App(KPropertyItem):
     """App of a KItem."""
```

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/attachments.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/authors.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/contacts.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/numerical.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/custom_datatype/numerical.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/external_links.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/external_links.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/hdf5.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/linked_kitems.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/user_groups.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/properties/user_groups.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/base.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/queries/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/base.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/conversion.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/conversion.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/sparql.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/sparql.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/utils.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/semantics/units/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc1/dsms/knowledge/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         ) from excep
     return [KItem(**item) for item in dumped]
 
 
 def _slugify(input_string: str, replacement: str = ""):
     """Turn any arbitrary string into a slug."""
     slug = re.sub(
-        r"[^\w\s]", replacement, input_string
+        r"[^\w\s\-_]", replacement, input_string
     )  # Remove all non-word characters (everything except numbers and letters)
     slug = re.sub(r"\s+", "", slug)  # Replace all runs of whitespace
     slug = slug.lower()  # Convert the string to lowercase.
     return slug
 
 
 def _slug_is_available(ktype_id: Union[str, UUID], value: str) -> bool:
```

### Comparing `dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc0
+Version: 1.4.0rc1
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc1/dsms_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/setup.cfg` & `dsms_sdk-1.4.0rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.4.0rc0
+version = v1.4.0rc1
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `dsms_sdk-1.4.0rc0/tests/conftest.py` & `dsms_sdk-1.4.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/tests/test_kitem.py` & `dsms_sdk-1.4.0rc1/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc0/tests/test_utils.py` & `dsms_sdk-1.4.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

