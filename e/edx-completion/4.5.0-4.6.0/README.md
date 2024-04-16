# Comparing `tmp/edx-completion-4.5.0.tar.gz` & `tmp/edx_completion-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-completion-4.5.0.tar", last modified: Thu Mar 21 13:56:18 2024, max compression
+gzip compressed data, was "edx_completion-4.6.0.tar", last modified: Tue Apr 16 15:41:10 2024, max compression
```

## Comparing `edx-completion-4.5.0.tar` & `edx_completion-4.6.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.226426 edx-completion-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-03-21 13:56:14.000000 edx-completion-4.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-21 13:56:14.000000 edx-completion-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-21 13:56:14.000000 edx-completion-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-21 13:56:18.226426 edx-completion-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-21 13:56:14.000000 edx-completion-4.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/migrations/0002_auto_20180125_1510.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/migrations/0003_learning_context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.222427 edx-completion-4.5.0/completion/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/settings/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.226426 edx-completion-4.5.0/completion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-21 13:56:14.000000 edx-completion-4.5.0/completion/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.226426 edx-completion-4.5.0/edx_completion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 13:56:18.000000 edx-completion-4.5.0/edx_completion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:56:18.226426 edx-completion-4.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-21 13:56:14.000000 edx-completion-4.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-21 13:56:14.000000 edx-completion-4.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-21 13:56:14.000000 edx-completion-4.5.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-21 13:56:18.226426 edx-completion-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-21 13:56:14.000000 edx-completion-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 15:41:05.000000 edx_completion-4.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-16 15:41:05.000000 edx_completion-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 15:41:05.000000 edx_completion-4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-16 15:41:10.539149 edx_completion-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-16 15:41:05.000000 edx_completion-4.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.535149 edx_completion-4.6.0/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.535149 edx_completion-4.6.0/completion/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0002_auto_20180125_1510.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0003_learning_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/edx_completion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 15:41:10.543149 edx_completion-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-16 15:41:05.000000 edx_completion-4.6.0/setup.py
```

### Comparing `edx-completion-4.5.0/CHANGELOG.rst` & `edx_completion-4.6.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,211 +1,213 @@
 Change Log
-----------
+==========
 
 ..
    All enhancements and patches to completion will be documented
    in this file.  It adheres to the structure of http://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
