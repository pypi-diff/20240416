# Comparing `tmp/darker-2.1.0.tar.gz` & `tmp/darker-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darker-2.1.0.tar", last modified: Wed Mar 27 21:12:57 2024, max compression
+gzip compressed data, was "darker-2.1.1.tar", last modified: Tue Apr 16 12:19:20 2024, max compression
```

## Comparing `darker-2.1.0.tar` & `darker-2.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 21:12:57.651857 darker-2.1.0/
--rw-r--r--   0 akaihola  (1000) users      (100)     1556 2023-08-05 18:33:16.000000 darker-2.1.0/LICENSE.rst
--rw-r--r--   0 akaihola  (1000) users      (100)    40946 2024-03-27 21:12:57.651857 darker-2.1.0/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)    85781 2024-03-27 21:12:49.000000 darker-2.1.0/README.rst
--rw-r--r--   0 akaihola  (1000) users      (100)     2035 2024-03-17 20:17:29.000000 darker-2.1.0/pyproject.toml
--rw-r--r--   0 akaihola  (1000) users      (100)     2290 2024-03-27 21:12:57.651857 darker-2.1.0/setup.cfg
--rw-r--r--   0 akaihola  (1000) users      (100)     1792 2023-08-05 18:33:16.000000 darker-2.1.0/setup.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 21:12:57.644857 darker-2.1.0/src/
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 21:12:57.646856 darker-2.1.0/src/darker/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)    25870 2024-03-16 14:38:51.000000 darker-2.1.0/src/darker/__main__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     8337 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/black_diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2960 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/chooser.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3464 2024-03-27 20:49:22.000000 darker-2.1.0/src/darker/command_line.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2368 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/concurrency.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3055 2024-03-27 20:49:22.000000 darker-2.1.0/src/darker/config.py
--rw-r--r--   0 akaihola  (1000) users      (100)     6411 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)      436 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/exceptions.py
--rw-r--r--   0 akaihola  (1000) users      (100)      980 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/files.py
--rw-r--r--   0 akaihola  (1000) users      (100)     4878 2024-03-16 14:38:51.000000 darker-2.1.0/src/darker/fstring.py
--rw-r--r--   0 akaihola  (1000) users      (100)    11741 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/git.py
--rw-r--r--   0 akaihola  (1000) users      (100)     5104 2024-03-19 17:46:15.000000 darker-2.1.0/src/darker/help.py
--rw-r--r--   0 akaihola  (1000) users      (100)     6241 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/import_sorting.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2584 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/multiline_strings.py
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/py.typed
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 21:12:57.648856 darker-2.1.0/src/darker/tests/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/tests/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1044 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/tests/git_diff_example_output.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1693 2024-03-16 14:38:51.000000 darker-2.1.0/src/darker/tests/helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)    14874 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_black_diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1105 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/tests/test_chooser.py
--rw-r--r--   0 akaihola  (1000) users      (100)    21642 2024-03-27 20:49:22.000000 darker-2.1.0/src/darker/tests/test_command_line.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1479 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/tests/test_concurrency.py
--rw-r--r--   0 akaihola  (1000) users      (100)     4785 2024-03-20 19:28:01.000000 darker-2.1.0/src/darker/tests/test_config.py
--rw-r--r--   0 akaihola  (1000) users      (100)     6025 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1625 2023-08-05 18:33:16.000000 darker-2.1.0/src/darker/tests/test_difflib.py
--rw-r--r--   0 akaihola  (1000) users      (100)      710 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_files.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1799 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_fstring.py
--rw-r--r--   0 akaihola  (1000) users      (100)    14448 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_git.py
--rw-r--r--   0 akaihola  (1000) users      (100)     9050 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_import_sorting.py
--rw-r--r--   0 akaihola  (1000) users      (100)    31139 2024-03-16 12:07:32.000000 darker-2.1.0/src/darker/tests/test_main.py
--rw-r--r--   0 akaihola  (1000) users      (100)     5779 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_main_blacken_and_flynt_single_file.py
--rw-r--r--   0 akaihola  (1000) users      (100)     5023 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_main_revision.py
--rw-r--r--   0 akaihola  (1000) users      (100)     5420 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_main_stdin_filename.py
--rw-r--r--   0 akaihola  (1000) users      (100)     5311 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_multiline_strings.py
--rw-r--r--   0 akaihola  (1000) users      (100)      712 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_utils.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2226 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/tests/test_verification.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1204 2024-03-11 21:00:09.000000 darker-2.1.0/src/darker/utils.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3467 2024-03-16 14:38:59.000000 darker-2.1.0/src/darker/verification.py
--rw-r--r--   0 akaihola  (1000) users      (100)       84 2024-03-27 21:12:49.000000 darker-2.1.0/src/darker/version.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 21:12:57.648856 darker-2.1.0/src/darker.egg-info/
--rw-r--r--   0 akaihola  (1000) users      (100)    40946 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)     1461 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/SOURCES.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/dependency_links.txt
--rw-r--r--   0 akaihola  (1000) users      (100)       68 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/entry_points.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      601 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/requires.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        7 2024-03-27 21:12:57.000000 darker-2.1.0/src/darker.egg-info/top_level.txt
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-16 12:19:20.496892 darker-2.1.1/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1556 2023-08-05 18:33:16.000000 darker-2.1.1/LICENSE.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)    41421 2024-04-16 12:19:20.496892 darker-2.1.1/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)    87421 2024-04-16 12:18:59.000000 darker-2.1.1/README.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)     2138 2024-04-15 17:18:11.000000 darker-2.1.1/pyproject.toml
+-rw-r--r--   0 akaihola  (1000) users      (100)     2227 2024-04-16 12:19:20.497892 darker-2.1.1/setup.cfg
+-rw-r--r--   0 akaihola  (1000) users      (100)     1792 2023-08-05 18:33:16.000000 darker-2.1.1/setup.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-16 12:19:20.490891 darker-2.1.1/src/
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-16 12:19:20.492891 darker-2.1.1/src/darker/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2023-08-05 18:33:16.000000 darker-2.1.1/src/darker/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    26213 2024-04-16 06:33:51.000000 darker-2.1.1/src/darker/__main__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     8337 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/black_diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2960 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/chooser.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3992 2024-04-15 17:18:11.000000 darker-2.1.1/src/darker/command_line.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2368 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/concurrency.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3160 2024-04-15 17:18:11.000000 darker-2.1.1/src/darker/config.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     6411 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      436 2023-08-05 18:33:16.000000 darker-2.1.1/src/darker/exceptions.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      980 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/files.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     4878 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/fstring.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    12849 2024-04-16 06:33:51.000000 darker-2.1.1/src/darker/git.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     5116 2024-04-15 17:18:11.000000 darker-2.1.1/src/darker/help.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     6241 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/import_sorting.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2584 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/multiline_strings.py
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/py.typed
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-16 12:19:20.494892 darker-2.1.1/src/darker/tests/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2023-08-05 18:33:16.000000 darker-2.1.1/src/darker/tests/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1044 2023-08-05 18:33:16.000000 darker-2.1.1/src/darker/tests/git_diff_example_output.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1693 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    14874 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_black_diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1105 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_chooser.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    23754 2024-04-15 17:18:11.000000 darker-2.1.1/src/darker/tests/test_command_line.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1479 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_concurrency.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     4785 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_config.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     6025 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1625 2023-08-05 18:33:16.000000 darker-2.1.1/src/darker/tests/test_difflib.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      710 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_files.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1799 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_fstring.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    17157 2024-04-16 06:33:51.000000 darker-2.1.1/src/darker/tests/test_git.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     9253 2024-04-15 17:18:11.000000 darker-2.1.1/src/darker/tests/test_import_sorting.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    31139 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_main.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     5779 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_main_blacken_and_flynt_single_file.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     5023 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_main_revision.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     5420 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_main_stdin_filename.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     5311 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_multiline_strings.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      712 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_utils.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2226 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/tests/test_verification.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1204 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/utils.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3467 2024-04-06 20:23:15.000000 darker-2.1.1/src/darker/verification.py
+-rw-r--r--   0 akaihola  (1000) users      (100)       84 2024-04-16 12:18:59.000000 darker-2.1.1/src/darker/version.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-16 12:19:20.494892 darker-2.1.1/src/darker.egg-info/
+-rw-r--r--   0 akaihola  (1000) users      (100)    41421 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)     1461 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/SOURCES.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/dependency_links.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)       68 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/entry_points.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      536 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/requires.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        7 2024-04-16 12:19:20.000000 darker-2.1.1/src/darker.egg-info/top_level.txt
```

### Comparing `darker-2.1.0/LICENSE.rst` & `darker-2.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/PKG-INFO` & `darker-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darker
-Version: 2.1.0
+Version: 2.1.1
 Summary: Apply Black formatting only in regions changed since last commit
 Home-page: https://github.com/akaihola/darker
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darker
 Project-URL: Change Log, https://github.com/akaihola/darker/blob/master/CHANGES.rst
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: black>=22.3.0
-Requires-Dist: darkgraylib~=1.1.1
-Requires-Dist: graylint~=1.0.1
+Requires-Dist: darkgraylib~=1.2.0
+Requires-Dist: graylint~=1.1.1
 Requires-Dist: toml>=0.10.0
 Provides-Extra: flynt
 Requires-Dist: flynt>=0.76; extra == "flynt"
 Provides-Extra: isort
 Requires-Dist: isort>=5.0.1; extra == "isort"
 Provides-Extra: color
 Requires-Dist: Pygments>=2.4.0; extra == "color"
