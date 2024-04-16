# Comparing `tmp/scikit-base-0.7.5.tar.gz` & `tmp/scikit_base-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.7.5.tar", last modified: Sat Mar  2 12:08:47 2024, max compression
+gzip compressed data, was "scikit_base-0.7.6.tar", last modified: Tue Apr 16 15:35:17 2024, max compression
```

## Comparing `scikit-base-0.7.5.tar` & `scikit_base-0.7.6.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.864796 scikit-base-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-02 12:08:38.000000 scikit-base-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-02 12:08:47.864796 scikit-base-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-02 12:08:38.000000 scikit-base-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.848796 scikit-base-0.7.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-03-02 12:08:38.000000 scikit-base-0.7.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-02 12:08:38.000000 scikit-base-0.7.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.860795 scikit-base-0.7.5/scikit_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 12:08:47.000000 scikit-base-0.7.5/scikit_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-02 12:08:47.864796 scikit-base-0.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/skbase/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.852795 scikit-base-0.7.5/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38218 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/deep_equals/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/deep_equals/_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/utils/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/dependencies/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.856795 scikit-base-0.7.5/skbase/utils/dependencies/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/dependencies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/dependencies/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.860795 scikit-base-0.7.5/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.860795 scikit-base-0.7.5/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:08:47.860795 scikit-base-0.7.5/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-03-02 12:08:38.000000 scikit-base-0.7.5/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.785763 scikit_base-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-16 15:35:10.000000 scikit_base-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-16 15:35:17.785763 scikit_base-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-16 15:35:10.000000 scikit_base-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.769763 scikit_base-0.7.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.769763 scikit_base-0.7.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-16 15:35:10.000000 scikit_base-0.7.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-16 15:35:10.000000 scikit_base-0.7.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.781763 scikit_base-0.7.6/scikit_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-16 15:35:17.000000 scikit_base-0.7.6/scikit_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-16 15:35:17.000000 scikit_base-0.7.6/scikit_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:35:17.000000 scikit_base-0.7.6/scikit_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 15:35:17.000000 scikit_base-0.7.6/scikit_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 15:35:17.000000 scikit_base-0.7.6/scikit_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:35:14.000000 scikit_base-0.7.6/scikit_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 15:35:17.785763 scikit_base-0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_pretty_printing/_pprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/base/_pretty_printing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_pretty_printing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_pretty_printing/tests/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38218 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36167 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.773763 scikit_base-0.7.6/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/testing/utils/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/deep_equals/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/deep_equals/_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/utils/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/dependencies/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/utils/dependencies/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/dependencies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/dependencies/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.777763 scikit_base-0.7.6/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.781763 scikit_base-0.7.6/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:35:17.781763 scikit_base-0.7.6/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-16 15:35:10.000000 scikit_base-0.7.6/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.7.5/LICENSE` & `scikit_base-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/PKG-INFO` & `scikit_base-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.5
+Version: 0.7.6
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -110,15 +110,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.4 is now available. Check out our
+:rocket: Version 0.7.6 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit-base-0.7.5/README.md` & `scikit_base-0.7.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.4 is now available. Check out our
+:rocket: Version 0.7.6 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_b_a_s_e_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_b_a_s_e_-_l_o_g_o_-
 _w_i_t_h_-_n_a_m_e_._p_n_g_]# Welcome to skbase > A framework factory for scikit-learn-like
 and sktime-like parametric objects `skbase` provides base classes for creating
 scikit-learn-like parametric objects, along with tools to make it easier to
 build your own packages that follow these design patterns. :rocket: Version