-Unreleased
-~~~~~~~~~~
+[4.6.0] - 2024-4-16
+-------------------
+
+* Add support for Python 3.11 and 3.12
 
 [4.5.0] - 2024-3-19
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added ``clear_learning_context_completion`` to enable clearing a learner's
   completion for a course
 
 [4.4.1] - 2023-10-27
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Fix RemovedInDjango41Warning by removing `django_app_config`
 
 [4.4.0] - 2023-10-20
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added tracking logs for completion events
 
 [4.3.0]- 2023-07-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added support for Django 4.2
 
 [4.2.1]- 2023-04-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
 
 [4.0.2] - 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Future-proof usage of ``edx_toggles.toggles``
 
 
 [4.0.1] - 2021-01-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Replace reference to deprecated import path ``student.models``
   with ``common.djangoapps.student.models``.
 * Updated the build status badge in README.rst to point to travis-ci.com instead of travis-ci.org
 
 
 [4.0.0] - 2020-11-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove soon-to-be-deprecated WaffleSwitchNamespace class instances
 * BACKWARD INCOMPATIBLE: Removes ``waffle()``, which returned a (now deprecated) WaffleSwitchNamespace. This should only affect tests in edx-platform.
 * Requires edx-toggles>=1.2.0, which introduces a new API to waffle objects.
 * Refactors ``ENABLE_COMPLETION_TRACKING_SWITCH`` from a ``LegacyWaffleSwitch`` to the updated ``WaffleSwitch``.  We don't expect uses of this updated switch to require changes, unless there are surprise uses of deprecated methods from ``LegacyWaffleSwitch``.
 
 [3.2.5] - 2020-10-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix waffle switch override in tests by relying on newest edx_toggles API
 
 [3.2.4] - 2020-07-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix AttributeError raised by `vertical_is_complete`.
   * by ensuring `get_completable_children` doesn't return null
 
 [3.2.3] - 2020-07-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated the children lookup for `vertical_is_complete` to utilize the XBlockCompletion model. There are
   three completion modes to consider: EXCLUDED, AGGREGATOR, COMPLETABLE.
 
   * This method will now ignore any block with XBlockCompletion.EXCLUDED.
   * This method will now recurse down any child of a vertical if that child has XBlockCompletion.AGGREGATOR.
   * This method will consider all children blocks with XBlockCompletion.COMPLETABLE as candidates to
     determine if the vertical is complete.
 
 [3.2.2] - 2020-06-30
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Adding recursive lookup for children of a vertical to the `vertical_is_complete` method in services.py.
 
   * This was added because verticals containing children that had their own children were not being properly marked
     as complete. Since the vertical was only looking one layer deep, it was possible to have children lower in the tree
     incomplete, but the vertical would still be marked as complete. Now it looks at all leaves under the vertical.
 
 [3.1.1] - 2020-02-24
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove unnecessary constraint for edx-drf-extensions<3.0.0
 
 [3.1.0] - 2020-02-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Upgrades packages, drops support for Python 2.
 
 [3.0.1] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix the package long description to be valid rST, check this in CI.
 
 [3.0.0] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support tracking completion of XBlocks in any "learning context", such as in
   a content library, and not just in courses. To keep the code clean, this has
   been done as a **breaking change** to the python API. (The API has been
   simplified so that it's generally only necessary to pass in a block key /
   usage key rather than block key + course key.) The REST API is unchanged.
 
 [2.1.1] - 2019-10-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated credentials for PyPI deployment via token.
 
 [2.1.0] - 2019-10-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Switch blocks_to_mark_complete_on_view() to return a list of XBlocks instead of a set.  Many XBlocks aren't hashable;
   the old implementation allowed subtle bugs under Python 2.7 but triggers an immediate error under 3.5.
 
 [2.0.0] - 2019-04-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Unpin django-rest-framework requirements. This is a potentially **breaking change** if people were
   relying on this package to ensure the correct version of djangorestframework was being installed.
 * Remove the AUTHORS file and references to it.
 
 [1.0.2] - 2019-03-11
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 
 * Fix the 403 error occurring for completion-batch API for requests coming from the iOS devices
 
 [1.0.0] - 2018-10-16
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated edx-drf-extensions imports. Completion will no longer work with
   outdated versions of edx-drf-extensions.
 
 [0.1.14] - 2018-10-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added submit_completion and submit_group_completion methods on
   CompletionService.
 
 [0.1.7] - 2018-06-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added can_mark_block_complete_on_view() and blocks_to_mark_complete_on_view()
   methods on CompletionService and renamed get_completion_by_viewing_delay_ms()
   to get_complete_on_view_delay_ms().
 
 [0.1.6] - 2018-04-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove usage of deprecated CourseStructure api.
 
 [0.1.5] - 2018-04-03
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Delete enable_visual_progress methods and checks. Deprecate ENABLE_VISUAL_PROGRESS,
   ENABLE_COURSE_VISUAL_PROGRESS, and ENABLE_SITE_VISUAL_PROGRESS waffle flags
 
 [0.1.4] - 2018-03-28
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Site configurations must now explicitly disable visual progress for the
   enable_visual_progress() feature gating function to return False early.
 
 [0.1.3] - 2018-03-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added some documentation.
 
 [0.1.2] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix management of dependency versions
 
 [0.1.1] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes wildly inefficient raw query in BlockCompletion.latest_blocks_completed_all_courses()
 * Updates freezegun version, makes tests that use it somewhat faster.
 
 [0.1.0] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes https://openedx.atlassian.net/browse/EDUCATOR-2540
 
 [0.0.11] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "subsection-completion/{username}/{course_key}/{subsection_id}" API
   endpoint, to be used with the completion milestones experiment.
 
 [0.0.9] - 2018-02-27
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "utilities.py", which houses methods for working with BlockCompletion
   data.
 
 [0.0.8] - 2018-03-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add model method for superlative “last completed block” - for site awareness
   include every last completed block by course, for later sorting in business
   layer.
 
 [0.0.7] - 2018-02-15
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add settings and service method for determining completion-by-viewing delay.
 
 [0.0.6] - 2018-02-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add the additional completion logic into the service and models from edx-platform
 
 [0.0.2] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix up edx-lint requirements shenanigans.
 
 [0.0.1] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Initial release
```

### Comparing `edx-completion-4.5.0/LICENSE` & `edx_completion-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/PKG-INFO` & `edx_completion-4.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,350 +1,390 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.5.0
+Version: 4.6.0
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock>=1.2.2
 Requires-Dist: django-model-utils
 Requires-Dist: djangorestframework
 Requires-Dist: edx-drf-extensions>=1.11.0
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles>=1.2.0
 Requires-Dist: event-tracking
 Requires-Dist: pytz
+Requires-Dist: setuptools
 
 completion
-=============================
+##########
 
-|pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
-|license-badge|
+|pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
+|license-badge| |status-badge|
 
-A library for tracking completion of blocks by learners in edX courses.
+Purpose
+*******
 
-Overview
-________
+A library for tracking completion of blocks by learners in Open edX courses.
 
 This repository provides a Django model `BlockCompletion` that is intended to be plugged into ``edx-platform``.  It
 provides various handlers and services for the recording of completion data.  It also provides a DRF API for submitting
 completion data in batches.
 
 Enabling in the LMS