@@ -49,47 +49,43 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 =================================================
  Darker – reformat and lint modified Python code
 =================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darker/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darker/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/darker/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darker
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darker/
+   :target: https://pypi.org/project/darker/
 .. |downloads-badge| image:: https://pepy.tech/badge/darker
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darker
+   :target: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/24?color=red&label=release%202.1.1
+   :target: https://github.com/akaihola/darker/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/25?color=red&label=release%202.1.2
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/24
+   :target: https://github.com/akaihola/darker/milestone/24
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -180,19 +176,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=2.1.0
+  pip install --upgrade darker~=2.1.1
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=2.1.0 isort
+  conda install -c conda-forge darker~=2.1.1 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -410,30 +406,41 @@
        binary, or a full quoted command line with the command and options. Linters read
        their configuration as normally, and aren't affected by ``-c`` / ``--config``.
        Linter output is syntax highlighted when the ``pygments`` package is available if
        run on a terminal and or enabled by explicitly (see ``--color``).
 -S, --skip-string-normalization
        Don't normalize string quotes or prefixes
 --no-skip-string-normalization
-       Normalize string quotes or prefixes. This can be used to override
-       ``skip_string_normalization = true`` from a configuration file.
+       Normalize string quotes or prefixes. This can be used to override ``skip-string-
+       normalization = true`` from a Black configuration file.
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
-       to override ``skip_magic_trailing_comma = true`` from a configuration file.
+       to override ``skip-magic-trailing-comma = true`` from a Black configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
        [py33\|py34\|py35\|py36\|py37\|py38\|py39\|py310\|py311\|py312] Python versions
        that should be supported by Black's output. [default: per-file auto-detection]
 
 To change default values for these options for a given project,
-add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
-project's root directory, or to a different TOML file specified using the ``-c`` /
-``--config`` option. For example:
+add a ``[tool.darker]`` section to ``pyproject.toml`` in the project's root directory,
+or to a different TOML file specified using the ``-c`` / ``--config`` option.
+
+You should configure invoked tools like Black_, isort_ and flynt_
+using their own configuration files.
+
+As an exception, the ``line-length`` and ``target-version`` options in ``[tool.darker]``
+can be used to override corresponding options for individual tools.
+
+Note that Black_ honors only the options listed in the below example
+when called by ``darker``, because ``darker`` reads the Black configuration
+and passes it on when invoking Black_ directly through its Python API.
+
+An example ``pyproject.toml`` configuration file:
 
 .. code-block:: toml
 
    [tool.darker]
    src = [
        "src/mypackage",
    ]
@@ -442,34 +449,31 @@
    check = true
    isort = true
    flynt = true
    lint = [
        "pylint",
    ]
    line-length = 80                  # Passed to isort and Black, override their config
+   target-version = ["py312"]        # Passed to Black, overriding its config
    log_level = "INFO"
 
    [tool.black]
    line-length = 88                  # Overridden by [tool.darker] above
    skip-magic-trailing-comma = false
    skip-string-normalization = false
-   target-version = ["py38", "py39", "py310", "py311", "py312"]
+   target-version = ["py38", "py39", "py310", "py311", "py312"]  # Overridden above
    exclude = "test_*\.py"
    extend_exclude = "/generated/"
    force_exclude = ".*\.pyi"
 
    [tool.isort]
    profile = "black"
    known_third_party = ["pytest"]
    line_length = 88                  # Overridden by [tool.darker] above
 
-While isort_ reads all of its options from the configuration file, Black_ only honors
-the ones listed above when called by ``darker``. Other tools are invoked as
-subprocesses and use their configuration mechanisms unmodified.
-
 Be careful to not use options which generate output which is unexpected for
 other tools. For example, VSCode only expects the reformat diff, so
 ``lint = [ ... ]`` can't be used with it.
 
 *New in version 1.0.0:*
 
 - The ``-c``, ``-S`` and ``-l`` command line options.
@@ -496,14 +500,17 @@
 *New in version 1.5.0:* The ``-W`` / ``--workers``, ``--color`` and ``--no-color``
 command line options
 
 *New in version 1.7.0:* The ``-t`` / ``--target-version`` command line option
 
 *New in version 1.7.0:* The ``-f`` / ``--flynt`` command line option
 
+*New in version 2.1.1:* In ``[tool.darker]``, deprecate the the Black options
+``skip_string_normalization`` and ``skip_magic_trailing_comma``
+
 .. _Black documentation about pyproject.toml: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
 .. _isort documentation about config files: https://timothycrosley.github.io/isort/docs/configuration/config_files/
 .. _public GitHub repositories which install and run Darker: https://github.com/search?q=%2Fpip+install+.*darker%2F+path%3A%2F%5E.github%5C%2Fworkflows%5C%2F.*%2F&type=code
 .. _flynt documentation about configuration files: https://github.com/ikamensh/flynt#configuration-files
 .. _command line arguments: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#command-line-options
 
 Editor integration
@@ -592,23 +599,29 @@
      /usr/local/bin/darker  # possible location
 
    On Windows::
 
      $ where darker
      %LocalAppData%\Programs\Python\Python36-32\Scripts\darker.exe  # possible location
 
-3. Add these configuration options to VS code, ``Cmd-Shift-P``, ``Open Settings (JSON)``::
+3. Make sure you have the `VSCode black-formatter extension`__ installed.
+
+__ https://github.com/microsoft/vscode-black-formatter
+
+4. Add these configuration options to VSCode
+   (``⌘ Command / Ctrl`` + ``⇧ Shift`` + ``P``
+   and select ``Open Settings (JSON)``)::
 
-    "python.formatting.provider": "black",
-    "python.formatting.blackPath": "<install_location_from_step_2>",
-    "python.formatting.blackArgs": [],
+    "python.editor.defaultFormatter": "ms-python.black-formatter",
+    "black-formatter.path": "<install_location_from_step_2>",
+    "black-formatter.args": ["-d"],
 
 VSCode will always add ``--diff --quiet`` as arguments to Darker,
-but you can also pass additional arguments in the ``blackArgs`` option
-(e.g. ``["--isort", "--revision=master..."]``).
+but you can also pass additional arguments in the ``black-formatter.args`` option
+(e.g. ``["-d", "--isort", "--revision=master..."]``).
 Be sure to *not* enable any linters here or in ``pyproject.toml``
 since VSCode won't be able to understand output from them.
 
 Note that VSCode first copies the file to reformat into a temporary
 ``<filename>.py.<hash>.tmp`` file, then calls Black (or Darker in this case) on that
 file, and brings the changes in the modified files back into the editor.
 Darker is aware of this behavior, and will correctly compare ``.py.<hash>.tmp`` files
@@ -682,15 +695,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: v2.1.0
+        rev: v2.1.1
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -701,15 +714,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args:
            - --isort
            - --lint
            - mypy
            - --lint
@@ -732,15 +745,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -777,19 +790,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/darker@2.1.0
+         - uses: akaihola/darker@2.1.1
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=2.1.0"
+             version: "~=2.1.1"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
```

### Comparing `darker-2.1.0/README.rst` & `darker-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 =================================================
  Darker – reformat and lint modified Python code
 =================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darker/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darker/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/darker/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darker
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darker/
+   :target: https://pypi.org/project/darker/
 .. |downloads-badge| image:: https://pepy.tech/badge/darker
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darker
+   :target: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/24?color=red&label=release%202.1.1
+   :target: https://github.com/akaihola/darker/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/25?color=red&label=release%202.1.2
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/24
+   :target: https://github.com/akaihola/darker/milestone/24
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -133,19 +133,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=2.1.0
+  pip install --upgrade darker~=2.1.1
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=2.1.0 isort
+  conda install -c conda-forge darker~=2.1.1 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -363,30 +363,41 @@
        binary, or a full quoted command line with the command and options. Linters read
        their configuration as normally, and aren't affected by ``-c`` / ``--config``.
        Linter output is syntax highlighted when the ``pygments`` package is available if
        run on a terminal and or enabled by explicitly (see ``--color``).
 -S, --skip-string-normalization
        Don't normalize string quotes or prefixes
 --no-skip-string-normalization
-       Normalize string quotes or prefixes. This can be used to override
-       ``skip_string_normalization = true`` from a configuration file.
+       Normalize string quotes or prefixes. This can be used to override ``skip-string-
+       normalization = true`` from a Black configuration file.
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
-       to override ``skip_magic_trailing_comma = true`` from a configuration file.
+       to override ``skip-magic-trailing-comma = true`` from a Black configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
        [py33\|py34\|py35\|py36\|py37\|py38\|py39\|py310\|py311\|py312] Python versions
        that should be supported by Black's output. [default: per-file auto-detection]
 
 To change default values for these options for a given project,
-add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
-project's root directory, or to a different TOML file specified using the ``-c`` /
-``--config`` option. For example:
+add a ``[tool.darker]`` section to ``pyproject.toml`` in the project's root directory,
+or to a different TOML file specified using the ``-c`` / ``--config`` option.
+
+You should configure invoked tools like Black_, isort_ and flynt_
+using their own configuration files.
+
+As an exception, the ``line-length`` and ``target-version`` options in ``[tool.darker]``
+can be used to override corresponding options for individual tools.
+
+Note that Black_ honors only the options listed in the below example
+when called by ``darker``, because ``darker`` reads the Black configuration
+and passes it on when invoking Black_ directly through its Python API.
+
+An example ``pyproject.toml`` configuration file:
 
 .. code-block:: toml
 
    [tool.darker]
    src = [
        "src/mypackage",
    ]