-0.7.4 is now available. Check out our [release notes](https://
+0.7.6 is now available. Check out our [release notes](https://
 skbase.readthedocs.io/en/latest/changelog.html). | Overview | | |---|---| |
 **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/
 test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/
 workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/
 main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [!
 [Documentation Status](https://readthedocs.org/projects/skbase/badge/
 ?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [!
```

### Comparing `scikit-base-0.7.5/docs/source/conf.py` & `scikit_base-0.7.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/pyproject.toml` & `scikit_base-0.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
-version = "0.7.5"
+version = "0.7.6"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
 ]
 maintainers = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
```

### Comparing `scikit-base-0.7.5/scikit_base.egg-info/PKG-INFO` & `scikit_base-0.7.6/scikit_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.5
+Version: 0.7.6
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -110,15 +110,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.4 is now available. Check out our
+:rocket: Version 0.7.6 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit-base-0.7.5/scikit_base.egg-info/SOURCES.txt` & `scikit_base-0.7.6/scikit_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 skbase/base/__init__.py
 skbase/base/_base.py
 skbase/base/_meta.py
 skbase/base/_tagmanager.py
 skbase/base/_pretty_printing/__init__.py
 skbase/base/_pretty_printing/_object_html_repr.py
 skbase/base/_pretty_printing/_pprint.py
+skbase/base/_pretty_printing/tests/__init__.py
+skbase/base/_pretty_printing/tests/test_pprint.py
 skbase/lookup/__init__.py
 skbase/lookup/_lookup.py
 skbase/lookup/tests/__init__.py
 skbase/lookup/tests/test_lookup.py
 skbase/testing/__init__.py
 skbase/testing/test_all_objects.py
 skbase/testing/utils/__init__.py
 skbase/testing/utils/_conditional_fixtures.py
-skbase/testing/utils/inspect.py
+skbase/testing/utils/_inspect.py
 skbase/tests/__init__.py
 skbase/tests/conftest.py
 skbase/tests/test_base.py
 skbase/tests/test_baseestimator.py
 skbase/tests/test_exceptions.py
 skbase/tests/test_meta.py
 skbase/tests/mock_package/__init__.py
```

### Comparing `scikit-base-0.7.5/scikit_base.egg-info/requires.txt` & `scikit_base-0.7.6/scikit_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/_exceptions.py` & `scikit_base-0.7.6/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/_nopytest_tests.py` & `scikit_base-0.7.6/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/base/__init__.py` & `scikit_base-0.7.6/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/base/_base.py` & `scikit_base-0.7.6/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/base/_meta.py` & `scikit_base-0.7.6/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit_base-0.7.6/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,43 +18,45 @@
     """HTML Representation of BaseObject.
 
     Parameters
     ----------
     kind : {'serial', 'parallel', 'single'}
         kind of HTML block
 
-    objs : list of BaseObjects or `_VisualBlock`s or a single BaseObject
-        If kind != 'single', then `objs` is a list of
-        BaseObjects. If kind == 'single', then `objs` is a single BaseObject.
+    estimators : list of ``BaseObject``s or ``_VisualBlock`s or a single ``BaseObject``
+        If ``kind != 'single'``, then ``estimators`` is a list of ``BaseObjects``.
+        If ``kind == 'single'``, then ``estimators`` is a single ``BaseObject``.
 
     names : list of str, default=None
-        If kind != 'single', then `names` corresponds to BaseObjects.
-        If kind == 'single', then `names` is a single string corresponding to
-        the single BaseObject.
+        If ``kind != 'single'``, then ``names`` corresponds to ``BaseObjects``.
+        If ``kind == 'single'``, then ``names`` is a single string corresponding to
+        the single ``BaseObject``.
 
     name_details : list of str, str, or None, default=None
-        If kind != 'single', then `name_details` corresponds to `names`.
-        If kind == 'single', then `name_details` is a single string
-        corresponding to the single BaseObject.
+        If ``kind != 'single'``, then ``name_details`` corresponds to ``names``.
+        If ``kind == 'single'``, then ``name_details`` is a single string
+        corresponding to the single ``BaseObject``.
 
     dash_wrapped : bool, default=True
         If true, wrapped HTML element will be wrapped with a dashed border.
-        Only active when kind != 'single'.
+        Only active when ``kind != 'single'``.
     """
 
-    def __init__(self, kind, objs, *, names=None, name_details=None, dash_wrapped=True):
+    def __init__(
+        self, kind, estimators, *, names=None, name_details=None, dash_wrapped=True
+    ):
         self.kind = kind
-        self.objs = objs
+        self.estimators = estimators
         self.dash_wrapped = dash_wrapped
 
         if self.kind in ("parallel", "serial"):
             if names is None:
-                names = (None,) * len(objs)
+                names = (None,) * len(estimators)
             if name_details is None:
-                name_details = (None,) * len(objs)
+                name_details = (None,) * len(estimators)
 
         self.names = names
         self.name_details = name_details
 
     def _sk_visual_block_(self):
         return self
 
@@ -131,15 +133,15 @@
         out.write(f'<div class="sk-item{dash_cls}">')
 
         if base_object_label:
             _write_label_html(out, base_object_label, base_object_label_details)
 
         kind = est_block.kind
         out.write(f'<div class="sk-{kind}">')
-        est_infos = zip(est_block.objs, est_block.names, est_block.name_details)
+        est_infos = zip(est_block.estimators, est_block.names, est_block.name_details)
 
         for est, name, name_details in est_infos:
             if kind == "serial":
                 _write_base_object_html(out, est, name, name_details)
             else:  # parallel
                 out.write('<div class="sk-parallel-item">')
                 # wrap element in a serial visualblock
```

### Comparing `scikit-base-0.7.5/skbase/base/_pretty_printing/_pprint.py` & `scikit_base-0.7.6/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/base/_tagmanager.py` & `scikit_base-0.7.6/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/lookup/__init__.py` & `scikit_base-0.7.6/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/lookup/_lookup.py` & `scikit_base-0.7.6/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/lookup/tests/test_lookup.py` & `scikit_base-0.7.6/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/testing/test_all_objects.py` & `scikit_base-0.7.6/skbase/testing/test_all_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pytest
 
 from skbase.base import BaseObject
 from skbase.lookup import all_objects
 from skbase.testing.utils._conditional_fixtures import (
     create_conditional_fixtures_and_names,
 )
-from skbase.testing.utils.inspect import _get_args
+from skbase.testing.utils._inspect import _get_args
 from skbase.utils.deep_equals import deep_equals
 from skbase.utils.dependencies import _check_soft_dependencies
 
 __author__: List[str] = ["fkiraly"]
 
 
 class BaseFixtureGenerator:
```

### Comparing `scikit-base-0.7.5/skbase/testing/utils/_conditional_fixtures.py` & `scikit_base-0.7.6/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/testing/utils/inspect.py` & `scikit_base-0.7.6/skbase/testing/utils/_inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/tests/conftest.py` & `scikit_base-0.7.6/skbase/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "skbase.lookup.tests",
     "skbase.lookup.tests.test_lookup",
     "skbase.lookup._lookup",
     "skbase.testing",
     "skbase.testing.test_all_objects",
     "skbase.testing.utils",
     "skbase.testing.utils._conditional_fixtures",
-    "skbase.testing.utils.inspect",
+    "skbase.testing.utils._inspect",
     "skbase.testing.utils.tests",
     "skbase.testing.utils.tests.test_deep_equals",
     "skbase.tests",
     "skbase.tests.conftest",
     "skbase.tests.test_base",
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
@@ -63,15 +63,14 @@
     "skbase.base",
     "skbase.lookup",
     "skbase.lookup.tests",
     "skbase.lookup.tests.test_lookup",
     "skbase.testing",
     "skbase.testing.test_all_objects",
     "skbase.testing.utils",
-    "skbase.testing.utils.inspect",
     "skbase.testing.utils.tests",
     "skbase.testing.utils.tests.test_deep_equals",
     "skbase.tests",
     "skbase.tests.conftest",
     "skbase.tests.test_base",
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
@@ -200,15 +199,15 @@
             "_walk",
             "_filter_by_tags",
             "_filter_by_class",
             "_import_module",
             "_check_object_types",
             "_get_module_info",
         ),
-        "skbase.testing.utils.inspect": ("_get_args",),
+        "skbase.testing.utils._inspect": ("_get_args",),
         "skbase.utils._check": ("_is_scalar_nan",),
         "skbase.utils.dependencies": (
             "_check_soft_dependencies",
             "_check_python_version",
             "_check_estimator_deps",
         ),
         "skbase.utils._iter": (
```

### Comparing `scikit-base-0.7.5/skbase/tests/mock_package/test_mock_package.py` & `scikit_base-0.7.6/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/tests/test_base.py` & `scikit_base-0.7.6/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/tests/test_baseestimator.py` & `scikit_base-0.7.6/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/tests/test_exceptions.py` & `scikit_base-0.7.6/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/tests/test_meta.py` & `scikit_base-0.7.6/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/__init__.py` & `scikit_base-0.7.6/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/_check.py` & `scikit_base-0.7.6/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/_iter.py` & `scikit_base-0.7.6/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/_nested_iter.py` & `scikit_base-0.7.6/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/_utils.py` & `scikit_base-0.7.6/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/deep_equals/_common.py` & `scikit_base-0.7.6/skbase/utils/deep_equals/_common.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/deep_equals/_deep_equals.py` & `scikit_base-0.7.6/skbase/utils/deep_equals/_deep_equals.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,28 +118,39 @@
         x = [x]
     if isinstance(x, tuple):
         x = list(x)
 
     return x
 
 
-def _numpy_equals_plugin(x, y, return_msg=False):
+def _numpy_equals_plugin(x, y, return_msg=False, deep_equals=None):
     numpy_available = _softdep_available("numpy")
 
     if not numpy_available or not _is_npndarray(x):
         return None
     else:
         import numpy as np
 
     ret = _make_ret(return_msg)
 
+    if x.ndim != y.ndim:
+        return ret(False, f".ndim, x.ndim = {x.ndim} != y.ndim = {y.ndim}")
+    if x.shape != y.shape:
+        return ret(False, f".shape, x.shape = {x.shape} != y.shape = {y.shape}")
     if x.dtype != y.dtype:
         return ret(False, f".dtype, x.dtype = {x.dtype} != y.dtype = {y.dtype}")
-    if x.dtype in ["object", "str"]:
+    if x.dtype == "str":
         return ret(np.array_equal(x, y), ".values")
+    elif x.dtype == "object":
+        x_flat = x.flatten()
+        y_flat = y.flatten()
+        for i in range(len(x_flat)):
+            is_equal, msg = deep_equals(x_flat[i], y_flat[i], return_msg=True)
+            return ret(is_equal, f"[{i}]" + msg)
+        return ret(True, "")  # catches len(x_flat) == 0
     else:
         return ret(np.array_equal(x, y, equal_nan=True), ".values")
 
 
 def _pandas_equals_plugin(x, y, return_msg=False, deep_equals=None):
     pandas_available = _softdep_available("pandas")
```

### Comparing `scikit-base-0.7.5/skbase/utils/dependencies/_dependencies.py` & `scikit_base-0.7.6/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/dependencies/tests/test_check_dependencies.py` & `scikit_base-0.7.6/skbase/utils/dependencies/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/random_state.py` & `scikit_base-0.7.6/skbase/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_check.py` & `scikit_base-0.7.6/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_deep_equals.py` & `scikit_base-0.7.6/skbase/utils/tests/test_deep_equals.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,21 @@
         [np.array([2, 3, 4]), np.array([4, 3, 2])],
         # test case to cover branch re dtype and equal_nan
         np.array([0.1, 1], dtype="object"),
         np.array([0.2, 1], dtype="object"),
         np.array([0.2, 1, 4], dtype="object"),
     ]
 
+    # test cases with nested numpy arrays
+    a = np.array(["a", "b"], dtype="object")
+    a[0] = np.array([1, 2, 3])
+    b = np.array(["a", "b", 42], dtype="object")
+    b[1] = a
+    EXAMPLES += [a, b]
+
 if _check_soft_dependencies("pandas", severity="none"):
     import pandas as pd
 
     EXAMPLES += [
         pd.DataFrame({"a": [4, 2]}),
         pd.DataFrame({"a": [4, 3]}),
         pd.DataFrame({"a": [4, 3, 5]}),
@@ -76,15 +83,15 @@
 @pytest.mark.parametrize("fixture", EXAMPLES)
 def test_deep_equals_positive(fixture):
     """Tests that deep_equals correctly identifies equal objects as equal."""
     x = copy_except_if_sklearn(fixture)
     y = copy_except_if_sklearn(fixture)
 
     msg = (
-        f"deep_copy incorrectly returned False for two identical copies of "
+        f"deep_equals incorrectly returned False for two identical copies of "
         f"the following object: {x}"
     )
     assert deep_equals(x, y), msg
 
 
 n = len(EXAMPLES)
 DIFFERENT_PAIRS = [
@@ -95,15 +102,15 @@
 @pytest.mark.parametrize("fixture1,fixture2", DIFFERENT_PAIRS)
 def test_deep_equals_negative(fixture1, fixture2):
     """Tests that deep_equals correctly identifies unequal objects as unequal."""
     x = copy_except_if_sklearn(fixture1)
     y = copy_except_if_sklearn(fixture2)
 
     msg = (
-        f"deep_copy incorrectly returned True when comparing "
+        f"deep_equals incorrectly returned True when comparing "
         f"the following, different objects: x={x}, y={y}"
     )
     assert not deep_equals(x, y), msg
 
 
 def copy_except_if_sklearn(obj):
     """Copy obj if it is not a scikit-learn estimator.
```

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_iter.py` & `scikit_base-0.7.6/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_nested_iter.py` & `scikit_base-0.7.6/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_random_state.py` & `scikit_base-0.7.6/skbase/utils/tests/test_random_state.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/utils/tests/test_utils.py` & `scikit_base-0.7.6/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/validate/__init__.py` & `scikit_base-0.7.6/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/validate/_named_objects.py` & `scikit_base-0.7.6/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/validate/_types.py` & `scikit_base-0.7.6/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/validate/tests/test_iterable_named_objects.py` & `scikit_base-0.7.6/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.7.5/skbase/validate/tests/test_type_validations.py` & `scikit_base-0.7.6/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