--------------------
-By default, the Open edX LMS does not use this library. To turn it on, go to http://localhost:18000/admin/waffle/switch/ (substitute your LMS URL for http://localhost:18000/), and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
+*******************
+
+By default, the Open edX LMS does not use this library. To turn it on, go to http://your.lms.site/admin/waffle/switch/, and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
 
 See `Completion Tool <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/completion.html>`_ in the Open edX documentation for details on what will happen once enabled.
 
-License
--------
+Getting Started with Development
+********************************
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
-Please see ``LICENSE.txt`` for details.
+To install the ``completion`` app, run these commands from the `completion` root directory:
 
-How To Contribute
------------------
+.. code:: bash
 
-Contributions are very welcome.
+    pip install -e
 
-Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
+To run the test suite:
 
-PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+.. code:: bash
 
-Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+    pip install tox
+    tox # to run only a single environment, do e.g. tox -e py38-django42-drflatest
 
-Reporting Security Issues
--------------------------
 
-Please do not report security issues in public. Please email security@openedx.org.
+To use a Django shell to test commands:
 
-Using with Docker Devstack
---------------------------
+.. code:: bash
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
+    make install
+    python manage.py migrate
+    python manage.py shell
+    >>> from completion.models import BlockCompletion
+    >>> <other commands...>
 
-Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
-directory and are on a command prompt inside the LMS container.
 
-#. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
-   directory in a way that is accessible to the lms container.
+Deploying
+*********
 
-#. From inside the lms, uninstall completion and reinstall your local copy. You can just copy the following line::
+Tagged versions of the completion library are released to pypi.org.
 
-    pip uninstall completion -y; pip install -e /edx/src/completion/
+To use the latest release in your project, add the following to your pip requirements file:
 
-#. Now, get your completion development environment set up::
+.. code:: bash
 
-    cd /edx/src/completion
-    virtualenv completion-env
-    source completion-env/bin/activate
-    make install
+    edx-completion
+
+Getting Help
+************
 
-#. Don't forget to enable the waffle switch as described above in "Enabling in the LMS"
+Documentation
+=============
 
-#. That's it!  In order to simulate a given tox environment ``(django18, django111, quality)``, run ``tox -e <env>`` for the env in question.  If you want to run ``pytest`` directly::
+Start by going through `the documentation`_ (generated from `/docs </docs/index.rst>`_).  If you need more help see below.
 
-    pytest completion/tests/test_models.py
+.. _the documentation: https://docs.openedx.org/projects/completion
 
-Getting Help
-------------
+License
+*******
+
+The code in this repository is licensed under version 3 of the AGPL unless
+otherwise noted.
 
-Have a question about this repository, or about Open edX in general?  Please
-refer to this `list of resources`_ if you need any assistance.
+Please see `LICENSE <LICENSE>`_ for details.
 
-.. _list of resources: https://open.edx.org/getting-help
+Contributing
+************
 
+Contributions are very welcome.
+Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
+
+This project is currently accepting all types of contributions, bug fixes,
+security fixes, maintenance work, or new features.  However, please make sure
+to have a discussion about your new feature idea with the maintainers prior to
+beginning development to maximize the chances of your change being accepted.
+You can start a conversation by creating a new issue on this repo summarizing
+your idea.
+
+The Open edX Code of Conduct
+****************************
+
+All community members are expected to follow the `Open edX Code of Conduct`_.
+
+.. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
+
+People
+******
+
+The assigned maintainers for this component and other project details may be
+found in `Backstage`_. Backstage pulls this data from the ``catalog-info.yaml``
+file in this repo.
+
+.. _Backstage: https://backstage.openedx.org/catalog/default/component/completion
+
+Reporting Security Issues
+*************************
+
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/completion/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions/workflows/ci.yml?branch=master
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
-    :target: http://completion.readthedocs.io/en/latest/
+    :target: https://docs.openedx.org/projects/completion
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
     :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
 
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Experimental-yellow
+.. |status-badge| image:: https://img.shields.io/badge/Status-Maintained-brightgreen
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
+
 
 Change Log
-----------
+==========
 
 ..
    All enhancements and patches to completion will be documented
    in this file.  It adheres to the structure of http://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