@@ -395,34 +406,31 @@
    check = true
    isort = true
    flynt = true
    lint = [
        "pylint",
    ]
    line-length = 80                  # Passed to isort and Black, override their config
+   target-version = ["py312"]        # Passed to Black, overriding its config
    log_level = "INFO"
 
    [tool.black]
    line-length = 88                  # Overridden by [tool.darker] above
    skip-magic-trailing-comma = false
    skip-string-normalization = false
-   target-version = ["py38", "py39", "py310", "py311", "py312"]
+   target-version = ["py38", "py39", "py310", "py311", "py312"]  # Overridden above
    exclude = "test_*\.py"
    extend_exclude = "/generated/"
    force_exclude = ".*\.pyi"
 
    [tool.isort]
    profile = "black"
    known_third_party = ["pytest"]
    line_length = 88                  # Overridden by [tool.darker] above
 
-While isort_ reads all of its options from the configuration file, Black_ only honors
-the ones listed above when called by ``darker``. Other tools are invoked as
-subprocesses and use their configuration mechanisms unmodified.
-
 Be careful to not use options which generate output which is unexpected for
 other tools. For example, VSCode only expects the reformat diff, so
 ``lint = [ ... ]`` can't be used with it.
 
 *New in version 1.0.0:*
 
 - The ``-c``, ``-S`` and ``-l`` command line options.
@@ -449,14 +457,17 @@
 *New in version 1.5.0:* The ``-W`` / ``--workers``, ``--color`` and ``--no-color``
 command line options
 
 *New in version 1.7.0:* The ``-t`` / ``--target-version`` command line option
 
 *New in version 1.7.0:* The ``-f`` / ``--flynt`` command line option
 
+*New in version 2.1.1:* In ``[tool.darker]``, deprecate the the Black options
+``skip_string_normalization`` and ``skip_magic_trailing_comma``
+
 .. _Black documentation about pyproject.toml: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
 .. _isort documentation about config files: https://timothycrosley.github.io/isort/docs/configuration/config_files/
 .. _public GitHub repositories which install and run Darker: https://github.com/search?q=%2Fpip+install+.*darker%2F+path%3A%2F%5E.github%5C%2Fworkflows%5C%2F.*%2F&type=code
 .. _flynt documentation about configuration files: https://github.com/ikamensh/flynt#configuration-files
 .. _command line arguments: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#command-line-options
 
 Editor integration
@@ -545,23 +556,29 @@
      /usr/local/bin/darker  # possible location
 
    On Windows::
 
      $ where darker
      %LocalAppData%\Programs\Python\Python36-32\Scripts\darker.exe  # possible location
 
-3. Add these configuration options to VS code, ``Cmd-Shift-P``, ``Open Settings (JSON)``::
+3. Make sure you have the `VSCode black-formatter extension`__ installed.
+
+__ https://github.com/microsoft/vscode-black-formatter
 
-    "python.formatting.provider": "black",
-    "python.formatting.blackPath": "<install_location_from_step_2>",
-    "python.formatting.blackArgs": [],
+4. Add these configuration options to VSCode
+   (``⌘ Command / Ctrl`` + ``⇧ Shift`` + ``P``
+   and select ``Open Settings (JSON)``)::
+
+    "python.editor.defaultFormatter": "ms-python.black-formatter",
+    "black-formatter.path": "<install_location_from_step_2>",
+    "black-formatter.args": ["-d"],
 
 VSCode will always add ``--diff --quiet`` as arguments to Darker,
-but you can also pass additional arguments in the ``blackArgs`` option
-(e.g. ``["--isort", "--revision=master..."]``).
+but you can also pass additional arguments in the ``black-formatter.args`` option
+(e.g. ``["-d", "--isort", "--revision=master..."]``).
 Be sure to *not* enable any linters here or in ``pyproject.toml``
 since VSCode won't be able to understand output from them.
 
 Note that VSCode first copies the file to reformat into a temporary
 ``<filename>.py.<hash>.tmp`` file, then calls Black (or Darker in this case) on that
 file, and brings the changes in the modified files back into the editor.
 Darker is aware of this behavior, and will correctly compare ``.py.<hash>.tmp`` files
@@ -635,15 +652,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: v2.1.0
+        rev: v2.1.1
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -654,15 +671,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args:
            - --isort
            - --lint
            - mypy
            - --lint
@@ -685,15 +702,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -730,19 +747,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/darker@2.1.0
+         - uses: akaihola/darker@2.1.1
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=2.1.0"
+             version: "~=2.1.1"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
@@ -1344,14 +1361,15 @@
            <br />
            <sub>
              <b>Dominik Kutra</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/search?q=commenter%3Ak-dominik&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/akaihola/darker/discussions?discussions_q=author%3Ak-dominik" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/virtuald">
            <img src="https://avatars.githubusercontent.com/u/567900?v=3" width="100px;" alt="@virtuald" />
            <br />
            <sub>
              <b>Dustin Spicuzza</b>
@@ -1392,14 +1410,25 @@
              <b>Eyob Kibret</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/discussions?discussions_q=author%3AEyobkibret15" title="Bug reports">🐛</a>
        </td>
        <td align="center">
+         <a href="https://github.com/felixvd">
+           <img src="https://avatars.githubusercontent.com/u/4535737?v=3" width="100px;" alt="@felixvd" />
+           <br />
+           <sub>
+             <b>Felix von Drigalski</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Afelixvd" title="Code">💻</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/philipgian">
            <img src="https://avatars.githubusercontent.com/u/6884633?v=3" width="100px;" alt="@philipgian" />
            <br />
            <sub>
              <b>Filippos Giannakos</b>
            </sub>
          </a>
@@ -1435,27 +1464,27 @@
            <sub>
              <b>Gergely Polonkai</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Agergelypolonkai" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/muggenhor">
            <img src="https://avatars.githubusercontent.com/u/484066?v=3" width="100px;" alt="@muggenhor" />
            <br />
            <sub>
              <b>Giel van Schijndel</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=muggenhor" title="Code">💻</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/jabesq">
            <img src="https://avatars.githubusercontent.com/u/12049794?v=3" width="100px;" alt="@jabesq" />
            <br />
            <sub>
              <b>Hugo Dupras</b>
            </sub>
@@ -1505,39 +1534,50 @@
              <b>Jasleen Kaur</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Ajasleen19" title="Bug reports">🐛</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3Ajasleen19" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/jedie">
            <img src="https://avatars.githubusercontent.com/u/71315?v=3" width="100px;" alt="@jedie" />
            <br />
            <sub>
              <b>Jens Diemer</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Ajedie" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/jenshnielsen">
            <img src="https://avatars.githubusercontent.com/u/548266?v=3" width="100px;" alt="@jenshnielsen" />
            <br />
            <sub>
              <b>Jens Hedegaard Nielsen</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/search?q=jenshnielsen" title="Bug reports">🐛</a>
        </td>
        <td align="center">
+         <a href="https://github.com/jvacek">
+           <img src="https://avatars.githubusercontent.com/u/1302278?v=3" width="100px;" alt="@jvacek" />
+           <br />
+           <sub>
+             <b>Jonas Vacek</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/search?q=jvacek" title="Bug reports">🐛</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/wkentaro">
            <img src="https://avatars.githubusercontent.com/u/4310419?v=3" width="100px;" alt="@wkentaro" />
            <br />
            <sub>
              <b>Kentaro Wada</b>
            </sub>
          </a>
@@ -1562,14 +1602,16 @@
            <sub>
              <b>Krischtopp</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3AKrischtopp" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/leotrs">
            <img src="https://avatars.githubusercontent.com/u/1096704?v=3" width="100px;" alt="@leotrs" />
            <br />
            <sub>
              <b>Leo Torres</b>
            </sub>
@@ -1584,16 +1626,14 @@
            <sub>
              <b>Magnus N. Malmquist</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Amagnunm" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/markddavidoff">
            <img src="https://avatars.githubusercontent.com/u/1360543?v=3" width="100px;" alt="@markddavidoff" />
            <br />
            <sub>
              <b>Mark Davidoff</b>
            </sub>
@@ -1632,14 +1672,16 @@
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=Carreau" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/commits?author=Carreau" title="Documentation">📖</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3ACarreau" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/MatthijsBurgh">
            <img src="https://avatars.githubusercontent.com/u/18014833?v=3" width="100px;" alt="@MatthijsBurgh" />
            <br />
            <sub>
              <b>Matthijs van der Burgh</b>
            </sub>
@@ -1654,16 +1696,14 @@
            <sub>
              <b>Min RK</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/conda-forge/darker-feedstock/search?q=darker+author%3Aminrk&type=issues" title="Code">💻</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/my-tien">
            <img src="https://avatars.githubusercontent.com/u/3898364?v=3" width="100px;" alt="@my-tien" />
            <br />
            <sub>
              <b>My-Tien Nguyen</b>
            </sub>
@@ -1703,14 +1743,16 @@
            <sub>
              <b>Nutchanon Ninyawee</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Awasdee" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/Pacu2">
            <img src="https://avatars.githubusercontent.com/u/21290461?v=3" width="100px;" alt="@Pacu2" />
            <br />
            <sub>
              <b>Pacu2</b>
            </sub>
@@ -1726,16 +1768,14 @@
            <sub>
              <b>Patrick Jordan</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/discussions?discussions_q=author%3APatrickJordanCongenica" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/ivanov">
            <img src="https://avatars.githubusercontent.com/u/118211?v=3" width="100px;" alt="@ivanov" />
            <br />
            <sub>
              <b>Paul Ivanov</b>
            </sub>
@@ -1774,14 +1814,16 @@
            <sub>
              <b>Rishi Kumar Ray</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/search?q=RishiKumarRay" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/ioggstream">
            <img src="https://avatars.githubusercontent.com/u/1140844?v=3" width="100px;" alt="@ioggstream" />
            <br />
            <sub>
              <b>Roberto Polli</b>
            </sub>
@@ -1796,16 +1838,14 @@
            <sub>
              <b>Ronie Martinez</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Aroniemartinez" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/rossbar">
            <img src="https://avatars.githubusercontent.com/u/1268991?v=3" width="100px;" alt="@rossbar" />
            <br />
            <sub>
              <b>Ross Barnowski</b>
            </sub>
@@ -1842,14 +1882,16 @@
            <sub>
              <b>Sean Hammond</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3Asherbie" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/hauntsaninja">
            <img src="https://avatars.githubusercontent.com/u/12621235?v=3" width="100px;" alt="@hauntsaninja" />
            <br />
            <sub>
              <b>Shantanu</b>
            </sub>
@@ -1864,16 +1906,14 @@
            <sub>
              <b>Simone Gaiarin</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/search?q=commenter%3Asimgunz&type=issues" title="Reviewed Pull Requests">👀</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/soxofaan">
            <img src="https://avatars.githubusercontent.com/u/44946?v=3" width="100px;" alt="@soxofaan" />
            <br />
            <sub>
              <b>Stefaan Lippens</b>
            </sub>
@@ -1910,14 +1950,16 @@
            <sub>
              <b>TJ Kolleh</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Atkolleh" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/talhajunaidd">
            <img src="https://avatars.githubusercontent.com/u/6547611?v=3" width="100px;" alt="@talhajunaidd" />
            <br />
            <sub>
              <b>Talha Juanid</b>
            </sub>
@@ -1932,16 +1974,14 @@
            <sub>
              <b>Thomas Güttler</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Aguettli" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/Timple">
            <img src="https://avatars.githubusercontent.com/u/5036851?v=3" width="100px;" alt="@Timple" />
            <br />
            <sub>
              <b>Tim Clephas</b>
            </sub>
@@ -1977,14 +2017,16 @@
            <sub>
              <b>Trevor Gross</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Atgross35" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/victorcui96">
            <img src="https://avatars.githubusercontent.com/u/14048976?v=3" width="100px;" alt="@victorcui96" />
            <br />
            <sub>
              <b>Victor Cui</b>
            </sub>
@@ -2000,16 +2042,14 @@
              <b>Vivek Kushwaha</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Ayoursvivek" title="Bug reports">🐛</a>
          <a href="https://github.com/akaihola/darker/commits?author=yoursvivek" title="Documentation">📖</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/Hainguyen1210">
            <img src="https://avatars.githubusercontent.com/u/15359217?v=3" width="100px;" alt="@Hainguyen1210" />
            <br />
            <sub>
              <b>Will</b>
            </sub>
@@ -2047,14 +2087,16 @@
            <sub>
              <b>Zach Norton</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Azachnorton4C" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/clintonsteiner">
            <img src="https://avatars.githubusercontent.com/u/47841949?v=3" width="100px;" alt="@clintonsteiner" />
            <br />
            <sub>
              <b>csteiner</b>
            </sub>
@@ -2069,16 +2111,14 @@
            <sub>
              <b>deadkex</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/discussions?discussions_q=author%3Adeadkex" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/dsmanl">
            <img src="https://avatars.githubusercontent.com/u/67360039?v=3" width="100px;" alt="@dsmanl" />
            <br />
            <sub>
              <b>dsmanl</b>
            </sub>
@@ -2116,14 +2156,16 @@
              <b>martinRenou</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/conda-forge/staged-recipes/search?q=darker&type=issues&author=martinRenou" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3AmartinRenou" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/mayk0gan">
            <img src="https://avatars.githubusercontent.com/u/96263702?v=3" width="100px;" alt="@mayk0gan" />
            <br />
            <sub>
              <b>mayk0gan</b>
            </sub>
@@ -2138,16 +2180,14 @@
            <sub>
              <b>okuuva</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/search?q=commenter%3Aokuuva&type=issues" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/overratedpro">
            <img src="https://avatars.githubusercontent.com/u/1379994?v=3" width="100px;" alt="@overratedpro" />
            <br />
            <sub>
              <b>overratedpro</b>
            </sub>
```

### Comparing `darker-2.1.0/pyproject.toml` & `darker-2.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -49,7 +49,11 @@
 "src/darker/tests/*.py" = [
     "ANN001",  # Missing type annotation for function argument
     "ANN201",  # Missing return type annotation for public function
     "ANN204",  # Missing return type annotation for special method `__init__`
     "C408",  # Unnecessary `dict` call (rewrite as a literal)
     "S101",  # Use of `assert` detected
 ]
+
+[tool.ruff.lint.isort]
+known-first-party = ["darkgraylib", "graylint"]
+known-third-party = ["pytest"]
```

### Comparing `darker-2.1.0/setup.cfg` & `darker-2.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 [options]
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	black>=22.3.0
-	darkgraylib~=1.1.1
-	graylint~=1.0.1
+	darkgraylib~=1.2.0
+	graylint~=1.1.1
 	toml>=0.10.0
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 darker = 
 	py.typed
+	.pyi
 
 [options.entry_points]
 console_scripts = 
 	darker = darker.__main__:main_with_error_handling
 
 [options.extras_require]
 flynt = 
@@ -71,19 +72,15 @@
 	ruff>=0.0.292
 	twine>=2.0.0
 	types-requests>=2.27.9
 	types-toml>=0.10.4
 	urllib3>=1.25.9  # through requests-cache and twine, fixes CVE-2020-26137
 	wheel>=0.21.0
 release = 
-	airium>=0.2.3
-	click>=8.0.0
-	darkgray-dev-tools~=0.0.1
-	defusedxml>=0.7.1
-	requests_cache>=0.7
+	darkgray-dev-tools~=0.0.2
 
 [flake8]
 max-line-length = 88
 ignore = 
 	C408
 	D400
 	D415
```

### Comparing `darker-2.1.0/setup.py` & `darker-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/__main__.py` & `darker-2.1.1/src/darker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -512,18 +512,22 @@
     if args.target_version:
         black_config["target_version"] = {args.target_version}
     if args.skip_string_normalization is not None:
         black_config["skip_string_normalization"] = args.skip_string_normalization
     if args.skip_magic_trailing_comma is not None:
         black_config["skip_magic_trailing_comma"] = args.skip_magic_trailing_comma
 
-    paths, root = resolve_paths(args.stdin_filename, args.src)
+    paths, common_root = resolve_paths(args.stdin_filename, args.src)
+    # `common_root` is now the common root of given paths,
+    # not necessarily the repository root.
+    # `paths` are the unmodified paths from `--stdin-filename` or `SRC`,
+    # so either relative to the current working directory or absolute paths.
 
     revrange = RevisionRange.parse_with_common_ancestor(
-        args.revision, root, args.stdin_filename is not None
+        args.revision, common_root, args.stdin_filename is not None
     )
     output_mode = OutputMode.from_args(args)
     write_modified_files = not args.check and output_mode == OutputMode.NOTHING
     if write_modified_files:
         if args.revision == PRE_COMMIT_FROM_TO_REFS and revrange.rev2 == "HEAD":
             warnings.warn(
                 "Darker was called by pre-commit, comparing HEAD to an older commit."
@@ -535,43 +539,43 @@
             raise ArgumentError(
                 Action(["-r", "--revision"], "revision"),
                 f"Can't write reformatted files for revision {revrange.rev2!r}."
                 " Either --diff or --check must be used.",
             )
 
     if revrange.rev2 != STDIN:
-        missing = get_missing_at_revision(paths, revrange.rev2, root)
+        missing = get_missing_at_revision(paths, revrange.rev2, common_root)
         if missing:
             missing_reprs = " ".join(repr(str(path)) for path in missing)
             rev2_repr = (
                 "the working tree" if revrange.rev2 == WORKTREE else revrange.rev2
             )
             raise ArgumentError(
                 Action(["PATH"], "path"),
                 f"Error: Path(s) {missing_reprs} do not exist in {rev2_repr}",
             )
 
-    # These paths are relative to `root`:
-    files_to_process = filter_python_files(paths, root, {})
-    files_to_blacken = filter_python_files(paths, root, black_config)
+    # These paths are relative to `common_root`:
+    files_to_process = filter_python_files(paths, common_root, {})
+    files_to_blacken = filter_python_files(paths, common_root, black_config)
     # Now decide which files to reformat (Black & isort). Note that this doesn't apply
     # to linting.
     if output_mode == OutputMode.CONTENT or revrange.rev2 == STDIN:
         # With `-d` / `--stdout` and `--stdin-filename`, process the file whether
         # modified or not. Paths have previously been validated to contain exactly one
         # existing file.
         changed_files_to_reformat = files_to_process
         black_exclude = set()
     else:
         # In other modes, only reformat files which have been modified.
-        if git_is_repository(root):
+        if git_is_repository(common_root):
             # Get the modified files only.
-            repo_root = find_project_root((str(root),))
+            repo_root = find_project_root((str(common_root),))
             changed_files = {
-                (repo_root / file).relative_to(root)
+                (repo_root / file).relative_to(common_root)
                 for file in git_get_modified_python_files(paths, revrange, repo_root)
             }
             # Filter out changed files that are not supposed to be processed
             changed_files_to_reformat = files_to_process.intersection(changed_files)
 
         else:
             changed_files_to_reformat = files_to_process
@@ -580,15 +584,15 @@
             for path in changed_files_to_reformat
             if path not in files_to_blacken
         }
     use_color = should_use_color(config["color"])
     formatting_failures_on_modified_lines = False
     for path, old, new in sorted(
         format_edited_parts(
-            root,
+            common_root,
             changed_files_to_reformat,
             Exclusions(
                 black=black_exclude,
                 isort=set() if args.isort else {"**/*"},
                 flynt=set() if args.flynt else {"**/*"},
             ),
             revrange,
@@ -598,24 +602,24 @@
         ),
     ):
         # 10. A re-formatted Python file which produces an identical AST was
         #     created successfully - write an updated file or print the diff if
         #     there were any changes to the original
         formatting_failures_on_modified_lines = True
         if output_mode == OutputMode.DIFF:
-            print_diff(path, old, new, root, use_color)
+            print_diff(path, old, new, common_root, use_color)
         elif output_mode == OutputMode.CONTENT:
             print_source(new, use_color)
         if write_modified_files:
             modify_file(path, new)
     linter_failures_on_modified_lines = run_linters(
         args.lint,
-        root,
+        common_root,
         # paths to lint are not limited to modified files or just Python files:
-        {p.resolve().relative_to(root) for p in paths},
+        {p.resolve().relative_to(common_root) for p in paths},
         revrange,
         use_color,
     )
     return (
         1
         if linter_failures_on_modified_lines
         or (args.check and formatting_failures_on_modified_lines)
```

### Comparing `darker-2.1.0/src/darker/black_diff.py` & `darker-2.1.1/src/darker/black_diff.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/chooser.py` & `darker-2.1.1/src/darker/chooser.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/command_line.py` & `darker-2.1.1/src/darker/command_line.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Command line parsing for the ``darker`` binary"""
 
+import warnings
 from argparse import ArgumentParser, Namespace
 from functools import partial
 from typing import List, Optional, Tuple
 
 from black import TargetVersion
 
 import darkgraylib.command_line
 from darker import help as hlp
-from darker.config import DarkerConfig, OutputMode
+from darker.config import DEPRECATED_CONFIG_OPTIONS, DarkerConfig, OutputMode
 from darkgraylib.command_line import add_parser_argument
 from graylint.command_line import add_lint_arg
 
 
 def make_argument_parser(require_src: bool) -> ArgumentParser:
     """Create the argument parser object
 
@@ -74,14 +75,25 @@
         dest="target_version",
         metavar="VERSION",
         choices=[v.name.lower() for v in TargetVersion],
     )
     return parser
 
 
+def show_config_deprecations(config: DarkerConfig) -> None:
+    """Show deprecation warnings for configuration keys from the config file."""
+    for option in DEPRECATED_CONFIG_OPTIONS & set(config):
+        warnings.warn(
+            f"The configuration option `{option}` in [tool.darker] is deprecated"
+            " and will be removed in Darker 3.0.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+
 def parse_command_line(
     argv: Optional[List[str]],
 ) -> Tuple[Namespace, DarkerConfig, DarkerConfig]:
     """Return the parsed command line, using defaults from a configuration file
 
     Also return the effective configuration which combines defaults, the configuration
     read from ``pyproject.toml`` (or the path given in ``--config``), environment
@@ -92,12 +104,16 @@
     :param argv: Command line arguments to parse (excluding the path of the script). If
                  ``None``, use ``sys.argv``.
     :return: A tuple of the parsed command line, the effective configuration, and the
              set of modified configuration options from the defaults.
 
     """
     args, effective_cfg, modified_cfg = darkgraylib.command_line.parse_command_line(
-        make_argument_parser, argv, "darker", DarkerConfig
+        make_argument_parser,
+        argv,
+        "darker",
+        DarkerConfig,
+        show_config_deprecations,
     )
     OutputMode.validate_diff_stdout(args.diff, args.stdout)
     OutputMode.validate_stdout_src(args.stdout, args.src, args.stdin_filename)
     return args, effective_cfg, modified_cfg
```

### Comparing `darker-2.1.0/src/darker/concurrency.py` & `darker-2.1.1/src/darker/concurrency.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/config.py` & `darker-2.1.1/src/darker/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from typing import Dict, List, Optional, Set, Union
 
 from darkgraylib.config import BaseConfig, ConfigurationError
 
 UnvalidatedConfig = Dict[str, Union[List[str], str, bool, int]]
 
 
+DEPRECATED_CONFIG_OPTIONS = {"skip_string_normalization", "skip_magic_trailing_comma"}
+
+
 class DarkerConfig(BaseConfig, total=False):
     """Dictionary representing ``[tool.darker]`` from ``pyproject.toml``"""
 
     diff: bool
     check: bool
     isort: bool
     lint: List[str]
@@ -53,15 +56,15 @@
         stdout: bool, src: List[str], stdin_filename: Optional[str]
     ) -> None:
         """Raise an exception in ``stdout`` mode if not exactly one input is provided"""
         if not stdout:
             return
         if stdin_filename is None and len(src) == 1 and Path(src[0]).is_file():
             return
-        if stdin_filename is not None and len(src) == 0:
+        if stdin_filename is not None and len(src) == 0 or src == ["-"]:
             return
         raise ConfigurationError(
             "Either --stdin-filename=<path> or exactly one Python source file which"
             " exists on disk must be provided when using the `stdout` option"
         )
```

### Comparing `darker-2.1.0/src/darker/diff.py` & `darker-2.1.1/src/darker/diff.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/files.py` & `darker-2.1.1/src/darker/files.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/fstring.py` & `darker-2.1.1/src/darker/fstring.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/git.py` & `darker-2.1.1/src/darker/git.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,92 +72,101 @@
     :param path: The path to inspect
     :return: ``False`` if the path doesn't exist or is not a ``.py`` file
 
     """
     return path.exists() and get_path_in_repo(path).suffix == ".py"
 
 
-def _git_exists_in_revision(path: Path, rev2: str, cwd: Path) -> bool:
+def _git_exists_in_revision(path: Path, rev2: str, git_cwd: Path) -> bool:
     """Return ``True`` if the given path exists in the given Git revision
 
-    :param path: The path of the file or directory to check
+    :param path: The path of the file or directory to check, either relative to current
+                 working directory or absolute
     :param rev2: The Git revision to look at
-    :param cwd: The Git repository root
+    :param git_cwd: The working directory to use when invoking Git. This has to be
+                    either the root of the working tree, or another directory inside it.
     :return: ``True`` if the file or directory exists at the revision, or ``False`` if
              it doesn't.
 
     """
-    if (cwd / path).resolve() == cwd.resolve():
-        return True
+    while not git_cwd.exists():
+        # The working directory for running Git doesn't exist. Walk up the directory
+        # tree until we find an existing directory. This is necessary because `git
+        # cat-file` doesn't work if the current working directory doesn't exist.
+        git_cwd = git_cwd.parent
+    relative_path = (Path.cwd() / path).relative_to(git_cwd.resolve())
     # Surprise: On Windows, `git cat-file` doesn't work with backslash directory
     # separators in paths. We need to use Posix paths and forward slashes instead.
-    cmd = ["git", "cat-file", "-e", f"{rev2}:{path.as_posix()}"]
-    logger.debug("[%s]$ %s", cwd, " ".join(cmd))
+    # Surprise #2: `git cat-file` assumes paths are relative to the repository root.
+    # We need to prepend `./` to paths relative to the working directory.
+    cmd = ["git", "cat-file", "-e", f"{rev2}:./{relative_path.as_posix()}"]
+    logger.debug("[%s]$ %s", git_cwd, " ".join(cmd))
     result = run(  # nosec
         cmd,
-        cwd=str(cwd),
+        cwd=str(git_cwd),
         check=False,
         stderr=DEVNULL,
         env=make_git_env(),
     )
     return result.returncode == 0
 
 
 def get_missing_at_revision(paths: Iterable[Path], rev2: str, cwd: Path) -> Set[Path]:
     """Return paths missing in the given revision
 
     In case of ``WORKTREE``, just check if the files exist on the filesystem instead of
     asking Git.
 
-    :param paths: Paths to check
+    :param paths: Paths to check, relative to the current working directory or absolute
     :param rev2: The Git revision to look at, or ``WORKTREE`` for the working tree
-    :param cwd: The Git repository root
+    :param cwd: The working directory to use when invoking Git. This has to be either
+                the root of the working tree, or another directory inside it.
     :return: The set of file or directory paths which are missing in the revision
 
     """
     if rev2 == WORKTREE:
         return {path for path in paths if not path.exists()}
     return {path for path in paths if not _git_exists_in_revision(path, rev2, cwd)}
 
 
 def _git_diff_name_only(
-    rev1: str, rev2: str, relative_paths: Iterable[Path], cwd: Path
+    rev1: str, rev2: str, relative_paths: Iterable[Path], repo_root: Path
 ) -> Set[Path]:
     """Collect names of changed files between commits from Git
 
     :param rev1: The old commit to compare to
     :param rev2: The new commit to compare, or the string ``":WORKTREE:"`` to compare
                  current working tree to ``rev1``