-Unreleased
-~~~~~~~~~~
+[4.6.0] - 2024-4-16
+-------------------
+
+* Add support for Python 3.11 and 3.12
 
 [4.5.0] - 2024-3-19
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added ``clear_learning_context_completion`` to enable clearing a learner's
   completion for a course
 
 [4.4.1] - 2023-10-27
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Fix RemovedInDjango41Warning by removing `django_app_config`
 
 [4.4.0] - 2023-10-20
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added tracking logs for completion events
 
 [4.3.0]- 2023-07-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added support for Django 4.2
 
 [4.2.1]- 2023-04-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
 
 [4.0.2] - 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Future-proof usage of ``edx_toggles.toggles``
 
 
 [4.0.1] - 2021-01-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Replace reference to deprecated import path ``student.models``
   with ``common.djangoapps.student.models``.
 * Updated the build status badge in README.rst to point to travis-ci.com instead of travis-ci.org
 
 
 [4.0.0] - 2020-11-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove soon-to-be-deprecated WaffleSwitchNamespace class instances
 * BACKWARD INCOMPATIBLE: Removes ``waffle()``, which returned a (now deprecated) WaffleSwitchNamespace. This should only affect tests in edx-platform.
 * Requires edx-toggles>=1.2.0, which introduces a new API to waffle objects.
 * Refactors ``ENABLE_COMPLETION_TRACKING_SWITCH`` from a ``LegacyWaffleSwitch`` to the updated ``WaffleSwitch``.  We don't expect uses of this updated switch to require changes, unless there are surprise uses of deprecated methods from ``LegacyWaffleSwitch``.
 
 [3.2.5] - 2020-10-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix waffle switch override in tests by relying on newest edx_toggles API
 
 [3.2.4] - 2020-07-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix AttributeError raised by `vertical_is_complete`.
   * by ensuring `get_completable_children` doesn't return null
 
 [3.2.3] - 2020-07-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated the children lookup for `vertical_is_complete` to utilize the XBlockCompletion model. There are
   three completion modes to consider: EXCLUDED, AGGREGATOR, COMPLETABLE.
 
   * This method will now ignore any block with XBlockCompletion.EXCLUDED.
   * This method will now recurse down any child of a vertical if that child has XBlockCompletion.AGGREGATOR.
   * This method will consider all children blocks with XBlockCompletion.COMPLETABLE as candidates to
     determine if the vertical is complete.
 
 [3.2.2] - 2020-06-30
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Adding recursive lookup for children of a vertical to the `vertical_is_complete` method in services.py.
 
   * This was added because verticals containing children that had their own children were not being properly marked
     as complete. Since the vertical was only looking one layer deep, it was possible to have children lower in the tree
     incomplete, but the vertical would still be marked as complete. Now it looks at all leaves under the vertical.
 
 [3.1.1] - 2020-02-24
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove unnecessary constraint for edx-drf-extensions<3.0.0
 
 [3.1.0] - 2020-02-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Upgrades packages, drops support for Python 2.
 
 [3.0.1] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix the package long description to be valid rST, check this in CI.
 
 [3.0.0] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support tracking completion of XBlocks in any "learning context", such as in
   a content library, and not just in courses. To keep the code clean, this has
   been done as a **breaking change** to the python API. (The API has been
   simplified so that it's generally only necessary to pass in a block key /
   usage key rather than block key + course key.) The REST API is unchanged.
 
 [2.1.1] - 2019-10-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated credentials for PyPI deployment via token.
 
 [2.1.0] - 2019-10-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Switch blocks_to_mark_complete_on_view() to return a list of XBlocks instead of a set.  Many XBlocks aren't hashable;
   the old implementation allowed subtle bugs under Python 2.7 but triggers an immediate error under 3.5.
 
 [2.0.0] - 2019-04-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Unpin django-rest-framework requirements. This is a potentially **breaking change** if people were
   relying on this package to ensure the correct version of djangorestframework was being installed.
 * Remove the AUTHORS file and references to it.
 
 [1.0.2] - 2019-03-11
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 
 * Fix the 403 error occurring for completion-batch API for requests coming from the iOS devices
 
 [1.0.0] - 2018-10-16
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated edx-drf-extensions imports. Completion will no longer work with
   outdated versions of edx-drf-extensions.
 
 [0.1.14] - 2018-10-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added submit_completion and submit_group_completion methods on
   CompletionService.
 
 [0.1.7] - 2018-06-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added can_mark_block_complete_on_view() and blocks_to_mark_complete_on_view()
   methods on CompletionService and renamed get_completion_by_viewing_delay_ms()
   to get_complete_on_view_delay_ms().
 
 [0.1.6] - 2018-04-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove usage of deprecated CourseStructure api.
 
 [0.1.5] - 2018-04-03
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Delete enable_visual_progress methods and checks. Deprecate ENABLE_VISUAL_PROGRESS,
   ENABLE_COURSE_VISUAL_PROGRESS, and ENABLE_SITE_VISUAL_PROGRESS waffle flags
 
 [0.1.4] - 2018-03-28
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Site configurations must now explicitly disable visual progress for the
   enable_visual_progress() feature gating function to return False early.
 
 [0.1.3] - 2018-03-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added some documentation.
 
 [0.1.2] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix management of dependency versions
 
 [0.1.1] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes wildly inefficient raw query in BlockCompletion.latest_blocks_completed_all_courses()
 * Updates freezegun version, makes tests that use it somewhat faster.
 
 [0.1.0] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes https://openedx.atlassian.net/browse/EDUCATOR-2540
 
 [0.0.11] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "subsection-completion/{username}/{course_key}/{subsection_id}" API
   endpoint, to be used with the completion milestones experiment.
 
 [0.0.9] - 2018-02-27
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "utilities.py", which houses methods for working with BlockCompletion
   data.
 
 [0.0.8] - 2018-03-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add model method for superlative “last completed block” - for site awareness
   include every last completed block by course, for later sorting in business
   layer.
 
 [0.0.7] - 2018-02-15
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add settings and service method for determining completion-by-viewing delay.
 
 [0.0.6] - 2018-02-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add the additional completion logic into the service and models from edx-platform
 
 [0.0.2] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix up edx-lint requirements shenanigans.
 
 [0.0.1] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Initial release