-    :param relative_paths: Relative paths to the files to compare
-    :param cwd: The Git repository root
+    :param relative_paths: Relative paths from repository root to the files to compare
+    :param repo_root: The Git repository root
     :return: Relative paths of changed files
 
     """
     diff_cmd = [
         "diff",
         "--name-only",
         "--relative",
         rev1,
         # rev2 is inserted here if not WORKTREE
         "--",
         *{path.as_posix() for path in relative_paths},
     ]
     if rev2 != WORKTREE:
         diff_cmd.insert(diff_cmd.index("--"), rev2)
-    lines = git_check_output_lines(diff_cmd, cwd)
+    lines = git_check_output_lines(diff_cmd, repo_root)
     return {Path(line) for line in lines}
 
 
 def _git_ls_files_others(relative_paths: Iterable[Path], cwd: Path) -> Set[Path]:
     """Collect names of untracked non-excluded files from Git
 
     This will return those files in ``relative_paths`` which are untracked and not
     excluded by ``.gitignore`` or other Git's exclusion mechanisms.
 
-    :param relative_paths: Relative paths to the files to consider
+    :param relative_paths: Relative paths from repository root to the files to consider
     :param cwd: The Git repository root
     :return: Relative paths of untracked files
 
     """
     ls_files_cmd = [
         "ls-files",
         "--others",
@@ -166,31 +175,34 @@
         *{path.as_posix() for path in relative_paths},
     ]
     lines = git_check_output_lines(ls_files_cmd, cwd)
     return {Path(line) for line in lines}
 
 
 def git_get_modified_python_files(
-    paths: Iterable[Path], revrange: RevisionRange, cwd: Path
+    paths: Iterable[Path], revrange: RevisionRange, repo_root: Path
 ) -> Set[Path]:
     """Ask Git for modified and untracked ``*.py`` files
 
     - ``git diff --name-only --relative <rev> -- <path(s)>``
     - ``git ls-files --others --exclude-standard -- <path(s)>``
 
-    :param paths: Relative paths to the files to diff
+    :param paths: Files to diff, either relative to the current working dir or absolute
     :param revrange: Git revision range to compare
-    :param cwd: The Git repository root
+    :param repo_root: The Git repository root
     :return: File names relative to the Git repository root
 
     """
-    changed_paths = _git_diff_name_only(revrange.rev1, revrange.rev2, paths, cwd)
+    repo_paths = [path.resolve().relative_to(repo_root) for path in paths]
+    changed_paths = _git_diff_name_only(
+        revrange.rev1, revrange.rev2, repo_paths, repo_root
+    )
     if revrange.rev2 == WORKTREE:
-        changed_paths.update(_git_ls_files_others(paths, cwd))
-    return {path for path in changed_paths if should_reformat_file(cwd / path)}
+        changed_paths.update(_git_ls_files_others(repo_paths, repo_root))
+    return {path for path in changed_paths if should_reformat_file(repo_root / path)}
 
 
 def _revision_vs_lines(
     root: Path, path_in_repo: Path, rev1: str, content: TextDocument, context_lines: int
 ) -> List[int]:
     """Return changed line numbers between the given revision and given text content
```

### Comparing `darker-2.1.0/src/darker/help.py` & `darker-2.1.1/src/darker/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,21 +120,21 @@
 )
 
 VERSION = "Show the version of `darker`"
 
 SKIP_STRING_NORMALIZATION = "Don't normalize string quotes or prefixes"
 NO_SKIP_STRING_NORMALIZATION = (
     "Normalize string quotes or prefixes. This can be used to override"
-    " `skip_string_normalization = true` from a configuration file."
+    " `skip-string-normalization = true` from a Black configuration file."
 )
 SKIP_MAGIC_TRAILING_COMMA = (
     "Skip adding trailing commas to expressions that are split by comma"
     " where each element is on its own line. This includes function signatures."
     " This can be used to override"
-    " `skip_magic_trailing_comma = true` from a configuration file."
+    " `skip-magic-trailing-comma = true` from a Black configuration file."
 )
 
 LINE_LENGTH = "How many characters per line to allow [default: 88]"
 
 TARGET_VERSION = (
     f"[{'|'.join(v.name.lower() for v in TargetVersion)}] Python versions that should"
     " be supported by Black's output. [default: per-file auto-detection]"
```

### Comparing `darker-2.1.0/src/darker/import_sorting.py` & `darker-2.1.1/src/darker/import_sorting.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/multiline_strings.py` & `darker-2.1.1/src/darker/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/git_diff_example_output.py` & `darker-2.1.1/src/darker/tests/git_diff_example_output.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/helpers.py` & `darker-2.1.1/src/darker/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_black_diff.py` & `darker-2.1.1/src/darker/tests/test_black_diff.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_chooser.py` & `darker-2.1.1/src/darker/tests/test_chooser.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_command_line.py` & `darker-2.1.1/src/darker/tests/test_command_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from argparse import ArgumentError
 from importlib import reload
 from pathlib import Path
 from textwrap import dedent
 from unittest.mock import DEFAULT, Mock, call, patch
 
 import pytest
+import toml
 from black import TargetVersion
 
 import darker.help
 from darker import black_diff
 from darker.__main__ import main
 from darker.command_line import make_argument_parser, parse_command_line
 from darker.config import Exclusions
@@ -239,14 +240,70 @@
             assert modified_option not in modified_cfg
         else:
             assert (
                 modified_cfg[modified_option] == expect_modified_value  # type: ignore
             )
 
 
+@pytest.mark.kwparametrize(
+    dict(config={}, expect_warn=set()),
+    dict(config={"diff": True}, expect_warn=set()),
+    dict(config={"stdout": True}, expect_warn=set()),
+    dict(config={"check": True}, expect_warn=set()),
+    dict(config={"isort": True}, expect_warn=set()),
+    dict(config={"lint": ["pylint"]}, expect_warn=set()),
+    dict(
+        config={"skip_string_normalization": True},
+        expect_warn={
+            "The configuration option `skip_string_normalization` in [tool.darker] is"
+            " deprecated and will be removed in Darker 3.0."
+        },
+    ),
+    dict(
+        config={"skip_magic_trailing_comma": True},
+        expect_warn={
+            "The configuration option `skip_magic_trailing_comma` in [tool.darker] is"
+            " deprecated and will be removed in Darker 3.0."
+        },
+    ),
+    dict(config={"line_length": 88}, expect_warn=set()),
+    dict(config={"target_version": "py37"}, expect_warn=set()),
+    dict(
+        config={
+            "diff": True,
+            "stdout": False,
+            "check": True,
+            "isort": True,
+            "lint": ["pylint"],
+            "skip_string_normalization": True,
+            "skip_magic_trailing_comma": True,
+            "line_length": 88,
+            "target_version": "py37",
+        },
+        expect_warn={
+            "The configuration option `skip_magic_trailing_comma` in [tool.darker] is"
+            " deprecated and will be removed in Darker 3.0.",
+            "The configuration option `skip_string_normalization` in [tool.darker] is"
+            " deprecated and will be removed in Darker 3.0.",
+        },
+    ),
+)
+def test_parse_command_line_deprecated_option(
+    tmp_path, monkeypatch, config, expect_warn
+):
+    """`parse_command_line` warns about deprecated configuration options."""
+    monkeypatch.chdir(tmp_path)
+    (tmp_path / "pyproject.toml").write_text(toml.dumps({"tool": {"darker": config}}))
+    with patch("darker.command_line.warnings.warn") as warn:
+
+        parse_command_line(["-"])
+
+    assert {c.args[0] for c in warn.call_args_list} == expect_warn
+
+
 def test_help_description_without_isort_package(capsys):
     """``darker --help`` description shows how to add ``isort`` if it's not present"""
     with isort_present(False):
 
         assert (
             "Please run `pip install darker[isort]` to enable sorting of import "
             "definitions" in get_darker_help_output(capsys)
```

### Comparing `darker-2.1.0/src/darker/tests/test_concurrency.py` & `darker-2.1.1/src/darker/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_config.py` & `darker-2.1.1/src/darker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_diff.py` & `darker-2.1.1/src/darker/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_difflib.py` & `darker-2.1.1/src/darker/tests/test_difflib.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_files.py` & `darker-2.1.1/src/darker/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_fstring.py` & `darker-2.1.1/src/darker/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_git.py` & `darker-2.1.1/src/darker/tests/test_git.py`

 * *Files 21% similar despite different names*

```diff
@@ -65,72 +65,143 @@
     """``_git_exists_in_revision()`` calls Git and converts return value correctly"""
     with patch.object(git, "run") as run:
         run.return_value.returncode = retval
 
         result = git._git_exists_in_revision(Path("path.py"), "rev2", Path("."))
 
     run.assert_called_once_with(
-        ["git", "cat-file", "-e", "rev2:path.py"],
+        ["git", "cat-file", "-e", "rev2:./path.py"],
         cwd=".",
         check=False,
         stderr=DEVNULL,
         env={"LC_ALL": "C", "PATH": os.environ["PATH"]},
     )
     assert result == expect
 
 
 @pytest.mark.kwparametrize(
-    dict(rev2="{add}", path="dir/a.py", expect=True),
-    dict(rev2="{add}", path="dir/b.py", expect=True),
-    dict(rev2="{add}", path="dir/", expect=True),
-    dict(rev2="{add}", path="dir", expect=True),
-    dict(rev2="{del_a}", path="dir/a.py", expect=False),
-    dict(rev2="{del_a}", path="dir/b.py", expect=True),
-    dict(rev2="{del_a}", path="dir/", expect=True),
-    dict(rev2="{del_a}", path="dir", expect=True),
-    dict(rev2="HEAD", path="dir/a.py", expect=False),
-    dict(rev2="HEAD", path="dir/b.py", expect=False),
-    dict(rev2="HEAD", path="dir/", expect=False),
-    dict(rev2="HEAD", path="dir", expect=False),
+    dict(cwd=".", rev2="{add}", path="x/dir/a.py", expect=True),
+    dict(cwd=".", rev2="{add}", path="x/dir/sub/b.py", expect=True),
+    dict(cwd=".", rev2="{add}", path="x/dir/", expect=True),
+    dict(cwd=".", rev2="{add}", path="x/dir", expect=True),
+    dict(cwd=".", rev2="{add}", path="x/dir/sub", expect=True),
+    dict(cwd=".", rev2="{del_a}", path="x/dir/a.py", expect=False),
+    dict(cwd=".", rev2="{del_a}", path="x/dir/sub/b.py", expect=True),
+    dict(cwd=".", rev2="{del_a}", path="x/dir/", expect=True),
+    dict(cwd=".", rev2="{del_a}", path="x/dir", expect=True),
+    dict(cwd=".", rev2="{del_a}", path="x/dir/sub", expect=True),
+    dict(cwd=".", rev2="HEAD", path="x/dir/a.py", expect=False),
+    dict(cwd=".", rev2="HEAD", path="x/dir/sub/b.py", expect=False),
+    dict(cwd=".", rev2="HEAD", path="x/dir/", expect=False),
+    dict(cwd=".", rev2="HEAD", path="x/dir", expect=False),
+    dict(cwd=".", rev2="HEAD", path="x/dir/sub", expect=False),
+    dict(cwd="x", rev2="{add}", path="dir/a.py", expect=True),
+    dict(cwd="x", rev2="{add}", path="dir/sub/b.py", expect=True),
+    dict(cwd="x", rev2="{add}", path="dir/", expect=True),
+    dict(cwd="x", rev2="{add}", path="dir", expect=True),
+    dict(cwd="x", rev2="{add}", path="dir/sub", expect=True),
+    dict(cwd="x", rev2="{del_a}", path="dir/a.py", expect=False),
+    dict(cwd="x", rev2="{del_a}", path="dir/sub/b.py", expect=True),
+    dict(cwd="x", rev2="{del_a}", path="dir/", expect=True),
+    dict(cwd="x", rev2="{del_a}", path="dir", expect=True),
+    dict(cwd="x", rev2="{del_a}", path="dir/sub", expect=True),
+    dict(cwd="x", rev2="HEAD", path="dir/a.py", expect=False),
+    dict(cwd="x", rev2="HEAD", path="dir/sub/b.py", expect=False),
+    dict(cwd="x", rev2="HEAD", path="dir/", expect=False),
+    dict(cwd="x", rev2="HEAD", path="dir", expect=False),
+    dict(cwd="x", rev2="HEAD", path="dir/sub", expect=False),
 )
-def test_git_exists_in_revision(git_repo, rev2, path, expect):
+def test_git_exists_in_revision(git_repo, monkeypatch, cwd, rev2, path, expect):
     """``_get_exists_in_revision()`` detects file/dir existence correctly"""
-    git_repo.add({"dir/a.py": "", "dir/b.py": ""}, commit="Add dir/*.py")
+    git_repo.add(
+        {"x/README": "", "x/dir/a.py": "", "x/dir/sub/b.py": ""},
+        commit="Add x/dir/*.py",
+    )
     add = git_repo.get_hash()
-    git_repo.add({"dir/a.py": None}, commit="Delete dir/a.py")
+    git_repo.add({"x/dir/a.py": None}, commit="Delete x/dir/a.py")
     del_a = git_repo.get_hash()
-    git_repo.add({"dir/b.py": None}, commit="Delete dir/b.py")
+    git_repo.add({"x/dir/sub/b.py": None}, commit="Delete x/dir/b.py")
+    monkeypatch.chdir(cwd)
 
     result = git._git_exists_in_revision(
-        Path(path), rev2.format(add=add, del_a=del_a), git_repo.root
+        Path(path), rev2.format(add=add, del_a=del_a), git_repo.root / "x/dir/sub"
     )
 
     assert result == expect
 
 
 @pytest.mark.kwparametrize(
-    dict(rev2="{add}", expect=set()),
-    dict(rev2="{del_a}", expect={Path("dir/a.py")}),
-    dict(rev2="HEAD", expect={Path("dir"), Path("dir/a.py"), Path("dir/b.py")}),
+    dict(
+        paths={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+        rev2="{add}",
+        expect=set(),
+    ),
+    dict(
+        paths={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+        rev2="{del_a}",
+        expect={"x/dir/a.py"},
+    ),
+    dict(
+        paths={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+        rev2="HEAD",
+        expect={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+    ),
+    dict(
+        paths={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+        rev2=":WORKTREE:",
+        expect={"x/dir", "x/dir/a.py", "x/dir/sub", "x/dir/sub/b.py"},
+    ),
+    dict(
+        paths={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+        cwd="x",
+        rev2="{add}",
+        expect=set(),
+    ),
+    dict(
+        paths={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+        cwd="x",
+        rev2="{del_a}",
+        expect={"dir/a.py"},
+    ),
+    dict(
+        paths={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+        cwd="x",
+        rev2="HEAD",
+        expect={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+    ),
+    dict(
+        paths={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+        cwd="x",
+        rev2=":WORKTREE:",
+        expect={"dir", "dir/a.py", "dir/sub", "dir/sub/b.py"},
+    ),
+    cwd=".",
+    git_cwd=".",
 )
-def test_get_missing_at_revision(git_repo, rev2, expect):
+def test_get_missing_at_revision(
+    git_repo, monkeypatch, paths, cwd, git_cwd, rev2, expect
+):
     """``get_missing_at_revision()`` returns missing files/directories correctly"""
-    git_repo.add({"dir/a.py": "", "dir/b.py": ""}, commit="Add dir/*.py")
+    git_repo.add(
+        {"x/README": "", "x/dir/a.py": "", "x/dir/sub/b.py": ""},
+        commit="Add x/dir/**/*.py",
+    )
     add = git_repo.get_hash()
-    git_repo.add({"dir/a.py": None}, commit="Delete dir/a.py")
+    git_repo.add({"x/dir/a.py": None}, commit="Delete x/dir/a.py")
     del_a = git_repo.get_hash()
-    git_repo.add({"dir/b.py": None}, commit="Delete dir/b.py")
+    git_repo.add({"x/dir/sub/b.py": None}, commit="Delete x/dir/sub/b.py")
+    monkeypatch.chdir(git_repo.root / cwd)
 
     result = git.get_missing_at_revision(
-        {Path("dir"), Path("dir/a.py"), Path("dir/b.py")},
+        {Path(p) for p in paths},
         rev2.format(add=add, del_a=del_a),
-        git_repo.root,
+        git_repo.root / git_cwd,
     )
 
-    assert result == expect
+    assert result == {Path(p) for p in expect}
 
 
 def test_get_missing_at_revision_worktree(git_repo):
     """``get_missing_at_revision()`` returns missing work tree files/dirs correctly"""
     paths = git_repo.add({"dir/a.py": "", "dir/b.py": ""}, commit="Add dir/*.py")
     paths["dir/a.py"].unlink()
     paths["dir/b.py"].unlink()
@@ -220,15 +291,15 @@
             absolute_path.unlink()
         else:
             absolute_path.parent.mkdir(parents=True, exist_ok=True)
             absolute_path.write_bytes(content.encode("ascii"))
     revrange = RevisionRange("HEAD", ":WORKTREE:")
 
     result = git.git_get_modified_python_files(
-        {root / p for p in paths}, revrange, cwd=root
+        {root / p for p in paths}, revrange, repo_root=root
     )
 
     assert result == {Path(p) for p in expect}
 
 
 @pytest.mark.kwparametrize(
     dict(
```

### Comparing `darker-2.1.0/src/darker/tests/test_import_sorting.py` & `darker-2.1.1/src/darker/tests/test_import_sorting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Tests for :mod:`darker.import_sorting`"""
 
 # pylint: disable=unused-argument,protected-access,too-many-arguments,use-dict-literal
 
 from importlib import reload
 from pathlib import Path
 from textwrap import dedent
+from typing import Any, Dict, Optional
 
 import pytest
 
 import darker.import_sorting
 from darker.git import EditedLinenumsDiffer
 from darker.tests.helpers import isort_present
 from darkgraylib.git import RevisionRange
+from darkgraylib.testtools.git_repo_plugin import GitRepoFixture
 from darkgraylib.utils import TextDocument, joinlines
 
 ORIGINAL_SOURCE = ("import sys", "import os", "", "print(42)")
 ISORTED_SOURCE = ("import os", "import sys", "", "print(42)")
 
 pytestmark = pytest.mark.usefixtures("find_project_root_cache_clear")
 
@@ -167,15 +169,21 @@
         expect={"settings_file": "myconfig.toml"},
     ),
     dict(line_length=42, expect={"settings_path": "{cwd}", "line_length": 42}),
     src=Path("file.py"),
     config=None,
     line_length=None,
 )
-def test_build_isort_args(src, config, line_length, expect):
+def test_build_isort_args(
+    git_repo: GitRepoFixture,
+    src: Path,
+    config: Optional[str],
+    line_length: int,
+    expect: Dict[str, Any],
+) -> None:
     """``_build_isort_args`` returns correct arguments for isort"""
     result = darker.import_sorting._build_isort_args(src, config, line_length)
 
     if "settings_path" in expect:
         expect["settings_path"] = str(expect["settings_path"].format(cwd=Path.cwd()))
     assert result == expect
```

### Comparing `darker-2.1.0/src/darker/tests/test_main.py` & `darker-2.1.1/src/darker/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_main_blacken_and_flynt_single_file.py` & `darker-2.1.1/src/darker/tests/test_main_blacken_and_flynt_single_file.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_main_revision.py` & `darker-2.1.1/src/darker/tests/test_main_revision.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_main_stdin_filename.py` & `darker-2.1.1/src/darker/tests/test_main_stdin_filename.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_multiline_strings.py` & `darker-2.1.1/src/darker/tests/test_multiline_strings.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_utils.py` & `darker-2.1.1/src/darker/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/tests/test_verification.py` & `darker-2.1.1/src/darker/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/utils.py` & `darker-2.1.1/src/darker/utils.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker/verification.py` & `darker-2.1.1/src/darker/verification.py`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker.egg-info/PKG-INFO` & `darker-2.1.1/src/darker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darker
-Version: 2.1.0
+Version: 2.1.1
 Summary: Apply Black formatting only in regions changed since last commit
 Home-page: https://github.com/akaihola/darker
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darker
 Project-URL: Change Log, https://github.com/akaihola/darker/blob/master/CHANGES.rst
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: black>=22.3.0
-Requires-Dist: darkgraylib~=1.1.1
-Requires-Dist: graylint~=1.0.1
+Requires-Dist: darkgraylib~=1.2.0
+Requires-Dist: graylint~=1.1.1
 Requires-Dist: toml>=0.10.0
 Provides-Extra: flynt
 Requires-Dist: flynt>=0.76; extra == "flynt"
 Provides-Extra: isort
 Requires-Dist: isort>=5.0.1; extra == "isort"
 Provides-Extra: color
 Requires-Dist: Pygments>=2.4.0; extra == "color"
@@ -49,47 +49,43 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 =================================================
  Darker – reformat and lint modified Python code
 =================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darker/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/darker/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darker/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/darker/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darker
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darker/
+   :target: https://pypi.org/project/darker/
 .. |downloads-badge| image:: https://pepy.tech/badge/darker
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darker
+   :target: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/24?color=red&label=release%202.1.1
+   :target: https://github.com/akaihola/darker/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/25?color=red&label=release%202.1.2
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/24
+   :target: https://github.com/akaihola/darker/milestone/24
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -180,19 +176,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=2.1.0
+  pip install --upgrade darker~=2.1.1
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=2.1.0 isort
+  conda install -c conda-forge darker~=2.1.1 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -410,30 +406,41 @@
        binary, or a full quoted command line with the command and options. Linters read
        their configuration as normally, and aren't affected by ``-c`` / ``--config``.
        Linter output is syntax highlighted when the ``pygments`` package is available if
        run on a terminal and or enabled by explicitly (see ``--color``).
 -S, --skip-string-normalization
        Don't normalize string quotes or prefixes
 --no-skip-string-normalization
-       Normalize string quotes or prefixes. This can be used to override
-       ``skip_string_normalization = true`` from a configuration file.
+       Normalize string quotes or prefixes. This can be used to override ``skip-string-
+       normalization = true`` from a Black configuration file.
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
-       to override ``skip_magic_trailing_comma = true`` from a configuration file.
+       to override ``skip-magic-trailing-comma = true`` from a Black configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
        [py33\|py34\|py35\|py36\|py37\|py38\|py39\|py310\|py311\|py312] Python versions
        that should be supported by Black's output. [default: per-file auto-detection]
 
 To change default values for these options for a given project,
-add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
-project's root directory, or to a different TOML file specified using the ``-c`` /
-``--config`` option. For example:
+add a ``[tool.darker]`` section to ``pyproject.toml`` in the project's root directory,
+or to a different TOML file specified using the ``-c`` / ``--config`` option.
+
+You should configure invoked tools like Black_, isort_ and flynt_
+using their own configuration files.
+
+As an exception, the ``line-length`` and ``target-version`` options in ``[tool.darker]``
+can be used to override corresponding options for individual tools.
+
+Note that Black_ honors only the options listed in the below example
+when called by ``darker``, because ``darker`` reads the Black configuration
+and passes it on when invoking Black_ directly through its Python API.
+
+An example ``pyproject.toml`` configuration file:
 
 .. code-block:: toml
 
    [tool.darker]
    src = [
        "src/mypackage",
    ]
@@ -442,34 +449,31 @@
    check = true
    isort = true
    flynt = true
    lint = [
        "pylint",
    ]
    line-length = 80                  # Passed to isort and Black, override their config
+   target-version = ["py312"]        # Passed to Black, overriding its config
    log_level = "INFO"
 
    [tool.black]
    line-length = 88                  # Overridden by [tool.darker] above
    skip-magic-trailing-comma = false
    skip-string-normalization = false
-   target-version = ["py38", "py39", "py310", "py311", "py312"]
+   target-version = ["py38", "py39", "py310", "py311", "py312"]  # Overridden above
    exclude = "test_*\.py"
    extend_exclude = "/generated/"
    force_exclude = ".*\.pyi"
 
    [tool.isort]
    profile = "black"
    known_third_party = ["pytest"]
    line_length = 88                  # Overridden by [tool.darker] above
 
-While isort_ reads all of its options from the configuration file, Black_ only honors
-the ones listed above when called by ``darker``. Other tools are invoked as
-subprocesses and use their configuration mechanisms unmodified.
-
 Be careful to not use options which generate output which is unexpected for
 other tools. For example, VSCode only expects the reformat diff, so
 ``lint = [ ... ]`` can't be used with it.
 
 *New in version 1.0.0:*
 
 - The ``-c``, ``-S`` and ``-l`` command line options.
@@ -496,14 +500,17 @@
 *New in version 1.5.0:* The ``-W`` / ``--workers``, ``--color`` and ``--no-color``
 command line options
 
 *New in version 1.7.0:* The ``-t`` / ``--target-version`` command line option
 
 *New in version 1.7.0:* The ``-f`` / ``--flynt`` command line option
 
+*New in version 2.1.1:* In ``[tool.darker]``, deprecate the the Black options
+``skip_string_normalization`` and ``skip_magic_trailing_comma``
+
 .. _Black documentation about pyproject.toml: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
 .. _isort documentation about config files: https://timothycrosley.github.io/isort/docs/configuration/config_files/
 .. _public GitHub repositories which install and run Darker: https://github.com/search?q=%2Fpip+install+.*darker%2F+path%3A%2F%5E.github%5C%2Fworkflows%5C%2F.*%2F&type=code
 .. _flynt documentation about configuration files: https://github.com/ikamensh/flynt#configuration-files
 .. _command line arguments: https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#command-line-options
 
 Editor integration
@@ -592,23 +599,29 @@
      /usr/local/bin/darker  # possible location
 
    On Windows::
 
      $ where darker
      %LocalAppData%\Programs\Python\Python36-32\Scripts\darker.exe  # possible location
 
-3. Add these configuration options to VS code, ``Cmd-Shift-P``, ``Open Settings (JSON)``::
+3. Make sure you have the `VSCode black-formatter extension`__ installed.
+
+__ https://github.com/microsoft/vscode-black-formatter
+
+4. Add these configuration options to VSCode
+   (``⌘ Command / Ctrl`` + ``⇧ Shift`` + ``P``
+   and select ``Open Settings (JSON)``)::
 
-    "python.formatting.provider": "black",
-    "python.formatting.blackPath": "<install_location_from_step_2>",
-    "python.formatting.blackArgs": [],
+    "python.editor.defaultFormatter": "ms-python.black-formatter",
+    "black-formatter.path": "<install_location_from_step_2>",
+    "black-formatter.args": ["-d"],
 
 VSCode will always add ``--diff --quiet`` as arguments to Darker,
-but you can also pass additional arguments in the ``blackArgs`` option
-(e.g. ``["--isort", "--revision=master..."]``).
+but you can also pass additional arguments in the ``black-formatter.args`` option
+(e.g. ``["-d", "--isort", "--revision=master..."]``).
 Be sure to *not* enable any linters here or in ``pyproject.toml``
 since VSCode won't be able to understand output from them.
 
 Note that VSCode first copies the file to reformat into a temporary
 ``<filename>.py.<hash>.tmp`` file, then calls Black (or Darker in this case) on that
 file, and brings the changes in the modified files back into the editor.
 Darker is aware of this behavior, and will correctly compare ``.py.<hash>.tmp`` files
@@ -682,15 +695,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: v2.1.0
+        rev: v2.1.1
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -701,15 +714,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args:
            - --isort
            - --lint
            - mypy
            - --lint
@@ -732,15 +745,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: v2.1.0
+     rev: v2.1.1
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -777,19 +790,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/darker@2.1.0
+         - uses: akaihola/darker@2.1.1
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=2.1.0"
+             version: "~=2.1.1"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
```

### Comparing `darker-2.1.0/src/darker.egg-info/SOURCES.txt` & `darker-2.1.1/src/darker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `darker-2.1.0/src/darker.egg-info/requires.txt` & `darker-2.1.1/src/darker.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 black>=22.3.0
-darkgraylib~=1.1.1
-graylint~=1.0.1
+darkgraylib~=1.2.0
+graylint~=1.1.1
 toml>=0.10.0
 
 [color]
 Pygments>=2.4.0
 
 [flynt]
 flynt>=0.76
 
 [isort]
 isort>=5.0.1
 
 [release]
-airium>=0.2.3
-click>=8.0.0
-darkgray-dev-tools~=0.0.1
-defusedxml>=0.7.1
-requests_cache>=0.7
+darkgray-dev-tools~=0.0.2
 
 [test]
 airium>=0.2.3
 black>=22.3.0
 cryptography>=3.3.2
 defusedxml>=0.7.1
 flynt>=0.76
```