```

### Comparing `edx-completion-4.5.0/README.rst` & `edx_completion-4.6.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,144 @@
 completion
-=============================
+##########
 
-|pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
-|license-badge|
+|pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
+|license-badge| |status-badge|
 
-A library for tracking completion of blocks by learners in edX courses.
+Purpose
+*******
 
-Overview
-________
+A library for tracking completion of blocks by learners in Open edX courses.
 
 This repository provides a Django model `BlockCompletion` that is intended to be plugged into ``edx-platform``.  It
 provides various handlers and services for the recording of completion data.  It also provides a DRF API for submitting
 completion data in batches.
 
 Enabling in the LMS
--------------------
-By default, the Open edX LMS does not use this library. To turn it on, go to http://localhost:18000/admin/waffle/switch/ (substitute your LMS URL for http://localhost:18000/), and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
+*******************
+
+By default, the Open edX LMS does not use this library. To turn it on, go to http://your.lms.site/admin/waffle/switch/, and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
 
 See `Completion Tool <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/completion.html>`_ in the Open edX documentation for details on what will happen once enabled.
 
-License
--------
+Getting Started with Development
+********************************
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
-Please see ``LICENSE.txt`` for details.
+To install the ``completion`` app, run these commands from the `completion` root directory:
 
-How To Contribute
------------------
+.. code:: bash
 
-Contributions are very welcome.
+    pip install -e
 
-Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
+To run the test suite:
 
-PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+.. code:: bash
 
-Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+    pip install tox
+    tox # to run only a single environment, do e.g. tox -e py38-django42-drflatest
 
-Reporting Security Issues
--------------------------
 
-Please do not report security issues in public. Please email security@openedx.org.
+To use a Django shell to test commands:
+
+.. code:: bash
 
-Using with Docker Devstack
---------------------------
+    make install
+    python manage.py migrate
+    python manage.py shell
+    >>> from completion.models import BlockCompletion
+    >>> <other commands...>
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
 
-Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
-directory and are on a command prompt inside the LMS container.
+Deploying
+*********
 
-#. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
-   directory in a way that is accessible to the lms container.
+Tagged versions of the completion library are released to pypi.org.
 
-#. From inside the lms, uninstall completion and reinstall your local copy. You can just copy the following line::
+To use the latest release in your project, add the following to your pip requirements file:
 
-    pip uninstall completion -y; pip install -e /edx/src/completion/
+.. code:: bash
 
-#. Now, get your completion development environment set up::
+    edx-completion
 
-    cd /edx/src/completion
-    virtualenv completion-env
-    source completion-env/bin/activate
-    make install
+Getting Help
+************
 
-#. Don't forget to enable the waffle switch as described above in "Enabling in the LMS"
+Documentation
+=============
 
-#. That's it!  In order to simulate a given tox environment ``(django18, django111, quality)``, run ``tox -e <env>`` for the env in question.  If you want to run ``pytest`` directly::
+Start by going through `the documentation`_ (generated from `/docs </docs/index.rst>`_).  If you need more help see below.
 
-    pytest completion/tests/test_models.py
+.. _the documentation: https://docs.openedx.org/projects/completion
 
-Getting Help
-------------
+License
+*******
 
-Have a question about this repository, or about Open edX in general?  Please
-refer to this `list of resources`_ if you need any assistance.
+The code in this repository is licensed under version 3 of the AGPL unless
+otherwise noted.
 
-.. _list of resources: https://open.edx.org/getting-help
+Please see `LICENSE <LICENSE>`_ for details.
 
+Contributing
+************
+
+Contributions are very welcome.
+Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
+
+This project is currently accepting all types of contributions, bug fixes,
+security fixes, maintenance work, or new features.  However, please make sure
+to have a discussion about your new feature idea with the maintainers prior to
+beginning development to maximize the chances of your change being accepted.
+You can start a conversation by creating a new issue on this repo summarizing
+your idea.
+
+The Open edX Code of Conduct
+****************************
+
+All community members are expected to follow the `Open edX Code of Conduct`_.
+
+.. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
+
+People
+******
+
+The assigned maintainers for this component and other project details may be
+found in `Backstage`_. Backstage pulls this data from the ``catalog-info.yaml``
+file in this repo.
+
+.. _Backstage: https://backstage.openedx.org/catalog/default/component/completion
+
+Reporting Security Issues
+*************************
+
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/completion/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions/workflows/ci.yml?branch=master
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
-    :target: http://completion.readthedocs.io/en/latest/
+    :target: https://docs.openedx.org/projects/completion
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
     :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
+
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Experimental-yellow
+.. |status-badge| image:: https://img.shields.io/badge/Status-Maintained-brightgreen
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
```

### Comparing `edx-completion-4.5.0/completion/api/permissions.py` & `edx_completion-4.6.0/completion/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/api/tests/test_permissions.py` & `edx_completion-4.6.0/completion/api/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/api/v1/urls.py` & `edx_completion-4.6.0/completion/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/api/v1/views.py` & `edx_completion-4.6.0/completion/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/apps.py` & `edx_completion-4.6.0/completion/apps.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/handlers.py` & `edx_completion-4.6.0/completion/handlers.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/migrations/0001_initial.py` & `edx_completion-4.6.0/completion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/migrations/0003_learning_context.py` & `edx_completion-4.6.0/completion/migrations/0003_learning_context.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/models.py` & `edx_completion-4.6.0/completion/models.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/services.py` & `edx_completion-4.6.0/completion/services.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/settings/common.py` & `edx_completion-4.6.0/completion/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/test_utils.py` & `edx_completion-4.6.0/completion/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/tests/test_models.py` & `edx_completion-4.6.0/completion/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         self._create_test_completions(self.other_user)
 
     def _create_test_completions(self, user):
         # Create random completions for `user` for all blocks in both test contexts
         models.BlockCompletion.objects.submit_batch_completion(
             user,
             [
-                (block, float(f"0.{randint(1,9)}"))
+                (block, float(f"0.{randint(1, 9)}"))
                 for block in self.blocks + self.other_blocks
             ]
         )
 
     def _set_up_course(self, course):
         """ Create a context with some blocks """
         blocks = [
```

### Comparing `edx-completion-4.5.0/completion/tests/test_services.py` & `edx_completion-4.6.0/completion/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/tests/test_utilities.py` & `edx_completion-4.6.0/completion/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/utilities.py` & `edx_completion-4.6.0/completion/utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/completion/waffle.py` & `edx_completion-4.6.0/completion/waffle.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/edx_completion.egg-info/PKG-INFO` & `edx_completion-4.6.0/edx_completion.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,350 +1,390 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.5.0
+Version: 4.6.0
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock>=1.2.2
 Requires-Dist: django-model-utils
 Requires-Dist: djangorestframework
 Requires-Dist: edx-drf-extensions>=1.11.0
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles>=1.2.0
 Requires-Dist: event-tracking
 Requires-Dist: pytz
+Requires-Dist: setuptools
 
 completion
-=============================
+##########
 
-|pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
-|license-badge|
+|pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
+|license-badge| |status-badge|
 
-A library for tracking completion of blocks by learners in edX courses.
+Purpose
+*******
 
-Overview
-________
+A library for tracking completion of blocks by learners in Open edX courses.
 
 This repository provides a Django model `BlockCompletion` that is intended to be plugged into ``edx-platform``.  It
 provides various handlers and services for the recording of completion data.  It also provides a DRF API for submitting
 completion data in batches.
 
 Enabling in the LMS
--------------------
-By default, the Open edX LMS does not use this library. To turn it on, go to http://localhost:18000/admin/waffle/switch/ (substitute your LMS URL for http://localhost:18000/), and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
+*******************
+
+By default, the Open edX LMS does not use this library. To turn it on, go to http://your.lms.site/admin/waffle/switch/, and add a new switch with Name ``completion.enable_completion_tracking`` and Active selected.
 
 See `Completion Tool <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/completion.html>`_ in the Open edX documentation for details on what will happen once enabled.
 
-License
--------
+Getting Started with Development
+********************************
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
-Please see ``LICENSE.txt`` for details.
+To install the ``completion`` app, run these commands from the `completion` root directory:
 
-How To Contribute
------------------
+.. code:: bash
 
-Contributions are very welcome.
+    pip install -e
 
-Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
+To run the test suite:
 
-PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+.. code:: bash
 
-Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+    pip install tox
+    tox # to run only a single environment, do e.g. tox -e py38-django42-drflatest
 
-Reporting Security Issues
--------------------------
 
-Please do not report security issues in public. Please email security@openedx.org.
+To use a Django shell to test commands:
 
-Using with Docker Devstack
---------------------------
+.. code:: bash
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
+    make install
+    python manage.py migrate
+    python manage.py shell
+    >>> from completion.models import BlockCompletion
+    >>> <other commands...>
 
-Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
-directory and are on a command prompt inside the LMS container.
 
-#. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
-   directory in a way that is accessible to the lms container.
+Deploying
+*********
 
-#. From inside the lms, uninstall completion and reinstall your local copy. You can just copy the following line::
+Tagged versions of the completion library are released to pypi.org.
 
-    pip uninstall completion -y; pip install -e /edx/src/completion/
+To use the latest release in your project, add the following to your pip requirements file:
 
-#. Now, get your completion development environment set up::
+.. code:: bash
 
-    cd /edx/src/completion
-    virtualenv completion-env
-    source completion-env/bin/activate
-    make install
+    edx-completion
+
+Getting Help
+************
 
-#. Don't forget to enable the waffle switch as described above in "Enabling in the LMS"
+Documentation
+=============
 
-#. That's it!  In order to simulate a given tox environment ``(django18, django111, quality)``, run ``tox -e <env>`` for the env in question.  If you want to run ``pytest`` directly::
+Start by going through `the documentation`_ (generated from `/docs </docs/index.rst>`_).  If you need more help see below.
 
-    pytest completion/tests/test_models.py
+.. _the documentation: https://docs.openedx.org/projects/completion
 
-Getting Help
-------------
+License
+*******
+
+The code in this repository is licensed under version 3 of the AGPL unless
+otherwise noted.
 
-Have a question about this repository, or about Open edX in general?  Please
-refer to this `list of resources`_ if you need any assistance.
+Please see `LICENSE <LICENSE>`_ for details.
 
-.. _list of resources: https://open.edx.org/getting-help
+Contributing
+************
 
+Contributions are very welcome.
+Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
+
+This project is currently accepting all types of contributions, bug fixes,
+security fixes, maintenance work, or new features.  However, please make sure
+to have a discussion about your new feature idea with the maintainers prior to
+beginning development to maximize the chances of your change being accepted.
+You can start a conversation by creating a new issue on this repo summarizing
+your idea.
+
+The Open edX Code of Conduct
+****************************
+
+All community members are expected to follow the `Open edX Code of Conduct`_.
+
+.. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
+
+People
+******
+
+The assigned maintainers for this component and other project details may be
+found in `Backstage`_. Backstage pulls this data from the ``catalog-info.yaml``
+file in this repo.
+
+.. _Backstage: https://backstage.openedx.org/catalog/default/component/completion
+
+Reporting Security Issues
+*************************
+
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/completion/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions/workflows/ci.yml?branch=master
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
-    :target: http://completion.readthedocs.io/en/latest/
+    :target: https://docs.openedx.org/projects/completion
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
     :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
 
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Experimental-yellow
+.. |status-badge| image:: https://img.shields.io/badge/Status-Maintained-brightgreen
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
+.. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
+
 
 Change Log
-----------
+==========
 
 ..
    All enhancements and patches to completion will be documented
    in this file.  It adheres to the structure of http://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
-Unreleased
-~~~~~~~~~~
+[4.6.0] - 2024-4-16
+-------------------
+
+* Add support for Python 3.11 and 3.12
 
 [4.5.0] - 2024-3-19
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added ``clear_learning_context_completion`` to enable clearing a learner's
   completion for a course
 
 [4.4.1] - 2023-10-27
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Fix RemovedInDjango41Warning by removing `django_app_config`
 
 [4.4.0] - 2023-10-20
-~~~~~~~~~~~~~~~~~~~~
+--------------------
 * Added tracking logs for completion events
 
 [4.3.0]- 2023-07-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added support for Django 4.2
 
 [4.2.1]- 2023-04-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
 
 [4.0.2] - 2021-02-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Future-proof usage of ``edx_toggles.toggles``
 
 
 [4.0.1] - 2021-01-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Replace reference to deprecated import path ``student.models``
   with ``common.djangoapps.student.models``.
 * Updated the build status badge in README.rst to point to travis-ci.com instead of travis-ci.org
 
 
 [4.0.0] - 2020-11-05
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove soon-to-be-deprecated WaffleSwitchNamespace class instances
 * BACKWARD INCOMPATIBLE: Removes ``waffle()``, which returned a (now deprecated) WaffleSwitchNamespace. This should only affect tests in edx-platform.
 * Requires edx-toggles>=1.2.0, which introduces a new API to waffle objects.
 * Refactors ``ENABLE_COMPLETION_TRACKING_SWITCH`` from a ``LegacyWaffleSwitch`` to the updated ``WaffleSwitch``.  We don't expect uses of this updated switch to require changes, unless there are surprise uses of deprecated methods from ``LegacyWaffleSwitch``.
 
 [3.2.5] - 2020-10-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix waffle switch override in tests by relying on newest edx_toggles API
 
 [3.2.4] - 2020-07-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix AttributeError raised by `vertical_is_complete`.
   * by ensuring `get_completable_children` doesn't return null
 
 [3.2.3] - 2020-07-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated the children lookup for `vertical_is_complete` to utilize the XBlockCompletion model. There are
   three completion modes to consider: EXCLUDED, AGGREGATOR, COMPLETABLE.
 
   * This method will now ignore any block with XBlockCompletion.EXCLUDED.
   * This method will now recurse down any child of a vertical if that child has XBlockCompletion.AGGREGATOR.
   * This method will consider all children blocks with XBlockCompletion.COMPLETABLE as candidates to
     determine if the vertical is complete.
 
 [3.2.2] - 2020-06-30
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Adding recursive lookup for children of a vertical to the `vertical_is_complete` method in services.py.
 
   * This was added because verticals containing children that had their own children were not being properly marked
     as complete. Since the vertical was only looking one layer deep, it was possible to have children lower in the tree
     incomplete, but the vertical would still be marked as complete. Now it looks at all leaves under the vertical.
 
 [3.1.1] - 2020-02-24
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove unnecessary constraint for edx-drf-extensions<3.0.0
 
 [3.1.0] - 2020-02-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Upgrades packages, drops support for Python 2.
 
 [3.0.1] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix the package long description to be valid rST, check this in CI.
 
 [3.0.0] - 2019-10-22
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Support tracking completion of XBlocks in any "learning context", such as in
   a content library, and not just in courses. To keep the code clean, this has
   been done as a **breaking change** to the python API. (The API has been
   simplified so that it's generally only necessary to pass in a block key /
   usage key rather than block key + course key.) The REST API is unchanged.
 
 [2.1.1] - 2019-10-21
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated credentials for PyPI deployment via token.
 
 [2.1.0] - 2019-10-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Switch blocks_to_mark_complete_on_view() to return a list of XBlocks instead of a set.  Many XBlocks aren't hashable;
   the old implementation allowed subtle bugs under Python 2.7 but triggers an immediate error under 3.5.
 
 [2.0.0] - 2019-04-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Unpin django-rest-framework requirements. This is a potentially **breaking change** if people were
   relying on this package to ensure the correct version of djangorestframework was being installed.
 * Remove the AUTHORS file and references to it.
 
 [1.0.2] - 2019-03-11
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 
 * Fix the 403 error occurring for completion-batch API for requests coming from the iOS devices
 
 [1.0.0] - 2018-10-16
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Updated edx-drf-extensions imports. Completion will no longer work with
   outdated versions of edx-drf-extensions.
 
 [0.1.14] - 2018-10-04
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added submit_completion and submit_group_completion methods on
   CompletionService.
 
 [0.1.7] - 2018-06-18
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added can_mark_block_complete_on_view() and blocks_to_mark_complete_on_view()
   methods on CompletionService and renamed get_completion_by_viewing_delay_ms()
   to get_complete_on_view_delay_ms().
 
 [0.1.6] - 2018-04-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Remove usage of deprecated CourseStructure api.
 
 [0.1.5] - 2018-04-03
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Delete enable_visual_progress methods and checks. Deprecate ENABLE_VISUAL_PROGRESS,
   ENABLE_COURSE_VISUAL_PROGRESS, and ENABLE_SITE_VISUAL_PROGRESS waffle flags
 
 [0.1.4] - 2018-03-28
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Site configurations must now explicitly disable visual progress for the
   enable_visual_progress() feature gating function to return False early.
 
 [0.1.3] - 2018-03-26
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added some documentation.
 
 [0.1.2] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix management of dependency versions
 
 [0.1.1] - 2018-03-23
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes wildly inefficient raw query in BlockCompletion.latest_blocks_completed_all_courses()
 * Updates freezegun version, makes tests that use it somewhat faster.
 
 [0.1.0] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fixes https://openedx.atlassian.net/browse/EDUCATOR-2540
 
 [0.0.11] - 2018-03-20
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "subsection-completion/{username}/{course_key}/{subsection_id}" API
   endpoint, to be used with the completion milestones experiment.
 
 [0.0.9] - 2018-02-27
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Added "utilities.py", which houses methods for working with BlockCompletion
   data.
 
 [0.0.8] - 2018-03-01
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add model method for superlative “last completed block” - for site awareness
   include every last completed block by course, for later sorting in business
   layer.
 
 [0.0.7] - 2018-02-15
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add settings and service method for determining completion-by-viewing delay.
 
 [0.0.6] - 2018-02-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Add the additional completion logic into the service and models from edx-platform
 
 [0.0.2] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Fix up edx-lint requirements shenanigans.
 
 [0.0.1] - 2018-01-31
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------
 * Initial release
```

### Comparing `edx-completion-4.5.0/edx_completion.egg-info/SOURCES.txt` & `edx_completion-4.6.0/edx_completion.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 completion/__init__.py
 completion/apps.py
 completion/exceptions.py
 completion/handlers.py
 completion/models.py
 completion/services.py
 completion/test_utils.py
+completion/urls.py
 completion/utilities.py
 completion/waffle.py
 completion/api/__init__.py
 completion/api/permissions.py
 completion/api/urls.py
 completion/api/tests/__init__.py
 completion/api/tests/test_permissions.py
```

### Comparing `edx-completion-4.5.0/requirements/test.in` & `edx_completion-4.6.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-completion-4.5.0/setup.py` & `edx_completion-4.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,17 @@
     tests_require=load_requirements('requirements/test.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

