# Comparing `tmp/cace-2.1.9.tar.gz` & `tmp/cace-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.1.9.tar", last modified: Fri Mar 15 16:00:12 2024, max compression
+gzip compressed data, was "cace-2.2.0.tar", last modified: Tue Apr 16 18:35:31 2024, max compression
```

## Comparing `cace-2.1.9.tar` & `cace-2.2.0.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.073902 cace-2.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.077902 cace-2.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-15 15:59:50.000000 cace-2.1.9/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-15 15:59:50.000000 cace-2.1.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-15 15:59:50.000000 cace-2.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-15 15:59:50.000000 cace-2.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-15 15:59:50.000000 cace-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-15 15:59:50.000000 cace-2.1.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 16:00:12.089902 cace-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-15 15:59:50.000000 cace-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.077902 cace-2.1.9/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24829 2024-03-15 15:59:50.000000 cace-2.1.9/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    80400 2024-03-15 15:59:50.000000 cace-2.1.9/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.081902 cace-2.1.9/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26066 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14386 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14647 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10773 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47991 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8701 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    52969 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/netlist_precheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.081902 cace-2.1.9/cace/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-15 15:59:50.000000 cace-2.1.9/cace/doc/characterize_help.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25405 2024-03-15 15:59:50.000000 cace-2.1.9/cace/doc/format.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29537 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27947 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9775 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5747 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16358 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/simhints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 15:59:50.000000 cace-2.1.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 15:59:50.000000 cace-2.1.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22353 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-15 15:59:50.000000 cace-2.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 15:59:50.000000 cace-2.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-15 15:59:50.000000 cace-2.1.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-15 15:59:50.000000 cace-2.1.9/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 16:00:12.089902 cace-2.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 15:59:50.000000 cace-2.1.9/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 15:59:50.000000 cace-2.1.9/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.565713 cace-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.569712 cace-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-16 18:35:07.000000 cace-2.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-16 18:35:07.000000 cace-2.2.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 18:35:07.000000 cace-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-16 18:35:07.000000 cace-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 18:35:07.000000 cace-2.2.0/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 18:35:07.000000 cace-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 18:35:07.000000 cace-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-16 18:35:31.581713 cace-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-16 18:35:07.000000 cace-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.569712 cace-2.2.0/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-16 18:35:07.000000 cace-2.2.0/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-16 18:35:07.000000 cace-2.2.0/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 18:35:07.000000 cace-2.2.0/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-16 18:35:07.000000 cace-2.2.0/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45016 2024-04-16 18:35:07.000000 cace-2.2.0/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.573713 cace-2.2.0/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7231 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2451 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14650 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19173 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-16 18:35:07.000000 cace-2.2.0/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.577713 cace-2.2.0/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-16 18:35:07.000000 cace-2.2.0/cace/gui/tooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 18:35:31.000000 cace-2.2.0/cace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.577713 cace-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-16 18:35:07.000000 cace-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 18:35:07.000000 cace-2.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.577713 cace-2.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.577713 cace-2.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 18:35:07.000000 cace-2.2.0/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 18:35:07.000000 cace-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 18:35:07.000000 cace-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 18:35:07.000000 cace-2.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 18:35:07.000000 cace-2.2.0/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:35:31.581713 cace-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:31.581713 cace-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 18:35:07.000000 cace-2.2.0/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 18:35:07.000000 cace-2.2.0/tests/test1.py
```

### Comparing `cace-2.1.9/.github/workflows/ci.yaml` & `cace-2.2.0/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         run: |
           make build
       - name: Install Package
         run: |
           make install
       - name: Run CACE
         run: |
-          cace -help
+          cace --help
 
   docs:
     runs-on: ubuntu-22.04
     needs: [lint]
     name: Build Documentation
     steps:
       - name: Check out repo
```

### Comparing `cace-2.1.9/.github/workflows/pypi.yaml` & `cace-2.2.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/.readthedocs.yaml` & `cace-2.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/LICENSE` & `cace-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/Makefile` & `cace-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/PKG-INFO` & `cace-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.1.9
+Version: 2.2.0
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -42,14 +42,18 @@
 	$ python3 -m pip install --upgrade cace
 Prerequisite design tools:
 
 - xschem:  [https://github.com/stefanschippers/xschem](https://github.com/stefanschippers/xschem)
 - ngspice: git://git.code.sf.net/p/ngspice/ngspice
 - magic:	 [https://github.com/RTimothyEdwards/magic](https://github.com/RTimothyEdwards/magic)
 
+Some of the measurements require:
+
+- octave: [https://octave.org/](https://octave.org/)
+
 ## Usage
 
 If installed as Python package, CACE can be started from the command line using:
 
 ```
 $ cace
 ```
@@ -100,21 +104,21 @@
 ```
 $ make docs
 ```
 
 To host the docs, run:
 
 ```
-make host-docs
+$ make host-docs
 ```
 
 To automatically refresh the docs upon changes, run:
 
 ```
-make auto-docs
+$ make auto-docs
 ```
 
 > [!NOTE]
 > The latest documentation can be viewed online at [cace.readthedocs.io](https://cace.readthedocs.io/). 
 
 ## Examples
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.1.9 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.0 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
@@ -17,26 +17,27 @@
 testbenches and analysis scripts to characterize a circuit and to produce a
 datasheet showing the circuit performance. ## Installation You'll need the
 following: - Python 3.8 or higher with PIP and Tkinter CACE can be installed
 directly from PyPI: $ python3 -m pip install --upgrade cace Prerequisite design
 tools: - xschem: [https://github.com/stefanschippers/xschem](https://
 github.com/stefanschippers/xschem) - ngspice: git://git.code.sf.net/p/ngspice/
 ngspice - magic: [https://github.com/RTimothyEdwards/magic](https://github.com/
-RTimothyEdwards/magic) ## Usage If installed as Python package, CACE can be
-started from the command line using: ``` $ cace ``` Or to start the GUI: ``` $
-cace-gui ``` Information on how to use CACE can be found in the documentation
-at [cace.readthedocs.io](https://cace.readthedocs.io/). ## Development ###
-Dependencies > [!IMPORTANT] > You may need to set up a Python [virtual
-environment](https://docs.python.org/3/library/venv.html). To install the
-dependencies for CACE, run: $ make dependencies ### Python Package To build the
-Python package, run: ``` $ make build ``` To install the package, run: ``` $
-make install ``` To install the package in editable mode, run: ``` $ make
+RTimothyEdwards/magic) Some of the measurements require: - octave: [https://
+octave.org/](https://octave.org/) ## Usage If installed as Python package, CACE
+can be started from the command line using: ``` $ cace ``` Or to start the GUI:
+``` $ cace-gui ``` Information on how to use CACE can be found in the
+documentation at [cace.readthedocs.io](https://cace.readthedocs.io/). ##
+Development ### Dependencies > [!IMPORTANT] > You may need to set up a Python
+[virtual environment](https://docs.python.org/3/library/venv.html). To install
+the dependencies for CACE, run: $ make dependencies ### Python Package To build
+the Python package, run: ``` $ make build ``` To install the package, run: ```
+$ make install ``` To install the package in editable mode, run: ``` $ make
 editable ``` ### Documentation To build the documentation, run: ``` $ make docs
-``` To host the docs, run: ``` make host-docs ``` To automatically refresh the
-docs upon changes, run: ``` make auto-docs ``` > [!NOTE] > The latest
+``` To host the docs, run: ``` $ make host-docs ``` To automatically refresh
+the docs upon changes, run: ``` $ make auto-docs ``` > [!NOTE] > The latest
 documentation can be viewed online at [cace.readthedocs.io](https://
 cace.readthedocs.io/). ## Examples The following repositories contain example
 circuit designs, each having a "cace/" subdirectory with a specification input
 file in the format described below, and a set of testbench schematics which are
 used by CACE to measure all specified electrical and physical parameters,
 generate results, and analyze them to determine circuit performance over
 corners. > [!NOTE] > Example repositories, like CACE itself, are currently a
```

### Comparing `cace-2.1.9/README.md` & `cace-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 	$ python3 -m pip install --upgrade cace
 Prerequisite design tools:
 
 - xschem:  [https://github.com/stefanschippers/xschem](https://github.com/stefanschippers/xschem)
 - ngspice: git://git.code.sf.net/p/ngspice/ngspice
 - magic:	 [https://github.com/RTimothyEdwards/magic](https://github.com/RTimothyEdwards/magic)
 
+Some of the measurements require:
+
+- octave: [https://octave.org/](https://octave.org/)
+
 ## Usage
 
 If installed as Python package, CACE can be started from the command line using:
 
 ```
 $ cace
 ```
@@ -83,21 +87,21 @@
 ```
 $ make docs
 ```
 
 To host the docs, run:
 
 ```
-make host-docs
+$ make host-docs
 ```
 
 To automatically refresh the docs upon changes, run:
 
 ```
-make auto-docs
+$ make auto-docs
 ```
 
 > [!NOTE]
 > The latest documentation can be viewed online at [cace.readthedocs.io](https://cace.readthedocs.io/). 
 
 ## Examples
```

#### html2text {}

```diff
@@ -8,26 +8,27 @@
 testbenches and analysis scripts to characterize a circuit and to produce a
 datasheet showing the circuit performance. ## Installation You'll need the
 following: - Python 3.8 or higher with PIP and Tkinter CACE can be installed
 directly from PyPI: $ python3 -m pip install --upgrade cace Prerequisite design
 tools: - xschem: [https://github.com/stefanschippers/xschem](https://
 github.com/stefanschippers/xschem) - ngspice: git://git.code.sf.net/p/ngspice/
 ngspice - magic: [https://github.com/RTimothyEdwards/magic](https://github.com/
-RTimothyEdwards/magic) ## Usage If installed as Python package, CACE can be
-started from the command line using: ``` $ cace ``` Or to start the GUI: ``` $
-cace-gui ``` Information on how to use CACE can be found in the documentation
-at [cace.readthedocs.io](https://cace.readthedocs.io/). ## Development ###
-Dependencies > [!IMPORTANT] > You may need to set up a Python [virtual
-environment](https://docs.python.org/3/library/venv.html). To install the
-dependencies for CACE, run: $ make dependencies ### Python Package To build the
-Python package, run: ``` $ make build ``` To install the package, run: ``` $
-make install ``` To install the package in editable mode, run: ``` $ make
+RTimothyEdwards/magic) Some of the measurements require: - octave: [https://
+octave.org/](https://octave.org/) ## Usage If installed as Python package, CACE
+can be started from the command line using: ``` $ cace ``` Or to start the GUI:
+``` $ cace-gui ``` Information on how to use CACE can be found in the
+documentation at [cace.readthedocs.io](https://cace.readthedocs.io/). ##
+Development ### Dependencies > [!IMPORTANT] > You may need to set up a Python
+[virtual environment](https://docs.python.org/3/library/venv.html). To install
+the dependencies for CACE, run: $ make dependencies ### Python Package To build
+the Python package, run: ``` $ make build ``` To install the package, run: ```
+$ make install ``` To install the package in editable mode, run: ``` $ make
 editable ``` ### Documentation To build the documentation, run: ``` $ make docs
-``` To host the docs, run: ``` make host-docs ``` To automatically refresh the
-docs upon changes, run: ``` make auto-docs ``` > [!NOTE] > The latest
+``` To host the docs, run: ``` $ make host-docs ``` To automatically refresh
+the docs upon changes, run: ``` $ make auto-docs ``` > [!NOTE] > The latest
 documentation can be viewed online at [cace.readthedocs.io](https://
 cace.readthedocs.io/). ## Examples The following repositories contain example
 circuit designs, each having a "cace/" subdirectory with a specification input
 file in the format described below, and a set of testbench schematics which are
 used by CACE to measure all specified electrical and physical parameters,
 generate results, and analyze them to determine circuit performance over
 corners. > [!NOTE] > Example repositories, like CACE itself, are currently a
```

### Comparing `cace-2.1.9/cace/__init__.py` & `cace-2.2.0/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/__main__.py` & `cace-2.2.0/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/__version__.py` & `cace-2.2.0/cace/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.1.9'
+__version__ = '2.2.0'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.1.9/cace/cace_cli.py` & `cace-2.2.0/cace/common/cace_collate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,726 +1,679 @@
 #!/usr/bin/env python3
+# --------------------------------------------------------------------------
+# cace_collate.py
+# --------------------------------------------------------------------------
+#
+# This script follows cace_measure by taking the collection of output
+# results generated for each set of conditions by the simulation and
+# following measurements, calculating minimum/typical/maximum values
+# for the set, and using the results to annotate the original
+# characterization dataset.
 #
-# --------------------------------------------------------
-# Circuit Automatic Characterization Engine (CACE) system
-# cace.py ---
-# Read a text file in CACE (ASCII) format 4.0, run
-# all simulations and analysis on electrical and physical
-# parameters, as appropriate, and write out a modified
-# file with simulation and analysis results.
-#
-# --------------------------------------------------------
-# Written by Tim Edwards
-# Efabless Corporation
-# November 22, 2023
-# For CACE version 4.0
-# --------------------------------------------------------
+# --------------------------------------------------------------------------
 
 import os
 import sys
+import shutil
 import json
-import signal
+import re
+import math
+import subprocess
+
+from .spiceunits import spice_unit_unconvert
+from .spiceunits import spice_unit_convert
+
+from .cace_calculate import twos_complement
+
+# ---------------------------------------------------------------------------
+# find_limits ---
+#
+# Calculation of results from collected data for an output record, given
+# the type of calculation to perform in 'calctype'.  The primary calculations
+# are minimum, maximum, and typical, although these definitions are nuanced
+# and the actual calculation performed is provided as a parameter.
+#
+# Future development:
+# Add "minimax", "maximin", and "typical" to calctypes (needs extra record(s))
+# Add "range" to limittypes (needs extra record or tuple for target)
+#
+#    "spectype" is one of "minimum", "maximum", or "typical".
+#    "spec" is the list value of spectype in a parameter's "spec" dictionary.
+# 	This is a numerical value that is the spec target, optionally followed
+# 	by "pass" or "fail", where "fail" implies that exceeding the value is
+# 	a failure to meet spec; and optionally followed by "calctype"-"limittype":
+# 	"calctype" is one of:  average, minimum, maximum
+# 	"limittype" is one of: above, below, exact
+#    "results" is a list of rsult values
+#    "units" is the units type (string) of the result value.
+#
+# The return value is a list in the same format as "spec" but where the
+# first entry is the measured result, the second entry is the score
+# ("pass" or "fail"), and there is no third entry.
+#
+# ---------------------------------------------------------------------------
+
+
+def find_limits(spectype, spec, results, units, debug=False):
+
+    # 'spec' is a list of [value, pass|fail, calculation-limit], but
+    # if only "value" is present it may be interpreted as a string.
+
+    if isinstance(spec, list):
+        target = spec[0]
+        penalty = spec[1] if len(spec) > 1 else 'pass'
+        calcrec = spec[2] if len(spec) > 2 else spectype
+    elif isinstance(spec, str):
+        target = spec
+        penalty = 'pass'
+        calcrec = spectype
+
+    # Prepare a list to return
+    specresult = []
+
+    binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
+
+    # Note:
+    # calctype = "minimum" alone implies "minimum-above"
+    # calctype = "maximum" alone implies "maximum-below"
+    # calctype = "average" alone implies "average-exact"
+    # calctype = "typical" alone implies "average-exact"
+
+    if debug:
+        print('Diagnostic:  find_limits')
+        print('spectype = ' + spectype)
+        print('spec = ' + str(spec))
+        print('results = ' + str(results))
+        print('units = ' + units)
+        print('target = ' + target)
+        print('penalty = ' + penalty)
+        print('calcrec = ' + calcrec)
 
-from .common.cace_read import *
-from .common.cace_compat import *
-from .common.cace_write import *
-from .common.cace_gensim import *
-from .common.cace_launch import *
-from .common.cace_collate import *
-from .common.cace_evaluate import *
-from .common.cace_regenerate import *
-from .common.cace_makeplot import *
-
-import multiprocessing.pool
-
-# -----------------------------------------------------------------------------
-# Create a multiprocessing class that can be nested
-# Solution pulled from discussion at:
-# https://stackoverflow.com/questions/6974695/python-process-pool-non-daemonic
-# -----------------------------------------------------------------------------
-
-
-class NoDaemonProcess(multiprocessing.Process):
-    @property
-    def daemon(self):
-        return False
-
-    @daemon.setter
-    def daemon(self, value):
-        pass
-
-
-class NoDaemonContext(type(multiprocessing.get_context())):
-    Process = NoDaemonProcess
-
-
-# We sub-class multiprocessing.pool.Pool instead of multiprocessing.Pool
-# because the latter is only a wrapper function, not a proper class.
-class NestablePool(multiprocessing.pool.Pool):
-    def __init__(self, *args, **kwargs):
-        kwargs['context'] = NoDaemonContext()
-        super(NestablePool, self).__init__(*args, **kwargs)
-
-
-# -----------------------------------------------------------------
-# Exit the child process when SIGUSR1 is given to the process
-# -----------------------------------------------------------------
-
-
-def child_process_exit(signum, frame):
-    print('CACE:  Received forced stop.')
     try:
-        multiprocessing.current_process().terminate()
-    except AttributeError:
-        print('Terminate failed; Child PID is ' + str(os.getpid()))
-        print('Waiting on process to finish.')
-
-
-# -----------------------------------------------------------------
-# cace_run_eparam
-#
-# Run complete characterization of a single electrical parameter
-#
-# Electrical parameter evaluation is a three-step process.  First,
-# generate all of the simulation netlists to simulate.  Then,
-# run all the simulations.  Finally, collect the simulation results
-# and create plots and/or determine parameter performance limits.
-#
-# "datasheet" is the CACE characterization dataset
-# "eparam" is the dictionary of a single electrical parameter
-# -----------------------------------------------------------------
-
-
-def cace_run_eparam(datasheet, eparam):
-
-    # Quick check for skipped or blocked parameter.
-    if 'status' in eparam:
-        status = eparam['status']
-        if status == 'skip' or status == 'blocked':
-            return eparam
-
-    noplot = False
-    if 'runtime_options' in datasheet:
-        runtime_options = datasheet['runtime_options']
-        if 'noplot' in runtime_options:
-            noplot = True
-        if 'pid' in runtime_options:
-            os.setpgid(os.getpid(), runtime_options['pid'])
-            signal.signal(signal.SIGUSR1, child_process_exit)
-
-    needplot = True if 'plot' in eparam else False
-    needcollate = True if 'spec' in eparam else False
-
-    eparamname = eparam['name']
-    print('Evaluating electrical parameter ' + eparamname)
-    cace_gensim(datasheet, eparam)
-
-    print('Launching Simulations')
-    cace_launch(datasheet, eparam)
-
-    if needplot:
-        print('Plotting results')
-        cace_makeplot(datasheet, eparam)
-
-    if needcollate:
-        print('Collating results')
-        eparam = cace_collate(datasheet, eparam)
-
-    return eparam
-
-
-# -----------------------------------------------------------------------
-# cace_run_pparam
-#
-# Physical parameter evaluation is done by running scripts which do
-# the task of running a tool to perform some calculation on the physical
-# design, such as area measurement, DRC, or LVS.
-#
-# "datasheet" is the CACE characterization dataset
-# "pparam" is the dictionary of a single physical parameter
-# -----------------------------------------------------------------------
+        calctype, limittype = calcrec.split('-')
+    except ValueError:
+        calctype = calcrec
+        if calctype == 'minimum':
+            limittype = 'above'
+        elif calctype == 'maximum':
+            limittype = 'below'
+        elif calctype == 'average':
+            limittype = 'exact'
+        elif calctype == 'typical':
+            limittype = 'exact'
+        elif calctype == 'diffmin':
+            limittype = 'above'
+        elif calctype == 'diffmax':
+            limittype = 'below'
+        else:
+            # Diagnostic:
+            print('Failure:  Unknown calculation type ' + calctype)
+            return ['failure', 'fail']
+
+    # Quick format sanity check---may need binary or hex conversion
+    # using the units nomenclature of 'b or 'h, etc.
+    # (to be done:  signed conversion, see cace_makeplot.py)
+
+    if isinstance(results[0], str):
+        bmatch = binrex.match(units)
+        if bmatch:
+            digits = bmatch.group(1)
+            if digits == '':
+                digits = len(results[0])
+            else:
+                digits = int(digits)
+            base = bmatch.group(2)
+            if base == 'b':
+                a = list(int(x, 2) for x in results)
+            elif base == 'o':
+                a = list(int(x, 8) for x in results)
+            elif base == 'd':
+                a = list(int(x, 10) for x in results)
+            else:
+                a = list(int(x, 16) for x in results)
+            results = list(twos_complement(x, digits) for x in a)
+        elif results[0] != 'failure':
+            print('Warning: result data do not correspond to specified units.')
+            print('Data = ' + str(results))
+            return ['failure', 'fail']
+
+    # The target and result should both match the specified units, so convert
+    # the target if it is a binary, hex, etc., value.
+    if target != 'any':
+        targval = target
+        bmatch = binrex.match(units)
+        if bmatch:
+            digits = bmatch.group(1)
+            base = bmatch.group(2)
+            if digits == '':
+                digits = len(targval)
+            else:
+                digits = int(digits)
+            try:
+                if base == 'b':
+                    a = int(targval, 2)
+                elif base == 'o':
+                    a = int(targval, 8)
+                elif base == 'd':
+                    a = int(targval, 10)
+                else:
+                    a = int(targval, 16)
+                targval = twos_complement(a, digits)
+            except:
+                print(
+                    'Warning: target data do not correspond to units; assuming integer.'
+                )
 
+    # First run the calculation to get the single result value
 
-def cace_run_pparam(datasheet, pparam):
+    if calctype == 'minimum':
+        # Result is the minimum of the data
+        value = min(results)
+    elif calctype == 'maximum':
+        # Result is the maximum of the data
+        value = max(results)
+    elif calctype == 'average' or calctype == 'typical':
+        # Result is the average of the data
+        value = sum(results) / len(results)
+    elif calctype[0:3] == 'std':
+        # Result is the standard deviation of the data
+        mean = sum(results) / len(results)
+        value = pow(
+            sum([((i - mean) * (i - mean)) for i in results]) / len(results),
+            0.5,
+        )
+        # For "stdX", where "X" is an integer, multiply the standard deviation by X
+        if len(calctype) > 3:
+            value *= int(calctype[3])
+
+        if len(calctype) > 4:
+            # For "stdXn", subtract X times the standard deviation from the mean
+            if calctype[4] == 'n':
+                value = mean - value
+            # For "stdXp", add X times the standard deviation to the mean
+            elif calctype[4] == 'p':
+                value = mean + value
+    elif calctype == 'diffmax':
+        value = max(results) - min(results)
+    elif calctype == 'diffmin':
+        value = min(results) - max(results)
+    else:
+        return ['failure', 'fail']
 
-    # Quick check for skipped or blocked parameter.
-    if 'status' in pparam:
-        status = pparam['status']
-        if status == 'skip' or status == 'blocked':
-            return pparam
+    try:
+        specresult.append('{0:.4g}'.format(value))
+    except ValueError:
+        print(
+            'Warning: Min/Typ/Max value is not not numeric; value is '
+            + str(value)
+        )
+        return ['failure', 'fail']
+
+    # Next calculate the score based on the limit type
+
+    score = 'pass'
+    if limittype == 'above':
+        # Score a penalty if value is below the target
+        if target != 'any' and penalty == 'fail':
+            targval = float(target)
 
-    if 'runtime_options' in datasheet:
-        runtime_options = datasheet['runtime_options']
-        if 'pid' in runtime_options:
-            os.setpgid(os.getpid(), runtime_options['pid'])
-            signal.signal(signal.SIGUSR1, child_process_exit)
+            if debug:
+                print('minimum = ' + str(value))
+            # NOTE: 0.0005 value corresponds to formatting above, so the
+            # value is not marked in error unless it would show a different
+            # value in the display.
+            if value < targval - 0.0005:
+                score = 'fail'
+                if debug:
+                    print('fail: target = ' + str(score) + '\n')
+            elif math.isnan(value):
+                score = 'fail'
+
+    elif limittype == 'below':
+        # Score a penalty if value is above the target
+        if target != 'any' and penalty == 'fail':
+            targval = float(target)
 
-    pparamname = pparam['name']
-    print('Evaluating physical parameter ' + pparamname)
-    return cace_evaluate(datasheet, pparam)
+            if debug:
+                print('maximum = ' + str(value))
+            # NOTE: 0.0005 value corresponds to formatting above, so the
+            # value is not marked in error unless it would show a different
+            # value in the display.
+            if value > targval + 0.0005:
+                score = 'fail'
+                if debug:
+                    print('fail: target = ' + str(score))
+            elif math.isnan(value):
+                score = 'fail'
+
+    elif limittype == 'exact':
+        # Score a penalty if value is not equal to the target
+        if target != 'any' and penalty == 'fail':
+            targval = float(target)
+
+            if value != targval:
+                score = 'fail'
+                if debug:
+                    print('off-target failure')
+            elif math.isnan(value):
+                score = 'fail'
+
+    # Note:  Calctype 'none' performs no calculation.  Record is unchanged,
+    # and "score" is returned unchanged.
+
+    specresult.append(score)
+    return specresult
+
+
+# ----------------------------------------------------------------------
+# incompleteresult --
+#
+# Handle errors where simulation generated no output.
+# This is the one case where 'typical' can be treated as pass-fail.
+# score will be set to "incomplete" for any of "minimum", "maximum",
+# and "typical" that exists in the electrical parameters record
+# and which specifies a target value.  "value" is set to "failure"
+# for display.
+# ----------------------------------------------------------------------
+
+
+def incompleteresult(param, noplotmode=False):
+
+    resultdict = {}
+
+    if 'plot' in param:
+        if noplotmode == False:
+            resultdict['status'] = 'incomplete'
+
+    if 'spec' not in param:
+        return resultdict
+
+    spec = param['spec']
+
+    if 'typical' in spec:
+        typrec = spec['typical']
+        typresult = ['failure']
+        if typrec[0] != 'any':
+            typresult.append('incomplete')
+        resultdict['typical'] = typresult
+
+    if 'maximum' in spec:
+        maxrec = spec['maximum']
+        maxresult = ['failure']
+        if maxrec[0] != 'any':
+            maxresult.append('incomplete')
+        resultdict['maximum'] = maxresult
+
+    if 'minimum' in spec:
+        minrec = spec['minimum']
+        minresult = ['failure']
+        if minrec[0] != 'any':
+            minresult.append('incomplete')
+        resultdict['minimum'] = minresult
+
+    return resultdict
+
+
+# -------------------------------------------------------------
+# addnewresult --
+#
+# If the result dictionary has the same name as one in the
+# datasheet, then it replaces it.  Otherwise it is appended
+# to the list.
+# -------------------------------------------------------------
+
+
+def addnewresult(param, resultdict):
+    replaced = False
+    if 'results' in param:
+        newresultlist = []
+        paramresults = param['results']
+        if not isinstance(paramresults, list):
+            paramresults = [paramresults]
+        for result in paramresults:
+            if result['name'] == resultdict['name']:
+                newresultlist.append(resultdict)
+                replaced = True
+            else:
+                newresultlist.append(result)
+        if replaced == False:
+            newresultlist.append(resultdict)
+        param['results'] = newresultlist
+    else:
+        param['results'] = resultdict
 
 
-# -----------------------------------------------------------------------
-# cace_run_all_eparams
+# ---------------------------------------------------------------------------
+# Main entry point of cace_collate
 #
-# Run all electrical parameters simulations and measurements.
-# This routine contains a nested multiprocessing pool.
+# "param" is an electrical parameter dictionary to be evaluated.
+# The "param" dictionary is annotated with results; and the modified
+# dictionary is returned.
 #
-# "datasheet" is the CACE characterization dataset
-# -----------------------------------------------------------------------
+# At the end of running all measurements, there should be a number of
+# "testbench" records for the parameter, each containing a unique set of
+# conditions, and a "results" section which is normally a single value
+# (see code comments about dealing with multiple values).
+# ---------------------------------------------------------------------------
 
 
-def cace_run_all_eparams(datasheet):
+def cace_collate(dsheet, param):
 
-    runtime_options = datasheet['runtime_options']
-    if 'pid' in runtime_options:
-        os.setpgid(os.getpid(), runtime_options['pid'])
-        signal.signal(signal.SIGUSR1, child_process_exit)
+    runtime_options = dsheet['runtime_options']
+    try:
+        debug = runtime_options['debug']
+    except:
+        debug = False
 
     try:
         keepmode = runtime_options['keep']
     except:
         keepmode = False
 
     try:
-        sequential = runtime_options['sequential']
+        noplotmode = runtime_options['noplot']
     except:
-        sequential = False
+        noplotmode = False
 
-    if sequential:
-        for eparam in datasheet['electrical_parameters']:
-            cace_run_eparam(datasheet, eparam)
+    if 'default_conditions' in dsheet:
+        default_conditions = dsheet['default_conditions']
     else:
-        alleparams = []
-        with NestablePool() as pool:
-            results = []
-            idx = 0
-            for eparam in datasheet['electrical_parameters']:
-                eparam['sequence'] = idx
-                results.append(
-                    pool.apply_async(
-                        cace_run_eparam,
-                        (datasheet, eparam),
-                    )
-                )
-                idx += 1
+        default_conditions = []
 
-            # Replace the electrical parameter list in the datasheet with the
-            # number of electrical parameters
-            datasheet['electrical_parameters'] = len(
-                datasheet['electrical_parameters']
-            )
-
-            for result in results:
-                try:
-                    presult = result.get(timeout=300)
-                except Exception as e:
-                    print('cace_run_eparam failed with exception:')
-                    print(e)
-                    presult = None
-                if presult:
-                    alleparams.append(presult)
-
-        # After joining forks, 'results' contains an unordered list of
-        # parameters.  Because the forks do not share memory, these
-        # parameters are no longer the same as the ones in the datasheet,
-        # so put everything back together here.
-
-        maxidx = datasheet['electrical_parameters']
-        datasheet['electrical_parameters'] = []
-        for idx in range(0, maxidx):
-            for param in alleparams:
-                if param['sequence'] == idx:
-                    datasheet['electrical_parameters'].append(param)
-                    break
-
-        for param in alleparams:
-            param.pop('sequence')
-
-    # Files to clean up that may have been generated
-    if os.path.exists('b3v32check.log'):
-        os.remove('b3v32check.log')
-
-    # Final cleanup step:  Remove any '.tv' files from the work area.
-    if keepmode == False:
-        paths = datasheet['paths']
-        root_path = paths['root']
-        simulation_path = paths['simulation']
+    total = 0
 
-        files = os.listdir(os.path.join(root_path, simulation_path))
-        for filename in files:
-            try:
-                fileext = os.path.splitext(filename)[1]
-            except:
-                pass
-            else:
-                if fileext == '.tv':
-                    os.remove(
-                        os.path.join(root_path, simulation_path, filename)
-                    )
-
-    # Because this comes back from multiprocessing as an unordered result,
-    # add an entry to the front of the list to distinguish it.
-
-    alleparams = []
-    alleparams.append(0)
-    alleparams.extend(datasheet['electrical_parameters'])
-    return alleparams
-
-
-# -----------------------------------------------------------------------
-# cace_run_all_pparams
-#
-# Run all physical parameter measurements.
-# This routine contains a nested multiprocessing pool.
-#
-# "datasheet" is the CACE characterization dataset
-# -----------------------------------------------------------------------
+    if 'status' in param:
+        status = param['status']
+    else:
+        status = 'active'
+        param['status'] = status
 
+    if status == 'skip' or status == 'blocked' or 'testbenches' not in param:
+        if debug:
+            print('Parameter ' + param['name'] + ' skipped for evaluation.')
+        return param
 
-def cace_run_all_pparams(datasheet):
+    paramname = param['name']
+    status = param['status']
 
-    runtime_options = datasheet['runtime_options']
-    if 'pid' in runtime_options:
-        os.setpgid(os.getpid(), runtime_options['pid'])
-        signal.signal(signal.SIGUSR1, child_process_exit)
+    # Process only entries in dataset that have 'testbenches' record
+    if status == 'skip' or status == 'blocked':
+        return param
 
-    try:
-        sequential = runtime_options['sequential']
-    except:
-        sequential = False
+    elif 'testbenches' not in param:
+        if debug:
+            print(
+                'Error:  Parameter '
+                + paramname
+                + ' specified to be evaluated, but no testbench record exists.'
+            )
+        return param
+    elif debug:
+        print('Collating results for parameter ' + paramname)
 
-    if sequential:
-        for pparam in datasheet['physical_parameters']:
-            cace_run_pparam(datasheet, pparam)
+    if 'spec' in param:
+        spec = param['spec']
     else:
-        allpparams = []
-        with NestablePool() as pool:
-            results = []
-            idx = 0
-            for pparam in datasheet['physical_parameters']:
-                pparam['sequence'] = idx
-                results.append(
-                    pool.apply_async(
-                        cace_run_pparam,
-                        (datasheet, pparam),
-                    )
-                )
-                idx += 1
+        spec = {}
+    testbenches = param['testbenches']
 
-            # Replace the physical parameter list in the datasheet with the
-            # number of physical parameters
-            datasheet['physical_parameters'] = len(
-                datasheet['physical_parameters']
-            )
+    # Each item in "testbenches" has a filename (was simulated in
+    # cace_launch and is no longer used), a set of conditions (prepared
+    # by cace_gensim), and a set of results (read back from simulation
+    # output by cace_launch).  There may be multiple results which are
+    # dependent on variables not in the "conditions" list;  these
+    # variables are listed in the "format" line of the "measure"
+    # dictionary that was used to understand the simulation output.
+
+    # This information is used to create a single large matrix of the
+    # result vs. all conditions and variables for the electrical
+    # parameter as a whole.  That matrix may be passed through additional
+    # evaluators (specified in the "evaluate" dictionary) to modify the
+    # result and potentially reduce the number of variables.  The final
+    # output is stored in the "results" list for the electrical parameter.
+    # Finally, the "results" list is scanned to extract minimum, typical,
+    # and maximum values as required for the datasheet.
+
+    # Policy regarding testbench failures:  If any testbench has failed,
+    # the score is set to "incomplete".  If a portion of testbench
+    # simulations ran and some failed, then the score may be changed to
+    # "fail".
+
+    score = 'pass'
+    for testbench in testbenches:
+        filename = testbench['filename']
+        if 'results' not in testbench:
+            print('Error: testbench ' + filename + ' has no results!')
+            score = 'incomplete'
+            break
+        else:
+            results = testbench['results']
+            if len(results) == 0:
+                print(
+                    'Error: testbench '
+                    + filename
+                    + ' has zero-length results!'
+                )
+                score = 'incomplete'
+                break
 
-            for result in results:
+    typresults = []
+    if 'typical' in spec:
+        # Generate a list of results that were made under conditions
+        # that were either typical or did not specify a typical value.
+
+        for testbench in testbenches:
+            istypical = True
+            for condition in testbench['conditions']:
+                # Pull record of the condition (by definition this must
+                # exist in either the electrical parameter conditions list
+                # or the default conditions list).
                 try:
-                    presult = result.get(timeout=300)
-                except Exception as e:
-                    print('cace_run_pparam failed with exception:')
-                    print(e)
-                    presult = None
-                if presult:
-                    allpparams.append(presult)
-
-        # After joining forks, 'results' contains an unordered list of
-        # parameters.  Because the forks do not share memory, these
-        # parameters are no longer the same as the ones in the datasheet,
-        # so put everything back together here.
-
-        maxidx = datasheet['physical_parameters']
-        datasheet['physical_parameters'] = []
-        for idx in range(0, maxidx):
-            for param in allpparams:
-                if param['sequence'] == idx:
-                    datasheet['physical_parameters'].append(param)
-                    break
-
-        for param in allpparams:
-            param.pop('sequence')
-
-        allpparams = []
-        allpparams.append(1)
-        allpparams.extend(datasheet['physical_parameters'])
-        return allpparams
-
-
-# -----------------------------------------------------------------
-# cace_run
-#
-# Run CACE on a characterization datasheet.
-#
-# "datasheet" is the CACE characterization dataset
-# "paramname" is an optional parameter name, which if present may
-# 	be the name of either an electrical parameter or a physical
-# 	parameter.  If omitted, then characterization is run on
-# 	the full set of electrical and physical parameters in the
-# 	datasheet.
-# -----------------------------------------------------------------
-
-
-def cace_run(datasheet, paramname=None):
-
-    if 'runtime_options' in datasheet:
-        runtime_options = datasheet['runtime_options']
-        source = runtime_options['netlist_source']
-    else:
-        source = 'best'
-        runtime_options = {}
-        runtime_options['netlist_source'] = source
-        runtime_options['debug'] = False
-        runtime_options['keep'] = False
-        runtime_options['sequential'] = False
-        datasheet['runtime_options'] = runtime_options
-
-    valid_sources = ['best', 'all', 'schematic', 'layout', 'pex', 'rcx']
-    if source not in valid_sources:
-        print('Invalid value for the netlist source.  Valid values are:')
-        print('    ' + ' '.join(valid_sources))
-        print('No characterization will be done.')
-        runtime_options['status'] = 'failed'
-        return datasheet
-
-    try:
-        debug = runtime_options['debug']
-    except:
-        debug = False
+                    condrec = next(
+                        item
+                        for item in param['conditions']
+                        if item['name'] == condition[0]
+                    )
+                except StopIteration:
+                    condrec = next(
+                        item
+                        for item in default_conditions
+                        if item['name'] == condition[0]
+                    )
 
-    try:
-        sequential = runtime_options['sequential']
-    except:
-        sequential = False
+                if 'typical' in condrec:
+                    typvalue = condrec['typical']
+                    if typvalue != condition[-1]:
+                        istypical = False
+                        break
+            if istypical == True:
+                if 'results' in testbench:
+                    typresults.extend(testbench['results'])
+
+    allresults = []
+    for testbench in testbenches:
+        if 'results' in testbench:
+            allresults.extend(testbench['results'])
+
+    # Results is still a list of lists.  Pull out the inner list.
+    # Flag a warning if the inner list isn't just a single item
+    # (the result), unless 'plot' is specified and not 'spec',
+    # in which case this is normal.
 
-    # Get the set of paths from the characterization file
-    paths = datasheet['paths']
+    isplotdata = True if 'spec' not in param and 'plot' in param else False
 
-    # Simulation path is where the output is dumped.  If it doesn't
-    # exist, then create it.
-    root_path = paths['root']
-    simulation_path = paths['simulation']
-
-    if not os.path.isdir(os.path.join(root_path, simulation_path)):
-        print('Creating simulation path ' + simulation_path)
-        os.makedirs(os.path.join(root_path, simulation_path))
-
-    # Start by regenerating the netlists for the circuit-under-test
-    # (This may not be quick but all tests depend on the existence
-    # of the netlist, so it has to be done here and cannot be
-    # parallelized).
-
-    fullnetlistpath = regenerate_netlists(datasheet)
-    if not fullnetlistpath:
-        print('Failed to regenerate project netlist;  stopping.')
-        runtime_options['status'] = 'failed'
-        return datasheet
-
-    # Generate testbench netlists if needed
-    result = regenerate_testbenches(datasheet, paramname)
-    if result == 1:
-        print('Failed to regenerate testbench netlists;  stopping.')
-        runtime_options['status'] = 'failed'
-        return datasheet
-
-    # Handle a single parameter specified on the
-
-    if paramname:
-        # Special option paramname = "check" is used to run the
-        # proceeding code to regenerate DUT and testbench netlists,
-        # and then return.
-        if paramname == 'check':
-            runtime_options['status'] = 'passed'
-            return datasheet
-
-        # Scan the names of electrical and physical parameters to
-        # see whether the indicated parameter to check is an
-        # electrical or physical parameter, and call the appropriate
-        # routine to handle it.
-
-        found = False
-        if 'electrical_parameters' in datasheet:
-            for eparam in datasheet['electrical_parameters']:
-                if eparam['name'] == paramname:
-                    cace_run_eparam(datasheet, eparam)
-                    found = True
-                    break
-        if 'physical_parameters' in datasheet:
-            for pparam in datasheet['physical_parameters']:
-                if pparam['name'] == paramname:
-                    cace_run_pparam(datasheet, pparam)
-                    found = True
-                    break
-
-        if not found:
-            print('\nError:  No parameter named ' + paramname + ' found!')
-            print('Valid electrical parameter names are:')
-            for eparam in datasheet['electrical_parameters']:
-                print('   ' + eparam['name'])
-            print('Valid physical parameter names are:')
-            for pparam in datasheet['physical_parameters']:
-                print('   ' + pparam['name'])
-
-        return datasheet
-
-    # From this point:  Running characterization on the entire datasheet
-    # (all electrical and physical parameters)
-
-    if sequential:
-        cace_run_all_eparams(datasheet)
-        cace_run_all_pparams(datasheet)
+    if len(allresults) == 0:
+        scaled_results = []
     else:
-        poolresult = []
-        with NestablePool() as top_pool:
-            results = []
-            # Note:  datasheet must be cast as a list if it is a single argument.
-            results.append(
-                top_pool.apply_async(
-                    cace_run_all_eparams,
-                    [datasheet],
-                )
-            )
-            results.append(
-                top_pool.apply_async(
-                    cace_run_all_pparams,
-                    [datasheet],
-                )
-            )
-
-            for result in results:
+        reduced_results = []
+        if isinstance(allresults[0], list):
+            for result in allresults:
+                if len(result) > 1:
+                    if not isplotdata:
+                        print(
+                            'Error:  There are multiple results per testbench!'
+                        )
                 try:
-                    presult = result.get(timeout=300)
-                except Exception as e:
-                    print('cace_run_all_[e|p]param failed with exception:')
-                    print(e)
-                    presult = None
-                if presult:
-                    poolresult.append(presult)
-
-        # The pool results may arrive in either order, so arrange them properly.
-        idx0 = poolresult[0][0]
-        idx1 = poolresult[1][0]
-        datasheet['electrical_parameters'] = poolresult[idx0][1:]
-        datasheet['physical_parameters'] = poolresult[idx1][1:]
-
-    return datasheet
-
-
-# -----------------------------------------------------------------
-# Print usage statement
-# -----------------------------------------------------------------
-
-
-def usage():
-    print('Usage:')
-    print('')
-    print('cace.py <filename_in> <filename_out> [options]')
-    print('  Where <filename_in> is a format 4.0 ASCII CACE file.')
-    print('  And <filename_out> is the name of the file to write.')
-    print('')
-    print('options may be one of:')
-    print('  -source=schematic|layout|rcx|all|best')
-    print('  -param=<parameter_name>')
-    print('  -force')
-    print('  -json')
-    print('  -keep')
-    print('  -debug')
-    print('  -sequential')
-    print('  -summary')
-    print('')
-    print('When run from the top level, this program parses the CACE')
-    print('characterization file, runs simulations, and outputs a')
-    print('modified file annotated with characterization results.')
-    print('')
-    print('With option "-source", restrict characterization to the')
-    print('specific netlist source, which is either schematic capture,')
-    print('layout extracted, or full R-C parasitic extracted.  If not')
-    print('specified, then characterization is run on the full R-C')
-    print('parasitic extracted layout netlist if available, and the')
-    print('schematic captured netlist if not (option "best").')
-    print('')
-    print('Option "-param=<parameter_name>" runs simulations on only')
-    print('the named electrical or physical parameter.')
-    print('')
-    print('Option "-force" forces new regeneration of all netlists.')
-    print('')
-    print('Option "-json" generates an output file in JSON format.')
-    print('')
-    print('Option "-keep" retains files generated for characterization.')
-    print('')
-    print('Option "-noplot" will not generate any graphs.')
-    print('')
-    print('Option "-debug" generates additional diagnostic output.')
-    print('')
-    print('Option "-sequential" runs simulations sequentially.')
-    print('')
-    print(
-        'Option "-nosim" does not re-run simulations if the output file exists.'
-    )
-    print('   (Warning---does not check if simulations are out of date).')
-    print('')
-    print('Option "-summary" prints a summary of results at the end.')
-
-
-# -----------------------------------------------------------------
-# Top level call to cace.py
-# If called from the command line
-# -----------------------------------------------------------------
-
-
-def cli():
-    options = []
-    arguments = []
-    for item in sys.argv[1:]:
-        if item.find('-', 0) == 0:
-            options.append(item)
+                    rvalue = float(result[0])
+                except:
+                    try:
+                        print(
+                            'Error:  Result '
+                            + str(result[0])
+                            + ' is not numeric!'
+                        )
+                    except:
+                        print('Error:  No result!')
+                    rvalue = 0.0
+                reduced_results.append(rvalue)
         else:
-            arguments.append(item)
-
-    debug = False
-    dojson = False
-    doforce = False
-    dokeep = False
-    noplot = False
-    nosim = False
-    dosequential = False
-    dosummary = False
-    source = 'best'
-    paramname = None
-
-    for item in options.copy():
-        if item == '-debug':
-            debug = True
-            options.remove(item)
-        elif item == '-json':
-            dojson = True
-            options.remove(item)
-        elif item == '-force':
-            doforce = True
-            options.remove(item)
-        elif item == '-keep':
-            dokeep = True
-            options.remove(item)
-        elif item == '-noplot':
-            noplot = True
-            options.remove(item)
-        elif item == '-nosim':
-            nosim = True
-            options.remove(item)
-        elif item == '-summary':
-            dosummary = True
-            options.remove(item)
-        elif item == '-sequential':
-            dosequential = True
-            options.remove(item)
-        elif item == '-help':
-            options.remove(item)
-            usage()
-            sys.exit(0)
-        elif item.startswith('-source'):
-            optargs = item.split('=')
-            source = optargs[1]
-            options.remove(item)
-            # Accept a few alternative names
-            if source == 'schem':
-                source = 'schematic'
-            elif source == 'lvs':
-                source = 'layout'
-        elif item.startswith('-param'):
-            optargs = item.split('=')
-            paramname = optargs[1]
-            options.remove(item)
-
-    result = 0
-    if len(arguments) == 2 and len(options) == 0:
-        filename = arguments[0]
-        outfile = arguments[1]
-
-        # If the file is a JSON file, read it with json.load
-        if os.path.splitext(filename)[1] == '.json':
-            with open(filename, 'r') as ifile:
-                dataset = json.load(ifile)
-                if 'data-sheet' in dataset:
-                    dataset = dataset['data-sheet']
-                    # Attempt to upgrade this to format 4.0
-                    dataset = cace_compat(dataset, debug)
-        else:
-            dataset = cace_read(filename, debug)
-
-        if dataset == {}:
-            result = 1
+            for result in allresults:
+                try:
+                    rvalue = float(result)
+                except:
+                    print('Error:  Result ' + str(result) + ' is not numeric!')
+                    rvalue = 0.0
+                reduced_results.append(rvalue)
+
+        # scaled_results is 'results' scaled to the units used by param.
+        if 'unit' in param:
+            scaled_results = spice_unit_unconvert(
+                [param['unit'], reduced_results]
+            )
         else:
-            # If there is a "paths" dictionary in dataset and it does
-            # not have an entry for "root", then find the name of the
-            # directory where "filename" exists and set that to root.
-            filepath = os.path.split(os.path.realpath(filename))[0]
-            if 'paths' in dataset:
-                paths = dataset['paths']
-                if 'root' not in paths:
-                    paths['root'] = filepath
-
-            # Set the current working directory to the root by first
-            # setting the current working directory to the path of
-            # the testbench file and then setting it to root (assuming
-            # root is a relative path, although it could be an absolute
-            # path).
-            os.chdir(filepath)
-            os.chdir(paths['root'])
-            paths['root'] = os.getcwd()
-            if debug:
-                print(
-                    'Working directory set to project root at ' + paths['root']
-                )
+            scaled_results = reduced_results
 
-            # All run-time options are dropped into a dictionary,
-            # passed to all routines, and removed at the end.
-            runtime_options = {}
-            runtime_options['debug'] = debug
-            runtime_options['force'] = doforce
-            runtime_options['json'] = dojson
-            runtime_options['keep'] = dokeep
-            runtime_options['noplot'] = noplot
-            runtime_options['nosim'] = nosim
-            runtime_options['sequential'] = dosequential
-            runtime_options['netlist_source'] = source
+    # Now do the same to the typical result set.
 
-            # Add the name of the file to the top-level dictionary
-            runtime_options['filename'] = os.path.split(filename)[1]
-
-            dataset['runtime_options'] = runtime_options
+    if len(typresults) == 0:
+        scaled_typresults = []
+    else:
+        reduced_results = []
+        if isinstance(typresults[0], list):
+            for result in typresults:
+                if len(result) > 1:
+                    if not isplotdata:
+                        print(
+                            'Error:  There are multiple results per testbench!'
+                        )
+                try:
+                    rvalue = float(result[0])
+                except:
+                    try:
+                        print(
+                            'Error:  Result '
+                            + str(result[0])
+                            + ' is not numeric!'
+                        )
+                    except:
+                        print('Error:  No result!')
+                    rvalue = 0.0
+                reduced_results.append(rvalue)
+        else:
+            for result in typresults:
+                try:
+                    rvalue = float(result)
+                except:
+                    print('Error:  Result ' + str(result) + ' is not numeric!')
+                    rvalue = 0.0
+                reduced_results.append(rvalue)
+
+        # scaled_results is 'results' scaled to the units used by param.
+        if 'unit' in param:
+            scaled_typresults = spice_unit_unconvert(
+                [param['unit'], reduced_results]
+            )
+        else:
+            scaled_typresults = reduced_results
 
-            # Run CACE.  Use only as directed.
-            charresult = cace_run(dataset, paramname)
-            if debug:
-                print('Done with CACE simulations and evaluations.')
+    # Set the value of "units" passed to find_limits()
+    if 'unit' in param:
+        units = param['unit']
+    else:
+        units = ''
 
-        if charresult == {}:
-            result = 1
+    # Diagnostic
+    if debug:
+        print('Scaled results are:')
+        if len(scaled_results) > 20:
+            print('(truncated due to length)')
+            print(str(scaled_results[0:10]))
+            print('...')
+            print(str(scaled_results[-10:-1]))
         else:
-            if debug:
-                print('Writing final output file ' + outfile)
-            if dojson:
-                # Dump the result as a JSON file
-                jsonfile = os.path.splitext(outfile)[0] + '_debug.json'
-                with open(jsonfile, 'w') as ofile:
-                    json.dump(charresult, ofile, indent=4)
+            print(str(scaled_results))
+        if 'typical' in spec:
+            print('Scaled typical results are:')
+            if len(scaled_typresults) > 20:
+                print('(truncated due to length)')
+                print(str(scaled_typresults[0:10]))
+                print('...')
+                print(str(scaled_typresults[-10:-1]))
             else:
-                # Write the result in CACE ASCII format version 4.0
-                cace_write(charresult, outfile, doruntime=False)
-
-            if dosummary:
-                print('')
-                print('CACE Summary of results:')
-                print('------------------------')
-                cace_summary(charresult, paramname)
+                print(str(scaled_typresults))
 
+    # Calculate minimum/typical/maximum results for the electrical parameter
+    if len(scaled_results) == 0:
+        if 'minimum' in spec or 'maximum' in spec:
+            resultdict = incompleteresult(param, noplotmode)
+        else:
+            resultdict = {}
     else:
-        if debug:
-            print('arguments = ' + ' '.join(arguments))
-            print('options = ' + ' '.join(options))
-        usage()
-        sys.exit(1)
+        resultdict = {}
+        if 'minimum' in spec:
+            spectype = 'minimum'
+            minrec = spec['minimum']
+            minresult = find_limits(
+                spectype, minrec, scaled_results, units, debug
+            )
+            if score == 'incomplete' and minresult[1] == 'fail':
+                score = 'fail'
+            elif score != 'fail':
+                score = minresult[1]
+            resultdict['minimum'] = minresult
+
+        if 'maximum' in spec:
+            spectype = 'maximum'
+            maxrec = spec['maximum']
+            maxresult = find_limits(
+                spectype, maxrec, scaled_results, units, debug
+            )
+            if score == 'incomplete' and maxresult[1] == 'fail':
+                score = 'fail'
+            elif score != 'fail':
+                score = maxresult[1]
+            resultdict['maximum'] = maxresult
+
+    if len(scaled_typresults) == 0:
+        if 'typical' in spec:
+            resultdict = incompleteresult(param, noplotmode)
+    else:
+        if 'typical' in spec:
+            spectype = 'typical'
+            typrec = spec['typical']
+            typresult = find_limits(
+                spectype, typrec, scaled_typresults, units, debug
+            )
+            if score == 'incomplete' and typresult == 'fail':
+                score = 'fail'
+            elif score != 'fail':
+                score = typresult[1]
+            resultdict['typical'] = typresult
+
+    # Results belong to a key name in the electrical parameter that
+    # depends on where the source netlists came from.
+
+    resultdict['name'] = runtime_options['netlist_source']
+    if debug:
+        print(
+            'Adding new result set '
+            + resultdict['name']
+            + ' for '
+            + param['name']
+        )
+    addnewresult(param, resultdict)
 
-    sys.exit(result)
+    # Return the annotated electrical parameter
+    return param
 
 
-if __name__ == '__main__':
-    cli()
+# ---------------------------------------------------------------------------
```

### Comparing `cace-2.1.9/cace/cace_gui.py` & `cace-2.2.0/cace/common/cace_gensim.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,2142 +1,1735 @@
 #!/usr/bin/env python3
 #
-# --------------------------------------------------------
-# cace_gui.py
-# Project Manager GUI.
+# cace_gensim.py
 #
-# This is a Python tkinter script that handles local
-# project management.  Much of this involves the
-# running of ng-spice for characterization, allowing
-# the user to determine where a circuit is failing
-# characterization.
+# This is the main part of the automatic characterization engine.  It takes
+# a simulation template file as input and parses it for information on
+# how to construct files for the characterization simulations.  Output is
+# a number of simulation files (for now, at least, in ngspice format).
 #
-# --------------------------------------------------------
-# Written by Tim Edwards
-# Efabless Corporation
-# Created September 9, 2016
-# 	Version 1.0
-# 	System running on the Efabless Open Galaxy
-# 	servers.
+# Note:  Unlike the former version of this script, the simulations are
+# done independently by cace_launch., which is not invoked from
+# cace_gensim.  cace_gensim only generates the set of simulation netlists.
 #
-# (Some intermediate versions were not recorded)
+# There is no command line usage of cace_gensim.py.  It is called from
+# either cace.py (command line) or cace_gui.py (GUI)
 #
-# Updated March 14, 2023
-# 	Version 3.0
-# 	Ported from the Efabless Open Galaxy servers
-# 	to open_pdks.
-#
-# Updated November 22, 2023
-# 	Version 4.0
-# 	Ported from open_pdks to a standalone repository
-# 	renamed from cace.py to cace_gui.py
-# --------------------------------------------------------
 
-import io
-import re
 import os
 import sys
-import copy
 import json
+import re
 import time
-import signal
-import select
-import datetime
-import contextlib
+import shutil
 import subprocess
-import multiprocessing
-
-import tkinter
-from tkinter import ttk
-from tkinter import filedialog
-
-from .gui.tksimpledialog import *
-from .gui.tooltip import *
-from .gui.consoletext import ConsoleText
-from .gui.helpwindow import HelpWindow
-from .gui.failreport import FailReport
-from .gui.textreport import TextReport
-from .gui.editparam import EditParam
-from .gui.settings import Settings
-from .gui.simhints import SimHints
-
-from .common.cace_read import *
-from .common.cace_compat import *
-from .common.cace_write import *
-from .cace_cli import *
-
-# User preferences file (if it exists)
-prefsfile = '~/design/.profile/prefs.json'
-
-# Application path (path where this script is located)
-apps_path = os.path.realpath(os.path.dirname(__file__))
-
-# ------------------------------------------------------
-# Simple dialog for confirming quit
-# ------------------------------------------------------
-
-
-class ConfirmDialog(Dialog):
-    def body(self, master, warning, seed):
-        ttk.Label(master, text=warning, wraplength=500).grid(
-            row=0, columnspan=2, sticky='wns'
-        )
-        return self
+from functools import reduce
 
-    def apply(self):
-        return 'okay'
+from .spiceunits import spice_unit_convert
+from .spiceunits import numeric
 
-
-# ------------------------------------------------------
-# Simple dialog with no "OK" button (can only cancel)
-# ------------------------------------------------------
-
-
-class PuntDialog(Dialog):
-    def body(self, master, warning, seed):
-        if warning:
-            ttk.Label(master, text=warning, wraplength=500).grid(
-                row=0, columnspan=2, sticky='wns'
+from .cace_write import *
+from .cace_regenerate import get_pdk_root
+from .safe_eval import safe_eval
+
+# -----------------------------------------------------------------------
+# Read the indicated file, find the .subckt line, and copy out the
+# pin names and DUT name.  Complain if pin names don't match pin names
+# in the datasheet.
+# NOTE:  There may be more than one subcircuit in the netlist, so
+# insist upon the actual DUT (pname)
+# -----------------------------------------------------------------------
+
+
+def construct_dut_from_path(pname, pathname, pinlist):
+
+    subrex = re.compile('^[^\*]*[ \t]*.subckt[ \t]+(.*)$', re.IGNORECASE)
+    outline = ''
+    dutname = ''
+    if not os.path.isfile(pathname):
+        print('Error:  No design netlist file ' + pathname + ' found.')
+        return outline
+
+    # First pull in all lines of the file and concatenate all continuation
+    # lines.
+    with open(pathname, 'r') as ifile:
+        duttext = ifile.read()
+
+    dutlines = duttext.replace('\n+', ' ').splitlines()
+    found = 0
+    for line in dutlines:
+        lmatch = subrex.match(line)
+        if lmatch:
+            rest = lmatch.group(1)
+            tokens = rest.split()
+            dutname = tokens[0]
+            if dutname == pname:
+                outline = outline + 'X' + dutname + ' '
+                for pin in tokens[1:]:
+                    upin = pin.upper()
+                    try:
+                        pinmatch = next(
+                            item
+                            for item in pinlist
+                            if item['name'].upper() == upin
+                        )
+                    except StopIteration:
+                        # Maybe this is not the DUT?
+                        found = 0
+                        # Try the next line (to be done)
+                        break
+                    else:
+                        outline = outline + pin + ' '
+                        found += 1
+                break
+
+    if found == 0 and dutname == '':
+        print('File ' + pathname + ' does not contain any subcircuits!')
+        raise SyntaxError(
+            'File ' + pathname + ' does not contain any subcircuits!'
+        )
+    elif found == 0:
+        if dutname != pname:
+            print(
+                'File '
+                + pathname
+                + ' does not have a subcircuit named '
+                + pname
+                + '!'
+            )
+            raise SyntaxError(
+                'File '
+                + pathname
+                + ' does not have a subcircuit named '
+                + pname
+                + '!'
             )
-        return self
-
-    def buttonbox(self):
-        # Add button box with "Cancel" only.
-        box = ttk.Frame(self.obox)
-        w = ttk.Button(box, text='Cancel', width=10, command=self.cancel)
-        w.pack(side='left', padx=5, pady=5)
-        self.bind('<Escape>', self.cancel)
-        box.pack(fill='x', expand='true')
-
-    def apply(self):
-        return 'okay'
-
-
-# ---------------------------------------------------------
-# Routine for a child process to capture signal SIGUSR1
-# and exit gracefully.
-# ---------------------------------------------------------
-
-
-def child_process_exit(signum, frame):
-    print('CACE GUI:  Received forced stop.')
-    try:
-        multiprocessing.current_process().terminate()
-    except AttributeError:
-        print('Terminate failed; Child PID is ' + str(os.getpid()))
-        print('Waiting on process to finish.')
-
-
-# ------------------------------------------------------
-# Main class for this application
-# ------------------------------------------------------
-
-
-class CACECharacterize(ttk.Frame):
-    """local characterization GUI."""
-
-    def __init__(self, parent, *args, **kwargs):
-        ttk.Frame.__init__(self, parent, *args, **kwargs)
-        self.root = parent
-        self.init_gui()
-        parent.protocol('WM_DELETE_WINDOW', self.on_quit)
-
-    def on_quit(self):
-        """Exits program."""
-        if not self.check_saved():
-            warning = 'Warning:  Simulation results have not been saved.'
-            confirm = ConfirmDialog(self, warning).result
-            if not confirm == 'okay':
-                print('Quit canceled.')
-                return
-        if self.logfile:
-            self.logfile.close()
-        quit()
-
-    def on_mousewheel(self, event):
-        if event.num == 5:
-            self.datasheet_viewer.yview_scroll(1, 'units')
-        elif event.num == 4:
-            self.datasheet_viewer.yview_scroll(-1, 'units')
-
-    def init_gui(self):
-        """Builds GUI."""
-        global prefsfile
-
-        message = []
-        fontsize = 11
-
-        # Read user preferences file, get default font size from it.
-        prefspath = os.path.expanduser(prefsfile)
-        if os.path.exists(prefspath):
-            with open(prefspath, 'r') as f:
-                self.prefs = json.load(f)
-            if 'fontsize' in self.prefs:
-                fontsize = self.prefs['fontsize']
         else:
-            self.prefs = {}
-
-        s = ttk.Style()
-
-        available_themes = s.theme_names()
-        s.theme_use(available_themes[0])
-
-        s.configure('bg.TFrame', background='gray40')
-        s.configure('italic.TLabel', font=('Helvetica', fontsize, 'italic'))
-        s.configure(
-            'title.TLabel',
-            font=('Helvetica', fontsize, 'bold italic'),
-            foreground='brown',
-            anchor='center',
-        )
-        s.configure('normal.TLabel', font=('Helvetica', fontsize))
-        s.configure(
-            'red.TLabel', font=('Helvetica', fontsize), foreground='red'
-        )
-        s.configure(
-            'green.TLabel', font=('Helvetica', fontsize), foreground='green3'
-        )
-        s.configure(
-            'blue.TLabel', font=('Helvetica', fontsize), foreground='blue'
-        )
-        s.configure(
-            'hlight.TLabel', font=('Helvetica', fontsize), background='gray93'
-        )
-        s.configure(
-            'rhlight.TLabel',
-            font=('Helvetica', fontsize),
-            foreground='red',
-            background='gray93',
-        )
-        s.configure(
-            'ghlight.TLabel',
-            font=('Helvetica', fontsize),
-            foreground='green3',
-            background='gray93',
-        )
-        s.configure(
-            'blue.TLabel', font=('Helvetica', fontsize), foreground='blue'
-        )
-        s.configure(
-            'blue.TMenubutton',
-            font=('Helvetica', fontsize),
-            foreground='blue',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'red.TButton',
-            font=('Helvetica', fontsize),
-            foreground='red',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'green.TButton',
-            font=('Helvetica', fontsize),
-            foreground='green3',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'hlight.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-            background='gray93',
-        )
-        s.configure(
-            'rhlight.TButton',
-            font=('Helvetica', fontsize),
-            foreground='red',
-            border=3,
-            relief='raised',
-            background='gray93',
-        )
-        s.configure(
-            'ghlight.TButton',
-            font=('Helvetica', fontsize),
-            foreground='green3',
-            border=3,
-            relief='raised',
-            background='gray93',
-        )
-        s.configure(
-            'blue.TButton',
-            font=('Helvetica', fontsize),
-            foreground='blue',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'redtitle.TButton',
-            font=('Helvetica', fontsize, 'bold italic'),
-            foreground='red',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'bluetitle.TButton',
-            font=('Helvetica', fontsize, 'bold italic'),
-            foreground='blue',
-            border=3,
-            relief='raised',
-        )
-
-        # Create the help window
-        self.help = HelpWindow(self, fontsize=fontsize)
-
-        with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-            helpfile = os.path.join(apps_path, 'doc', 'characterize_help.txt')
-            self.help.add_pages_from_file(helpfile)
-            helpfile = os.path.join(apps_path, 'doc', 'format.txt')
-            self.help.add_pages_from_file(helpfile)
-            message = buf.getvalue()
-
-        # Set the help display to the first page
-        self.help.page(0)
-
-        # Create the failure report window
-        self.failreport = FailReport(self, fontsize=fontsize)
-
-        # LVS results get a text window of results
-        self.textreport = TextReport(self, fontsize=fontsize)
-
-        # Create the settings window
-        self.settings = Settings(self, fontsize=fontsize)
-
-        # Create the simulation hints window
-        self.simhints = SimHints(self, fontsize=fontsize)
-
-        # Create the edit parameter window
-        self.editparam = EditParam(self, fontsize=fontsize)
-
-        # Variables used by option menus and other stuff
-        self.origin = tkinter.StringVar(self)
-        self.cur_project = tkinter.StringVar(self)
-        self.filename = '(no selection)'
-        self.datasheet = {}
-        self.status = {}
-        self.procs_pending = {}
-        self.logfile = None
-
-        # Create a multiprocessing data queue for passing information between
-        # the parent and child processes (cace_run)
-        self.queue = multiprocessing.Queue()
-
-        # Root window title
-        self.root.title('Characterization')
-        self.root.option_add('*tearOff', 'FALSE')
-        self.pack(side='top', fill='both', expand='true')
-
-        pane = tkinter.PanedWindow(
-            self, orient='vertical', sashrelief='groove', sashwidth=6
-        )
-        pane.pack(side='top', fill='both', expand='true')
-        self.toppane = ttk.Frame(pane)
-        self.botpane = ttk.Frame(pane)
-
-        self.toppane.title_frame = ttk.Frame(self.toppane)
-        self.toppane.title_frame.grid(column=0, row=2, sticky='nswe')
-        self.toppane.title_frame.datasheet_label = ttk.Label(
-            self.toppane.title_frame,
-            text='CACE Datasheet:',
-            style='normal.TLabel',
-        )
-        self.toppane.title_frame.datasheet_label.grid(column=0, row=0, ipadx=5)
-
-        # New datasheet select button
-        self.toppane.title_frame.datasheet_select = ttk.Button(
-            self.toppane.title_frame,
-            text=self.filename,
-            style='normal.TButton',
-            command=self.choose_datasheet,
-        )
-        self.toppane.title_frame.datasheet_select.grid(
-            column=1, row=0, ipadx=5
-        )
-
-        ToolTip(
-            self.toppane.title_frame.datasheet_select,
-            text='Select new datasheet file',
-        )
-
-        # Show path to datasheet
-        self.toppane.title_frame.path_label = ttk.Label(
-            self.toppane.title_frame, text=self.filename, style='normal.TLabel'
-        )
-        self.toppane.title_frame.path_label.grid(
-            column=2, row=0, ipadx=5, padx=10
-        )
-
-        # Spacer in middle moves selection button to right
-        self.toppane.title_frame.sep_label = ttk.Label(
-            self.toppane.title_frame, text=' ', style='normal.TLabel'
-        )
-        self.toppane.title_frame.sep_label.grid(
-            column=3, row=0, ipadx=5, padx=10
-        )
-        self.toppane.title_frame.columnconfigure(3, weight=1)
-        self.toppane.title_frame.rowconfigure(0, weight=0)
-
-        # Selection for origin of netlist
-        self.toppane.title_frame.origin_label = ttk.Label(
-            self.toppane.title_frame,
-            text='Netlist from:',
-            style='normal.TLabel',
-        )
-        self.toppane.title_frame.origin_label.grid(
-            column=4, row=0, ipadx=5, padx=10
-        )
-
-        self.origin.set('Schematic Capture')
-        self.toppane.title_frame.origin_select = ttk.OptionMenu(
-            self.toppane.title_frame,
-            self.origin,
-            'Schematic Capture',
-            'Schematic Capture',
-            'Layout Extracted',
-            'C Extracted',
-            'R-C Extracted',
-            style='blue.TMenubutton',
-            command=self.swap_results,
-        )
-        self.toppane.title_frame.origin_select.grid(column=5, row=0, ipadx=5)
-
-        # ---------------------------------------------
-        ttk.Separator(self.toppane, orient='horizontal').grid(
-            column=0, row=3, sticky='news'
-        )
-        # ---------------------------------------------
-
-        # Datasheet information goes here when datasheet is loaded.
-        self.mframe = ttk.Frame(self.toppane)
-        self.mframe.grid(column=0, row=4, sticky='news')
-
-        # Row 4 (mframe) is expandable, the other rows are not.
-        self.toppane.rowconfigure(0, weight=0)
-        self.toppane.rowconfigure(1, weight=0)
-        self.toppane.rowconfigure(2, weight=0)
-        self.toppane.rowconfigure(3, weight=0)
-        self.toppane.rowconfigure(4, weight=1)
-        self.toppane.columnconfigure(0, weight=1)
-
-        # ---------------------------------------------
-        # ttk.Separator(self, orient='horizontal').grid(column=0, row=5, sticky='ew')
-        # ---------------------------------------------
-
-        # Add a text window below the datasheet to capture output.  Redirect
-        # print statements to it.
-
-        self.botpane.console = ttk.Frame(self.botpane)
-        self.botpane.console.pack(side='top', fill='both', expand='true')
-
-        self.text_box = ConsoleText(
-            self.botpane.console, wrap='word', height=4
-        )
-        self.text_box.pack(side='left', fill='both', expand='true')
-        console_scrollbar = ttk.Scrollbar(self.botpane.console)
-        console_scrollbar.pack(side='right', fill='y')
-        # attach console to scrollbar
-        self.text_box.config(yscrollcommand=console_scrollbar.set)
-        console_scrollbar.config(command=self.text_box.yview)
-
-        # Add button bar at the bottom of the window
-        self.bbar = ttk.Frame(self.botpane)
-        self.bbar.pack(side='top', fill='x')
-        # Progress bar expands with the window, buttons don't
-        self.bbar.columnconfigure(7, weight=1)
-
-        # Define the "quit" button and action
-        self.bbar.quit_button = ttk.Button(
-            self.bbar,
-            text='Quit',
-            command=self.on_quit,
-            style='normal.TButton',
-        )
-        self.bbar.quit_button.grid(column=0, row=0, padx=5)
-
-        # Define the save button
-        self.bbar.save_button = ttk.Button(
-            self.bbar,
-            text='Save',
-            command=self.save_results,
-            style='normal.TButton',
-        )
-        self.bbar.save_button.grid(column=1, row=0, padx=5)
-
-        # Define the save-as button
-        self.bbar.saveas_button = ttk.Button(
-            self.bbar,
-            text='Save As',
-            command=self.save_manual,
-            style='normal.TButton',
-        )
-        self.bbar.saveas_button.grid(column=2, row=0, padx=5)
-
-        # Also a load button
-        self.bbar.load_button = ttk.Button(
-            self.bbar,
-            text='Load',
-            command=self.load_manual,
-            style='normal.TButton',
-        )
-        self.bbar.load_button.grid(column=3, row=0, padx=5)
-
-        # Define the HTML generate button
-        self.bbar.html_button = ttk.Button(
-            self.bbar,
-            text='HTML',
-            command=self.generate_html,
-            style='normal.TButton',
+            print('Pins in schematic: ' + str(tokens[1:]))
+            print('Pins in datasheet: ', end='')
+            for pin in pinlist:
+                print(pin['name'] + ' ', end='')
+            print('')
+            print(
+                'File '
+                + pathname
+                + ' subcircuit '
+                + pname
+                + ' does not have expected pins!'
+            )
+            raise SyntaxError(
+                'File '
+                + pathname
+                + ' subcircuit '
+                + pname
+                + ' does not have expected pins!'
+            )
+    elif found != len(pinlist):
+        print(
+            'File ' + pathname + ' does not contain the project DUT ' + pname
         )
-        self.bbar.html_button.grid(column=4, row=0, padx=5)
-
-        # Define help button
-        self.bbar.help_button = ttk.Button(
-            self.bbar,
-            text='Help',
-            command=self.help.open,
-            style='normal.TButton',
+        print('or not all pins of the DUT were found.')
+        print('Pinlist is : ', end='')
+        for pinrec in pinlist:
+            print(pinrec['name'] + ' ', end='')
+        print('')
+
+        print('Length of pinlist is ' + str(len(pinlist)))
+        print('Number of pins found in subcircuit call is ' + str(found))
+        raise SyntaxError(
+            'File ' + pathname + ' does not contain the project DUT!'
         )
-        self.bbar.help_button.grid(column=5, row=0, padx=5)
+    else:
+        outline = outline + dutname + '\n'
+    return outline
 
-        # Define settings button
-        self.bbar.settings_button = ttk.Button(
-            self.bbar,
-            text='Settings',
-            command=self.settings.open,
-            style='normal.TButton',
-        )
-        self.bbar.settings_button.grid(column=6, row=0, padx=5)
 
-        ToolTip(self.bbar.quit_button, text='Exit characterization tool')
-        ToolTip(
-            self.bbar.save_button, text='Save current characterization state'
-        )
-        ToolTip(
-            self.bbar.saveas_button, text='Save current characterization state'
-        )
-        ToolTip(self.bbar.html_button, text='Generate HTML output')
-        ToolTip(
-            self.bbar.load_button, text='Load characterization state from file'
-        )
-        ToolTip(self.bbar.help_button, text='Start help tool')
-        ToolTip(
-            self.bbar.settings_button,
-            text='Manage characterization tool settings',
-        )
+# -----------------------------------------------------------------------
+# floating-point linear numeric sequence generator, to be used with
+# condition generator
+# -----------------------------------------------------------------------
+
+
+def linseq(condition, unit, start, stop, step):
+    a = numeric(start)
+    e = numeric(stop)
+    s = numeric(step)
+    while a < e + s:
+        if a > e:
+            yield (condition, unit, stop)
+        else:
+            yield (condition, unit, str(a))
+        a = a + s
 
-        # Inside frame with main electrical parameter display and scrollbar
-        # To make the frame scrollable, it must be a frame inside a canvas.
-        self.datasheet_viewer = tkinter.Canvas(self.mframe)
-        self.datasheet_viewer.grid(row=0, column=0, sticky='nsew')
-        self.datasheet_viewer.dframe = ttk.Frame(
-            self.datasheet_viewer, style='bg.TFrame'
-        )
-        # Place the frame in the canvas
-        self.datasheet_viewer.create_window(
-            (0, 0),
-            window=self.datasheet_viewer.dframe,
-            anchor='nw',
-            tags='self.frame',
-        )
 
-        # Make sure the main window resizes, not the scrollbars.
-        self.mframe.rowconfigure(0, weight=1)
-        self.mframe.columnconfigure(0, weight=1)
-        # X scrollbar for datasheet viewer
-        main_xscrollbar = ttk.Scrollbar(self.mframe, orient='horizontal')
-        main_xscrollbar.grid(row=1, column=0, sticky='nsew')
-        # Y scrollbar for datasheet viewer
-        main_yscrollbar = ttk.Scrollbar(self.mframe, orient='vertical')
-        main_yscrollbar.grid(row=0, column=1, sticky='nsew')
-        # Attach console to scrollbars
-        self.datasheet_viewer.config(xscrollcommand=main_xscrollbar.set)
-        main_xscrollbar.config(command=self.datasheet_viewer.xview)
-        self.datasheet_viewer.config(yscrollcommand=main_yscrollbar.set)
-        main_yscrollbar.config(command=self.datasheet_viewer.yview)
-
-        # Make sure that scrollwheel pans window
-        self.datasheet_viewer.bind_all('<Button-4>', self.on_mousewheel)
-        self.datasheet_viewer.bind_all('<Button-5>', self.on_mousewheel)
-
-        # Set up configure callback
-        self.datasheet_viewer.dframe.bind('<Configure>', self.frame_configure)
-
-        # Add the panes once the internal geometry is known
-        pane.add(self.toppane)
-        pane.add(self.botpane)
-        pane.paneconfig(self.toppane, stretch='first')
-
-        # Initialize variables
-
-        # Capture time of start to compare against the annotated
-        # output file timestamp.
-        self.starttime = time.time()
-
-        # Redirect stdout and stderr to the console as the last thing to do. . .
-        # Otherwise errors in the GUI get sucked into the void.
-        self.stdout = sys.stdout
-        self.stderr = sys.stderr
-        sys.stdout = ConsoleText.StdoutRedirector(self.text_box)
-        sys.stderr = ConsoleText.StderrRedirector(self.text_box)
-
-        if message:
-            print(message)
-
-    def frame_configure(self, event):
-        self.update_idletasks()
-        self.datasheet_viewer.configure(
-            scrollregion=self.datasheet_viewer.bbox('all')
-        )
+# -----------------------------------------------------------------------
+# floating-point logarithmic numeric sequence generator, to be used with
+# condition generator
+# -----------------------------------------------------------------------
+
+
+def logseq(condition, unit, start, stop, step):
+    a = numeric(start)
+    e = numeric(stop)
+    s = numeric(step)
+    while a < e * s:
+        if a > e:
+            yield (condition, unit, stop)
+        else:
+            yield (condition, unit, str(a))
+        a = a * s
 
-    def logstart(self):
-        # Start a logfile (or append to it, if it already exists)
-        # Disabled by default, as it can get very large.
-        # Can be enabled from Settings.
-        if self.settings.get_log() == True:
-            dataroot = os.path.splitext(self.filename)[0]
-            if not self.logfile:
-                self.logfile = open(dataroot + '.log', 'a')
-
-                # Print some initial information to the logfile.
-                self.logprint('-------------------------')
-                self.logprint(
-                    'Starting new log file '
-                    + datetime.datetime.now().strftime('%c'),
-                    doflush=True,
-                )
 
-    def logstop(self):
-        if self.logfile:
-            self.logprint('-------------------------', doflush=True)
-            self.logfile.close()
-            self.logfile = []
-
-    def logprint(self, message, doflush=False):
-        if self.logfile:
-            self.logfile.buffer.write(message.encode('utf-8'))
-            self.logfile.buffer.write('\n'.encode('utf-8'))
-            if doflush:
-                self.logfile.flush()
-
-    def set_working_directory(self, datasheet):
-        # CACE should be run from the location of the datasheet's root
-        # directory.  Typically, the datasheet is in the "cace" subdirectory
-        # and "root" is "..".
-
-        rootpath = None
-        if 'paths' in datasheet:
-            paths = datasheet['paths']
-            if 'root' in paths:
-                rootpath = paths['root']
-
-        dspath = os.path.split(self.filename)[0]
-        if rootpath:
-            dspath = os.path.join(dspath, rootpath)
-            paths['root'] = '.'
+# -----------------------------------------------------------------------
+# binary (integer) numeric sequence generators, to be used with
+# condition generator
+# -----------------------------------------------------------------------
 
-        os.chdir(dspath)
-        print(
-            'Working directory set to '
-            + dspath
-            + ' ('
-            + os.path.abspath(dspath)
-            + ')'
-        )
 
-    def set_datasheet(self, datasheet):
-        if self.logfile:
-            self.logprint('end of log.')
-            self.logprint('-------------------------', doflush=True)
-            self.logfile.close()
-            self.logfile = None
-
-        if not os.path.isfile(datasheet):
-            print('Error:  File ' + datasheet + ' not found.')
-            return
-
-        debug = self.settings.get_debug()
-
-        [dspath, dsname] = os.path.split(datasheet)
-        # Read the datasheet
-        if os.path.splitext(datasheet)[1] == '.json':
-            with open(datasheet) as ifile:
-                try:
-                    # "data-sheet" as a sub-entry of the input file is deprecated.
-                    datatop = json.load(ifile)
-                    if 'data-sheet' in datatop:
-                        datatop = datatop['data-sheet']
-                except json.decoder.JSONDecodeError as e:
-                    print(
-                        'Error:  Parse error reading JSON file '
-                        + datasheet
-                        + ':'
-                    )
-                    print(str(e))
-                    return
-        else:
-            datatop = cace_read(datasheet, debug)
+def bindigits(n, bits):
+    s = bin(n & int('1' * bits, 2))[2:]
+    return ('{0:0>%s}' % (bits)).format(s)
 
-        # Ensure that datasheet complies with CACE version 4.0 format
-        dsheet = cace_compat(datatop, debug)
 
-        self.filename = datasheet
-        self.datasheet = dsheet
-        self.create_datasheet_view()
-        self.toppane.title_frame.datasheet_select.configure(text=dsname)
-        self.toppane.title_frame.path_label.configure(text=datasheet)
-
-        # Attempt to set the datasheet viewer width to the interior width
-        # but do not set it larger than the available desktop.
-        self.update_idletasks()
-        widthnow = self.datasheet_viewer.winfo_width()
-        width = self.datasheet_viewer.dframe.winfo_width()
-        screen_width = self.root.winfo_screenwidth()
-        if width > widthnow:
-            if width < screen_width - 10:
-                self.datasheet_viewer.configure(width=width)
-            else:
-                self.datasheet_viewer.configure(width=screen_width - 10)
-        elif widthnow > screen_width:
-            self.datasheet_viewer.configure(width=screen_width - 10)
-        elif widthnow > width:
-            self.datasheet_viewer.configure(width=width)
-
-        # Likewise for the height, up to 3/5 of the desktop height.
-        height = self.datasheet_viewer.dframe.winfo_height()
-        heightnow = self.datasheet_viewer.winfo_height()
-        screen_height = self.root.winfo_screenheight()
-        if height > heightnow:
-            if height < screen_height * 0.6:
-                self.datasheet_viewer.configure(height=height)
-            else:
-                self.datasheet_viewer.configure(height=screen_height * 0.6)
-        elif heightnow > screen_height:
-            self.datasheet_viewer.configure(height=screen_height - 10)
-        elif heightnow > height:
-            self.datasheet_viewer.configure(height=height)
-
-        # Set the current working directory from the datasheet's "path"
-        # dictionary, then reset the root path to the current working
-        # directory.
-        self.set_working_directory(dsheet)
-
-    def choose_datasheet(self):
-        datasheet = filedialog.askopenfilename(
-            multiple=False,
-            initialdir=os.getcwd(),
-            filetypes=(
-                ('Text file', '*.txt'),
-                ('JSON File', '*.json'),
-                ('All Files', '*.*'),
-            ),
-            title='Find a datasheet.',
-        )
-        if datasheet != '':
-            self.set_datasheet(datasheet)
+# -----------------------------------------------------------------------
+# compute the 2's compliment of integer value val
+# -----------------------------------------------------------------------
 
-    def topfilter(self, line):
-        # Check output for ubiquitous "Reference value" lines and remove them.
-        # This happens before logging both to the file and to the console.
-        refrex = re.compile('Reference value')
-        rmatch = refrex.match(line)
-        if not rmatch:
-            return line
-        else:
-            return None
 
-    def spicefilter(self, line):
-        # Check for the alarmist 'tran simulation interrupted' message and remove it.
-        # Check for error or warning and print as stderr or stdout accordingly.
-        intrex = re.compile('tran simulation interrupted')
-        warnrex = re.compile('.*warning', re.IGNORECASE)
-        errrex = re.compile('.*error', re.IGNORECASE)
-
-        imatch = intrex.match(line)
-        if not imatch:
-            ematch = errrex.match(line)
-            wmatch = warnrex.match(line)
-            if ematch or wmatch:
-                print(line, file=sys.stderr)
-            else:
-                print(line, file=sys.stdout)
+def twos_comp(val, bits):
+    if (
+        val & (1 << (bits - 1))
+    ) != 0:   # if sign bit is set e.g., 8bit: 128-255
+        val = val - (1 << bits)        # compute negative value
+    return val                         # return positive value as is
 
-    def printwarn(self, output):
-        # Check output for warning or error
-        if not output:
-            return 0
-
-        warnrex = re.compile('.*warning', re.IGNORECASE)
-        errrex = re.compile('.*error', re.IGNORECASE)
-
-        errors = 0
-        outlines = output.splitlines()
-        for line in outlines:
-            try:
-                wmatch = warnrex.match(line)
-            except TypeError:
-                line = line.decode('utf-8')
-                wmatch = warnrex.match(line)
-            ematch = errrex.match(line)
-            if ematch:
-                errors += 1
-            if ematch or wmatch:
-                print(line)
-        return errors
-
-    def sim_all(self):
-        if self.procs_pending != {}:
-            # Failsafe
-            print('Simulation in progress must finish first.')
-            return
-
-        # Create netlist if necessary, check for valid result
-        if self.sim_param('check') == False:
-            return
-
-        # Simulate all of the electrical parameters in turn.  These
-        # are multiprocessed.
-        for pname in self.status:
-            self.sim_param(pname)
-
-        # Button now stops the simulations
-        self.allsimbutton.configure(
-            style='redtitle.TButton',
-            text='Stop Simulations',
-            command=self.stop_sims,
-        )
 
-    def stop_sims(self):
-        # Make sure there will be no more simulations
+# -----------------------------------------------------------------------
+# Binary sequence counter (used for linear stepping of binary vectors)
+# -----------------------------------------------------------------------
 
-        if self.procs_pending == {}:
-            print('No simulation running.')
-            return
-
-        # Force termination of threads and wait for them to exit.
-        # NOTE:  The processes are nested, so do *not* use "terminate".
-        # Instead, have each process set the same process group and then
-        # send all process groups the SIGUSR1 signal.  Each child will
-        # catch the SIGUSR1 and then terminate itself.
-
-        os.killpg(os.getpid(), signal.SIGUSR1)
-        print('Waiting for all processes to stop.')
-        for procname in self.procs_pending.copy().keys():
-            proc = self.procs_pending[procname]
-            proc.join()
-            self.procs_pending.pop(procname)
-
-        print('All processes have stopped.')
-        self.allsimbutton.configure(
-            style='bluetitle.TButton',
-            text='Simulate All',
-            command=self.sim_all,
-        )
 
-        # Return all individual "Simulate" buttons to normal text
-        for simbname in self.simbuttons.keys():
-            simbutton = self.simbuttons[simbname]
-            simbutton.configure(text='Simulate')
-
-    def edit_param(self, param):
-        # Edit the conditions under which the parameter is tested.
-        if (
-            'editable' in param and param['editable'] == True
-        ) or self.settings.get_edit() == True:
-            self.editparam.populate(param)
-            self.editparam.open()
+def bcount(condition, unit, start, stop, step):
+    blen = len(start)
+    a = safe_eval('0b' + start)
+    e = safe_eval('0b' + stop)
+    if a > e:
+        a = twos_comp(a, blen)
+        e = twos_comp(e, blen)
+    s = int(step)
+    while a < e + s:
+        if a > e:
+            bstr = bindigits(e, blen)
         else:
-            print('Parameter is not editable')
-
-    def copy_param(self, param):
-        # Make a copy of the parameter (for editing)
-        newparam = param.copy()
-        # Make the copied parameter editable
-        newparam['editable'] = True
-        # Append this to the electrical parameter list after the item being copied
-        if 'display' in param:
-            newparam['display'] = param['display'] + ' (copy)'
-        dsheet = self.datasheet
-        eparams = dsheet['electrical_parameters']
-        eidx = eparams.index(param)
-        eparams.insert(eidx + 1, newparam)
-        self.create_datasheet_view()
-
-    def delete_param(self, param):
-        # Remove an electrical parameter from the datasheet.  This is only
-        # allowed if the parameter has been copied from another and so does
-        # not belong to the original set of parameters.
-        dsheet = self.datasheet
-        eparams = dsheet['electrical_parameters']
-        eidx = eparams.index(param)
-        eparams.pop(eidx)
-        self.create_datasheet_view()
-
-    def add_hints(self, param, simbutton):
-        # Raise hints window and configure appropriately for the parameter.
-        # Fill in any existing hints.
-        self.simhints.populate(param, simbutton)
-        self.simhints.open()
-
-    # Run cace_run and drop output onto the indicated queue
-    def cace_process(self, datasheet, name):
-        # Restore output, as the I/O redirection does not work inside
-        # the child process (to do:  fix this?)
-        sys.stdout = self.stdout
-        sys.stderr = self.stderr
-
-        # Set group ID for signaling.  Use the parent process ID as the group ID
-        runtime_options = datasheet['runtime_options']
-        if 'pid' in runtime_options:
-            os.setpgid(os.getpid(), runtime_options['pid'])
-            signal.signal(signal.SIGUSR1, child_process_exit)
-
-        charresult = cace_run(datasheet, name)
-        charresult['simname'] = name
-        self.queue.put(charresult)
-        sys.stdout.flush()
-        sys.stderr.flush()
-
-    # Get the value for runtime options['netlist_source']
-    def get_netlist_source(self):
-        netlist_text = self.origin.get()
-        if netlist_text == 'Schematic Capture':
-            return 'schematic'
-        elif netlist_text == 'Layout Extracted':
-            return 'layout'
-        elif netlist_text == 'C Extracted':
-            return 'pex'
-        elif netlist_text == 'R-C Extracted':
-            return 'rcx'
+            bstr = bindigits(a, blen)
+        yield (condition, unit, bstr)
+        a = a + s
+
+
+# -----------------------------------------------------------------------
+# Binary sequence shifter (used for logarithmic stepping of binary
+# vectors)
+# -----------------------------------------------------------------------
+
+
+def bshift(condition, unit, start, stop, step):
+    a = safe_eval('0b' + start)
+    e = safe_eval('0b' + stop)
+    if a > e:
+        a = twos_comp(a, blen)
+        e = twos_comp(e, blen)
+    s = int(step)
+    while a < e * s:
+        if a > e:
+            bstr = bindigits(e, blen)
         else:
-            print('Unhandled netlist source ' + netlist_text)
-            print('Reverting to schematic.')
-            return 'schematic'
-
-    # Simulate a parameter (or run a physical parameter evaluation)
-    def sim_param(self, name):
-        dsheet = self.datasheet
+            bstr = bindigits(a, blen)
+        yield (condition, unit, bstr)
+        a = a * s
+
+
+# -----------------------------------------------------------------------
+# Define a generator for conditions.  Given a condition (dictionary),
+# return (as a yield) each specified condition as a 3-tuple
+# (condition_type, value, unit)
+# -----------------------------------------------------------------------
+
+
+def condition_gen(cond):
+    lcond = cond['name']
+    if 'unit' in cond:
+        unit = cond['unit']
+    else:
+        unit = ''
 
-        if 'runtime_options' in dsheet:
-            runtime_options = dsheet['runtime_options']
+    if 'enumerate' in cond:
+        for i in cond['enumerate']:
+            yield (lcond, unit, i)
+    elif 'maximum' in cond and 'step' in cond and cond['step'] == 'linear':
+        minimum = cond['minimum'] if 'minimum' in cond else 1
+        if unit == "'b" or '[' in lcond:
+            yield from bcount(
+                lcond, unit, minimum, cond['maximum'], cond['stepsize']
+            )
         else:
-            runtime_options = {}
-            dsheet['runtime_options'] = runtime_options
-
-        runtime_options['netlist_source'] = self.get_netlist_source()
-        runtime_options['force'] = self.settings.get_force()
-        runtime_options['keep'] = self.settings.get_keep()
-        runtime_options['sequential'] = self.settings.get_sequential()
-        runtime_options['noplot'] = self.settings.get_noplot()
-        runtime_options['debug'] = self.settings.get_debug()
-
-        if (
-            'electrical_parameters' not in dsheet
-            and 'physical_parameters' not in dsheet
-        ):
-            print('Error running parameter check on ' + name)
-            print('No parameters found in datasheet')
-            print('Datasheet entries are:')
-            for key in dsheet.keys():
-                print(key)
-            return
-
-        if name == 'check':
-            # For the special keyword "check", do not multiprocess,
-            # and return a pass/fail result according to the runtime status.
-            cace_run(dsheet, name)
-            if 'status' in runtime_options:
-                status = runtime_options['status']
-                runtime_options.pop('status')
-                if status == 'failed':
-                    return False
-            return True
-
-        try:
-            eparam = next(
-                item
-                for item in dsheet['electrical_parameters']
-                if item['name'] == name
+            print('Diagnostic: yield from linseq')
+            yield from linseq(
+                lcond, unit, minimum, cond['maximum'], cond['stepsize']
+            )
+    elif (
+        'maximum' in cond and 'step' in cond and cond['step'] == 'logarithmic'
+    ):
+        minimum = cond['minimum'] if 'minimum' in cond else 1
+        if unit == "'b" or '[' in lcond:
+            yield from bshift(
+                lcond, unit, minimum, cond['maximum'], cond['stepsize']
             )
-        except:
-            try:
-                pparam = next(
-                    item
-                    for item in dsheet['physical_parameters']
-                    if item['name'] == name
-                )
-            except:
-                print('Unknown parameter "' + name + '"')
-                if 'electrical_parameters' in dsheet:
-                    print('Known electrical parameters are:')
-                    for eparam in dsheet['electrical_parameters']:
-                        print(eparam['name'])
-                if 'physical_parameters' in dsheet:
-                    print('Known physical parameters are:')
-                    for pparam in dsheet['physical_parameters']:
-                        print(pparam['name'])
-                return
-            else:
-                param = pparam
         else:
-            param = eparam
-
-        if name in self.procs_pending:
-            print(
-                'Process already running. . . Cancel process before re-running'
+            yield from logseq(
+                lcond, unit, minimum, cond['maximum'], cond['stepsize']
             )
-            return
-
-        # From the GUI, simulation is forced, so clear any "skip" status.
-        # TO DO:  "gray out" entries marked as "skip" and require entry to
-        # be set to "active" before simulating.
-        if 'status' in param:
-            if param['status'] == 'skip':
-                print(
-                    'Note: Parameter status changed from "skip" to "active".'
-                )
-                param['status'] = 'active'
+    elif 'minimum' in cond and 'maximum' in cond and 'typical' in cond:
+        yield (lcond, unit, cond['minimum'])
+        yield (lcond, unit, cond['typical'])
+        yield (lcond, unit, cond['maximum'])
+    elif 'minimum' in cond and 'maximum' in cond:
+        yield (lcond, unit, cond['minimum'])
+        yield (lcond, unit, cond['maximum'])
+    elif 'minimum' in cond and 'typical' in cond:
+        yield (lcond, unit, cond['minimum'])
+        yield (lcond, unit, cond['typical'])
+    elif 'maximum' in cond and 'typical' in cond:
+        yield (lcond, unit, cond['typical'])
+        yield (lcond, unit, cond['maximum'])
+    elif 'minimum' in cond:
+        yield (lcond, unit, cond['minimum'])
+    elif 'maximum' in cond:
+        yield (lcond, unit, cond['maximum'])
+    elif 'typical' in cond:
+        yield (lcond, unit, cond['typical'])
+
+
+# -----------------------------------------------------------------------
+# Find the maximum time to run a simulation.  This is the maximum of:
+# (1) maximum value, if parameter is RISETIME or FALLTIME, and (2) maximum
+# RISETIME or FALLTIME of any condition.
+#
+# "lcondlist" is the list of local conditions extended by the list of
+# all global conditions that are not overridden by local values.
+#
+# NOTE:  This list is limited to rise and fall time values, as they are
+# the only time constraints known to cace_gensim at this time.  This list
+# will be extended as more simulation parameters are added.
+# -----------------------------------------------------------------------
 
-        # Set the "Simulate" button to say "in progress"
-        simbutton = self.simbuttons[name]
-        simbutton.configure(text='(in progress)')
 
-        # Diagnostic
-        print('Simulating parameter ' + name)
-        # NOTE: Commenting out the following line prevents the use of
-        # the process ID to set a common group ID that can be used to
-        # stop simulations by sending a kill signal to all threads.
-        # The method is not working, and on some systems os.setpgid()
-        # will not run.
-        #
-        # runtime_options['pid'] = os.getpid()
-        p = multiprocessing.Process(
-            target=self.cace_process,
-            args=(
-                dsheet,
-                name,
-            ),
-        )
-        # Save process pointer so it can be joined after it finishes.
-        self.procs_pending[name] = p
-        p.start()
-
-        # Call watchproc() to start periodically watching the queue for
-        # simulation results.
-        self.watchproc()
-
-    def watchproc(self):
-        # Routine which is turned on when a cace_run
-        # process is spawned, and periodically checks to see if a result
-        # is available on the queue.  If so, then it pulls the datasheet
-        # result from the queue, merges it back into the datasheet, joins
-        # the spawned process, and removes the process from the list of
-        # pending processes.  If the list of pending processes is not empty,
-        # then watchproc() sets a timer to repeat itself.
-
-        # If nothing is pending then return immediately and do not set a
-        # repeat check.
-        if self.procs_pending == {}:
-            return
-
-        # Check queue, non-blocking
-        debug = self.settings.get_debug()
-        try:
-            charresult = self.queue.get(block=False)
-        except:
-            if debug:
-                print(
-                    'Watchproc found nothing in the queue; will wait longer.'
+def findmaxtime(param, lcondlist):
+    maxtime = 0.0
+    try:
+        simunit = param['unit']
+    except KeyError:
+        # Plots has no min/max/typ so doesn't require units.
+        if 'plot' in param:
+            return maxtime
+
+    maxval = 0.0
+    found = False
+    if 'maximum' in param:
+        prec = param['maximum']
+        if 'target' in prec:
+            pmax = prec['target']
+            try:
+                maxval = numeric(spice_unit_convert([simunit, pmax], 'time'))
+                found = True
+            except:
+                pass
+    if not found and 'typical' in param:
+        prec = param['typical']
+        if 'target' in prec:
+            ptyp = prec['target']
+            try:
+                maxval = numeric(spice_unit_convert([simunit, ptyp], 'time'))
+                found = True
+            except:
+                pass
+    if not found and 'minimum' in param:
+        prec = param['minimum']
+        if 'target' in prec:
+            pmin = prec['target']
+            try:
+                maxval = numeric(spice_unit_convert([simunit, pmin], 'time'))
+                found = True
+            except:
+                pass
+    if maxval > maxtime:
+        maxtime = maxval
+    for cond in lcondlist:
+        condtype = cond['name'].split(':', 1)[0]
+        if condtype == 'RISETIME' or condtype == 'FALLTIME':
+            condunit = cond['unit']
+            maxval = 0.0
+            if 'maximum' in cond:
+                maxval = numeric(
+                    spice_unit_convert([condunit, cond['maximum']], 'time')
                 )
-            # Set watchproc to repeat after 1/2 second
-            self.after(500, lambda: self.watchproc())
-            return
-        else:
-            newparam = None
-            iseparam = True
-            pname = charresult['simname']
-
-            # Return "Simulate" button to original text
-            simbutton = self.simbuttons[pname]
-            simbutton.configure(text='Simulate')
-
-            print('Simulation of ' + pname + ' has completed.')
-            if 'electrical_parameters' in charresult:
-                eparams = charresult['electrical_parameters']
-                for param in eparams:
-                    if param['name'] == pname:
-                        newparam = param
-                        break
-            if newparam == None and 'physical_parameters' in charresult:
-                pparams = charresult['physical_parameters']
-                for param in pparams:
-                    if param['name'] == pname:
-                        newparam = param
-                        iseparam = False
-                        break
-            if newparam == None:
-                print('Simulation failure on ' + pname + '.')
-                return
-
-            if not param:
-                print('Error:  parameter ' + pname + ' not found in results!')
-                return
-
-            if pname in self.procs_pending:
-                p = self.procs_pending[pname]
-                self.procs_pending.pop(pname)
-                if debug:
-                    print('Now waiting to join process')
-                p.join()
-                if self.procs_pending == {}:
-                    self.allsimbutton.configure(
-                        style='bluetitle.TButton',
-                        text='Simulate All',
-                        command=self.sim_all,
+            elif 'enumerate' in cond:
+                maxval = numeric(
+                    spice_unit_convert(
+                        [condunit, cond['enumerate'][-1]], 'time'
                     )
-            else:
-                print(
-                    'Error:  Parameter '
-                    + pname
-                    + ' has results but no process!'
                 )
+            elif 'typical' in cond:
+                maxval = numeric(
+                    spice_unit_convert([condunit, cond['typical']], 'time')
+                )
+            elif 'minimum' in cond:
+                maxval = numeric(
+                    spice_unit_convert([condunit, cond['minimum']], 'time')
+                )
+            if maxval > maxtime:
+                maxtime = maxval
 
-            # Replace the parameter in the master datasheet
-            if 'electrical_parameters' in charresult and iseparam:
-                eparamlist = self.datasheet['electrical_parameters']
-                for i in range(0, len(eparamlist)):
-                    checkparam = eparamlist[i]
-                    if checkparam['name'] == pname:
-                        eparamlist[i] = newparam
-                        break
-
-            if 'physical_parameters' in charresult and not iseparam:
-                pparamlist = self.datasheet['physical_parameters']
-                for i in range(0, len(pparamlist)):
-                    checkparam = pparamlist[i]
-                    if checkparam['name'] == pname:
-                        pparamlist[i] = newparam
-                        break
-
-            # Regenerate datasheet view with parameter results
-            self.create_datasheet_view()
+    return maxtime
 
-    def clear_results(self, dsheet):
-        # Remove results from the window by clearing parameter results
-        paramstodo = []
-        if 'electrical_parameters' in dsheet:
-            paramstodo.extend(dsheet['electrical_parameters'])
-        if 'physical_parameters' in dsheet:
-            paramstodo.extend(dsheet['physical_parameters'])
-
-        for param in paramstodo:
-            # Fill frame with electrical parameter information
-            if 'max' in param:
-                maxrec = param['max']
-                if 'value' in maxrec:
-                    maxrec.pop('value')
-                if 'score' in maxrec:
-                    maxrec.pop('score')
-            if 'typ' in param:
-                typrec = param['typ']
-                if 'value' in typrec:
-                    typrec.pop('value')
-                if 'score' in typrec:
-                    typrec.pop('score')
-            if 'min' in param:
-                minrec = param['min']
-                if 'value' in minrec:
-                    minrec.pop('value')
-                if 'score' in minrec:
-                    minrec.pop('score')
-            if 'results' in param:
-                param.pop('results')
-
-            if 'plot' in param:
-                plotrec = param['plot']
-                if 'status' in plotrec:
-                    plotrec.pop('status')
-
-        # Regenerate datasheet view
-        self.create_datasheet_view()
-
-    def annotate(self, suffix, checktime):
-        # Pull results back from datasheet_anno.json.  Do NOT load this
-        # file if it predates the unannotated datasheet (that indicates
-        # simulator failure, and no results).
-        dspath = os.path.split(self.filename)[0]
-        if dspath == '':
-            dspath = '.'
-        dsdir = dspath + '/ngspice'
-        anno = dsdir + '/datasheet_' + suffix + '.json'
-        unanno = dsdir + '/datasheet.json'
-
-        if os.path.exists(anno):
-            statbuf = os.stat(anno)
-            mtimea = statbuf.st_mtime
-            if checktime >= mtimea:
-                # print('original = ' + str(checktime) + ' annotated = ' + str(mtimea))
-                print(
-                    'Error in simulation, no update to results.',
-                    file=sys.stderr,
-                )
-            elif statbuf.st_size == 0:
-                print('Error in simulation, no results.', file=sys.stderr)
-            elif os.path.splitext(anno)[1] == '.json':
-                with open(anno, 'r') as file:
-                    self.datasheet = json.load(file)
-            else:
-                debug = self.settings.get_debug()
-                self.datasheet = cace_read(file, debug)
-        else:
-            print(
-                'Error in simulation, no update to results.', file=sys.stderr
-            )
 
-        # Regenerate datasheet view
-        self.create_datasheet_view()
+# -----------------------------------------------------------------------
+# Picked up from StackOverflow:  Procedure to remove non-unique entries
+# in a list of lists (as always, thanks StackOverflow!).
+# -----------------------------------------------------------------------
 
-        # Close log file, if it was enabled in the settings
-        self.logstop()
 
-    def save_results(self):
-        # Write datasheet_save with all the locally processed results.
-        dspath = os.path.split(self.filename)[0]
-
-        # Save to simulation directory (may want to change this)
-        dsheet = self.datasheet
-        paths = dsheet['paths']
-        dsdir = os.path.join(dspath, paths['root'], paths['simulation'])
-
-        dfile = os.path.split(self.filename)[1]
-        dfileroot = os.path.splitext(dfile)[0]
-        dfileext = os.path.splitext(dfile)[1]
-
-        # Output filename is the input datasheet filename + "_save",
-        # and the same file extension.
-        doutname = dfileroot + '_save' + dfileext
-        doutfile = os.path.join(dsdir, doutname)
-
-        if dfileext == '.json':
-            with open(doutfile, 'w') as ofile:
-                json.dump(self.datasheet, ofile, indent=4)
-        else:
-            # NOTE:  This file contains the run-time settings dictionary
-            cace_write(self.datasheet, doutfile)
+def uniquify(seq):
+    seen = set()
+    return [x for x in seq if str(x) not in seen and not seen.add(str(x))]
 
-        self.last_save = os.path.getmtime(doutfile)
 
-        print('Characterization results saved.')
+# -----------------------------------------------------------------------
+# Replace the substitution token {INCLUDE_DUT} with the contents of the
+# DUT subcircuit netlist file.  "functional" is a list of IP block names
+# that are to be searched for in .include lines in the netlist and
+# replaced with functional view equivalents (if such exist).
+# -----------------------------------------------------------------------
 
-    def check_saved(self):
-        # Check if there is a file 'datasheet_save' and if it is more
-        # recent than 'datasheet_anno'.  If so, return True, else False.
 
-        [dspath, dsname] = os.path.split(self.filename)
-        dsdir = dspath + '/ngspice'
+def inline_dut(filename, functional, rootpath, ofile):
 
-        savefile = dsdir + '/datasheet_save.json'
+    # SPICE comment
+    comtrex = re.compile(r'^\*')
 
-        annofile = dsdir + '/datasheet_anno.json'
-        if os.path.exists(annofile):
-            annotime = os.path.getmtime(annofile)
+    # SPICE include statement
+    inclrex = re.compile(
+        r'[ \t]*\.include[ \t]+["\']?([^"\' \t]+)["\']?', re.IGNORECASE
+    )
 
-            # If nothing has been updated since the characterization
-            # tool was started, then there is no new information to save.
-            if annotime < self.starttime:
-                return True
+    # Node name with brackets
+    braktrex = re.compile(r'([^ \t]+)\[([^ \t])\]', re.IGNORECASE)
 
-            if os.path.exists(savefile):
-                savetime = os.path.getmtime(savefile)
-                # return True if (savetime > annotime) else False
-                if savetime > annotime:
-                    print('Save is more recent than sim, so no need to save.')
-                    return True
-                else:
-                    print('Sim is more recent than save, so need to save.')
-                    return False
-            else:
-                # There is a datasheet_anno file but no datasheet_save,
-                # so there are necessarily unsaved results.
-                print('no datasheet_save, so any results have not been saved.')
-                return False
-        else:
-            # There is no datasheet_anno file, so datasheet_save
-            # is either current or there have been no simulations.
-            print('no datasheet_anno, so there are no results to save.')
-            return True
-
-    def save_manual(self, value={}):
-        dspath = self.filename
-        # Set initialdir to the project where datasheet is located
-        dsparent = os.path.split(dspath)[0]
-
-        datasheet = filedialog.asksaveasfilename(
-            initialdir=dsparent,
-            confirmoverwrite=True,
-            defaultextension='.txt',
-            filetypes=(
-                ('Text file', '*.txt'),
-                ('JSON File', '*.json'),
-                ('All Files', '*.*'),
-            ),
-            title='Select filename for saved datasheet.',
-        )
+    # SPICE subcircuit line
+    subcrex = re.compile(r'[ \t]*x([^ \t]+)[ \t]+(.*)$', re.IGNORECASE)
 
-        if isinstance(datasheet, str):
-            if os.path.splitext(datasheet)[1] == '.json':
-                with open(datasheet, 'w') as ofile:
-                    json.dump(self.datasheet, ofile, indent=4)
+    librex = re.compile(r'(.*)__(.*)', re.IGNORECASE)
+    endrex = re.compile(r'[ \t]*\.end[ \t]*', re.IGNORECASE)
+    endsrex = re.compile(r'[ \t]*\.ends[ \t]*', re.IGNORECASE)
+
+    # IP names in the form
+    # <user_path>/design/<project>/spi/<spice-type>/<proj_netlist>
+
+    locpathrex = re.compile(r'(.+)/design/([^/]+)/spi/([^/]+)/([^/ \t]+)')
+    altpathrex = re.compile(r'(.+)/design/([^/]+)/([^/]+)/([^/]+)/([^/ \t]+)')
+
+    # To be completed
+    with open(filename, 'r') as ifile:
+        nettext = ifile.read()
+
+    netlines = nettext.replace('\n+', ' ').splitlines()
+    for line in netlines:
+        subsline = line
+        cmatch = comtrex.match(line)
+        if cmatch:
+            print(line, file=ofile)
+            continue
+        # Check for ".end" which should be removed (but not ".ends", which must remain)
+        ematch = endrex.match(line)
+        if ematch:
+            smatch = endsrex.match(line)
+            if not smatch:
+                continue
+        imatch = inclrex.match(line)
+        if imatch:
+            incpath = imatch.group(1)
+            # Substitution behavior is complicated due to the difference between netlist
+            # files from schematic capture vs. layout and read-only vs. read-write IP.
+            incroot = os.path.split(incpath)[1]
+            incname = os.path.splitext(incroot)[0]
+            lmatch = librex.match(incname)
+            if lmatch:
+                ipname = lmatch.group(2)
             else:
-                cace_write(self.datasheet, datasheet)
-
-    def load_manual(self, value={}):
-        dspath = self.filename
-        # Set initialdir to the project where datasheet is located
-        dsparent = os.path.split(dspath)[0]
-
-        datasheet = filedialog.askopenfilename(
-            multiple=False,
-            initialdir=dsparent,
-            filetypes=(
-                ('Text file', '*.txt'),
-                ('JSON File', '*.json'),
-                ('All Files', '*.*'),
-            ),
-            title='Find a datasheet.',
-        )
-        if datasheet != '':
-            print('Reading file ' + datasheet)
-            if os.path.splitext(datasheet)[1] == '.json':
-                with open(datasheet, 'r') as file:
-                    try:
-                        self.datasheet = json.load(file)
-                    except:
-                        print(
-                            'Error in file, no update to results.',
-                            file=sys.stderr,
+                ipname = incname
+            if ipname.upper() in functional:
+                # Search for functional view (depends on if this is a read-only IP or
+                # read-write local subcircuit)
+                funcpath = None
+                ippath = ippathrex.match(incpath)
+                if ippath:
+                    userpath = ippath.group(1)
+                    ipname2 = ippath.group(2)
+                    ipversion = ippath.group(3)
+                    spitype = ippath.group(4)
+                    ipname3 = ippath.group(5)
+                    ipnetlist = ippath.group(6)
+                    funcpath = (
+                        userpath
+                        + '/design/ip/'
+                        + ipname2
+                        + '/'
+                        + ipversion
+                        + '/spice-func/'
+                        + ipname
+                        + '.spice'
+                    )
+                else:
+                    locpath = locpathrex.match(incpath)
+                    if locpath:
+                        userpath = locpath.group(1)
+                        ipname2 = locpath.group(2)
+                        spitype = locpath.group(3)
+                        ipnetlist = locpath.group(4)
+                        funcpath = (
+                            userpath
+                            + '/design/'
+                            + ipname2
+                            + '/spi/func/'
+                            + ipname
+                            + '.spice'
                         )
                     else:
-                        # Regenerate datasheet view
-                        self.create_datasheet_view()
-            else:
-                debug = self.settings.get_debug()
-                try:
-                    self.datasheet = cace_read(datasheet, debug)
-                except:
+                        altpath = altpathrex.match(incpath)
+                        if altpath:
+                            userpath = altpath.group(1)
+                            ipname2 = altpath.group(2)
+                            spitype = altpath.group(3)
+                            ipname3 = altpath.group(4)
+                            ipnetlist = altpath.group(5)
+                            funcpath = (
+                                userpath
+                                + '/design/'
+                                + ipname2
+                                + '/spi/func/'
+                                + ipname
+                                + '.spice'
+                            )
+
+                funcpath = os.path.expanduser(funcpath)
+                if funcpath and os.path.exists(funcpath):
+                    print('Subsituting functional view for IP block ' + ipname)
+                    print('Original netlist is ' + incpath)
+                    print('Functional netlist is ' + funcpath)
+                    subsline = '.include ' + funcpath
+                elif funcpath:
+                    print('Original netlist is ' + incpath)
                     print(
-                        'Error in file, no update to results.', file=sys.stderr
+                        'Functional view specified but no functional view found.'
                     )
+                    print('Tried looking for ' + funcpath)
+                    print('Retaining original view.')
                 else:
-                    # Regenerate datasheet view
-                    self.set_working_directory(self.datasheet)
-                    self.create_datasheet_view()
-
-    def generate_html(self, value={}):
-        debug = self.settings.get_debug()
-        cace_generate_html(self.datasheet, None, debug)
-
-    def swap_results(self, value={}):
-        # This routine just calls self.create_datasheet_view(), but the
-        # button callback has an argument that needs to be handled even
-        # if it is just discarded.
-        self.create_datasheet_view()
-
-    def load_results(self, value={}):
-
-        # Check if datasheet_save exists and is more recent than the
-        # latest design netlist.  If so, load it;  otherwise, not.
-        # NOTE:  Name of .spice file comes from the project 'name'
-        # in the datasheet.
-
-        [dspath, dsname] = os.path.split(self.filename)
-        try:
-            dsheet = self.datasheet
-        except KeyError:
-            return
-
-        if dspath == '':
-            dspath = '.'
-
-        dsroot = dsheet['name']
-
-        # Remove any existing results from the datasheet records
-        self.clear_results(dsheet)
-
-        # Also must be more recent than datasheet
-        jtime = os.path.getmtime(self.filename)
-
-        # dsroot = os.path.splitext(dsname)[0]
-
-        paths = dsheet['paths']
-        dsdir = os.path.join(dspath, paths['root'], paths['simulation'])
-
-        if not os.path.exists(dsdir):
-            # Try 'spice' as a subdirectory of the datasheet directory as a
-            # fallback.
-            dsdir = dspath + '/spice'
-            if not os.path.exists(dsdir):
-                print('Error:  Cannot find directory spice/ in path ' + dspath)
-
-        if self.origin.get() == 'Layout Extracted':
-            spifile = dsdir + '/layout/' + dsroot + '.spice'
-        if self.origin.get() == 'C Extracted':
-            spifile = dsdir + '/pex/' + dsroot + '.spice'
-        elif self.origin.get() == 'R-C Extracted':
-            spifile = dsdir + '/rcx/' + dsroot + '.spice'
-        else:
-            spifile = dsdir + '/' + dsroot + '.spice'
+                    print('Original netlist is ' + incpath)
+                    print(
+                        'Cannot make sense of netlist path to find functional view.'
+                    )
 
-        dsdir = dspath + '/ngspice'
-        savefile = dsdir + '/datasheet_save.json'
+        # If include file name is in <lib>__<cell> format (from electric) and the
+        # functional view is not, then find the subcircuit call and replace the
+        # subcircuit name.  At least at the moment, the vice versa case does not
+        # happen.
+
+        smatch = subcrex.match(line)
+        if smatch:
+            subinst = smatch.group(1)
+            tokens = smatch.group(2).split()
+            # Need to test for parameters passed to subcircuit.  The actual subcircuit
+            # name occurs before any parameters.
+            params = []
+            pins = []
+            for token in tokens:
+                if '=' in token:
+                    params.append(token)
+                else:
+                    pins.append(token)
 
-        if os.path.exists(savefile):
-            savetime = os.path.getmtime(savefile)
+            subname = pins[-1]
+            pins = pins[0:-1]
+            lmatch = librex.match(subname)
+            if lmatch:
+                testname = lmatch.group(1)
+                if testname.upper() in functional:
+                    subsline = (
+                        'X'
+                        + subinst
+                        + ' '
+                        + ' '.join(pins)
+                        + ' '
+                        + testname
+                        + ' '
+                        + ' '.join(params)
+                    )
 
-        if os.path.exists(spifile):
-            spitime = os.path.getmtime(spifile)
-
-            if os.path.exists(savefile):
-                if savetime > spitime and savetime > jtime:
-                    self.annotate('save', 0)
-                    print('Characterization results loaded.')
-                    # print('(' + savefile + ' timestamp = ' + str(savetime) + '; ' + self.datasheet + ' timestamp = ' + str(jtime))
-                else:
-                    print('Saved datasheet is out-of-date, not loading')
-            else:
-                print('Datasheet file ' + savefile)
-                print('No saved datasheet file, nothing to pre-load')
-        else:
-            print('No netlist file ' + spifile + '!')
+        # Remove any array brackets from node names in the top-level subcircuit,
+        # because they interfere with the array notation used by XSPICE which may
+        # be present in functional views (replace bracket characters with
+        # underscores).
+        #
+        # subsline = subsline.replace('[', '_').replace(']', '_')
+        #
+        # Do this *only* when there are no spaces inside the brackets, or else
+        # any XSPICE primitives in the netlist containing arrays will get messed
+        # up.
+        subsline = braktrex.sub(r'\1_\2_', subsline)
 
-        # Remove outdated datasheet.json and datasheet_anno.json to prevent
-        # them from overwriting characterization document entries
+        ofile.write(subsline + '\n')
 
-        if os.path.exists(savefile):
-            if savetime < jtime:
-                print('Removing outdated save file ' + savefile)
-                os.remove(savefile)
-
-        savefile = dsdir + '/datasheet_anno.json'
-        if os.path.exists(savefile):
-            savetime = os.path.getmtime(savefile)
-            if savetime < jtime:
-                print('Removing outdated results file ' + savefile)
-                os.remove(savefile)
-
-        savefile = dsdir + '/datasheet.json'
-        if os.path.exists(savefile):
-            savetime = os.path.getmtime(savefile)
-            if savetime < jtime:
-                print('Removing outdated results file ' + savefile)
-                os.remove(savefile)
-
-    def create_datasheet_view(self):
-        dframe = self.datasheet_viewer.dframe
-
-        # Destroy the existing datasheet frame contents (if any)
-        for widget in dframe.winfo_children():
-            widget.destroy()
-        self.status = {}  	# Clear dictionary
-
-        dsheet = self.datasheet
-        if 'runtime_options' in dsheet:
-            runtime_options = dsheet['runtime_options']
-        else:
-            runtime_options = {}
-            dsheet['runtime_options'] = runtime_options
+    ofile.write('\n')
 
-        runtime_options['netlist_source'] = self.get_netlist_source()
 
-        # Add basic information at the top
+# -----------------------------------------------------------------------
+# Read a template file and record all of the variable names that will
+# be substituted, so it is clear which local and global conditions
+# need to be enumerated.  Vectors are reduced to just the vector name.
+#
+# Returns a dictionary with keys corresponding to condition names;
+# the dictionary values are unused and just set to "True".
+# -----------------------------------------------------------------------
 
-        n = 0
-        dframe.cframe = ttk.Frame(dframe)
-        dframe.cframe.grid(column=0, row=n, sticky='ewns', columnspan=10)
 
-        dframe.cframe.plabel = ttk.Label(
-            dframe.cframe, text='Project IP name:', style='italic.TLabel'
-        )
-        dframe.cframe.plabel.grid(column=0, row=n, sticky='ewns', ipadx=5)
-        dframe.cframe.pname = ttk.Label(
-            dframe.cframe, text=dsheet['name'], style='normal.TLabel'
-        )
-        dframe.cframe.pname.grid(column=1, row=n, sticky='ewns', ipadx=5)
-        if 'foundry' in dsheet:
-            dframe.cframe.fname = ttk.Label(
-                dframe.cframe, text=dsheet['foundry'], style='normal.TLabel'
-            )
-            dframe.cframe.fname.grid(column=2, row=n, sticky='ewns', ipadx=5)
-        if 'PDK' in dsheet:
-            dframe.cframe.fname = ttk.Label(
-                dframe.cframe, text=dsheet['PDK'], style='normal.TLabel'
-            )
-            dframe.cframe.fname.grid(column=3, row=n, sticky='ewns', ipadx=5)
-        if 'description' in dsheet:
-            dframe.cframe.pdesc = ttk.Label(
-                dframe.cframe,
-                text=dsheet['description'],
-                style='normal.TLabel',
-            )
-            dframe.cframe.pdesc.grid(column=4, row=n, sticky='ewns', ipadx=5)
+def get_condition_names_used(testbenchpath, testbench):
 
-        n = 1
-        ttk.Separator(dframe, orient='horizontal').grid(
-            column=0, row=n, sticky='ewns', columnspan=10
-        )
+    template = os.path.join(testbenchpath, testbench)
+    if not os.path.isfile(template):
+        print('Error:  No such template file ' + template)
+        return
 
-        # Title block
-        n += 1
-        dframe.desc_title = ttk.Label(
-            dframe, text='Parameter', style='title.TLabel'
-        )
-        dframe.desc_title.grid(column=0, row=n, sticky='ewns')
-        dframe.method_title = ttk.Label(
-            dframe, text='Testbench', style='title.TLabel'
-        )
-        dframe.method_title.grid(column=1, row=n, sticky='ewns')
-        dframe.min_title = ttk.Label(dframe, text='Min', style='title.TLabel')
-        dframe.min_title.grid(column=2, row=n, sticky='ewns', columnspan=2)
-        dframe.typ_title = ttk.Label(dframe, text='Typ', style='title.TLabel')
-        dframe.typ_title.grid(column=4, row=n, sticky='ewns', columnspan=2)
-        dframe.max_title = ttk.Label(dframe, text='Max', style='title.TLabel')
-        dframe.max_title.grid(column=6, row=n, sticky='ewns', columnspan=2)
-        dframe.stat_title = ttk.Label(
-            dframe, text='Status', style='title.TLabel'
-        )
-        dframe.stat_title.grid(column=8, row=n, sticky='ewns')
+    with open(template, 'r') as ifile:
+        simtext = ifile.read()
 
-        if self.procs_pending == {}:
-            self.allsimbutton = ttk.Button(
-                dframe,
-                text='Simulate All',
-                style='bluetitle.TButton',
-                command=self.sim_all,
-            )
-        else:
-            self.allsimbutton = ttk.Button(
-                dframe,
-                text='Stop Simulations',
-                style='redtitle.TButton',
-                command=self.stop_sims,
-            )
-        self.allsimbutton.grid(column=9, row=n, sticky='ewns')
+    simlines = simtext.splitlines()
+    condlist = {}
 
-        ToolTip(self.allsimbutton, text='Simulate all electrical parameters')
+    # Regular expressions
+    # varex:		variable name {name}
+    varex = re.compile(r'\{([^ \}\t]+)\}')
 
-        # Make all columns equally expandable
-        for i in range(10):
-            dframe.columnconfigure(i, weight=1)
-
-        # Parse the file for electrical parameters
-        n += 1
-        binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
-        paramstodo = []
-        if 'electrical_parameters' in dsheet:
-            paramstodo.extend(dsheet['electrical_parameters'])
-        if 'physical_parameters' in dsheet:
-            paramstodo.extend(dsheet['physical_parameters'])
+    # Vectors in name[number|range] format
+    vectrex = re.compile(r'([^\[]+)\[([0-9:]+)\]')
 
-        if self.origin.get() == 'Schematic Capture':
-            isschem = True
-        else:
-            isschem = False
+    for line in simlines:
+        for patmatch in varex.finditer(line):
+            pattern = patmatch.group(1)
 
-        # Track the "Simulate" buttons by parameter name (dictionary)
-        self.simbuttons = {}
+            # For condition names in the form {cond=value}, use only the name
+            if '=' in pattern:
+                pattern = pattern.split('=')[0]
 
-        for param in paramstodo:
-            pname = param['name']
-            # Fill frame with electrical parameter information
-            if 'simulate' in param:
-                mdict = param['simulate']
-                p = mdict['template']
-                if pname in self.status:
-                    # This method was used before, so give it a unique identifier
-                    j = 1
-                    while True:
-                        pname = p + '.' + str(j)
-                        if pname not in self.status:
-                            break
-                        else:
-                            j += 1
-                else:
-                    j = 0
-                paramtype = 'electrical'
-            elif 'evaluate' in param:
-                paramtype = 'physical'
-                mdict = param['evaluate']
-                p = mdict['tool']
-                if isinstance(p, list):
-                    p = p[0]
-                j = 0
-            else:
-                p = 'none'
-                paramtype = 'unknown'
-                print('Parameter ' + pname + ' unknown type.')
-
-            if 'editable' in param and param['editable'] == True:
-                normlabel = 'hlight.TLabel'
-                redlabel = 'rhlight.TLabel'
-                greenlabel = 'ghlight.TLabel'
-                normbutton = 'hlight.TButton'
-                redbutton = 'rhlight.TButton'
-                greenbutton = 'ghlight.TButton'
-            else:
-                normlabel = 'normal.TLabel'
-                redlabel = 'red.TLabel'
-                greenlabel = 'green.TLabel'
-                normbutton = 'normal.TButton'
-                redbutton = 'red.TButton'
-                greenbutton = 'green.TButton'
+            # For condition names in the form {cond|value}, use only the name
+            if '|' in pattern:
+                pstart = pattern.split('|')[0]
+                if pstart != 'PIN' and pstart != 'FUNCTIONAL':
+                    pattern = pstart
 
-            if 'display' in param:
-                dtext = param['display']
-            else:
-                dtext = p
+            pmatch = vectrex.match(pattern)
+            if pmatch:
+                pattern = pmatch.group(1) + '['
+            condlist[pattern] = True
 
-            # Special handling:  Change LVS_errors to "device check" when using
-            # schematic netlist.
-            if paramtype == 'physical':
-                if isschem:
-                    if p == 'cace_lvs':
-                        dtext = 'Invalid device check'
-                    if p == 'cace_area':
-                        dtext = 'Area estimate'
-
-            dframe.description = ttk.Label(dframe, text=dtext, style=normlabel)
-
-            dframe.description.grid(column=0, row=n, sticky='ewns')
-            dframe.method = ttk.Label(dframe, text=p, style=normlabel)
-            dframe.method.grid(column=1, row=n, sticky='ewns')
-            if 'plot' in param:
-                # For plots, the status still comes from the 'results' dictionary
-                status_style = normlabel
-                dframe.plots = ttk.Frame(dframe)
-                dframe.plots.grid(column=2, row=n, columnspan=6, sticky='ewns')
-                status_value = '(not checked)'
-
-                if 'results' in param:
-                    reslist = param['results']
-                    if 'netlist_source' in runtime_options:
-                        netlist_source = runtime_options['netlist_source']
-                    if isinstance(reslist, list):
-                        try:
-                            resdict = next(
-                                item
-                                for item in reslist
-                                if item['name'] == netlist_source
-                            )
-                        except:
-                            resdict = None
-                    elif reslist['name'] == netlist_source:
-                        resdict = reslist
-                    else:
-                        resdict = None
+    return condlist
 
-                    if resdict:
-                        if 'status' in resdict:
-                            status_value = resdict['status']
-
-                plotrec = param['plot']
-                if 'filename' in plotrec:
-                    plottext = plotrec['filename']
-                elif 'type' in plotrec:
-                    plottext = plotrec['type']
-                else:
-                    plottext = 'plot'
-                dframe_plot = ttk.Label(
-                    dframe.plots, text=plottext, style=normlabel
+
+# -----------------------------------------------------------------------
+# Define how to write a simulation file by making substitutions into a
+# template schematic.
+#
+# 	filename:  Root name of the simulatable output file
+# 	paths:	   Dictionary of paths from the characterization file
+# 	tool:	   Name of tool that uses the template (e.g., "ngspice")
+# 	template:  Name of the template file to be substituted
+# 	dutpath:   Path and filename of the design netlist
+# 	simvals:   Complete list of conditions to be enumerated
+# 	maxtime:   Value to use for {Tmax} substitution
+# 	schemline: DUT pin list from schematic, for ordering
+# 	pdkname:   Name of the PDK pulled from the datasheet
+# -----------------------------------------------------------------------
+
+
+def substitute(
+    filename,
+    paths,
+    tool,
+    template,
+    dutpath,
+    simvals,
+    schemline,
+    pdkname,
+    debug,
+):
+    """Simulation derived by substitution into template schematic"""
+
+    # Regular expressions
+    # varex:		variable name {name}
+    # defaultex:	name in {name=default} format
+    # condex:		name in {cond} format
+    # sweepex:		name in {cond|value} format
+    # pinex:		name in {PIN|pin_name|net_name} format
+    # funcrex:		name in {FUNCTIONAL|ip_name} format
+    # colonsepex:	a:b (colon-separated values)
+    # vectrex:		pin name is a vector signal
+    # vect2rex:		pin name is a vector signal (alternate style)
+    # vect3rex:		pin name is a vector signal (alternate style)
+    # libdirrex:	pick up library name from .lib
+    # vinclrex:		verilog include statement
+
+    varex = re.compile(r'(\{[^ \}\t]+\})')
+    defaultex = re.compile(r'\{([^=]+)=([^=\}]+)\}')
+    condex = re.compile(r'\{([^\}]+)\}')
+    sweepex = re.compile(r'\{([^|\}]+)\|([^|\}]+)\}')
+    pinex = re.compile(r'PIN\|([^|]+)\|([^|]+)')
+    funcrex = re.compile(r'FUNCTIONAL\|([^|]+)')
+    colonsepex = re.compile(r'^([^:]+):([^:]+)$')
+    vectrex = re.compile(r'([^\[]+)\[([0-9]+)\]')
+    vect2rex = re.compile(r'([^<]+)<([0-9]+)>')
+    vect3rex = re.compile(r'([a-zA-Z][^0-9]*)([0-9]+)')
+    libdirrex = re.compile(r'.lib[ \t]+(.*)[ \t]+')
+    vinclrex = re.compile(r'[ \t]*`include[ \t]+"([^"]+)"')
+    brackrex = re.compile(r'(\[[^]]+\])')
+
+    # Information about the DUT
+    simfilepath = paths['simulation']
+    schempath = paths['schematic']
+    testbenchpath = paths['testbench']
+    rootpath = paths['root']
+    schempins = schemline.upper().split()[1:-1]
+    simpins = [None] * len(schempins)
+
+    suffix = os.path.splitext(template)[1]
+    functional = []
+
+    # Read ifile into a list
+    # Concatenate any continuation lines
+    with open(template, 'r') as ifile:
+        simtext = ifile.read()
+
+    simlines = simtext.replace('\n+', ' ').splitlines()
+
+    # Make initial pass over contents of template file, looking for conditions
+    # with values (e.g., "Vdd|maximum").  These indicate that the condition is
+    # not enumerated over testbenches, so collapse simvals accordingly.
+
+    # NOTE:  "simvals" have already been enumerated from the electrical parameter
+    # description.  Values can be "minimum" or "maximum", "stepsize", or "steps".
+    # The first three are recovered from the list.  The last one is calculated
+    # by counting the number of values for the condition.
+
+    # TO DO:  It may be useful to use both values from an enumeration AND keep
+    # the enumeration;  e.g., have "{Vdd}" but also "{Vdd|maximum}" in the
+    # template.  In that case make the sweeps entry but do not collapse simvals.
+
+    sweeps = []
+    for line in simlines:
+        sublist = sweepex.findall(line)
+        for pattern in sublist:
+            condition = pattern[0]
+            if pattern == 'FUNCTIONAL':
+                # 'FUNCTIONAL' is a reserved name so don't throw an error.
+                continue
+            try:
+                entry = next(
+                    item for item in sweeps if item['name'] == condition
                 )
-                dframe_plot.grid(column=j, row=n, sticky='ewns')
-            else:
-                # For schematic capture, mark physical parameters that can't and won't be
-                # checked as "not applicable".
-                status_value = '(not checked)'
-                if paramtype == 'physical':
-                    if isschem:
-                        if (
-                            p == 'cace_width'
-                            or p == 'cace_height'
-                            or p == 'cace_drc'
-                        ):
-                            status_value = '(N/A)'
-
-                # Grab the electrical parameter's 'spec' and 'result' dictionaries
-                if 'spec' in param:
-                    specdict = param['spec']
-                else:
-                    specdict = {}
+            except (StopIteration, KeyError):
+                if debug:
+                    print('New sweeps entry ' + condition + ' found.')
+                    # print('Line = ' + line)
+                    # print('Substitution list = ' + str(sublist))
+                entry = {'name': condition}
+                sweeps.append(entry)
+
+                # Find each entry in simvals with the same condition.
+                # Record the minimum, maximum, and step for substitution, at the same
+                # time removing that item from the entry.
+                lvals = []
+                units = ''
+                for simval in simvals:
+                    try:
+                        simrec = next(
+                            item for item in simval if item[0] == condition
+                        )
+                    except StopIteration:
+                        print('No condition = ' + condition + ' in record:\n')
+                        ptext = str(simval) + '\n'
+                        sys.stdout.buffer.write(ptext.encode('utf-8'))
+                    else:
+                        units = simrec[1]
+                        lvals.append(numeric(simrec[2]))
+                        simval.remove(simrec)
+
+                # Remove non-unique entries from lvals
+                lvals = list(set(lvals))
+                if not lvals:
+                    print(
+                        'CACE gensim error:  No substitution for "'
+                        + condition
+                        + '"'
+                    )
+                    continue
 
-                # Which information is provided depends on which origin is
-                # selected.
+                # Now parse lvals for minimum/maximum
+                entry['unit'] = units
+                minval = min(lvals)
+                maxval = max(lvals)
+                entry['minimum'] = str(minval)
+                entry['maximum'] = str(maxval)
+                numvals = len(lvals)
+                if numvals > 1:
+                    entry['steps'] = str(numvals)
+                    entry['stepsize'] = str((maxval - minval) / (numvals - 1))
+                else:
+                    entry['steps'] = '1'
+                    entry['stepsize'] = str(minval)
 
-                valid = False
-                if 'results' in param:
-                    resultlist = param['results']
-                    if not isinstance(resultlist, list):
-                        resultlist = [resultlist]
-
-                    if self.origin.get() == 'R-C Extracted':
-                        for resultdict in resultlist:
-                            if resultdict['name'] == 'rcx':
-                                valid = True
-                                break
-                    elif self.origin.get() == 'C Extracted':
-                        for resultdict in resultlist:
-                            if resultdict['name'] == 'pex':
-                                valid = True
-                                break
-                    elif self.origin.get() == 'Layout Extracted':
-                        for resultdict in resultlist:
-                            if resultdict['name'] == 'layout':
-                                valid = True
-                                break
-                    else:  	# Schematic capture
-                        for resultdict in resultlist:
-                            if resultdict['name'] == 'schematic':
-                                valid = True
-                                break
-
-                if valid == False:
-                    # No result dictionary exists for this netlist origin type
-                    resultdict = {}
-
-                # Fill in information for the spec minimum and result
-                if 'minimum' in specdict:
-                    status_style = normlabel
-                    pmin = specdict['minimum']
-                    if isinstance(pmin, list):
-                        penalty = pmin[1]
-                        pmin = pmin[0]
-                    else:
-                        penalty = None
+    # Remove non-unique entries from simvals
+    simvals = uniquify(simvals)
 
-                    if 'minimum' in resultdict:
-                        value = resultdict['minimum']
-                        if isinstance(value, list):
-                            score = value[1]
-                            value = value[0]
-                        else:
-                            score = None
+    simnum = 0
+    testbenches = []
+    for simval in simvals:
+        # Create the file
+        simnum += 1
+        testbenchname = filename + '_' + str(simnum)
+        simfilename = os.path.join(simfilepath, testbenchname + suffix)
+        with open(simfilename, 'w') as ofile:
+            for line in simlines:
+
+                # This will be replaced
+                subsline = line
+
+                # Find all variables to substitute
+                for patmatch in varex.finditer(line):
+                    pattern = patmatch.group(1)
+                    # If variable is in {x=y} format, it declares a default value
+                    # Remove the =y default part and keep it for later if needed.
+                    defmatch = defaultex.match(pattern)
+                    if defmatch:
+                        default = defmatch.group(2)
+                        vpattern = '{' + defmatch.group(1) + '}'
                     else:
-                        value = None
-                        score = None
+                        default = []
+                        vpattern = pattern
 
-                    if pmin == 'any':
-                        dframe.min = ttk.Label(
-                            dframe, text='(no limit)', style=normlabel
+                    repl = []
+                    no_repl_ok = False
+                    vtype = -1
+                    sweeprec = sweepex.match(vpattern)
+                    if sweeprec:
+                        sweeptype = sweeprec.group(2)
+                        condition = sweeprec.group(1)
+
+                        entry = next(
+                            item
+                            for item in sweeps
+                            if item['name'] == condition
                         )
+                        if 'unit' in entry:
+                            uval = spice_unit_convert(
+                                (entry['unit'], entry[sweeptype])
+                            )
+                            repl = str(uval)
                     else:
-                        if 'unit' in param and not binrex.match(param['unit']):
-                            targettext = pmin + ' ' + param['unit']
-                        else:
-                            targettext = pmin
-                        dframe.min = ttk.Label(
-                            dframe, text=targettext, style=normlabel
+                        cond = condex.match(vpattern)
+                        if cond:
+                            condition = cond.group(1)
+
+                            # Check if the condition contains a pin vector
+                            lmatch = vectrex.match(condition)
+                            if lmatch:
+                                pinidx = int(lmatch.group(2))
+                                vcondition = lmatch.group(1)
+                                vtype = 0
+                            else:
+                                lmatch = vect2rex.match(condition)
+                                if lmatch:
+                                    pinidx = int(lmatch.group(2))
+                                    vcondition = lmatch.group(1)
+                                    vtype = 1
+                                else:
+                                    lmatch = vect3rex.match(condition)
+                                    if lmatch:
+                                        pinidx = int(lmatch.group(2))
+                                        vcondition = lmatch.group(1)
+                                        vtype = 3
+
+                            try:
+                                entry = next(
+                                    (
+                                        item
+                                        for item in simval
+                                        if item[0] == condition
+                                    )
+                                )
+                            except (StopIteration, KeyError):
+                                # check against known keys that are not conditions
+                                if condition == 'N':
+                                    repl = str(simnum)
+                                elif condition == 'PDK_ROOT':
+                                    repl = get_pdk_root()
+                                elif condition == 'PDK':
+                                    repl = pdkname
+                                elif condition == 'steptime':
+                                    maxtime = simvals('Tmax')
+                                    repl = str(maxtime / 100)
+                                elif condition == 'DUT_path':
+                                    repl = dutpath + '\n'
+                                elif condition == 'include_DUT':
+                                    if len(functional) == 0:
+                                        repl = '.include ' + dutpath + '\n'
+                                    else:
+                                        inline_dut(
+                                            dutpath,
+                                            functional,
+                                            rootpath,
+                                            ofile,
+                                        )
+                                        repl = (
+                                            '** End of in-line DUT subcircuit'
+                                        )
+                                elif condition == 'DUT_call':
+                                    repl = schemline
+                                elif condition == 'DUT_name':
+                                    # This verifies pin list of schematic vs. the netlist.
+                                    repl = schemline.split()[-1]
+                                elif condition == 'filename':
+                                    repl = filename
+                                elif condition == 'simpath':
+                                    repl = simfilepath
+                                elif condition == 'random':
+                                    repl = str(
+                                        int(time.time() * 1000) & 0x7FFFFFFF
+                                    )
+                                # Stack math operators.  Perform specified math
+                                # operation on the last two values and replace.
+                                #
+                                # Note that ngspice is finicky about space around "=" so
+                                # handle this in a way that keeps ngspice happy.
+                                elif condition == '+':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                numeric(ltok[-2])
+                                                + numeric(ltok[-1])
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition == '-':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                numeric(ltok[-2])
+                                                - numeric(ltok[-1])
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition == '*':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                numeric(ltok[-2])
+                                                * numeric(ltok[-1])
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition == '/':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                numeric(ltok[-2])
+                                                / numeric(ltok[-1])
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition == 'MAX':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                max(
+                                                    numeric(ltok[-2]),
+                                                    numeric(ltok[-1]),
+                                                )
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition == 'MIN':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    if len(ltok) >= 2:
+                                        ntok = ltok[:-2]
+                                        ntok.append(
+                                            str(
+                                                min(
+                                                    numeric(ltok[-2]),
+                                                    numeric(ltok[-1]),
+                                                )
+                                            )
+                                        )
+                                        subsline = (
+                                            ' '.join(ntok).replace(' = ', '=')
+                                            + line[patmatch.end() :]
+                                        )
+                                    else:
+                                        print(
+                                            'CACE gensim: substitution error in "'
+                                            + subsline
+                                            + '"'
+                                        )
+                                    repl = ''
+                                    no_repl_ok = True
+                                # 'NEG' acts on only the previous value in the string.
+                                elif condition == 'NEG':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    ntok = ltok[:-1]
+                                    ntok.append(str(-numeric(ltok[-1])))
+                                    subsline = (
+                                        ' '.join(ntok).replace(' = ', '=')
+                                        + line[patmatch.end() :]
+                                    )
+                                    repl = ''
+                                    no_repl_ok = True
+                                # 'INT' also acts on only the previous value in the string.
+                                elif condition == 'INT':
+                                    smatch = varex.search(subsline)
+                                    watchend = smatch.start()
+                                    ltok = (
+                                        subsline[0:watchend]
+                                        .replace('=', ' = ')
+                                        .split()
+                                    )
+                                    ntok = ltok[:-1]
+                                    ntok.append(str(int(ltok[-1])))
+                                    subsline = (
+                                        ' '.join(ntok).replace(' = ', '=')
+                                        + line[patmatch.end() :]
+                                    )
+                                    repl = ''
+                                    no_repl_ok = True
+                                elif condition.find('PIN|') == 0:
+                                    # Parse for {PIN|<pin_name>|<net_name>}
+                                    # Replace <pin_name> with index of pin from DUT subcircuit
+                                    pinrec = pinex.match(condition)
+                                    if pinrec:
+                                        pinname = pinrec.group(1).upper()
+                                        netname = pinrec.group(2).upper()
+                                    else:
+                                        print(
+                                            'Error: Bad PIN variable '
+                                            + condition
+                                            + ' in DUT!'
+                                        )
+                                        continue
+                                    try:
+                                        idx = schempins.index(pinname)
+                                    except ValueError:
+                                        repl = netname
+                                    else:
+                                        repl = '{PIN}'
+                                        simpins[idx] = netname
+                                elif condition.find('FUNCTIONAL|') == 0:
+                                    # Parse for {FUNCTIONAL|<ip_name>}
+                                    # Add <ip_name> to "functional" array.
+                                    # 'FUNCTIONAL' declarations must come before 'INCLUDE_DUT' or else
+                                    # substitution will not be made.  'INCLUDE_DUT' must be used in place
+                                    # of 'DUT_path' to get the correct behavior.
+                                    funcrec = funcrex.match(condition)
+                                    ipname = funcrec.group(1)
+                                    functional.append(ipname.upper())
+                                    repl = (
+                                        '** Using functional view for '
+                                        + ipname
+                                    )
+                                else:
+                                    if lmatch:
+                                        try:
+                                            entry = next(
+                                                (
+                                                    item
+                                                    for item in simval
+                                                    if item[0]
+                                                    .split('[')[0]
+                                                    .split('<')[0]
+                                                    == vcondition
+                                                )
+                                            )
+                                        except:
+                                            if vtype == 3:
+                                                for entry in simval:
+                                                    lmatch = vect3rex.match(
+                                                        entry[0]
+                                                    )
+                                                    if lmatch:
+                                                        if (
+                                                            lmatch.group(1)
+                                                            == vcondition
+                                                        ):
+                                                            vlen = len(
+                                                                entry[2]
+                                                            )
+                                                            uval = entry[2][
+                                                                (vlen - 1)
+                                                                - pinidx
+                                                            ]
+                                                            repl = str(uval)
+                                                            break
+                                            else:
+                                                # if no match, subsline remains as-is.
+                                                pass
+                                        else:
+                                            # Handle as vector bit slice (see below)
+                                            vlen = len(entry[2])
+                                            uval = entry[2][
+                                                (vlen - 1) - pinidx
+                                            ]
+                                            repl = str(uval)
+                                    # else if no match, subsline remains as-is.
+
+                            else:
+                                if lmatch:
+                                    # pull signal at pinidx out of the vector.
+                                    # Note: DIGITAL assumes binary value.  May want to
+                                    # allow general case of real-valued vectors, which would
+                                    # require a spice unit conversion routine without indexing.
+                                    vlen = len(entry[2])
+                                    uval = entry[2][(vlen - 1) - pinidx]
+                                else:
+                                    uval = spice_unit_convert(entry[1:])
+                                repl = str(uval)
+
+                    if not repl and default:
+                        # Use default if no match was found and default was specified
+                        repl = default
+
+                    if repl:
+                        # Make the variable substitution
+                        subsline = subsline.replace(pattern, repl)
+                    elif not no_repl_ok:
+                        print(
+                            'Warning: Variable '
+                            + pattern
+                            + ' had no substitution'
                         )
 
-                    if score:
-                        if score != 'fail':
-                            status_style = greenlabel
-                            if status_value != 'fail':
-                                status_value = 'pass'
+                # Check if {PIN} are in line.  If so, order by index and
+                # rewrite pins in order
+                for i in range(len(simpins)):
+                    if '{PIN}' in subsline:
+                        if simpins[i]:
+                            subsline = subsline.replace('{PIN}', simpins[i], 1)
                         else:
-                            status_style = redlabel
-                            status_value = 'fail'
-                    if value:
-                        if value == 'failure' or value == 'fail':
-                            status_value = '(not checked)'
-                            status_style = redlabel
-                            valuetext = value
-                        elif 'unit' in param and not binrex.match(
-                            param['unit']
-                        ):
-                            valuetext = value + ' ' + param['unit']
+                            print('Error:  simpins is ' + str(simpins) + '\n')
+                            print('        subsline is ' + subsline + '\n')
+                            print('        i is ' + str(i) + '\n')
+
+                # Check for a verilog include file, and if any is found, copy it
+                # to the target simulation directory.  Replace any leading path
+                # with the local current working directory '.'.
+                vmatch = vinclrex.match(subsline)
+                if vmatch:
+                    incfile = vmatch.group(1)
+                    incroot = os.path.split(incfile)[1]
+                    curpath = os.path.split(template)[0]
+                    incpath = os.path.abspath(os.path.join(curpath, incfile))
+                    shutil.copy(incpath, simfilepath + '/' + incroot)
+                    subsline = '   `include "./' + incroot + '"'
+
+                # Check if there is a bracket expression.  This is a simplified
+                # and cleaner way of handling the RPN notation, and allows for
+                # any expression to be used as long as it evaluates to a
+                # number in python.
+
+                for bmatch in brackrex.finditer(subsline):
+                    brackexpr = bmatch.group(1)
+                    bexpr = brackexpr.strip('[]')
+                    try:
+                        # Avoid catching simple array indexes like "v[0]".
+                        # Other non-expressions will just throw exceptions
+                        # when passed to safe_eval().
+                        btest = int(bexpr)
+                    except:
+                        try:
+                            brackval = str(safe_eval(bexpr))
+                        except:
+                            pass
                         else:
-                            valuetext = value
-                        dframe.value = ttk.Label(
-                            dframe, text=valuetext, style=status_style
-                        )
-                        dframe.value.grid(column=3, row=n, sticky='ewns')
-                else:
-                    dframe.min = ttk.Label(
-                        dframe, text='(no limit)', style=normlabel
-                    )
+                            subsline = subsline.replace(brackexpr, brackval)
 
-                dframe.min.grid(column=2, row=n, sticky='ewns')
+                # Write the modified output line (with variable substitutions)
+                ofile.write(subsline + '\n')
 
-                # Fill in information for the spec typical and result
-                if 'typical' in specdict:
-                    status_style = normlabel
-                    ptyp = specdict['typical']
-                    if isinstance(ptyp, list):
-                        penalty = ptyp[1]
-                        ptyp = ptyp[0]
-                    else:
-                        penalty = None
+        # Add information about testbench file and conditions to datasheet,
+        # which can be parsed by cace_launch.py.
+        testbench = {}
 
-                    if 'typical' in resultdict:
-                        value = resultdict['typical']
-                        if isinstance(value, list):
-                            score = value[1]
-                            value = value[0]
-                        else:
-                            score = None
-                    else:
-                        value = None
-                        score = None
+        testbench['filename'] = simfilename
+        testbench['conditions'] = simval
+        testbenches.append(testbench)
 
-                    if ptyp == 'any':
-                        dframe.typ = ttk.Label(
-                            dframe, text='(no target)', style=normlabel
-                        )
-                    else:
-                        if 'unit' in param and not binrex.match(param['unit']):
-                            targettext = ptyp + ' ' + param['unit']
-                        else:
-                            targettext = ptyp
-                        dframe.typ = ttk.Label(
-                            dframe, text=targettext, style=normlabel
-                        )
+    return testbenches
 
-                    if score:
-                        # Note:  You can't fail a "typ" score, but there is only one "Status",
-                        # so if it is a "fail", it must remain a "fail".
-                        if score != 'fail':
-                            status_style = greenlabel
-                            if status_value != 'fail':
-                                status_value = 'pass'
-                        else:
-                            status_style = redlabel
-                            status_value = 'fail'
-                    if value:
-                        if value == 'failure' or value == 'fail':
-                            status_value = '(not checked)'
-                            status_style = redlabel
-                            valuetext = value
-                        elif 'unit' in param and not binrex.match(
-                            param['unit']
-                        ):
-                            valuetext = value + ' ' + param['unit']
-                        else:
-                            valuetext = value
-                        dframe.value = ttk.Label(
-                            dframe, text=valuetext, style=status_style
-                        )
-                        dframe.value.grid(column=5, row=n, sticky='ewns')
-                else:
-                    dframe.typ = ttk.Label(
-                        dframe, text='(no target)', style=normlabel
-                    )
-                dframe.typ.grid(column=4, row=n, sticky='ewns')
 
-                # Fill in information for the spec maximum and result
-                if 'maximum' in specdict:
-                    status_style = normlabel
-                    pmax = specdict['maximum']
-                    if isinstance(pmax, list):
-                        penalty = pmax[1]
-                        pmax = pmax[0]
-                    else:
-                        penalty = None
+# -----------------------------------------------------------------------
+# cace_gensim
+#
+# Generate simulation testbenches for a single electrical parameter.
+#
+# "dataset" is the datasheet characterization dictionary.
+# "param" is the dictionary of one parameter in the dataset.
+# -----------------------------------------------------------------------
 
-                    if 'maximum' in resultdict:
-                        value = resultdict['maximum']
-                        if isinstance(value, list):
-                            score = value[1]
-                            value = value[0]
-                        else:
-                            score = None
-                    else:
-                        value = None
-                        score = None
 
-                    if pmax == 'any':
-                        dframe.max = ttk.Label(
-                            dframe, text='(no limit)', style=normlabel
-                        )
-                    else:
-                        if 'unit' in param and not binrex.match(param['unit']):
-                            targettext = pmax + ' ' + param['unit']
-                        else:
-                            targettext = pmax
-                        dframe.max = ttk.Label(
-                            dframe, text=targettext, style=normlabel
-                        )
+def cace_gensim(dataset, param):
 
-                    if score:
-                        if score != 'fail':
-                            status_style = greenlabel
-                            if status_value != 'fail':
-                                status_value = 'pass'
-                        else:
-                            status_style = redlabel
-                            status_value = 'fail'
-                    if value:
-                        if value == 'failure' or value == 'fail':
-                            status_value = '(not checked)'
-                            status_style = redlabel
-                            valuetext = value
-                        elif 'unit' in param and not binrex.match(
-                            param['unit']
-                        ):
-                            valuetext = value + ' ' + param['unit']
-                        else:
-                            valuetext = value
-                        dframe.value = ttk.Label(
-                            dframe, text=valuetext, style=status_style
-                        )
-                        dframe.value.grid(column=7, row=n, sticky='ewns')
-                else:
-                    dframe.max = ttk.Label(
-                        dframe, text='(no limit)', style=normlabel
-                    )
-                dframe.max.grid(column=6, row=n, sticky='ewns')
+    runtime_options = dataset['runtime_options']
+    debug = runtime_options['debug']
+    source = runtime_options['netlist_source']
+    pdkname = dataset['PDK']
 
-            if paramtype == 'electrical':
-                if 'hints' in param:
-                    simtext = '\u2022Simulate'
-                else:
-                    simtext = 'Simulate'
+    # Grab values held in 'paths'
+    paths = dataset['paths']
+    testbenchpath = paths['testbench']
+    root_path = paths['root']
+
+    paramname = param['name']
+
+    # Electrical parameter list comes from argument "parameters" if non-NULL.
+    # Otherwise, enumerate all electrical parameters.
+
+    if 'status' in param:
+        status = param['status']
+    else:
+        status = 'active'
+    if status == 'skip' or status == 'blocked':
+        if debug:
+            print('Parameter ' + paramname + ' is marked for skipping.')
+
+        return param
+
+    if debug:
+        print('Generating simulation files for parameter ' + paramname)
+
+    # Get list of default conditions and generate a list of the condition names
+    defcondlist = dataset['default_conditions']
+    defcondnames = []
+    for defcond in defcondlist:
+        defcondnames.append(defcond['name'])
+
+    # Make a copy of the pin list in the datasheet, and expand any vectors.
+    pinlist = []
+    vectrex = re.compile(r'([^\[]+)\[([0-9]+):([0-9]+)\]')
+    vect2rex = re.compile(r'([^<]+)\<([0-9]+):([0-9]+)\>')
+    vect3rex = re.compile(r'([^0-9]+)([0-9]+):([0-9]+)')
+
+    for pinrec in dataset['pins']:
+        vmatch = vectrex.match(pinrec['name'])
+        if vmatch:
+            pinname = vmatch.group(1)
+            pinmin = vmatch.group(2)
+            pinmax = vmatch.group(3)
+            if int(pinmin) > int(pinmax):
+                pinmin = vmatch.group(3)
+                pinmax = vmatch.group(2)
+            for i in range(int(pinmin), int(pinmax) + 1):
+                newpinrec = pinrec.copy()
+                pinlist.append(newpinrec)
+                newpinrec['name'] = pinname + '[' + str(i) + ']'
+        else:
+            vmatch = vect2rex.match(pinrec['name'])
+            if vmatch:
+                pinname = vmatch.group(1)
+                pinmin = vmatch.group(2)
+                pinmax = vmatch.group(3)
+                if int(pinmin) > int(pinmax):
+                    pinmin = vmatch.group(3)
+                    pinmax = vmatch.group(2)
+                for i in range(int(pinmin), int(pinmax) + 1):
+                    newpinrec = pinrec.copy()
+                    pinlist.append(newpinrec)
+                    newpinrec['name'] = pinname + '<' + str(i) + '>'
             else:
-                simtext = 'Check'
+                vmatch = vect3rex.match(pinrec['name'])
+                if vmatch:
+                    pinname = vmatch.group(1)
+                    pinmin = vmatch.group(2)
+                    pinmax = vmatch.group(3)
+                    if int(pinmin) > int(pinmax):
+                        pinmin = vmatch.group(3)
+                        pinmax = vmatch.group(2)
+                    for i in range(int(pinmin), int(pinmax) + 1):
+                        newpinrec = pinrec.copy()
+                        pinlist.append(newpinrec)
+                        newpinrec['name'] = pinname + str(i)
+                else:
+                    pinlist.append(pinrec)
 
-            if self.procs_pending:
-                if pname in self.procs_pending:
-                    simtext = '(in progress)'
-
-            simbutton = ttk.Menubutton(dframe, text=simtext, style=normbutton)
-            self.simbuttons[pname] = simbutton
-
-            # Generate pull-down menu on Simulate button.  Most items apply
-            # only to electrical parameters (at least for now)
-            simmenu = tkinter.Menu(simbutton)
-            simmenu.add_command(
-                label='Run', command=lambda pname=pname: self.sim_param(pname)
-            )
-            simmenu.add_command(label='Stop', command=self.stop_sims)
-            if paramtype == 'electrical':
-                # simmenu.add_command(label='Hints',
-                # 	command = lambda param=param, simbutton=simbutton: self.add_hints(param, simbutton))
-                simmenu.add_command(
-                    label='Edit',
-                    command=lambda param=param: self.edit_param(param),
-                )
-                simmenu.add_command(
-                    label='Copy',
-                    command=lambda param=param: self.copy_param(param),
-                )
-                if 'editable' in param and param['editable'] == True:
-                    simmenu.add_command(
-                        label='Delete',
-                        command=lambda param=param: self.delete_param(param),
-                    )
+    # Find DUT netlist file and capture the subcircuit call line
+    pname = dataset['name']
 
-            # Attach the menu to the button
-            simbutton.config(menu=simmenu)
+    if source != 'schematic':
+        if source == 'layout':
+            layoutpath = os.path.join(paths['netlist'], 'layout')
+        elif source == 'pex':
+            layoutpath = os.path.join(paths['netlist'], 'pex')
+        else:
+            layoutpath = os.path.join(paths['netlist'], 'rcx')
+        layoutname = pname + '.spice'
+        dutpath = os.path.join(root_path, layoutpath, layoutname)
+
+    if source == 'schematic' or not os.path.isfile(dutpath):
+        if source == 'schematic':
+            schempath = os.path.join(paths['netlist'], 'schematic')
+            schemname = pname + '.spice'
+            dutpath = os.path.join(root_path, schempath, schemname)
 
-            # simbutton = ttk.Button(dframe, text=simtext, style = normbutton)
-            # 		command = lambda pname=pname: self.sim_param(pname))
+    if not os.path.isfile(dutpath):
+        if 'verilog' not in paths:
+            print(
+                'No SPICE netlist exists at '
+                + dutpath
+                + ' and no verilog path exists.'
+            )
+            print('This is an error condition.')
+            return param
 
-            simbutton.grid(column=9, row=n, sticky='ewns')
+    # Get the DUT definition from the SPICE netlist.  Note that this
+    # only applies to parameters being simulated with SPICE, so only
+    # flag an error when applicable.
 
-            if paramtype == 'electrical':
-                ToolTip(simbutton, text='Simulate one electrical parameter')
-            else:
-                ToolTip(simbutton, text='Check one physical parameter')
+    try:
+        schemline = construct_dut_from_path(pname, dutpath, pinlist)
+    except SyntaxError:
+        schemline = ''
+
+    # Dictionary "simulate" key "template" is the name of the template
+    # file to use as source.  The output file is the name (key "name")
+    # of the electrical parameter followed by an index suffix uniquely
+    # identifying it.
+    #
+    # There is no check here for duplicate electrical parameter names,
+    # which is not allowed.
+    #
+    # In the following code:
+    #   "condnames" is the full list of conditions found in the template
+    # 		testbench netlists that will need substitution, looking
+    # 		at all testbenches that are required by the parameter.
+    #   "pcondnames" is the list of conditions found in the datasheet
+    # 		for the parameter.
+    # 	"defcondnames" is a list of conditions found in the default set.
+    # 	"lcondnames" is the list of parameter conditions + defaults that
+    # 		should match the "condnames" list.
+
+    # Get the simulation dictionary and find the tool and template
+    # NOTE:  The "simulate" value could be a list in the case of, for
+    # example, co-simulation.
+
+    simulatedict = param['simulate']
+    if isinstance(simulatedict, list):
+        tools = []
+        testbenches = []
+        for simulation in simulatedict:
+            tools.append(simulation['tool'])
+            testbenches.append(simulation['template'])
+    else:
+        tools = [simulatedict['tool']]
+        testbenches = [simulatedict['template']]
 
-            # If 'pass', then just display message.  If 'fail', then create a button that
-            # opens and configures the failure report window.
-            if status_value == '(not checked)':
-                bstyle = normbutton
-                stat_label = ttk.Label(dframe, text=status_value, style=bstyle)
+    # Get the list of parameters that get substituted in the template
+    condnames = []
+    for testbench in testbenches:
+        newnames = get_condition_names_used(testbenchpath, testbench)
+        if not newnames:
+            print('Error:  No conditions for testbench ' + testbench)
+        else:
+            # Convert the dictionary of names into a list
+            for name in newnames:
+                if name not in condnames:
+                    condnames.append(name)
+
+    # Get the list of parameters specific to the electrical parameter
+    # definition
+    pcondlist = param['conditions']
+    pcondnames = []
+    for pcond in pcondlist:
+        pcondnames.append(pcond['name'])
+
+    # Add any missing unit types that exist in the default conditions
+    # but have been made implicit in the parameter's condition list
+    # need to be added so that units are handled correctly everywhere.
+
+    newpcondlist = []
+    for pcond in pcondlist:
+        newpcond = pcond
+        if 'unit' not in pcondlist:
+            try:
+                defcond = next(
+                    item
+                    for item in defcondlist
+                    if item['name'] == pcond['name']
+                )
+            except:
+                pass
             else:
-                if status_value == 'fail' or status_value == 'failure':
-                    bstyle = redbutton
-                else:
-                    bstyle = greenbutton
-                if paramtype == 'electrical':
-                    stat_label = ttk.Button(
-                        dframe,
-                        text=status_value,
-                        style=bstyle,
-                        command=lambda param=param, dsheet=dsheet: self.failreport.display(
-                            param, dsheet, self.datasheet
-                        ),
+                if 'unit' in defcond:
+                    newpcond = pcond.copy()
+                    newpcond['unit'] = defcond['unit']
+        newpcondlist.append(newpcond)
+    pcondlist = newpcondlist
+
+    # For each vector type in pcondlist and defcondlist, reduce to
+    # just the name portion of the vector and the opening delimiter.
+
+    vectrex = re.compile(r'([^\[]+)\[([0-9:]+)\]')  # name[number]
+
+    newdefcondnames = []
+    for defcondname in defcondnames:
+        vmatch = vectrex.match(defcondname)
+        if vmatch:
+            newdefcondnames.append(vmatch.group(1) + '[')
+        else:
+            newdefcondnames.append(defcondname)
+
+    defcondnames = newdefcondnames
+
+    newpcondnames = []
+    for pcondname in pcondnames:
+        vmatch = vectrex.match(pcondname)
+        if vmatch:
+            newpcondnames.append(vmatch.group(1) + '[')
+        else:
+            newpcondnames.append(pcondname)
+
+    pcondnames = newpcondnames
+
+    # Get the full list of conditions for which the parameter will be
+    # simulated by merging together both the conditions defined for
+    # the electrical parameter and the fallback of the default conditions,
+    # only keeping those conditions that get substituted.
+    # Run a sanity check:  All names in "condnames" should be found in
+    # either the parameter list or the defaults list except for specific
+    # items that have reserved names, and the pins which have a fixed
+    # format.
+
+    reserved = [
+        'filename',
+        'simpath',
+        'DUT_name',
+        'N',
+        'DUT_path',
+        'PDK_ROOT',
+        'PDK',
+        'include_DUT',
+        'DUT_call',
+        'steptime',
+        'random',
+        '+',
+        '-',
+        '*',
+        '/',
+        'MIN',
+        'NEG',
+        'INT',
+        'FUNCTIONAL',
+    ]
+
+    lcondlist = []
+    for cond in condnames:
+        if cond[-1] == '[':
+            if cond in pcondnames:
+                lcondlist.extend(
+                    list(
+                        item
+                        for item in pcondlist
+                        if item['name'].startswith(cond)
                     )
-                elif p == 'LVS_errors':
-                    dspath = os.path.split(self.filename)[0]
-                    datasheet = os.path.split(self.filename)[1]
-                    dsheet = self.datasheet
-                    designname = dsheet['name']
-                    if self.origin.get() == 'Schematic Capture':
-                        lvs_file = dspath + '/mag/precheck.log'
-                    else:
-                        lvs_file = dspath + '/mag/comp.out'
-                    if not os.path.exists(lvs_file):
-                        if os.path.exists(dspath + '/mag/precheck.log'):
-                            lvs_file = dspath + '/mag/precheck.log'
-                        elif os.path.exists(dspath + '/mag/comp.out'):
-                            lvs_file = dspath + '/mag/comp.out'
-
-                    stat_label = ttk.Button(
-                        dframe,
-                        text=status_value,
-                        style=bstyle,
-                        command=lambda lvs_file=lvs_file: self.textreport.display(
-                            lvs_file
-                        ),
+                )
+            elif cond in defcondnames:
+                lcondlist.extend(
+                    list(
+                        item
+                        for item in defcondlist
+                        if item['name'].startswith(cond)
                     )
-                else:
-                    stat_label = ttk.Label(
-                        dframe, text=status_value, style=bstyle
+                )
+            elif not cond.startswith('PIN|') and not '=' in cond:
+                if cond not in reserved:
+                    print(
+                        'Error:  Unknown/unhandled condition name "'
+                        + cond
+                        + '"'
                     )
-                ToolTip(
-                    stat_label,
-                    text='Show detail view of simulation conditions and results',
+        else:
+            if cond in pcondnames:
+                lcondlist.extend(
+                    list(item for item in pcondlist if item['name'] == cond)
                 )
-            stat_label.grid(column=8, row=n, sticky='ewns')
-            self.status[pname] = stat_label
-            n += 1
-
-        for child in dframe.winfo_children():
-            child.grid_configure(ipadx=5, ipady=1, padx=2, pady=2)
-
+            elif cond in defcondnames:
+                lcondlist.extend(
+                    list(item for item in defcondlist if item['name'] == cond)
+                )
+            elif not cond.startswith('PIN|') and not '=' in cond:
+                if cond not in reserved:
+                    print(
+                        'Error:  Unknown/unhandled condition name "'
+                        + cond
+                        + '"'
+                    )
 
-# --------------------------------------------------------------------------
-# Print usage information for cace_gui.py
-# --------------------------------------------------------------------------
+    # Get the list of parameters that are collated (simulated together
+    # and results passed as a list to the measurement).  These go first
+    # in the list so that their testbenches are all grouped together:
+    collnames = []
+    if 'collate' in simulatedict:
+        if isinstance(simulatedict['collate'], list):
+            collnames = simulatedict['collate']
+        else:
+            collnames = [simulatedict['collate']]
 
+        # Now reorder lcondlist so that conditions listed in 'collate' are at
+        # the beginning of the list.
 
-def usage():
-    print('')
-    print('CACE GUI')
-    print(
-        '   Graphical interface for the Circuit Automatic Characterization Engine,'
-    )
-    print('   an analog and mixed-signal design flow system.')
-    print('')
-    print('Usage:')
-    print('   cace_gui.py [characterization_file] [option]')
-    print('')
-    print('where:')
-    print('   characterization_file is a text or JSON file with the')
-    print('       specification of the circuit.')
-    print('')
-    print('and valid options are:')
-    print('   -term')
-    print('       Generate all output to the terminal, not the window.')
-    print('   -help')
-    print('       Print this help text.')
-    print('')
-
-
-# --------------------------------------------------------------------------
-# Main entry point for cace_gui.py
-# --------------------------------------------------------------------------
-
-
-def gui():
-    options = []
-    arguments = []
-    for item in sys.argv[1:]:
-        if item.find('-', 0) == 0:
-            options.append(item.strip('-'))
-        else:
-            arguments.append(item)
+        collnames.reverse()
+        goodcollnames = collnames.copy()
+        for collname in collnames:
+            try:
+                collidx = next(
+                    (
+                        index
+                        for (index, d) in enumerate(lcondlist)
+                        if d['name'] == collname
+                    )
+                )
+            except:
+                print(
+                    'Error:  Request to collate '
+                    + collname
+                    + ' which is not a condition of parameter '
+                    + paramname
+                )
+                goodcollnames.remove(collname)
+            else:
+                lcondlist.insert(0, lcondlist.pop(collidx))
+        # It would presumably be a serious error if a wrong name is in the
+        # 'collate' list, but try to track the good entries so the count of
+        # testbenches to collate doesn't get messed up.
+        collnames = goodcollnames
+
+    # Now revise the list of condition names to contain only the 'name'
+    # records from the condition dictionaries.
+    lcondnames = []
+    for lcond in lcondlist:
+        lcondnames.append(lcond['name'])
+
+    # Find the maximum simulation time required by this parameter
+    # Simulations are ordered so that "risetime" and "falltime" simulations
+    # on a pin will set the simulation time of any simulation of any other
+    # electrical parameter on that same pin.
+
+    if 'Tmax' in condnames:
+        if 'Tmax' not in lcondnames:
+            maxtime = findmaxtime(param, lcondlist)
+            print('maxtime is ' + str(maxtime))
+            maxtimedict = {}
+            maxtimedict['name'] = 'Tmax'
+            maxtimedict['unit'] = 's'
+            maxtimedict['maximum'] = maxtime
+            lcondlist.append(maxtimedict)
+
+    if lcondlist == []:
+        print('Error:  Empty condition list for electrical parameter.')
+        if debug:
+            print('conditions in testbench: ' + ' '.join(condnames))
+            print('conditions in parameter: ' + ' '.join(pcondnames))
+        return param
+
+    # Find the length of each generator
+    cgenlen = []
+    for cond in lcondlist:
+        cgenlen.append(len(list(condition_gen(cond))))
+
+    if debug:
+        print('Full condition list (lcondlist) is:')
+        print('   ' + ' '.join(lcondnames))
+
+    # The lengths of all generators multiplied together is the number of
+    # simulations to be run
+    numsims = reduce(lambda x, y: x * y, cgenlen)
+    rlen = [x for x in cgenlen]
+
+    # The portion of cgenlen that corresponds to collated results is used
+    # to find the number of simulations that are grouped together for
+    # collation after simulaton.
+
+    if collnames:
+        numcolvars = len(collnames)
+        numcollated = reduce(lambda x, y: x * y, cgenlen[0:numcolvars])
+        # Record the group size
+        simulatedict['group_size'] = numcollated
 
-    signal.signal(signal.SIGUSR1, signal.SIG_IGN)
-    root = tkinter.Tk()
-    app = CACECharacterize(root)
-
-    if 'term' in options or 'help' in options:
-        # Revert output to the terminal
-        sys.stdout = app.stdout
-        sys.stderr = app.stderr
-
-    if 'help' in options:
-        usage()
-        sys.exit(0)
-
-    if arguments:
-        print('Setting datasheet to ' + arguments[0])
-        app.set_datasheet(arguments[0])
+        # Diagnostic
+        if debug:
+            print('Collated variables = ' + ' '.join(collnames))
+            print('Number of grouped testbenches = ' + str(numcollated))
     else:
-        # Check the current working directory and determine if there
-        # is a .txt or .json file with the name of the directory, which
-        # is assumed to have the same name as the project circuit.  Also
-        # check subdirectories one level down.
-        curdir = os.getcwd()
-        dirname = os.path.split(curdir)[1]
-        dirlist = os.listdir(curdir)
-
-        # Look through all directories for a '.txt' file
-        found = False
-        for item in dirlist:
-            if os.path.isfile(item):
-                fileext = os.path.splitext(item)[1]
-                basename = os.path.splitext(item)[0]
-                if fileext == '.txt':
-                    if basename == dirname:
-                        print('Setting datasheet to ' + item)
-                        app.set_datasheet(item)
-                        found = True
-                        break
-            elif os.path.isdir(item):
-                subdirlist = os.listdir(item)
-                for subitem in subdirlist:
-                    subitemref = os.path.join(item, subitem)
-                    if os.path.isfile(subitemref):
-                        fileext = os.path.splitext(subitem)[1]
-                        basename = os.path.splitext(subitem)[0]
-                        if fileext == '.txt':
-                            if basename == dirname:
-                                print('Setting datasheet to ' + subitemref)
-                                app.set_datasheet(subitemref)
-                                found = True
-                                break
-
-        # Look through all directories for a '.json' file
-        # ('.txt') is preferred to ('.json')
-
-        if not found:
-            for item in dirlist:
-                if os.path.isfile(item):
-                    fileext = os.path.splitext(item)[1]
-                    basename = os.path.splitext(item)[0]
-                    if fileext == '.json':
-                        if basename == dirname:
-                            print('Setting datasheet to ' + item)
-                            app.set_datasheet(item)
-                            found = True
-                            break
-                elif os.path.isdir(item):
-                    subdirlist = os.listdir(item)
-                    for subitem in subdirlist:
-                        subitemref = os.path.join(item, subitem)
-                        if os.path.isfile(subitemref):
-                            fileext = os.path.splitext(subitem)[1]
-                            basename = os.path.splitext(subitem)[0]
-                            if fileext == '.json':
-                                if basename == dirname:
-                                    print('Setting datasheet to ' + subitemref)
-                                    app.set_datasheet(subitemref)
-                                    found = True
-                                    break
+        if debug:
+            print('No collation in parameter ' + param['name'])
 
-        if not found:
-            print('No datasheet found in local project (JSON or text file).')
+    # This code repeats each condition as necessary such that the final list
+    # (transposed) is a complete set of unique condition combinations.
+    cgensim = []
+    for i in range(len(rlen)):
+        mpre = reduce(lambda x, y: x * y, rlen[0:i], 1)
+        mpost = reduce(lambda x, y: x * y, rlen[i + 1 :], 1)
+        clist = list(condition_gen(lcondlist[i]))
+        duplist = [
+            item
+            for item in list(condition_gen(lcondlist[i]))
+            for j in range(mpre)
+        ]
+        cgensim.append(duplist * mpost)
+
+    # Transpose this list
+    simvals = list(map(list, zip(*cgensim)))
+
+    # Make parameter substitutions into each template file and generate
+    # an output simulatable file.  Record the names of the testbenches
+    # created.
+
+    for testbench, tool in zip(testbenches, tools):
+        template = os.path.join(testbenchpath, testbench)
+        if os.path.isfile(template):
+            param['testbenches'] = substitute(
+                paramname,
+                paths,
+                tool,
+                template,
+                dutpath,
+                simvals,
+                schemline,
+                pdkname,
+                debug,
+            )
+        else:
+            print('Error:  No testbench file ' + template + '.')
 
-    root.mainloop()
+    return param
 
 
-if __name__ == '__main__':
-    gui()
+# ------------------------------------------------------------------------
```

### Comparing `cace-2.1.9/cace/common/cace_calculate.py` & `cace-2.2.0/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/cace_collate.py` & `cace-2.2.0/cace/common/cace_unused.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,679 +1,498 @@
 #!/usr/bin/env python3
-# --------------------------------------------------------------------------
-# cace_collate.py
-# --------------------------------------------------------------------------
+#--------------------------------------------------------------------------
+# cace_unused.py
+#--------------------------------------------------------------------------
 #
-# This script follows cace_measure by taking the collection of output
-# results generated for each set of conditions by the simulation and
-# following measurements, calculating minimum/typical/maximum values
-# for the set, and using the results to annotate the original
-# characterization dataset.
+# Location of any code written for the original CACE system that has not
+# been folded into the new code but may be relevant.
 #
-# --------------------------------------------------------------------------
+#--------------------------------------------------------------------------
 
 import os
 import sys
 import shutil
 import json
 import re
-import math
+import datetime
 import subprocess
 
-from .spiceunits import spice_unit_unconvert
-from .spiceunits import spice_unit_convert
 
-from .cace_calculate import twos_complement
+def cace_measure_orig(testbench):
 
-# ---------------------------------------------------------------------------
-# find_limits ---
-#
-# Calculation of results from collected data for an output record, given
-# the type of calculation to perform in 'calctype'.  The primary calculations
-# are minimum, maximum, and typical, although these definitions are nuanced
-# and the actual calculation performed is provided as a parameter.
-#
-# Future development:
-# Add "minimax", "maximin", and "typical" to calctypes (needs extra record(s))
-# Add "range" to limittypes (needs extra record or tuple for target)
-#
-#    "spectype" is one of "minimum", "maximum", or "typical".
-#    "spec" is the list value of spectype in a parameter's "spec" dictionary.
-# 	This is a numerical value that is the spec target, optionally followed
-# 	by "pass" or "fail", where "fail" implies that exceeding the value is
-# 	a failure to meet spec; and optionally followed by "calctype"-"limittype":
-# 	"calctype" is one of:  average, minimum, maximum
-# 	"limittype" is one of: above, below, exact
-#    "results" is a list of rsult values
-#    "units" is the units type (string) of the result value.
-#
-# The return value is a list in the same format as "spec" but where the
-# first entry is the measured result, the second entry is the score
-# ("pass" or "fail"), and there is no third entry.
-#
-# ---------------------------------------------------------------------------
+    results = testbench['results']
+    format = testbench['format']
 
+    for rlist in results:
 
-def find_limits(spectype, spec, results, units, debug=False):
-
-    # 'spec' is a list of [value, pass|fail, calculation-limit], but
-    # if only "value" is present it may be interpreted as a string.
-
-    if isinstance(spec, list):
-        target = spec[0]
-        penalty = spec[1] if len(spec) > 1 else 'pass'
-        calcrec = spec[2] if len(spec) > 2 else spectype
-    elif isinstance(spec, str):
-        target = spec
-        penalty = 'pass'
-        calcrec = spectype
-
-    # Prepare a list to return
-    specresult = []
-
-    binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
+        # "variables" are similar to conditions but describe what is
+        # being output from ngspice.  There should be one entry for
+        # each (unique) column in the data file, matching the names
+        # given in the testbench file.
 
-    # Note:
-    # calctype = "minimum" alone implies "minimum-above"
-    # calctype = "maximum" alone implies "maximum-below"
-    # calctype = "average" alone implies "average-exact"
-    # calctype = "typical" alone implies "average-exact"
-
-    if debug:
-        print('Diagnostic:  find_limits')
-        print('spectype = ' + spectype)
-        print('spec = ' + str(spec))
-        print('results = ' + str(results))
-        print('units = ' + units)
-        print('target = ' + target)
-        print('penalty = ' + penalty)
-        print('calcrec = ' + calcrec)
-
-    try:
-        calctype, limittype = calcrec.split('-')
-    except ValueError:
-        calctype = calcrec
-        if calctype == 'minimum':
-            limittype = 'above'
-        elif calctype == 'maximum':
-            limittype = 'below'
-        elif calctype == 'average':
-            limittype = 'exact'
-        elif calctype == 'typical':
-            limittype = 'exact'
-        elif calctype == 'diffmin':
-            limittype = 'above'
-        elif calctype == 'diffmax':
-            limittype = 'below'
+        if 'variables' in param:
+            pvars = param['variables']
         else:
-            # Diagnostic:
-            print('Failure:  Unknown calculation type ' + calctype)
-            return ['failure', 'fail']
-
-    # Quick format sanity check---may need binary or hex conversion
-    # using the units nomenclature of 'b or 'h, etc.
-    # (to be done:  signed conversion, see cace_makeplot.py)
-
-    if isinstance(results[0], str):
-        bmatch = binrex.match(units)
-        if bmatch:
-            digits = bmatch.group(1)
-            if digits == '':
-                digits = len(results[0])
-            else:
-                digits = int(digits)
-            base = bmatch.group(2)
-            if base == 'b':
-                a = list(int(x, 2) for x in results)
-            elif base == 'o':
-                a = list(int(x, 8) for x in results)
-            elif base == 'd':
-                a = list(int(x, 10) for x in results)
-            else:
-                a = list(int(x, 16) for x in results)
-            results = list(twos_complement(x, digits) for x in a)
-        elif results[0] != 'failure':
-            print('Warning: result data do not correspond to specified units.')
-            print('Data = ' + str(results))
-            return ['failure', 'fail']
-
-    # The target and result should both match the specified units, so convert
-    # the target if it is a binary, hex, etc., value.
-    if target != 'any':
-        targval = target
-        bmatch = binrex.match(units)
-        if bmatch:
-            digits = bmatch.group(1)
-            base = bmatch.group(2)
-            if digits == '':
-                digits = len(targval)
-            else:
-                digits = int(digits)
-            try:
-                if base == 'b':
-                    a = int(targval, 2)
-                elif base == 'o':
-                    a = int(targval, 8)
-                elif base == 'd':
-                    a = int(targval, 10)
-                else:
-                    a = int(targval, 16)
-                targval = twos_complement(a, digits)
-            except:
-                print(
-                    'Warning: target data do not correspond to units; assuming integer.'
-                )
-
-    # First run the calculation to get the single result value
-
-    if calctype == 'minimum':
-        # Result is the minimum of the data
-        value = min(results)
-    elif calctype == 'maximum':
-        # Result is the maximum of the data
-        value = max(results)
-    elif calctype == 'average' or calctype == 'typical':
-        # Result is the average of the data
-        value = sum(results) / len(results)
-    elif calctype[0:3] == 'std':
-        # Result is the standard deviation of the data
-        mean = sum(results) / len(results)
-        value = pow(
-            sum([((i - mean) * (i - mean)) for i in results]) / len(results),
-            0.5,
-        )
-        # For "stdX", where "X" is an integer, multiply the standard deviation by X
-        if len(calctype) > 3:
-            value *= int(calctype[3])
-
-        if len(calctype) > 4:
-            # For "stdXn", subtract X times the standard deviation from the mean
-            if calctype[4] == 'n':
-                value = mean - value
-            # For "stdXp", add X times the standard deviation to the mean
-            elif calctype[4] == 'p':
-                value = mean + value
-    elif calctype == 'diffmax':
-        value = max(results) - min(results)
-    elif calctype == 'diffmin':
-        value = min(results) - max(results)
-    else:
-        return ['failure', 'fail']
+            pvars = []
 
-    try:
-        specresult.append('{0:.4g}'.format(value))
-    except ValueError:
-        print(
-            'Warning: Min/Typ/Max value is not not numeric; value is '
-            + str(value)
-        )
-        return ['failure', 'fail']
-
-    # Next calculate the score based on the limit type
-
-    score = 'pass'
-    if limittype == 'above':
-        # Score a penalty if value is below the target
-        if target != 'any' and penalty == 'fail':
-            targval = float(target)
-
-            if debug:
-                print('minimum = ' + str(value))
-            # NOTE: 0.0005 value corresponds to formatting above, so the
-            # value is not marked in error unless it would show a different
-            # value in the display.
-            if value < targval - 0.0005:
-                score = 'fail'
-                if debug:
-                    print('fail: target = ' + str(score) + '\n')
-            elif math.isnan(value):
-                score = 'fail'
+        # Parse all additional variables.  At least one (the
+        # analysis variable) must be specified.
+        data_args = []
+        extra = rest.split()
+
+        if len(extra) == 1:
+            # If the testbench specifies no vectors, then they
+            # must all be specified in order in 'variables' in
+            # the datasheet entry for the electrical parameters.
+            for var in pvars:
+                extra.append(var['condition'])
+            if not pvars:
+                print('Error:  No variables specified in testbench or datasheet.')
+                rest = ''
+
+        if len(extra) > 1:
+            for varname in extra[1:]:
+                if varname not in locvarresult:
+                    locvarresult[varname] = []
+                data_args.append(locvarresult[varname])
 
-    elif limittype == 'below':
-        # Score a penalty if value is above the target
-        if target != 'any' and penalty == 'fail':
-            targval = float(target)
-
-            if debug:
-                print('maximum = ' + str(value))
-            # NOTE: 0.0005 value corresponds to formatting above, so the
-            # value is not marked in error unless it would show a different
-            # value in the display.
-            if value > targval + 0.0005:
-                score = 'fail'
-                if debug:
-                    print('fail: target = ' + str(score))
-            elif math.isnan(value):
-                score = 'fail'
+            rsize = read_ascii_datafile(extra[0], *data_args)
+            # print('Read data file, rsize = ' + str(rsize))
 
-    elif limittype == 'exact':
-        # Score a penalty if value is not equal to the target
-        if target != 'any' and penalty == 'fail':
-            targval = float(target)
+            # All values in extra[1:] should be param['variables'].  If not, add
+            # an entry and flag a warning because information may be incomplete.
 
-            if value != targval:
-                score = 'fail'
-                if debug:
-                    print('off-target failure')
-            elif math.isnan(value):
-                score = 'fail'
-
-    # Note:  Calctype 'none' performs no calculation.  Record is unchanged,
-    # and "score" is returned unchanged.
-
-    specresult.append(score)
-    return specresult
+            for varname in extra[1:]:
+                try:
+                    var = next(item for item in pvars if item['condition'] == varname)
+                except StopIteration:
+                    print('Variable ' + varname + ' not specified;  ', end='')
+                    print('information may be incomplete.')
+                    var = {}
+                    var['condition'] = varname
+                    pvars.append(var)                                    
+
+            # By default, the 2nd result is the result
+            if len(extra) > 2:
+                varname = extra[2]
+                varrec = next(item for item in pvars if item['condition'] == varname)
+                varrec['result'] = True
+                print('Setting condition ' + varname + ' as the result vector.')
+
+            # "measure" records are applied to individual simulation outputs,
+            # usually to reduce a time-based vector to a single value by
+            # measuring a steady-state value, peak-peak, frequency, etc.
+
+            if 'measure' in param:
+                # Diagnostic
+                # print('Applying measurements.')
+
+                for measure in param['measure']:
+                    rsize = apply_measure(locvarresult, measure, pvars)
+                    # Diagnostic
+                    # print("after measure, rsize = " + str(rsize))
+                    # print("locvarresult = " + str(locvarresult))
+
+                # Now recast locvarresult back into loccondresult.
+                for varname in locvarresult:
+                    varrec = next(item for item in pvars if item['condition'] == varname)
+                    if 'result' in varrec:
+                        # print('Result for ' + varname + ' = ' + str(locvarresult[varname]))
+                        locparamresult = locvarresult[varname]
+                        paramname = varname
+                    else:
+                        # print('Condition ' + varname + ' = ' + str(locvarresult[varname]))
+                        loccondresult[varname] = locvarresult[varname]
+                    # Diagnostic
+                    # print("Variable " + varname + " length = " + str(len(locvarresult[varname])))
 
+            else:
+                # For plots, there is not necessarily any measurements.  Just
+                # copy values into locparamresult and loccondresult.
+                if len(locvarresult) == 0:
+                    print('Warning: No result data for plot!')
+                for varname in locvarresult:
+                    varrec = next(item for item in pvars if item['condition'] == varname)
+                    if 'result' in varrec:
+                        # print('Result for ' + varname + ' = ' + str(locvarresult[varname]))
+                        locparamresult = locvarresult[varname]
+                        rsize = len(locparamresult)
+                        paramname = varname
+                    else:
+                        # print('Condition ' + varname + ' = ' + str(locvarresult[varname]))
+                        loccondresult[varname] = locvarresult[varname]
+                rest = ''
+    else:
+        rsize = 0
 
-# ----------------------------------------------------------------------
-# incompleteresult --
-#
-# Handle errors where simulation generated no output.
-# This is the one case where 'typical' can be treated as pass-fail.
-# score will be set to "incomplete" for any of "minimum", "maximum",
-# and "typical" that exists in the electrical parameters record
-# and which specifies a target value.  "value" is set to "failure"
-# for display.
-# ----------------------------------------------------------------------
-
-
-def incompleteresult(param, noplotmode=False):
-
-    resultdict = {}
-
-    if 'plot' in param:
-        if noplotmode == False:
-            resultdict['status'] = 'incomplete'
-
-    if 'spec' not in param:
-        return resultdict
-
-    spec = param['spec']
-
-    if 'typical' in spec:
-        typrec = spec['typical']
-        typresult = ['failure']
-        if typrec[0] != 'any':
-            typresult.append('incomplete')
-        resultdict['typical'] = typresult
-
-    if 'maximum' in spec:
-        maxrec = spec['maximum']
-        maxresult = ['failure']
-        if maxrec[0] != 'any':
-            maxresult.append('incomplete')
-        resultdict['maximum'] = maxresult
-
-    if 'minimum' in spec:
-        minrec = spec['minimum']
-        minresult = ['failure']
-        if minrec[0] != 'any':
-            minresult.append('incomplete')
-        resultdict['minimum'] = minresult
+    # Simple outputs are followed by a single value
+    outrex = re.compile("[ \t]*\"?([^ \t\"]+)\"?(.*)$", re.IGNORECASE)
+    # conditions always follow as key=value pairs
+    dictrex = re.compile("[ \t]*([^ \t=]+)=([^ \t=]+)(.*)$", re.IGNORECASE)
+    # conditions specified as min:step:max match a result vector.
+    steprex = re.compile("[ \t]*([^:]+):([^:]+):([^:]+)$", re.IGNORECASE)
+    # specification of units as a binary, hex, etc., string in verilog format
+    binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
 
-    return resultdict
 
+                    # To-do:  Handle raw files in similar manner to ASCII files.
+                      
+                    while rest:
+                        # This code depends on values coming first, followed by conditions.
+                        matchtext = dictrex.match(rest)
+                        if matchtext:
+                            # Diagnostic!
+                            condname = matchtext.group(1)
+                            # Append to the condition list
+                            if condname not in loccondresult:
+                                loccondresult[condname] = []
+
+                            # Find the condition name in the condition list, so values can
+                            # be converted back to the expected units.
+                            try:
+                                condrec = next(item for item in param['conditions'] if item['condition'] == condname)
+                            except StopIteration:
+                                condunit = ''
+                            else:
+                                condunit = condrec['unit']
+
+                            rest = matchtext.group(3)
+                            matchstep = steprex.match(matchtext.group(2))
+                            if matchstep:
+                                # condition is in form min:step:max, and the
+                                # number of values must match rsize.
+                                cmin = float(matchstep.group(1))
+                                cstep = float(matchstep.group(2))
+                                cmax = float(matchstep.group(3))
+                                cnum = int(round((cmax + cstep - cmin) / cstep))
+                                if cnum != rsize:
+                                    print("Warning: Number of conditions (" + str(cnum) + ") is not")
+                                    print("equal to the number of results (" + str(rsize) + ")")
+                                    # Back-calculate the correct step size.  Usually this
+                                    # means that the testbench did not add margin to the
+                                    # DC or AC stop condition, and the steps fell 1 short of
+                                    # the max.
+                                    if rsize > 1:
+                                        cstep = (float(cmax) - float(cmin)) / float(rsize - 1)
+
+                                condvec = []
+                                for r in range(rsize):
+                                    condvec.append(cmin)
+                                    cmin += cstep
+
+                                cresult = spice_unit_unconvert([condunit, condvec])
+                                condval = loccondresult[condname]
+                                for cr in cresult:
+                                    condval.append(str(cr))
+
+                            else:
+                                # If there is a vector of results but only one condition, copy the
+                                # condition for each result.  Note that value may not be numeric.
+
+                                # (To do:  Apply 'measure' records here)
+                                condval = loccondresult[condname]
+                                try:
+                                    test = float(matchtext.group(2))
+                                except ValueError:
+                                    cval = matchtext.group(2)
+                                else:
+                                    cval = str(spice_unit_unconvert([condunit, test]))
+                                for r in range(rsize):
+                                    condval.append(cval)
+                        else:
+                            # Not a key=value pair, so must be a result value
+                            matchtext = outrex.match(rest)
+                            if matchtext:
+                                rest = matchtext.group(2)
+                                rsize += 1
+                                # Result value units come directly from the param record.
+                                if 'unit' in param:
+                                    condunit = param['unit']
+                                else:
+                                    condunit = ''
+                                if binrex.match(condunit):
+                                    # Digital result with units 'b, 'h, etc. are kept as strings.
+                                    locparamresult.append(matchtext.group(1))
+                                else:
+                                    locparamresult.append(float(matchtext.group(1)))
+                            else:
+                                print('Error:  Result line cannot be parsed.')
+                                print('Bad part of line is: ' + rest)
+                                print('Full line is: ' + line)
+                                break
+
+                    # Values passed in testbench['conditions'] are common to each result
+                    # value.  From one line there are rsize values, so append each known
+                    # condition to loccondresult rsize times.
+                    for condrec in testbench['conditions']:
+                        condname = condrec[0]
+                        if condname in locvarresult:
+                            print('Error:  name ' + condname + ' is both a variable and a condition!')
+                            print('Ignoring the condition.')
+                            continue
+                        if condname not in loccondresult:
+                            loccondresult[condname] = []
+                        condval = loccondresult[condname]
+                        if 'unit' in condrec:
+                            condunit = condrec['unit']
+                        else:
+                            condunit = ''
+                        for r in range(rsize):
+                            if condname.split(':')[0] == 'DIGITAL' or condname == 'CORNER':
+                                # Values that are known to be strings
+                                condval.append(condrec[2])
+                            elif binrex.match(condunit):
+                                # Alternate digital specification using units 'b, 'h, etc.
+                                condval.append(condrec[2])
+                            elif condname == 'ITERATIONS':
+                                # Values that are known to be integers
+                                condval.append(int(float(condrec[2])))
+                            else:
+                                # All other values to be treated as floats unless
+                                # they are non-numeric, in which case they are
+                                # treated as strings and copied as-is.
+                                try:
+                                    condval.append(float(condrec[2]))
+                                except ValueError:
+                                    # Values that are not numeric just get copied
+                                    condval.append(condrec[2])
+
+            if len(locparamresult) > 0:
+                # Fold local results into total results
+                paramresult.extend(locparamresult)
+                for key in loccondresult:
+                    if not key in condresult:
+                        condresult[key] = loccondresult[key]
+                    else:
+                        condresult[key].extend(loccondresult[key])
 
-# -------------------------------------------------------------
-# addnewresult --
-#
-# If the result dictionary has the same name as one in the
-# datasheet, then it replaces it.  Otherwise it is appended
-# to the list.
-# -------------------------------------------------------------
-
-
-def addnewresult(param, resultdict):
-    replaced = False
-    if 'results' in param:
-        newresultlist = []
-        paramresults = param['results']
-        if not isinstance(paramresults, list):
-            paramresults = [paramresults]
-        for result in paramresults:
-            if result['name'] == resultdict['name']:
-                newresultlist.append(resultdict)
-                replaced = True
             else:
-                newresultlist.append(result)
-        if replaced == False:
-            newresultlist.append(resultdict)
-        param['results'] = newresultlist
-    else:
-        param['results'] = resultdict
+                # Catch simulation failures
+                measurefailures += 1
 
+            measurements += 1
 
-# ---------------------------------------------------------------------------
-# Main entry point of cace_collate
-#
-# "param" is an electrical parameter dictionary to be evaluated.
-# The "param" dictionary is annotated with results; and the modified
-# dictionary is returned.
-#
-# At the end of running all measurements, there should be a number of
-# "testbench" records for the parameter, each containing a unique set of
-# conditions, and a "results" section which is normally a single value
-# (see code comments about dealing with multiple values).
-# ---------------------------------------------------------------------------
-
-
-def cace_collate(dsheet, param):
-
-    runtime_options = dsheet['runtime_options']
-    try:
-        debug = runtime_options['debug']
-    except:
-        debug = False
-
-    try:
-        keepmode = runtime_options['keep']
-    except:
-        keepmode = False
-
-    try:
-        noplotmode = runtime_options['noplot']
-    except:
-        noplotmode = False
+        #------end of loop over testbenches
 
-    if 'default_conditions' in dsheet:
-        default_conditions = dsheet['default_conditions']
-    else:
-        default_conditions = []
+        # Evaluate concatentated results after all files for this electrical parameter
+        # have been run through simulation.
 
-    total = 0
+        if paramresult:
+            print(testbenchname + ':')
 
-    if 'status' in param:
-        status = param['status']
-    else:
-        status = 'active'
-        param['status'] = status
-
-    if status == 'skip' or status == 'blocked' or 'testbenches' not in param:
-        if debug:
-            print('Parameter ' + param['name'] + ' skipped for evaluation.')
-        return param
-
-    paramname = param['name']
-    status = param['status']
-
-    # Process only entries in dataset that have 'testbenches' record
-    if status == 'skip' or status == 'blocked':
-        return param
-
-    elif 'testbenches' not in param:
-        if debug:
-            print(
-                'Error:  Parameter '
-                + paramname
-                + ' specified to be evaluated, but no testbench record exists.'
-            )
-        return param
-    elif debug:
-        print('Collating results for parameter ' + paramname)
+            # Diagnostic
+            # print("paramresult length " + str(len(paramresult)))
+            # for key in condresult:
+            #     print("condresult length " + str(len(condresult[key])))
 
-    if 'spec' in param:
-        spec = param['spec']
-    else:
-        spec = {}
-    testbenches = param['testbenches']
+            # Write out all results into the JSON file.
+            # Results are a list of lists;  the first list is a list of
+            # methods, and the rest are sets of values corresponding to unique
+            # conditions.  The first item in each lists is the result value
+            # for that set of conditions.
 
-    # Each item in "testbenches" has a filename (was simulated in
-    # cace_launch and is no longer used), a set of conditions (prepared
-    # by cace_gensim), and a set of results (read back from simulation
-    # output by cace_launch).  There may be multiple results which are
-    # dependent on variables not in the "conditions" list;  these
-    # variables are listed in the "format" line of the "measure"
-    # dictionary that was used to understand the simulation output.
-
-    # This information is used to create a single large matrix of the
-    # result vs. all conditions and variables for the electrical
-    # parameter as a whole.  That matrix may be passed through additional
-    # evaluators (specified in the "evaluate" dictionary) to modify the
-    # result and potentially reduce the number of variables.  The final
-    # output is stored in the "results" list for the electrical parameter.
-    # Finally, the "results" list is scanned to extract minimum, typical,
-    # and maximum values as required for the datasheet.
-
-    # Policy regarding testbench failures:  If any testbench has failed,
-    # the score is set to "incomplete".  If a portion of testbench
-    # simulations ran and some failed, then the score may be changed to
-    # "fail".
-
-    score = 'pass'
-    for testbench in testbenches:
-        filename = testbench['filename']
-        if 'results' not in testbench:
-            print('Error: testbench ' + filename + ' has no results!')
-            score = 'incomplete'
-            break
-        else:
-            results = testbench['results']
-            if len(results) == 0:
-                print(
-                    'Error: testbench '
-                    + filename
-                    + ' has zero-length results!'
-                )
-                score = 'incomplete'
-                break
-
-    typresults = []
-    if 'typical' in spec:
-        # Generate a list of results that were made under conditions
-        # that were either typical or did not specify a typical value.
-
-        for testbench in testbenches:
-            istypical = True
-            for condition in testbench['conditions']:
-                # Pull record of the condition (by definition this must
-                # exist in either the electrical parameter conditions list
-                # or the default conditions list).
-                try:
-                    condrec = next(
-                        item
-                        for item in param['conditions']
-                        if item['name'] == condition[0]
-                    )
-                except StopIteration:
-                    condrec = next(
-                        item
-                        for item in default_conditions
-                        if item['name'] == condition[0]
-                    )
-
-                if 'typical' in condrec:
-                    typvalue = condrec['typical']
-                    if typvalue != condition[-1]:
-                        istypical = False
-                        break
-            if istypical == True:
-                if 'results' in testbench:
-                    typresults.extend(testbench['results'])
-
-    allresults = []
-    for testbench in testbenches:
-        if 'results' in testbench:
-            allresults.extend(testbench['results'])
-
-    # Results is still a list of lists.  Pull out the inner list.
-    # Flag a warning if the inner list isn't just a single item
-    # (the result), unless 'plot' is specified and not 'spec',
-    # in which case this is normal.
+            # Always keep results, even for remote CACE.
 
-    isplotdata = True if 'spec' not in param and 'plot' in param else False
+            outnames = [paramname]
+            outunits = []
 
-    if len(allresults) == 0:
-        scaled_results = []
-    else:
-        reduced_results = []
-        if isinstance(allresults[0], list):
-            for result in allresults:
-                if len(result) > 1:
-                    if not isplotdata:
-                        print(
-                            'Error:  There are multiple results per testbench!'
-                        )
+            if 'unit' in param:
+                outunits.append(param['unit'])
+            else:
+                outunits.append('')
+            for key in condresult:
+                outnames.append(key)
                 try:
-                    rvalue = float(result[0])
+                    condrec = next(item for item in param['conditions'] if item['condition'] == key) 
                 except:
                     try:
-                        print(
-                            'Error:  Result '
-                            + str(result[0])
-                            + ' is not numeric!'
-                        )
+                        condrec = next(item for item in param['variables'] if item['condition'] == key) 
                     except:
-                        print('Error:  No result!')
-                    rvalue = 0.0
-                reduced_results.append(rvalue)
-        else:
-            for result in allresults:
+                        outunits.append('')
+                    else:
+                        if 'unit' in condrec:
+                            outunits.append(condrec['unit'])
+                            # 'variable' entries need to be unconverted
+                            cconv = spice_unit_unconvert([condrec['unit'], condresult[key]])
+                            condresult[key] = cconv
+                        else:
+                            outunits.append('')
+                else:
+                    if 'unit' in condrec:
+                        outunits.append(condrec['unit'])
+                    else:
+                        outunits.append('')
+
+            # Evaluate a script to transform the output, if there is a 'measure'
+            # record in the electrical parameter.
+
+            if 'measure' in param:
+
+                evalrec = param['measure']
                 try:
-                    rvalue = float(result)
+                    tool = evalrec['tool']
                 except:
-                    print('Error:  Result ' + str(result) + ' is not numeric!')
-                    rvalue = 0.0
-                reduced_results.append(rvalue)
-
-        # scaled_results is 'results' scaled to the units used by param.
-        if 'unit' in param:
-            scaled_results = spice_unit_unconvert(
-                [param['unit'], reduced_results]
-            )
-        else:
-            scaled_results = reduced_results
+                    print("Error:  Evaluate record does not indicate a tool to run.")
+                    break
+                else:
+                    if tool != 'octave' and tool != 'octave-cli' and tool != 'matlab':
+                        print("Error:  CACE does not know how to use tool '" + tool + "'")
+                        break
 
-    # Now do the same to the typical result set.
+                # Use the command-line-interface version of octave.
+                if tool == 'octave':
+                    tool = 'octave-cli'
 
-    if len(typresults) == 0:
-        scaled_typresults = []
-    else:
-        reduced_results = []
-        if isinstance(typresults[0], list):
-            for result in typresults:
-                if len(result) > 1:
-                    if not isplotdata:
-                        print(
-                            'Error:  There are multiple results per testbench!'
-                        )
                 try:
-                    rvalue = float(result[0])
+                    script = evalrec['filename']
                 except:
+                    print("Error:  Evaluate record does not indicate a script to run.")
+                    break
+                else:
+                    if os.path.isdir(os.path.join(root_path, testbench_path)):
+                        tb_path = os.path.join(root_path, testbench_path, script)
+                        if not os.path.exists(tb_path):
+                            if os.path.exists(tb_path + '.m'):
+                                tb_path += '.m'
+                            else:
+                                print("Error:  No script '" + script + "' found in testbench path.")
+                                break
+                    else:
+                        print("Error:  testbench directory not found in root path.")
+                        break
+
+                # General purpose tool-based measurement.  For complex operations of
+                # any kind, dump the simulation results to a file "results.json" and
+                # invoke the specified tool, which should read the results and
+                # generate an output in the form of modified 'paramresult'.
+                # e.g., input is an array of transient vectors, output is an FFT
+                # analysis.  Input is a voltage, output is an INL value.  Note that
+                # 'unit' is the unit produced by the script.  The script is supposed
+                # to know what units it gets as input and what it produces as output.
+
+            # pconv is paramresult scaled to the units used by param.
+            if 'unit' in param:
+                pconv = spice_unit_unconvert([param['unit'], paramresult])
+            else:
+                pconv = paramresult
+
+            outresult = []
+            outresult.append(outnames)
+            outresult.append(outunits)
+
+            for p in range(len(pconv)):
+                outvalues = []
+                outvalues.append(str(pconv[p]))
+                for key, value in condresult.items():
                     try:
-                        print(
-                            'Error:  Result '
-                            + str(result[0])
-                            + ' is not numeric!'
-                        )
-                    except:
-                        print('Error:  No result!')
-                    rvalue = 0.0
-                reduced_results.append(rvalue)
-        else:
-            for result in typresults:
-                try:
-                    rvalue = float(result)
-                except:
-                    print('Error:  Result ' + str(result) + ' is not numeric!')
-                    rvalue = 0.0
-                reduced_results.append(rvalue)
-
-        # scaled_results is 'results' scaled to the units used by param.
-        if 'unit' in param:
-            scaled_typresults = spice_unit_unconvert(
-                [param['unit'], reduced_results]
-            )
-        else:
-            scaled_typresults = reduced_results
+                        outvalues.append(str(value[p]))
+                    except IndexError:
+                        # Note:  This should not happen. . . 
+                        print("Error:  number of values in result and conditions do not match!")
+                        print("Result: " + str(len(pconv)))
+                        print("Conditions: " + str(len(condresult)))
+                        break
 
-    # Set the value of "units" passed to find_limits()
-    if 'unit' in param:
-        units = param['unit']
-    else:
-        units = ''
+                outresult.append(outvalues)
 
-    # Diagnostic
-    if debug:
-        print('Scaled results are:')
-        if len(scaled_results) > 20:
-            print('(truncated due to length)')
-            print(str(scaled_results[0:10]))
-            print('...')
-            print(str(scaled_results[-10:-1]))
-        else:
-            print(str(scaled_results))
-        if 'typical' in spec:
-            print('Scaled typical results are:')
-            if len(scaled_typresults) > 20:
-                print('(truncated due to length)')
-                print(str(scaled_typresults[0:10]))
-                print('...')
-                print(str(scaled_typresults[-10:-1]))
+            param['results'] = outresult
+
+            if 'unit' in param:
+                units = param['unit']
             else:
-                print(str(scaled_typresults))
+                units = ''
 
-    # Calculate minimum/typical/maximum results for the electrical parameter
-    if len(scaled_results) == 0:
-        if 'minimum' in spec or 'maximum' in spec:
-            resultdict = incompleteresult(param, noplotmode)
-        else:
-            resultdict = {}
-    else:
-        resultdict = {}
-        if 'minimum' in spec:
-            spectype = 'minimum'
-            minrec = spec['minimum']
-            minresult = find_limits(
-                spectype, minrec, scaled_results, units, debug
-            )
-            if score == 'incomplete' and minresult[1] == 'fail':
+            # Catch simulation failures.
+            if measurefailures > 0:
+                print('Measurement failures:  ' + str(measurefailures))
                 score = 'fail'
-            elif score != 'fail':
-                score = minresult[1]
-            resultdict['minimum'] = minresult
-
-        if 'maximum' in spec:
-            spectype = 'maximum'
-            maxrec = spec['maximum']
-            maxresult = find_limits(
-                spectype, maxrec, scaled_results, units, debug
-            )
-            if score == 'incomplete' and maxresult[1] == 'fail':
-                score = 'fail'
-            elif score != 'fail':
-                score = maxresult[1]
-            resultdict['maximum'] = maxresult
-
-    if len(scaled_typresults) == 0:
-        if 'typical' in spec:
-            resultdict = incompleteresult(param, noplotmode)
-    else:
-        if 'typical' in spec:
-            spectype = 'typical'
-            typrec = spec['typical']
-            typresult = find_limits(
-                spectype, typrec, scaled_typresults, units, debug
-            )
-            if score == 'incomplete' and typresult == 'fail':
-                score = 'fail'
-            elif score != 'fail':
-                score = typresult[1]
-            resultdict['typical'] = typresult
-
-    # Results belong to a key name in the electrical parameter that
-    # depends on where the source netlists came from.
-
-    resultdict['name'] = runtime_options['netlist_source']
-    if debug:
-        print(
-            'Adding new result set '
-            + resultdict['name']
-            + ' for '
-            + param['name']
-        )
-    addnewresult(param, resultdict)
 
-    # Return the annotated electrical parameter
-    return param
+            if 'minimum' in param:
+                minrec = param['minimum']
+                if 'calc' in minrec:
+                    calc = minrec['calc']
+                else:
+                    calc = 'min-above'
+                minscore = calculate(minrec, pconv, condresult, calc, score, units, param)
+                if score != 'fail':
+                    score = minscore
+
+            if 'maximum' in param:
+                maxrec = param['maximum']
+                if 'calc' in maxrec:
+                    calc = maxrec['calc']
+                else:
+                    calc = 'max-below'
+                maxscore = calculate(maxrec, pconv, condresult, calc, score, units, param)
+                if score != 'fail':
+                    score = maxscore
+
+            if 'typical' in param:
+                typrec = param['typical']
+                if 'calc' in typrec:
+                    calc = typrec['calc']
+                else:
+                    calc = 'avg-legacy'
+                typscore = calculate(typrec, pconv, condresult, calc, score, units, param)
+                if score != 'fail':
+                    score = typscore
+
+            if 'plot' in param:
+                # If in plotmode then create a plot and save it to a file.
+                plotrec = param['plot']
+                if plotmode == True:
+                    if 'variables' in param:
+                        variables = param['variables']
+                    else:
+                        variables = []
+                    result = cace_makeplot.makeplot(plotrec, param['results'], variables)
+                    if result:
+                        plotrec['status'] = 'done'
+                        has_aux_files = True
+                    else:
+                        print('Failure:  No plot from file ' + filename + '\n')
+                else:
+                    plotrec['status'] = 'done'
+        else:
+            try:
+                print('Failure:  No output from file ' + filename + '\n')
+            except NameError:
+                print('Failure:  No simulation file, so no output\n')
+                continue
+
+            # Handle errors where simulation generated no output.
+            # This is the one case where 'typical' can be treated as pass-fail.
+            # "score" will be set to "fail" for any of "minimum", "maximum",
+            # and "typical" that exists in the electrical parameters record
+            # and which specifies a target value.  "value" is set to "failure"
+            # for display.
+            score = 'fail'
+            if 'typical' in param:
+                typrec = param['typical']
+                if 'target' in typrec:
+                    typrec['score'] = 'fail'
+                typrec['value'] = 'failure'
+            if 'maximum' in param:
+                maxrec = param['maximum']
+                if 'target' in maxrec:
+                    maxrec['score'] = 'fail'
+                maxrec['value'] = 'failure'
+            if 'minimum' in param:
+                minrec = param['minimum']
+                if 'target' in minrec:
+                    minrec['score'] = 'fail'
+                minrec['value'] = 'failure'
+
+        # Pop the testbenches record, which has been replaced by the 'results' record.
+        if keepmode == False:
+            param.pop('testbenches')
+
+    # Report the final score, and save it to the JSON data
+
+    print('Completed ' + str(measurements) + ' of ' + str(totalmeasure) + ' measurements');
+    print('Circuit pre-extraction simulation total score (lower is better) = '
+			+ str(score))
 
+    # Return 1 if measurements were successful, 0 if not
+    return 0 if measurements == 0 else 1
 
-# ---------------------------------------------------------------------------
+#---------------------------------------------------------------------------
```

### Comparing `cace-2.1.9/cace/common/cace_compat.py` & `cace-2.2.0/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/cace_evaluate.py` & `cace-2.2.0/cace/common/cace_evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     rcfilename = get_magic_rcfile(dsheet)
 
     mproc = subprocess.Popen(
         ['magic', '-dnull', '-noconsole', '-rcfile', rcfilename],
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
-        universal_newlines=True,
+        text=True,
     )
     mproc.stdin.write(
         'if {[catch {puts namespace=$PDKNAMESPACE}]} {puts namespace=$PDKPATH}\n'
     )
     outlines = mproc.communicate()[0]
     retcode = mproc.returncode
     if retcode != 0:
@@ -85,15 +85,15 @@
     rcfilename = get_magic_rcfile(dsheet)
 
     areaproc = subprocess.Popen(
         ['magic', '-dnull', '-noconsole', '-rcfile', rcfilename],
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         cwd=layout_path,
-        universal_newlines=True,
+        text=True,
     )
     if is_mag:
         areaproc.stdin.write('load ' + layout_cellname + '\n')
     else:
         areaproc.stdin.write('gds read ' + layout_locname + '\n')
         areaproc.stdin.write('set toplist [cellname list top]\n')
         areaproc.stdin.write('set numtop [llength $toplist]\n')
@@ -320,15 +320,15 @@
 
     drcproc = subprocess.Popen(
         ['magic', '-dnull', '-noconsole', '-rcfile', rcfile],
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         env=newenv,
         cwd=layout_path,
-        universal_newlines=True,
+        text=True,
     )
 
     if is_mag:
         drcproc.stdin.write('load ' + layout_cellname + '\n')
     else:
         drcproc.stdin.write('gds read ' + layout_locname + '\n')
         drcproc.stdin.write('set toplist [cellname list top]\n')
```

### Comparing `cace-2.1.9/cace/common/cace_launch.py` & `cace-2.2.0/cace/common/cace_launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -313,15 +313,19 @@
                 idx += 1
             # Replace the testbench list in the parameter with the number of
             # testbenches.
             param['testbenches'] = len(param['testbenches'])
 
             for result in results:
                 try:
-                    presult = result.get(timeout=300)
+                    # Note:  Previously used result.get(timeout=300).
+                    # This was intended to prevent hung simulations from
+                    # hanging CACE.  But with multiprocessing, the timeout
+                    # itself causes CACE to hang, making it less than useless.
+                    presult = result.get()
                 except Exception as e:
                     print('simulate_and_measure failed with exception:')
                     print(e)
                     presult = None
                 if presult:
                     alltestbenches.append(presult)
                     simulations += group_size
```

### Comparing `cace-2.1.9/cace/common/cace_makeplot.py` & `cace-2.2.0/cace/common/cace_makeplot.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # For Fedora, for example, need "yum install python-pillow-tk"
 
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 
 from .cace_gensim import twos_comp
 from .cace_collate import addnewresult
+from .spiceunits import spice_unit_unconvert
 
 # -----------------------------------------------------------------------------
 # Given a plot record from a spec sheet and a full set of testbenches, generate
 # a plot.  The name of the plot file and the vectors to plot, labels, legends,
 # and so forth are all contained in the 'plotrec' dictionary.
 #
 # If run from a GUI then "parent" is a window passed by the caller that the
@@ -31,14 +32,17 @@
 #
 # Returns the canvas record generated by matplotlib.
 # -----------------------------------------------------------------------------
 
 
 def cace_makeplot(dsheet, param, parent=None):
 
+    # Regular expression for identifying digital values
+    binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
+
     if 'plot' not in param:
         return None
     else:
         plotrec = param['plot']
 
     if 'variables' not in param:
         variables = []
@@ -54,33 +58,14 @@
     if runtime_options:
         if 'noplot' in runtime_options:
             if runtime_options['noplot']:
                 return None
         if 'debug' in runtime_options:
             debug = runtime_options['debug']
 
-    # Development:  For now, just take the results from the 1st testbench
-    # All testbenches should have the same data, just with different sets
-    # of conditions.  Multiple testbench data will be steps in the graph.
-
-    numtbs = len(param['testbenches'])
-    if numtbs == 0:
-        print('Error:  Plot has no results.')
-
-    tbzero = param['testbenches'][0]
-    results = copy.deepcopy(tbzero['results'])
-
-    binrex = re.compile(r'([0-9]*)\'([bodh])', re.IGNORECASE)
-    # Organize data into plot lines according to formatting
-
-    if 'type' in plotrec:
-        plottype = plotrec['type']
-    else:
-        plottype = 'xyplot'
-
     # The 'format' record of the 'simulate' dictionary in the parameter
     # indicates how the simulation data should be formatted.  The first
     # two items describe how to read the file and are discarded.  The
     # routine that reads the simulation data always moves the "result"
     # entry to the 1st position, so the format needs to be adjusted
     # accordingly.
 
@@ -90,19 +75,41 @@
         if 'result' in simformat:
             ridx = simformat.index('result')
             if ridx != 0:
                 simformat.insert(0, simformat.pop(simformat.index('result')))
     else:
         simformat = ['result']
 
+    if 'type' in plotrec:
+        plottype = plotrec['type']
+    else:
+        plottype = 'xyplot'
+
     if plottype == 'histogram':
         xname = 'result'
     else:
         xname = plotrec['xaxis']
 
+    # Organize data into plot lines according to formatting
+    # Because the data may get rearranged, create a copy of all testbench
+    # results and reference only the copied data.
+    tbdata = copy.deepcopy(param['testbenches'])
+
+    numtbs = len(tbdata)
+    if numtbs == 0:
+        print('Error:  Plot has no results.')
+
+    # All testbenches should have results in the same format.  Use only the
+    # first testbench to determine which column of results represents the
+    # plot's x-axis data.
+
+    zerotb = tbdata[0]
+    results = zerotb['results']
+    conditions = zerotb['conditions']
+
     # In case results[] is not a vector. . .  This should have been handled
     # outside of cace_makeplot and probably needs to be fixed.
 
     if not isinstance(results[0], list):
         for i in range(len(results)):
             result = results[i]
             if not isinstance(result, list):
@@ -112,62 +119,104 @@
     # data, so pick up the number of items per result from the 1st entry.
 
     rlen = len(results[0])
     try:
         xidx = next(r for r in range(rlen) if simformat[r] == xname)
     except StopIteration:
 
+        if debug:
+            print('Refactoring testbench data for plot vs. ' + xname)
+
         # x-axis variable is not in the variable list.  If it exists as
         # a testbench condition and varies over the testbenches, then
         # add a column to each row of results to represent the variable,
-        # and add all testbench results to the <results> array.
+        # and then reorganize the testbenches.
 
-        conditions = tbzero['conditions']
         notfound = True
         for cond in conditions:
             if cond[0] == xname:
                 condvalue = cond[2]
                 notfound = False
                 break
 
         if notfound:
             print('Plot error:  No signal ' + xname + ' recorded in format.')
             return None
 
-        for result in results:
-            result.append(condvalue)
-
-        for tbi in param['testbenches'][1:]:
-            conditions = tbi['conditions']
+        # For each testbench, add the x-axis condition value to to the results.
+        # Also create a string representation of all condition values except
+        # the x-axis condition for each testbench, and save it.
+
+        for tbidx in range(0, numtbs):
+            thistb = tbdata[tbidx]
+            tbresults = thistb['results']
+            conditions = thistb['conditions']
+            condstr = ''
             for cond in conditions:
                 if cond[0] == xname:
                     condvalue = cond[2]
-                    break
-            for result in tbi['results']:
+                else:
+                    condstr += cond[2]
+            thistb['condstr'] = condstr
+            newtbresults = []
+            for result in tbresults:
                 if isinstance(result, list):
-                    newresult = result.copy()
+                    newresult = result
                 else:
                     newresult = [result]
                 newresult.append(condvalue)
-                results.append(newresult)
+                newtbresults.append(newresult)
+            thistb['results'] = newtbresults
+
+        # For each testbench, find all other testbenches that have the same
+        # conditions *except* for the x-axis condition, and combine them
+        # into one testbench
+
+        for tbidx in range(0, numtbs):
+            thistb = tbdata[tbidx]
+            condstr = thistb['condstr']
+            for tbcomp in range(tbidx + 1, numtbs):
+                comptb = tbdata[tbcomp]
+                if 'killed' in comptb:
+                    continue
+                compstr = comptb['condstr']
+                if compstr == condstr:
+                    thistb['results'].extend(comptb['results'])
+                    comptb['killed'] = True
+
+        # Generate new set of testbenches from the combined set.
+        newtbdata = []
+        for tbidx in range(0, numtbs):
+            thistb = tbdata[tbidx]
+            if not 'killed' in thistb:
+                newtbdata.append(thistb)
+
+        # Replace the old testbench data
+        tbdata = newtbdata
+
+        # Adjust the testbench count and the length of results, the
+        # index of the X-axis variable, and the simformat list.
 
+        numtbs = len(tbdata)
         rlen = len(results[0])
         xidx = rlen - 1
         simformat.append(xname)
 
-    # Find unique values of each variable (except results, traces, and iterations)
-
-    conditions = tbzero['conditions']
-    binconv = []
-
     if debug:
         print('Processing ' + str(rlen) + ' plot variables.')
 
+    # Redefine "results" and "conditions" after refactoring.
+    zerotb = tbdata[0]
+    results = zerotb['results']
+    conditions = zerotb['conditions']
+
+    # Find unique values of each variable (except results, traces, and iterations)
     # Collect the records of everything being plotted.
 
+    binconv = []
     tracedicts = []
     traces = []
     residx = 0
     for i in range(0, rlen):
         if i != xidx:
             # Keep track of which indexes have traces (i.e., not the X axis values)
             traces.append(i)
@@ -183,17 +232,17 @@
                     varrec['unit'] = param['unit']
                 residx = i
             else:
                 varrec = {}
 
         tracedicts.append(varrec)
 
-        # Mark which items need converting from digital.  Format is verilog-like.  Use
-        # a format width that is larger than the actual number of digits to force
-        # unsigned conversion.
+        # Mark which items need converting from digital.  Format is verilog-like.
+        # Use a format width that is larger than the actual number of digits to
+        # force unsigned conversion.
 
         if 'name' in varrec:
             varname = varrec['name']
         else:
             varname = conditions[i][0]
 
         bmatch = binrex.match(varname)
@@ -212,143 +261,218 @@
                 base = 10
             else:
                 base = 16
             binconv.append([base, digits])
         else:
             binconv.append([])
 
-    # Which stepped variables (ignoring X axis variable) have more than one value?
-    # watchsteps = list(i for i in range(1, rlen) if len(steps[i]) > 1 and i != xidx)
-    watchsteps = []
-
-    # Diagnostic
-    # print("Stepped conditions are: ")
-    # for j in watchsteps:
-    #      print(results[0][j] + '  (' + str(len(steps[j])) + ' steps)')  # FIXME
-
     needconvert = False
     if xname.split('|')[0] == 'digital' or binconv[xidx] != []:
         needconvert = True
 
-    # Collect results.  Make a separate record for each unique set of stepped conditions
-    # encountered.  Record has (X, Y) vector and a list of conditions.
-    pdata = {}
-
     # Limit the amount of data being processed.  NOTE:  This is a stupid-simple
     # way to do it and it needs much better handling;  e.g., import scipy and
     # resample to a constant time step.
 
     numpoints = len(results)
     if debug:
         print('Processing ' + str(numpoints) + ' data points.')
     if numpoints > 1000:
         stepsize = int(numpoints / 1000)
         if debug:
             print('Truncating data with step size ' + str(stepsize))
     else:
         stepsize = 1
 
-    for idx in range(0, numpoints, stepsize):
-        item = results[idx]
+    # Find which conditions are variable;  conditions which are constant do
+    # not need to be displayed in the plot key.  Make a list "stepped" which
+    # is True for each condition that is not constant.  If any condition is
+    # stepped, then a legend is created for the plot.  Ignore a condition if
+    # it is the x-axis condition.
+
+    tracelegend = False
+    stepped = []
+    for cidx in range(0, len(conditions)):
+        stepped.append(False)
+        cond = conditions[cidx][2]
+        # If condition has been set as the x-axis variable, then it is no
+        # longer a stepped condition.
+        if conditions[cidx][0] == xname:
+            continue
+        for tbidx in range(0, numtbs):
+            testtb = tbdata[tbidx]
+            tbcond = testtb['conditions'][cidx][2]
+            if tbcond != cond:
+                stepped[cidx] = True
+                tracelegend = True
+                break
 
-        if needconvert:
-            base = binconv[xidx][0]
-            digits = binconv[xidx][1]
-            # Recast binary strings as integers
-            # Watch for strings that have been cast to floats (need to find the source of this)
-            if '.' in item[xidx]:
-                item[xidx] = item[xidx].split('.')[0]
-            a = int(item[xidx], base)
-            b = twos_comp(a, digits)
-            xvalue = b
-        else:
-            xvalue = item[xidx]
+    if debug:
+        print('Stepped conditions are: ')
+        stepcond = []
+        for j in range(0, len(stepped)):
+            if j == True:
+                stepcond.append(conditions[j][0])
+        print('    ' + ' '.join(stepcond))
+
+    # Now plot the result from each testbench.  Each plot ends up as a
+    # dictionary entry "pdict" in a larger dictionary "pdata".  Each entry
+    # in "pdata" (i.e., each plot trace) is indexed by the list of variable
+    # conditions comprising that trace.  This index becomes the text in the
+    # plot's legend to identify each trace.
+
+    # Warning:  The existing code does not differentiate between plot traces
+    # that are stepped conditions vs. plot traces that are variables.  In
+    # general, the variables should not be assumed to have any relationship
+    # to each other;  one might be a voltage and another current.  They
+    # should be placed in separate sub-graphs.
+
+    pdata = {}
+
+    # Collect results.  Make a separate record for each unique set of stepped
+    # conditions encountered.  Record has (X, Y) vector and a list of conditions.
+
+    for tbidx in range(0, numtbs):
+
+        thistb = tbdata[tbidx]
+        if tbidx > 0:
+            results = thistb['results']
+            conditions = thistb['conditions']
+
+            # In case results[] is not a vector. . .  This should have been handled
+            # outside of cace_makeplot and probably needs to be fixed.
 
+            if not isinstance(results[0], list):
+                for i in range(len(results)):
+                    result = results[i]
+                    if not isinstance(result, list):
+                        results[i] = [result]
+
+        # Create a key index from the list of variable conditions.
+        # Also create the corresponding text for the plot legend
+
+        klist = []
         slist = []
-        for j in watchsteps:
-            slist.append(item[j])
-        istr = ','.join(slist)
-        if istr not in pdata:
-            stextlist = []
-            for j in watchsteps:
-                if results[1][j] == '':
-                    # FIXME:  results[0][x] is no longer the trace name
-                    stextlist.append(results[0][j] + '=' + item[j])
-                else:
-                    # FIXME:  results[0][x] is no longer the trace name
-                    stextlist.append(
-                        results[0][j] + '=' + item[j] + ' ' + results[1][j]
-                    )
-            pdict = {}
-            pdata[istr] = pdict
-            pdict['xdata'] = []
-            if stextlist:
-                tracelegnd = False
-            else:
-                tracelegnd = True
+        for i in range(0, len(conditions)):
+            if stepped[i] == True:
+                klist.append(conditions[i][2])
+                slist.append(
+                    conditions[i][0]
+                    + '='
+                    + str(conditions[i][2])
+                    + conditions[i][1]
+                )
+        dkey = ','.join(klist)
+        stextlist = ' '.join(slist)
 
-            for i in traces:
-                aname = 'ydata' + str(i)
-                pdict[aname] = []
-                alabel = 'ylabel' + str(i)
+        # An empty string seems to work for a key?  But give it a real name.
+        if dkey == '':
+            dkey = 'default'
 
-                # Get the name of the trace.
-                tracedict = tracedicts[i]
-                if 'display' in tracedict:
-                    tracename = tracedict['display']
-                else:
-                    tracename = tracedict['name']
+        # Diagnostic for debugging
+        if debug:
+            print('Testbench ' + str(tbidx) + ' key = ' + dkey)
+            print('Testbench ' + str(tbidx) + ' legend = "' + stextlist + '"')
 
-                # Get the units of the trace
-                if 'unit' in tracedict:
-                    if not binrex.match(tracedict['unit']):
-                        tracename += ' (' + tracedict['unit'] + ')'
+        # Collect results from this testbench into a plot trace
 
-                pdict[alabel] = tracename
+        pdict = {}
+        pdata[dkey] = pdict
 
-            pdict['sdata'] = ' '.join(stextlist)
-        else:
-            pdict = pdata[istr]
+        pdict['xdata'] = []
+        pdict['sdata'] = stextlist
 
-        try:
-            xfloat = float(xvalue)
-        except:
-            pdict['xdata'].append(xvalue)
-        else:
-            pdict['xdata'].append(xfloat)
+        # Each variable (trace) forms a separate trace in this plot.
+        # (See note above)
 
         for i in traces:
-            # For each trace, convert the value from digital to integer if needed
-            if binconv[i] != []:
-                base = binconv[i][0]
-                digits = binconv[i][1]
-                a = int(item[i], base)
+            aname = 'ydata' + str(i)
+            pdict[aname] = []
+            alabel = 'ylabel' + str(i)
+
+            # Get the name of the trace.
+            tracedict = tracedicts[i]
+            if 'display' in tracedict:
+                tracename = tracedict['display']
+            else:
+                tracename = tracedict['name']
+
+            # Get the units of the trace
+            if 'unit' in tracedict:
+                if not binrex.match(tracedict['unit']):
+                    tracename += ' (' + tracedict['unit'] + ')'
+
+            pdict[alabel] = tracename
+
+        # Now, for each entry in results, add an (X, Y) point to each
+        # plot trace.
+
+        for idx in range(0, numpoints, stepsize):
+            item = results[idx]
+
+            if needconvert:
+                base = binconv[xidx][0]
+                digits = binconv[xidx][1]
+                # Recast binary strings as integers
+                # Watch for strings that have been cast to floats
+                # (need to find the source of this)
+                if '.' in item[xidx]:
+                    item[xidx] = item[xidx].split('.')[0]
+                a = int(item[xidx], base)
                 b = twos_comp(a, digits)
-                yvalue = b
+                xvalue = b
             else:
-                yvalue = item[i]
+                xvalue = item[xidx]
 
-            aname = 'ydata' + str(i)
             try:
-                yfloat = float(yvalue)
+                xfloat = float(xvalue)
             except:
-                pdict[aname].append(yvalue)
+                pdict['xdata'].append(xvalue)
             else:
-                pdict[aname].append(yfloat)
+                pdict['xdata'].append(xfloat)
+
+            for i in traces:
+                tracedict = tracedicts[i]
+                # For each trace, convert the value from digital to integer if needed
+                if binconv[i] != []:
+                    base = binconv[i][0]
+                    digits = binconv[i][1]
+                    a = int(item[i], base)
+                    b = twos_comp(a, digits)
+                    yvalue = b
+                else:
+                    yvalue = item[i]
+
+                aname = 'ydata' + str(i)
+                try:
+                    yfloat = float(yvalue)
+                except:
+                    pdict[aname].append(yvalue)
+                else:
+                    if 'unit' in tracedict:
+                        yscaled = spice_unit_unconvert(
+                            [tracedict['unit'], yfloat]
+                        )
+                        pdict[aname].append(yscaled)
+                    else:
+                        pdict[aname].append(yfloat)
+
+    # NOTE:  Loop over testbenches (tbidx) ends here
 
     fig = Figure()
     if parent == None:
         canvas = FigureCanvasAgg(fig)
     else:
         canvas = FigureCanvasTkAgg(fig, parent)
 
     # With no parent, just make one plot and put the legend off to the side.  The
     # 'extra artists' capability of print_figure will take care of the bounding box.
     # For display, prepare two subplots so that the legend takes up the space of the
     # second one.
+
     if parent == None:
         ax = fig.add_subplot(111)
     else:
         ax = fig.add_subplot(121)
 
     # fig.hold(True)
     for record in pdata:
@@ -367,22 +491,50 @@
         if plottype == 'histogram':
             ax.hist(
                 xdata,
                 histtype='barstacked',
                 label=pdict['sdata'],
                 stacked=True,
             )
+        elif plottype == 'semilogx':
+            for i in traces:
+                aname = 'ydata' + str(i)
+                alabl = 'ylabel' + str(i)
+                ax.semilogx(
+                    xdata,
+                    pdict[aname],
+                    label=pdict['sdata'],
+                )
+        elif plottype == 'semilogy':
+            for i in traces:
+                aname = 'ydata' + str(i)
+                alabl = 'ylabel' + str(i)
+                ax.semilogy(
+                    xdata,
+                    pdict[aname],
+                    label=pdict['sdata'],
+                )
+        elif plottype == 'loglog':
+            for i in traces:
+                aname = 'ydata' + str(i)
+                alabl = 'ylabel' + str(i)
+                ax.loglog(
+                    xdata,
+                    pdict[aname],
+                    label=pdict['sdata'],
+                )
         else:
+            # plottype is 'xyplot'
             for i in traces:
                 aname = 'ydata' + str(i)
                 alabl = 'ylabel' + str(i)
                 ax.plot(
                     xdata,
                     pdict[aname],
-                    label=pdict[alabl] + ' ' + pdict['sdata'],
+                    label=pdict['sdata'],
                 )
 
         if not numeric:
             ax.set_xticks(xdata)
             ax.set_xticklabels(pdict['xdata'])
 
     # Automatically generate X axis label if not given alternate text
@@ -404,21 +556,21 @@
     else:
         ytext = tracerec['name']
     if 'unit' in tracerec:
         ytext += ' (' + tracerec['unit'] + ')'
     ax.set_ylabel(ytext)
 
     ax.grid(True)
-    if watchsteps or tracelegnd:
-        legnd = ax.legend(loc=2, bbox_to_anchor=(1.05, 1), borderaxespad=0.0)
+    if tracelegend:
+        legend = ax.legend(loc=2, bbox_to_anchor=(1.05, 1), borderaxespad=0.0)
     else:
-        legnd = None
+        legend = None
 
-    if legnd:
-        legnd.set_draggable(True)
+    if legend:
+        legend.set_draggable(True)
 
     if parent == None:
         paths = dsheet['paths']
         if 'plots' in paths:
             plotdir = paths['plots']
         else:
             plotdir = paths['simulation']
@@ -436,20 +588,35 @@
 
         filename = os.path.join(plotdir, netlist_source, plotname)
 
         # NOTE: print_figure only makes use of bbox_extra_artists if
         # bbox_inches is set to 'tight'.  This forces a two-pass method
         # that calculates the real maximum bounds of the figure.  Otherwise
         # the legend gets clipped.
-        if legnd:
+        if legend:
             canvas.print_figure(
-                filename, bbox_inches='tight', bbox_extra_artists=[legnd]
+                filename, bbox_inches='tight', bbox_extra_artists=[legend]
             )
         else:
             canvas.print_figure(filename, bbox_inches='tight')
 
-    resultdict = {}
+    # Do not overwrite a result dictionary.  Only add an entry if no result
+    # dictionary exists.
+    netlist_source = runtime_options['netlist_source']
+    if 'results' in param:
+        results = param['results']
+        if isinstance(results, dict):
+            results = [results]
+        try:
+            resultdict = next(
+                item for item in results if item['name'] == netlist_source
+            )
+        except:
+            resultdict = {}
+    else:
+        resultdict = {}
+
     resultdict['status'] = 'done'
-    resultdict['name'] = runtime_options['netlist_source']
+    resultdict['name'] = netlist_source
     addnewresult(param, resultdict)
 
     return canvas
```

### Comparing `cace-2.1.9/cace/common/cace_measure.py` & `cace-2.2.0/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/cace_read.py` & `cace-2.2.0/cace/common/cace_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         clines = ifile.read()
 
     # These keys correspond to lists of dictionaries.  All other keys
     # must have a single value which is a string or a dictionary.
     listkeys = [
         'conditions',
         'default_conditions',
+        'dependencies',
         'variables',
         'pins',
         'measure',
         'electrical_parameters',
         'physical_parameters',
         'testbenches',
         'results',
```

### Comparing `cace-2.1.9/cace/common/cace_regenerate.py` & `cace-2.2.0/cace/common/cace_regenerate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-#!/usr/bin/env python3
-# -----------------------------------------------------------------------
-# cace_regenerate.py
-# -----------------------------------------------------------------------
+# Copyright 2024 Efabless Corporation
 #
-# These procedures are used by cace_gensim to check if netlists need
-# to be automatically regenerated, and to run schematic capture or
-# layout extraction as needed.
-# -----------------------------------------------------------------------
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""
+These procedures are used by cace_gensim to check if netlists need
+to be automatically regenerated, and to run schematic capture or
+layout extraction as needed.
+"""
 
 import os
 import sys
 import re
 import shutil
 from datetime import date as datetime
 import subprocess
 
-# ----------------------------------------------------------------------
-# printwarn
-#
-# Print warnings output from a file run using the subprocess package
-# ----------------------------------------------------------------------
-
 
 def printwarn(output):
+    """Print warnings output from a file run using the subprocess package"""
     # Check output for warning or error
     if not output:
         return 0
 
     failrex = re.compile('.*failure', re.IGNORECASE)
     warnrex = re.compile('.*warning', re.IGNORECASE)
     errrex = re.compile('.*error', re.IGNORECASE)
@@ -50,70 +54,65 @@
         if mmatch:
             errors += 1
         if ematch or wmatch or fmatch or mmatch:
             print(line)
     return errors
 
 
-# ----------------------------------------------------------------------
-# printall
-#
-# Print all output from a file run using the subprocess package
-# ----------------------------------------------------------------------
-
-
 def printall(output):
+    """Print all output from a file run using the subprocess package"""
+
     # Check output for warning or error
     if not output:
         return 0
 
     outlines = output.splitlines()
     for line in outlines:
         print(line)
 
 
-# -----------------------------------------------------------------------
-# get_pdk_root
-#
-# Get a value for PDK_ROOT, either from an environment variable, or
-# from several standard locations (open_pdks install and IIC-tools
-# install and volare install).
-# -----------------------------------------------------------------------
-
-
 def get_pdk_root():
+    """
+    Get a value for PDK_ROOT, either from an environment variable, or
+    from several standard locations (open_pdks install and IIC-tools
+    install and volare install).
+    If found, set the environment variable PDK_ROOT.
+    """
+
     try:
         pdk_root = os.environ['PDK_ROOT']
     except KeyError:
         # Try a few common places where open_pdks might be installed
         pdk_root = '/usr/local/share/pdk'
         if not os.path.isdir(pdk_root):
             pdk_root = '/usr/share/pdk'
             if not os.path.isdir(pdk_root):
                 pdk_root = '/foss/pdks'
                 if not os.path.isdir(pdk_root):
                     pdk_root = os.path.join(os.path.expanduser('~'), '.volare')
                     if not os.path.isdir(pdk_root):
                         pdk_root = None
-    return pdk_root
 
+        if pdk_root:
+            os.environ['PDK_ROOT'] = pdk_root
+        else:
+            print('Could not locate PDK_ROOT!')
 
-# -----------------------------------------------------------------------
-# get_pdk
-#
-# Get a value for the PDK, either from the second line of a .mag file,
-# or from the environment as environment variable "PDK".
-#
-# NOTE:  Normally the PDK is provided as part of the datasheet, as
-# a project does not necessarily have a .mag file;  so there is no
-# source for automatically determining the project PDK.
-# -----------------------------------------------------------------------
+    return pdk_root
 
 
 def get_pdk(magicfilename):
+    """
+    Get a value for the PDK, either from the second line of a .mag file,
+    or from the environment as environment variable "PDK".
+
+    NOTE:  Normally the PDK is provided as part of the datasheet, as
+    a project does not necessarily have a .mag file;  so there is no
+    source for automatically determining the project PDK.
+    """
     if magicfilename and os.path.isfile(magicfilename):
         with open(magicfilename, 'r') as ifile:
             for line in ifile.readlines():
                 tokens = line.split()
                 if tokens[0] == 'tech':
                     pdk = tokens[1]
                     break
@@ -125,24 +124,22 @@
                 'Error:  No .mag file and PDK is not defined in the environment.'
             )
             pdk = None
 
     return pdk
 
 
-# -----------------------------------------------------------------------
-# Get the path and filename of the magic startup script corresponding
-# to the PDK.
-#
-# Returns a string containing the full path and filename of the startup
-# script (.magicrc file).
-# -----------------------------------------------------------------------
-
-
 def get_magic_rcfile(dsheet, magicfilename=None):
+    """
+    Get the path and filename of the magic startup script corresponding
+    to the PDK.
+
+    Returns a string containing the full path and filename of the startup
+    script (.magicrc file).
+    """
 
     if 'PDK_ROOT' in dsheet:
         pdk_root = dsheet['PDK_ROOT']
     else:
         pdk_root = get_pdk_root()
 
     if 'PDK' in dsheet:
@@ -162,24 +159,22 @@
 
     rcfile = os.path.join(
         pdk_root, pdk, 'libs.tech', 'magic', pdk + '.magicrc'
     )
     return rcfile
 
 
-# -----------------------------------------------------------------------
-# Get the path and filename of the netgen setup script corresponding
-# to the PDK.
-#
-# Returns a string containing the full path and filename of the setup
-# script (.tcl file).
-# -----------------------------------------------------------------------
-
-
 def get_netgen_setupfile(dsheet):
+    """
+    Get the path and filename of the netgen setup script corresponding
+    to the PDK.
+
+    Returns a string containing the full path and filename of the setup
+    script (.tcl file).
+    """
 
     if 'PDK_ROOT' in dsheet:
         pdk_root = dsheet['PDK_ROOT']
     else:
         pdk_root = get_pdk_root()
 
     if 'PDK' in dsheet:
@@ -197,29 +192,26 @@
 
     setupfile = os.path.join(
         pdk_root, pdk, 'libs.tech', 'netgen', pdk + '_setup.tcl'
     )
     return setupfile
 
 
-# -----------------------------------------------------------------------
-# check_simulation_out_of_date
-#
-# Check if a simulation result is out-of-date relative to both the
-# testbench and the DUT.  It can be assumed that the DUT netlist and
-# testbench have already been checked against their respective
-# schematics, only the netlists need to be compared.
-#
-# "simpath" is the path to simulation result (usually in root_path/ngspice)
-# "tbpath" is the path to testbench netlist (usually in root_path/cace)
-# "dutpath" is the path to the design netlist (depends on source setting)
-# -----------------------------------------------------------------------
-
-
 def check_simulation_out_of_date(simpath, tbpath, dutpath, debug=False):
+    """
+    Check if a simulation result is out-of-date relative to both the
+    testbench and the DUT.  It can be assumed that the DUT netlist and
+    testbench have already been checked against their respective
+    schematics, only the netlists need to be compared.
+
+    "simpath" is the path to simulation result (usually in root_path/ngspice)
+    "tbpath" is the path to testbench netlist (usually in root_path/cace)
+    "dutpath" is the path to the design netlist (depends on source setting)
+    """
+
     need_resimulate = False
     if not os.path.isfile(simpath):
         if debug:
             print('Simulation result does not exist.  Need to resimulate.')
         need_resimulate = True
     elif not os.path.isfile(tbpath):
         if debug:
@@ -256,20 +248,24 @@
 
     return need_simulation
 
 
 # -----------------------------------------------------------------------
 # check_layout_out_of_date
 #
-# Check if a netlist (spicepath) is out-of-date relative to the layouts
-# (layoutpath).  Need to read the netlist and check all of the subcells.
+
 # -----------------------------------------------------------------------
 
 
 def check_layout_out_of_date(spicepath, layoutpath, debug=False):
+    """
+    Check if a netlist (spicepath) is out-of-date relative to the layouts
+    (layoutpath).  Need to read the netlist and check all of the subcells.
+    """
+
     need_capture = False
     if not os.path.isfile(spicepath):
         if debug:
             print('Netlist does not exist, so netlist must be regenerated')
         need_capture = True
     elif not os.path.isfile(layoutpath):
         if debug:
@@ -323,27 +319,25 @@
                                 )
                                 print('---Subcell datestamp = ' + subtime)
                                 print('---Netlist datestamp = ' + nettime)
                             break
     return need_capture
 
 
-# -----------------------------------------------------------------------
-# check_schematic_out_of_date
-#
-# Check if a netlist (spicepath) is out-of-date relative to the schematics
-# (schempath).  Need to read the netlist and check all of the subcells.
-#
-# This routine can also be used to determine if a testbench netlist is
-# up-to-date with respect to its schematic.
-# -----------------------------------------------------------------------
-
-
 def check_schematic_out_of_date(spicepath, schempath, debug=False):
+    """
+    Check if a netlist (spicepath) is out-of-date relative to the schematics
+    (schempath).  Need to read the netlist and check all of the subcells.
+
+    This routine can also be used to determine if a testbench netlist is
+    up-to-date with respect to its schematic.
+    """
+
     need_capture = False
+
     if not os.path.isfile(spicepath):
         if debug:
             print(
                 'Schematic-captured netlist does not exist.  Need to regenerate.'
             )
         need_capture = True
     elif not os.path.isfile(schempath):
@@ -417,23 +411,16 @@
                                     '---Netlist datestamp = '
                                     + nettime.isoformat()
                                 )
                             break
     return need_capture
 
 
-# -----------------------------------------------------------------------
-# regenerate_rcx_netlist
-#
-# Regenerate the R-C parasitic extracted netlist if out-of-date or if
-# forced.
-# -----------------------------------------------------------------------
-
-
 def regenerate_rcx_netlist(dsheet):
+    """Regenerate the R-C parasitic extracted netlist if out-of-date or if forced."""
 
     runtime_options = dsheet['runtime_options']
     debug = runtime_options['debug']
     force_regenerate = runtime_options['force']
 
     dname = dsheet['name']
     netlistname = dname + '.spice'
@@ -595,24 +582,20 @@
             need_rcx_extract and not os.path.isfile(rcx_netlist)
         ):
             return False
 
     return rcx_netlist
 
 
-# -----------------------------------------------------------------------
-# regenerate_lvs_netlist
-#
-# Regenerate the layout-extracted netlist if out-of-date or if forced.
-# If argument "pex" is True, then generate parasitic capacitances in
-# the output.
-# -----------------------------------------------------------------------
-
-
 def regenerate_lvs_netlist(dsheet, pex=False):
+    """
+    Regenerate the layout-extracted netlist if out-of-date or if forced.
+    If argument "pex" is True, then generate parasitic capacitances in
+    the output.
+    """
 
     runtime_options = dsheet['runtime_options']
     debug = runtime_options['debug']
     force_regenerate = runtime_options['force']
 
     dname = dsheet['name']
     netlistname = dname + '.spice'
@@ -761,32 +744,29 @@
             need_lvs_extract and not os.path.isfile(lvs_netlist)
         ):
             return False
 
     return lvs_netlist
 
 
-# -----------------------------------------------------------------------
-# check_dependencies --
-#
-# Check the datasheet for listed dependencies and make sure they exist.
-# If not, and the dependency entry lists a repository, then clone the
-# dependency.
-#
-# Returns True if a dependency was cloned, and False if nothing needed
-# to be done.
-#
-# To do:  For each dependency, find a CACE datasheet and read the path
-# information to find the path to schematics, so this can be used to
-# add the correct search path to the xschemrc file.  For now, it is
-# assumed that the path name is 'xschem'.
-# -----------------------------------------------------------------------
-
-
 def check_dependencies(dsheet, debug=False):
+    """
+    Check the datasheet for listed dependencies and make sure they exist.
+    If not, and the dependency entry lists a repository, then clone the
+    dependency.
+
+    Returns True if a dependency was cloned, and False if nothing needed
+    to be done.
+
+    To do:  For each dependency, find a CACE datasheet and read the path
+    information to find the path to schematics, so this can be used to
+    add the correct search path to the xschemrc file.  For now, it is
+    assumed that the path name is 'xschem'.
+    """
+
     dependencies = []
     if 'dependencies' in dsheet:
         # If there is only one dependency it may be a dictionary and not a
         # list of dictionaries.
         if isinstance(dsheet['dependencies'], dict):
             dependencies = [dsheet['dependencies']]
         else:
@@ -837,37 +817,33 @@
                         + ' does not exist!'
                     )
                     # Maybe should return here, but what if dependency isn't used
                     # in the schematic?
     return False
 
 
-# -----------------------------------------------------------------------
-# set_xschem_paths ---
-#
-# 	Put together a set of Tcl commands that sets the search
-# 	path for xschem.
-#
-# 	If tclstr is not None, then it is assumed to be a valid
-# 	Tcl command, and the rest of the Tcl command string is
-# 	appended to it, with independent commands separated by
-# 	semicolons.
-#
-# 	Return the final Tcl command string.
-#
-# 	Note that this is used only when regenerating the schematic
-# 	netlist.  The testbenches are assumed to call the symbol as
-# 	a primitive, and rely on an include file to pull in the
-# 	netlist (either schematic or layout) from the appropriate
-# 	netlist directory.
-#
-# -----------------------------------------------------------------------
-
-
 def set_xschem_paths(dsheet, symbolpath, tclstr=None):
+    """
+    Put together a set of Tcl commands that sets the search
+    path for xschem.
+
+    If tclstr is not None, then it is assumed to be a valid
+    Tcl command, and the rest of the Tcl command string is
+    appended to it, with independent commands separated by
+    semicolons.
+
+    Return the final Tcl command string.
+
+    Note that this is used only when regenerating the schematic
+    netlist. The testbenches are assumed to call the symbol as
+    a primitive, and rely on an include file to pull in the
+    netlist (either schematic or layout) from the appropriate
+    netlist directory.
+    """
+
     paths = dsheet['paths']
 
     # Root path
     if 'root' in paths:
         root_path = paths['root']
     else:
         root_path = '.'
@@ -909,27 +885,34 @@
             dependencies = dsheet['dependencies']
 
         for dependency in dependencies:
             if 'path' in dependency and 'name' in dependency:
                 dependdir = os.path.join(
                     dependency['path'], dependency['name'], 'xschem'
                 )
-                tcllist.append('append XSCHEM_LIBRARY_PATH :' + dependdir)
+                if not os.path.isdir(dependdir):
+                    dependdir = os.path.join(
+                        dependency['path'], dependency['name']
+                    )
+                    if not os.path.isdir(dependdir):
+                        print(
+                            'Error:  Cannot find xschem library in '
+                            + dependency['name']
+                        )
+                        print('Current directory is: ' + os.getcwd())
+                        print('Dependdir is: ' + dependdir)
+                        dependdir = None
+                if dependdir:
+                    tcllist.append('append XSCHEM_LIBRARY_PATH :' + dependdir)
 
     return ' ; '.join(tcllist)
 
 
-# -----------------------------------------------------------------------
-# regenerate_schematic_netlist
-#
-# Regenerate the schematic-captured netlist if out-of-date or if forced.
-# -----------------------------------------------------------------------
-
-
 def regenerate_schematic_netlist(dsheet):
+    """Regenerate the schematic-captured netlist if out-of-date or if forced."""
 
     runtime_options = dsheet['runtime_options']
     debug = runtime_options['debug']
     force_regenerate = runtime_options['force']
 
     dname = dsheet['name']
     netlistname = dname + '.spice'
@@ -1111,22 +1094,16 @@
     if need_schem_capture:
         if not os.path.isfile(schem_netlist):
             return False
 
     return schem_netlist
 
 
-# -----------------------------------------------------------------------
-# regenerate_testbench
-#
-# Regenerate a testbench template (create SPICE from .sch)
-# -----------------------------------------------------------------------
-
-
 def regenerate_testbench(dsheet, testbenchpath, testbench):
+    """Regenerate a testbench template (create SPICE from .sch)"""
 
     runtime_options = dsheet['runtime_options']
     debug = runtime_options['debug']
     force_regenerate = runtime_options['force']
 
     paths = dsheet['paths']
 
@@ -1238,20 +1215,16 @@
     if not os.path.isfile(netlist_file):
         print('Error: No netlist found for the testbench ' + testbench + '!')
         return 1
 
     return 0
 
 
-# -----------------------------------------------------------------------
-# Regenerate all netlists as needed when out of date.
-# -----------------------------------------------------------------------
-
-
 def regenerate_netlists(dsheet):
+    """Regenerate all netlists as needed when out of date."""
 
     # 'netlist_source' determines whether to use the layout extracted netlist
     # or the schematic captured netlist.  Also, regenerate the netlist only if
     # it is out of date, or if the user has selected forced regeneration in the
     # settings.
 
     runtime_options = dsheet['runtime_options']
@@ -1293,24 +1266,22 @@
             regenerate_lvs_netlist(dsheet)
         if not made_schem_netlist:
             regenerate_schematic_netlist(dsheet)
 
     return result
 
 
-# -----------------------------------------------------------------------
-# Copy the schematic symbol to the testbench directory and remark its
-# type from 'schematic' to 'primitive', so that testbench netlists will
-# write an instance call but not the schematic itself.  That way, the
-# schematic can be brought in from an include file that can be set to
-# any one of schematic-captured or layout-extracted netlists.
-# -----------------------------------------------------------------------
-
-
 def make_symbol_primitive(dsheet):
+    """
+    Copy the schematic symbol to the testbench directory and remark its
+    type from 'schematic' to 'primitive', so that testbench netlists will
+    write an instance call but not the schematic itself.  That way, the
+    schematic can be brought in from an include file that can be set to
+    any one of schematic-captured or layout-extracted netlists.
+    """
 
     dname = dsheet['name']
     xschemname = dname + '.sym'
 
     paths = dsheet['paths']
 
     # Xschem schematic symbol
@@ -1337,23 +1308,19 @@
         symboldata = ifile.read()
         primdata = symboldata.replace('type=subcircuit', 'type=primitive')
 
     with open(primfilename, 'w') as ofile:
         ofile.write(primdata)
 
 
-# -----------------------------------------------------------------------
-# Regenerate all testbenches.
-#
-# If paramname is passed to regenerate_testbenches and is not None, then
-# only generate testbenches required by the specified parameter.
-# -----------------------------------------------------------------------
-
-
 def regenerate_testbenches(dsheet, paramname=None):
+    """
+    If paramname is passed to regenerate_testbenches and is not None, then
+    only generate testbenches required by the specified parameter.
+    """
 
     paths = dsheet['paths']
     if 'testbench' in paths:
         testbenchpath = paths['testbench']
     else:
         testbenchpath = 'testbench'
 
@@ -1384,10 +1351,7 @@
         testbenches_checked[testbench] = True
         result = regenerate_testbench(dsheet, testbenchpath, testbench)
         if result != 0:
             print('Error in testbench generation.  Halting characterization.')
             return result
 
     return 0
-
-
-# -----------------------------------------------------------------------
```

### Comparing `cace-2.1.9/cace/common/cace_simulate.py` & `cace-2.2.0/cace/common/cace_simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+c  #!/usr/bin/env python3
 # ---------------------------------------------------------------------------
 # cace_simulate.py
 #
 #    Run a simulation (or co-simulation) according to the "simulate"
 #    dictionary of electrical parameter "param".  This runs exactly
 #    one simulation for the conditions defined in the testbench
 #    dictionary "testbench".
@@ -154,14 +154,15 @@
             bufsize=1,
             start_new_session=True,
             universal_newlines=True,
         ) as spiceproc:
             pgroup = os.getpgid(spiceproc.pid)
             for line in spiceproc.stdout:
                 print(line, end='')
+                print('hi!')
                 sys.stdout.flush()
                 if 'Simulation interrupted' in line:
                     print('ngspice encountered an error. . . ending.')
                     spiceproc.kill()
 
         spiceproc.stdout.close()
         return_code = spiceproc.wait()
```

### Comparing `cace-2.1.9/cace/common/cace_write.py` & `cace-2.2.0/cace/common/cace_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 pdk_root = datasheet['PDK_ROOT']
             else:
                 pdk_root = get_pdk_root()
 
             if 'PDK' in datasheet:
                 pdk = datasheet['PDK']
             else:
-                pdk = get_pdk(magicfilename)
+                pdk = get_pdk(None)
 
             newenv = os.environ.copy()
             if pdk_root and 'PDK_ROOT' not in newenv:
                 newenv['PDK_ROOT'] = pdk_root
             if pdk and 'PDK' not in newenv:
                 newenv['PDK'] = pdk
 
@@ -846,15 +846,15 @@
 # Print a summary report of a single "results" block from a
 # datasheet.
 # ---------------------------------------------------------------
 
 
 def cace_summarize_result(param, result):
     spec = param['spec']
-    unit = param['unit']
+    unit = param['unit'] if 'unit' in param else ''
 
     keys = ['minimum', 'typical', 'maximum']
 
     print('   Source type: ' + result['name'])
     for key in keys:
         if key in spec and key in result:
             speclist = spec[key]
@@ -882,24 +882,25 @@
 
 # ---------------------------------------------------------------
 # cace_summary
 #
 # Print a summary report of results from a datasheet
 #
 # "datasheet" is a CACE characterization dataset
-# "paramname" is the name of a single parameter to summarize,
+# "paramname" is a list of parameters to summarize,
 # 	or if it is None, then all parameters should be output.
 # ---------------------------------------------------------------
 
 
-def cace_summary(datasheet, paramname):
+def cace_summary(datasheet, paramnames):
 
-    if 'electrical_parameters' in datasheet:
-        for eparam in datasheet['electrical_parameters']:
-            if not paramname or paramname == eparam['name']:
+    # Summarize all parameters
+    if not paramnames:
+        if 'electrical_parameters' in datasheet:
+            for eparam in datasheet['electrical_parameters']:
                 print('Electrical parameter ' + eparam['name'])
                 if 'description' in eparam:
                     print('   ' + eparam['description'])
                 if 'display' in eparam:
                     print('   ' + eparam['display'])
                 if 'spec' not in eparam:
                     print('   (Parameter does not have a spec)')
@@ -909,17 +910,16 @@
                     results = eparam['results']
                     if isinstance(results, list):
                         for result in eparam['results']:
                             cace_summarize_result(eparam, result)
                     else:
                         cace_summarize_result(eparam, results)
 
-    if 'physical_parameters' in datasheet:
-        for pparam in datasheet['physical_parameters']:
-            if not paramname or paramname == pparam['name']:
+        if 'physical_parameters' in datasheet:
+            for pparam in datasheet['physical_parameters']:
                 print('Physical parameter ' + pparam['name'])
                 if 'description' in pparam:
                     print('   ' + pparam['description'])
                 if 'display' in eparam:
                     print('   ' + eparam['display'])
                 if 'spec' not in pparam:
                     print('   (Parameter does not have a spec)')
@@ -929,14 +929,57 @@
                     results = pparam['results']
                     if isinstance(results, list):
                         for result in pparam['results']:
                             cace_summarize_result(pparam, result)
                     else:
                         cace_summarize_result(pparam, results)
 
+    # Only summarize the parameters in the list
+    else:
+        for paramname in paramnames:
+            if 'electrical_parameters' in datasheet:
+                for eparam in datasheet['electrical_parameters']:
+                    if paramname == eparam['name']:
+                        print('Electrical parameter ' + eparam['name'])
+                        if 'description' in eparam:
+                            print('   ' + eparam['description'])
+                        if 'display' in eparam:
+                            print('   ' + eparam['display'])
+                        if 'spec' not in eparam:
+                            print('   (Parameter does not have a spec)')
+                        elif 'results' not in eparam:
+                            print('   (No results to report)')
+                        else:
+                            results = eparam['results']
+                            if isinstance(results, list):
+                                for result in eparam['results']:
+                                    cace_summarize_result(eparam, result)
+                            else:
+                                cace_summarize_result(eparam, results)
+
+            if 'physical_parameters' in datasheet:
+                for pparam in datasheet['physical_parameters']:
+                    if paramname == pparam['name']:
+                        print('Physical parameter ' + pparam['name'])
+                        if 'description' in pparam:
+                            print('   ' + pparam['description'])
+                        if 'display' in eparam:
+                            print('   ' + eparam['display'])
+                        if 'spec' not in pparam:
+                            print('   (Parameter does not have a spec)')
+                        elif 'results' not in pparam:
+                            print('   (No results to report)')
+                        else:
+                            results = pparam['results']
+                            if isinstance(results, list):
+                                for result in pparam['results']:
+                                    cace_summarize_result(pparam, result)
+                            else:
+                                cace_summarize_result(pparam, results)
+
 
 # ---------------------------------------------------------------
 # Convert from unicode to text format
 # ---------------------------------------------------------------
 
 
 def uchar_sub(string):
@@ -1402,14 +1445,24 @@
 # dictionary.  If False, then leave it out of the output.
 # ---------------------------------------------------------------
 
 
 def cace_write(datasheet, filename, doruntime=False):
     outlines = []
 
+    # Rewrite paths['root'] as the cwd relative to filename.
+    oldroot = None
+    if 'paths' in datasheet:
+        paths = datasheet['paths']
+        if 'root' in paths:
+            oldroot = paths['root']
+            filepath = os.path.split(filename)[0]
+            newroot = os.path.relpath(os.curdir, filepath)
+            paths['root'] = newroot
+
     newline = '#---------------------------------------------------'
     outlines.append(newline)
 
     if filename:
         newline = '# CACE format 4.0 characterization file ' + filename
         outlines.append(newline)
         newline = '#---------------------------------------------------'
@@ -1417,14 +1470,18 @@
         newline = ''
         outlines.append(newline)
 
     outlines = cace_output_known_dict(
         'topmost', datasheet, outlines, doruntime, 0
     )
 
+    # Put back the old value of paths['root'] (should be '.')
+    if oldroot:
+        paths['root'] = oldroot
+
     # If filename is None, then write to stdout.
     if not filename:
         for line in outlines:
             print(line)
         return 0
 
     try:
```

### Comparing `cace-2.1.9/cace/common/layout_estimate.py` & `cace-2.2.0/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/netlist_precheck.py` & `cace-2.2.0/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/safe_eval.py` & `cace-2.2.0/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/common/spiceunits.py` & `cace-2.2.0/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/doc/characterize_help.txt` & `cace-2.2.0/docs/source/characterization.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,107 @@
-1.
-Selecting a datasheet
--------
-Start by selecting a datasheet.  This step is only necessary if the application is started from the command line.  If started from the project manager, then it can only be run if a datasheet exists for the project, in which case that datasheet is automatically loaded.
+# Characterization
 
-If running from the command line, there is a button at the top with the text 'Datasheet:' and '(no selection)'. Push this button to get a file browser.  Find a project datasheet, which is a JSON (.json) file.  A challenge datasheet should be found in the design folder for each accepted challenge.  The project design folders are in the 'design' subfolder in the user's home directory.  The challenge datasheet has the name of the project and the file extension '.json'.
+## Selecting a datasheet
+
+Start by selecting a datasheet. This step is only necessary if the application is started from the command line.
+
+%If started from the project manager, then it can only be run if a datasheet exists for the project, in which case that datasheet is automatically loaded.
+
+If running from the command line, there is a button at the top with the text `Datasheet:` and `(no selection)`. Push this button to get a file browser. Find a project datasheet, which is a text (`.txt`) file.  A challenge datasheet should be found in the design folder for each accepted challenge.
+
+%The project design folders are in the `design` subfolder in the user's home directory.
+
+The challenge datasheet has the name of the project and the file extension `.txt`
 
 When the JSON file is selected, a full display should be shown with each electrical parameter critical to the challenge, and its status.
-.
-2.
-Characterization
-------------
-The purpose of the characterization tool is to check the netlist against the official characterization specification for a circuit.  The tool allows a quick check of the circuit design against the datasheet specification values, and presents a summary of results to the user.  The purpose of these simulations is to see whether or not the design will pass or fail the specification.  Details from these simulations are limited to the characterization values.  They are not intended to replace the simulations done in the normal course of a circuit design.
-
-The list of electrical parameters will vary by the type of design.  However, each electrical paramater has a common set of properties that are listed in columns across the window.  These are:
-
-(1) "Parameter" --- The name of the electrical or physical parameter.
-(2) "Testbench" --- The testbench corresponds to a netlist filename with the extension ".spice" (SPICE netlist) that can be found in the "cace" folder of the project (or the "testbench" path declared in the characterization file).  The testbench netlists are in a special format that allows them to be altered by substitution for a specific measurement.
-(3) "Min" --- The minimum limit (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
-(4) "Typ" --- The typical value (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
-(5) "Max" --- The maximum limit (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
-(6) "Status" --- Is one of "(not checked)" if the circuit has not yet been simulated, "(in progress)" if the simulation is ongoing;  "pass" if the circuit has been simulated and passed the specification for the eletrical parameter, and "fail" if it failed the specification.   If the status is "pass" or "fail", this entry is a button that can be pressed to see a detailed view of the results.
-(7) "Simulate" --- This is a button that will initiate an ngspice simulation of the electrical parameter.
 
-At the bottom of the window is a space for program messages, warnings, and errors.  Below that is a button bar with the following buttons:
+## Characterization
 
-"Close" --- Quits the characterization tool.  If new results have been simulated but not saved, the user will have to respond to a prompt.
+The purpose of the characterization tool is to check the netlist against the official characterization specification for a circuit. The tool allows a quick check of the circuit design against the datasheet specification values, and presents a summary of results to the user. The purpose of these simulations is to see whether or not the design will pass or fail the specification. Details from these simulations are limited to the characterization values. They are not intended to replace the simulations done in the normal course of a circuit design.
 
-"Save" --- Saves the current characterization results.  These results will be loaded the next time the characterization tool is run, unless there is a design netlist newer than the saved results.
+The list of electrical parameters will vary by the type of design. However, each electrical paramater has a common set of properties that are listed in columns across the window. These are:
 
-"Help" --- Activates this help window.
+1. "Parameter" --- The name of the electrical or physical parameter.
+2. "Testbench" --- The testbench corresponds to a netlist filename with the extension ".spice" (SPICE netlist) that can be found in the "cace" folder of the project (or the "testbench" path declared in the characterization file).  The testbench netlists are in a special format that allows them to be altered by substitution for a specific measurement.
+3. "Min" --- The minimum limit (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
+4. "Typ" --- The typical value (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
+5. "Max" --- The maximum limit (if any) of the electrical parameter.  After simulation, also shows the measured result of the circuit.
+6. "Status" --- Is one of "(not checked)" if the circuit has not yet been simulated, "(in progress)" if the simulation is ongoing;  "pass" if the circuit has been simulated and passed the specification for the eletrical parameter, and "fail" if it failed the specification.   If the status is "pass" or "fail", this entry is a button that can be pressed to see a detailed view of the results.
+7. "Simulate" --- This is a button that will initiate an ngspice simulation of the electrical parameter.
 
-"Settings" --- Controls global settings for CACE.  The available settings are:
+At the bottom of the window is a space for program messages, warnings, and errors.  Below that is a button bar with the following buttons:
 
-	Print debug output ---
-		Produce additional output for diagnostic and debugging purposes.
-	Force netlist regeneration ---
-		Require netlists to be regenerated for every simulation.  Otherwise,
-		netlists are only regenerated when the source file (schematic or layout)
-		is found to post-date the netlist.
-	Allow edit of all parameters ---
-		Allow the use of "Simulate-->Edit", which provides a method for in-app
-		editing and copying of parameters (note that the characterization file
-		itself may always be edited).
-	Simulate single-threaded ---
-		Normally all simulations are done multi-threaded (with low priority).
-		Selecting this option forces simulations to run one at a time.
-	Keep simulation files ---
-		Normally simulation files are removed after simulation and only the
-		results are kept.  This option forces the files to remain after
-		simulation.
-	Do not create plot files ---
-		Normally plot files are generated for each plot.  If this option is
-		selected, plots may be viewed in-app but no file is generated.
-	Log simulation output ---
-		Copy all simulation output into a log file.
+- "Close" --- Quits the characterization tool.  If new results have been simulated but not saved, the user will have to respond to a prompt.
+- "Save" --- Saves the current characterization results.  These results will be loaded the next time the characterization tool is run, unless there is a design netlist newer than the saved results.
+- "Help" --- Activates this help window.
+- "Settings" --- Controls global settings for CACE.
+
+    The available settings are:
+
+	- Print debug output ---
+		    Produce additional output for diagnostic and debugging purposes.
+	- Force netlist regeneration ---
+		    Require netlists to be regenerated for every simulation.  Otherwise,
+		    netlists are only regenerated when the source file (schematic or layout)
+		    is found to post-date the netlist.
+	- Allow edit of all parameters ---
+		    Allow the use of "Simulate-->Edit", which provides a method for in-app
+		    editing and copying of parameters (note that the characterization file
+		    itself may always be edited).
+	- Simulate single-threaded ---
+		    Normally all simulations are done multi-threaded (with low priority).
+		    Selecting this option forces simulations to run one at a time.
+	- Keep simulation files ---
+		    Normally simulation files are removed after simulation and only the
+		    results are kept.  This option forces the files to remain after
+		    simulation.
+	- Do not create plot files ---
+		    Normally plot files are generated for each plot.  If this option is
+		    selected, plots may be viewed in-app but no file is generated.
+	- Log simulation output ---
+		    Copy all simulation output into a log file.
 	
 
-At the top of the window is the name and location of the datasheet, and on the right is a button that indicates what the source of the netlist being simulated is.  The netlist source can be one of the following choices:
+At the top of the window is the name and location of the datasheet, and on the right is a button that indicates what the source of the netlist being simulated is. The netlist source can be one of the following choices:
+
+- **Schematic Capture**:  Simulations are done from schematic
+- **Layout Extracted**:   Simulations are done from layout without parasitics
+- **R-C Extracted**:      Simulations are done from layout with parasitics
 
-	Schematic Capture:  Simulations are done from schematic
-	Layout Extracted:   Simulations are done from layout without parasitics
-	R-C Extracted:      Simulations are done from layout with parasitics
-
-Separate results are maintained for each of these source cases.  Proper sign-off characterization of a circuit should be done with a netlist from an R-C extracted layout.
-
-2.1
-Generating a netlist
--------
-Design your project schematic in a directory called "xschem" (or the path declared for "schematic" in the characterization file) using the xschem schematic tool.  See the xschem user manual and tutorials for details.  The netlist is generated automatically when running simulations in CACE.
-
-2.2
-Simulation
--------
-To simulate a single electrical parameter, click the 'Simulate' button for each electrical parameter.  Pressing the button creates a drop-down menu with the choices:
+Separate results are maintained for each of these source cases. Proper sign-off characterization of a circuit should be done with a netlist from an R-C extracted layout.
+
+### Generating a netlist
+
+
+Design your project schematic in a directory called "xschem" (or the path declared for "schematic" in the characterization file) using the xschem schematic tool. See the xschem user manual and tutorials for details. The netlist is generated automatically when running simulations in CACE.
+
+### Simulation
+
+To simulate a single electrical parameter, click the `Simulate` button for each electrical parameter. Pressing the button creates a drop-down menu with the choices:
 
 	Run
 	Stop
 	Edit
 	Copy
 
 Left-click on the selection to initiate it.
 
-Run:
-This will combine the design netlist with a testbench, simulate using ngspice, collate results, and display the resulting margin values.  While ngspice is running, the'Simulate' button says '(in progress)'.
+- **Run:**
+This will combine the design netlist with a testbench, simulate using ngspice, collate results, and display the resulting margin values. While ngspice is running, the `Simulate` button says `(in progress)`.
 
-Stop:
+- **Stop:**
 If a testbench is running, then selecting "Stop" will end the simulations.
 
-Edit:
-This allows a testbench definition to be edited through the GUI, to modify the conditions of simulation.  Note that the characterization definition file is text and can also be modified directly with an editor.  Note that parameters are not editable by default.  Go to "Settings" and select "Allow edit of all parameters" to allow parameters to be edited.
+- **Edit:**
+This allows a testbench definition to be edited through the GUI, to modify the conditions of simulation. Note that the characterization definition file is text and can also be modified directly with an editor. Note that parameters are not editable by default. Go to "Settings" and select "Allow edit of all parameters" to allow parameters to be edited.
+
+- **Copy:**
+This creates a new parameter that is a copy of the one selected. The new parameter can then be edited to simulate under a different set of conditions. This can also be done by directly modifying the characterization definition file with a text editor.
+
+### Results
 
-Copy:
-This creates a new parameter that is a copy of the one selected.  The new parameter can then be edited to simulate under a different set of conditions.  This can also be done by directly modifying the characterization definition file with a text editor.
+Every electrical parameter is specified over a range of conditions. This results in a series of simulations, usually one simulation run per unique set of conditions. Each simulation typically provides one result value, and the set of all values from all simulated conditions is used to find the minimum, typical, and maximum results that are printed on the main characterization page.
 
-2.3
-Results
---------
-Every electrical parameter is specified over a range of conditions.  This results in a series of simulations, usually one simulation run per unique set of conditions.  Each simulation typically provides one result value, and the set of all values from all simulated conditions is used to find the minimum, typical, and maximum results that are printed on the main characterization page.
+When an electrical parameter has finished simulating, clicking on the "Status" entry will generate a window showing details of the simulation. The window has one line per unique set of conditions simulated.  For each line, the result value is given in the leftmost column. The remaining columns show each variable condition, and the value it had for the given simulation.  The top of the column shows the range of values for the given parameter. This graph allows the user to quickly determine what are the conditions under which a circuit may be failing, and the degree to which the value is out of range of the specification. Rows in which the result is outside of the specified limit are shown in red.
 
-When an electrical parameter has finished simulating, clicking on the "Status" entry will generate a window showing details of the simulation.  The window has one line per unique set of conditions simulated.  For each line, the result value is given in the leftmost column.  The remaining columns show each variable condition, and the value it had for the given simulation.  The top of the column shows the range of values for the given parameter.  This graph allows the user to quickly determine what are the conditions under which a circuit may be failing, and the degree to which the value is out of range of the specification.  Rows in which the result is outside of the specified limit are shown in red.
+In the results window, click on the title `Results` to change the view from having results ordered highest to lowest, to lowest to highest. Click on the name (column header) of any condition or variable to change the tabular view to a graph showing results vs. the selected condition or variable.
 
-In the results window, click on the title 'Results' to change the view from having results ordered highest to lowest, to lowest to highest.  Click on the name (column header) of any condition or variable to change the tabular view to a graph showing results vs. the selected condition or variable.
-.
```

### Comparing `cace-2.1.9/cace/doc/format.txt` & `cace-2.2.0/docs/source/formats/format_description.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-3.
-CACE format description:  Characterization file syntax
------------------------------------------------------------------
+# Version 4.0 format description
+
+## NOTE
+
+CACE files prior to version 4 (November 2023) are in JSON format
+and can be run through the script `cace_compat.py` to produce a
+version 4.0 text format.
+
+## Syntax
 
 Every line is either a key:value pair or a key:dictionary or a key:list,
 or a blank line, or a comment.
 
-A comment is any line beginning with "#".
+A comment is any line beginning with `#`.
 
 A blank line is any line consisting only of spaces, tabs, and a newline.
 
 For key:value, the format is
 
 	<key>:	<value>
 
 1. Spaces outside of <key> and <value> are optional.
-2. A keyword must be alphanumeric only;  it cannot contain spaces.
+2. A keyword must be alphanumeric only; it cannot contain spaces.
 3. The value may not begin with a space character but may contain space
-   characters.  If the value is interpreted as a string, the spaces are
-   taken literally.  If the value has multiple parts, then the spaces
+   characters. If the value is interpreted as a string, the spaces are
+   taken literally. If the value has multiple parts, then the spaces
    (or tabs) separate the entries.
-4. The key: value assignment ends with a newline.  The <value> may be
+4. The key: value assignment ends with a newline. The <value> may be
    made multi-line by ending lines with backslash-newline.
 
 For key:dictionary, the format is
 
 	<key> {
 		<dictionary>
 	}
@@ -44,42 +50,41 @@
 		+
 		<dictionary>
 
 		...
 	}
 
 1. Each <dictionary> is a dictionary as described above (one or more newline-
-   separated key:value pairs, key:dictionary, or nested key:list).  
+   separated key:value pairs, key:dictionary, or nested key:list).
 2. The "+" may be on its own line or precede the first dictionary keyword,
    separated by space.  A blank line preceding the "+" is optional.
 3. Each key within a dictionary must be unique, but different dictionaries
    in the list will contain the same keywords.
 
-All entries in the file are from the ASCII character set.  Non-ASCII characters
+All entries in the file are from the ASCII character set. Non-ASCII characters
 can be handled with known keywords in braces, such as (but not limited to):
+
 	{degrees}
 	{micro}
 	{sigma}
 	{ohms}
 	{squared}
 	{sqrt}
 
 Dictionaries are generally searched for known keys but unknown keys are not
-flagged.  Therefore comments and other non-critical information can be put
-in otherwise unused dictionary keys.  The key "note" is considered the
+flagged. Therefore comments and other non-critical information can be put
+in otherwise unused dictionary keys. The key "note" is considered the
 proper way to pass comments about the contents of a specific dictionary;
 these can end up as notes in a formatted datasheet output.
-.
-4.
-CACE format description:  Characterization file contents
------------------------------------------------------------------
-
-The top level file itself is a dictionary of <key>:<value>, <key>:<dictionary>,
-or <key>:<list> entries.  The top-level dictionary does not have a key and is
-not delimited by braces.  The file starts with the first key in the dictionary.
+
+##  Characterization file contents
+
+The top level file itself is a dictionary of `<key>`:`<value>`, `<key>`:`<dictionary>`,
+or `<key>`:`<list>` entries. The top-level dictionary does not have a key and is
+not delimited by braces. The file starts with the first key in the dictionary.
 
 Top-level dictionary:
 
 	name:	<string>
 	Name of the design (cell name)
 
 	description:	<string>
@@ -99,21 +104,20 @@
 
 	electrical_parameters: <list>
 	List of specified electical parameters, for spec and measurement (see below).
 
 	physical_parameters: <list>
 	List of specified physical parameters, for spec and measurement (see below).
 
-The order of entries is not meaningful except that "default_conditions" must be
-declared before "electrical_parameters", since the electrical parameters will
+The order of entries is not meaningful except that `default_conditions` must be
+declared before `electrical_parameters`, since the electrical parameters will
 take default conditions before applying specific conditions.
 
-4.1
-Authorship
---------------
+### Authorship
+
 "authorship" dictionary:
 
 	designer:	<name>
 	The person to whom the design is attributed
 
 	company:	<name>
 	The name of a company, if applicable.  This is generally for
@@ -126,17 +130,16 @@
 	modification_date: <datestamp> 
 	Generally handled by the tools to specify when the characterization
 	file was last updated.
 
 	license:	<string>
 	A known license type, such as "Apache 2.0".
 
-4.2
-Paths
---------------
+### Paths
+
 "paths" dictionary:
 
 	documentation:	<path>
 	Location of any documentation for the design.
 
 	schematic:	<path>
 	Location of any schematics (xschem) and symbols for the design.
@@ -173,18 +176,18 @@
 	reports:	<path>
 	Reports and log files generated by CACE.
 
 	root:		<path>
 	This is the location of the project and the root of all the other
 	paths in this dictionary.  It is automatically inserted by CACE.
 
-4.3
-Dependencies
---------------
+### Dependencies
+
 "dependencies" list:
+
 	Each entry in the list is a project on which the design under
 	test is dependent.  Each entry lists a dictionary with the
 	following dictionary entries:
 
 	name:	<string>
 	Name of the dependency
 
@@ -198,17 +201,16 @@
 	target path on demand.
 	
 	commit: <hash>
 	Commit hash of the repository of the dependency to use in this
 	project.  TBD:  Various values that define actions such as updating
 	the repository.
 
-4.4
-Pins
---------------
+### Pins
+
 "pins" dictionary:
 	
 	name:	<string>
 	The pin name.  Must match the name on the schematic or netlist.
 	Vectors should be indexed with ":" and will be expanded when
 	needed.  "b7:0" expands to "b7, b6, b5, ..." while "b[7:0]"
 	expands to "b[7], b[6], b[5], ..." (Note that this is more
@@ -230,17 +232,16 @@
 	(e.g., "vss - 0.3").
 
 	Vmax:	<number>|<expression>
 	The pin minimum voltage may be a value or may be referenced to
 	another pin;  and may be referenced to another pin with an offset
 	(e.g., "vdd + 0.3").
 
-4.5
-Default conditions
---------------
+### Default conditions
+
 "default_conditions" dictionary:
 
 	name: <string>
 	The name of the condition;  this name is meaningful because it
 	will match a variable name used in a schematic or netlist.  The
 	representation in the netlist is always ${<string>} to prevent
 	accidental substitutions of matching strings.  Any set of signals
@@ -281,30 +282,28 @@
 	stepsize: <value>
 	If not present, then a stepsize of 1 is assumed for linear
 	enumeration or 2 for logarithmic enumeration.  Otherwise,
 	the enumeration steps by <value> additive values for linear
 	enumeration or <value> multiplicative values for logarithmic
 	enumeration.
 
-4.6
-Parameter conditions
---------------
+### Parameter conditions
+
 "conditions" dictionary:
 
 	The "conditions" dictionary entries are the same as the
 	"default_conditions" dictionary, above.  The "default_conditions"
 	dictionary is applied to every condition before adding or
 	overwriting with the specific conditions listed for the
 	electrical parameter.  Conditions are only meaningful when the
 	condition name exists in the netlist to be simulated or the file
 	to be evaluated (see "simulate" and "measure" entries).
 
-4.7
-Electrical conditions
---------------
+### Electrical conditions
+
 "electrical_parameters" dictionary:
 
 	name: <string>
 	A name for the electrical parameter (used only for bookkeeping
 	purposes).
 
 	description: <string>
@@ -357,17 +356,16 @@
 	of min/typ/max values).  Requires a corresponding "variables"
 	list.
 
 	testbenches: <list>
 	This entry is automatically generated by CACE and enumerates all
 	of the testbenches to be simulated and evaluated, and the results.
 
-4.8
-Specification
---------------
+### Specification
+
 "spec" dictionary:
 
 	minimum: <value>|any  [fail]	[<calculation>-<limit>]
 	Specifies the target value for the electrical parameter minimum
 	value.  If not specified, then no minimum is measured.  If "any"
 	is given as the value, then the minimum is measured but there
 	is no target value.  If "fail" is also specified, then electrical
@@ -390,18 +388,18 @@
 	value.  If not specified, then no maximum is measured.  If "any"
 	is given as the value, then the maximum is measured but there
 	is no target value.  If "fail" is also specified, then electrical
 	parameter is marked as failing if the measured value is out of
 	spec.  If <calculation>-<limit> is specified, then it overrides
 	the default calculation of "maximum-below"
 
-4.9
-Results
---------------
+### Results
+
 "results" dictionary:
+
 	A set of results that is the measurement counterpart to the
 	"spec" dictionary for an electrical parameter.  The difference
 	is that it includes a key "name" that specifies the netlist
 	source used for the simulations, which is one of "schematic"
 	(for schematic captured netlist), "layout" (layout extracted
 	netlists), "pex" (parasitic capacitance extracted layout), or
 	"rcx" (parasitic capacitance and resistance extracted layout).
@@ -410,18 +408,18 @@
 	"fail") indictating whether the value is in spec or not.
 
 	name: schematic|layout|pex|rcx
 	minimum: <value> [pass|fail]
 	typical: <value> [pass|fail]
 	maximum: <value> [pass|fail]
 
-4.10
-Variables
---------------
+### Variables
+
 "variables" list:
+
 	A variable is any property that affects the electrical parameter
 	result but which is not a condition.  A variable may be used in
 	a plot to graph the result vs. something that is not a condition.
 	Otherwise, all variables must be eliminated during the course of
 	evaluation.  Note:  Use of "collate" in a "simulate" dictionary
 	will force any condition in the collated list to become a
 	variable, as if it were produced by the simulation instead of
@@ -437,17 +435,16 @@
 	in a key if the value is not for data corresponding to the
 	graph X or Y axis.
 
 	unit: <value>
 	This is the unit that will be displayed after the display
 	string.
 
-4.11
-Simulation information
---------------
+### Simulation information
+
 "simulate" dictionary:
 
 	tool: <string>
 	This specifies the (software) tool that is used to make the
 	measurement or to evaluate the measurement result.  Typically
 	the first entry will always be "ngspice" for most electrical
 	parameters.  For physical parameters, it will be a scripting
@@ -481,18 +478,18 @@
 	simulated.  This is used for sweeps and plots.
 
 	collate: <condition> ...
 	This specifies that the simulation output should be collated from
 	runs over all the specified conditions before passing the result
 	to the first "measure" handler.
 
-4.12
-Measurement information
---------------
+### Measurement information
+
 "measure" dictionary:
+
 	Additional entries are tools that operate on the output of
 	the simulator to produce the final results for the datasheet.
 	They may be number-crunching tools like "octave" for compute-
 	intensive evaluations, or they may be a script like python
 	(using numpy or scipy) or bash.  The purpose of "measure" is
 	to modify the result produced by the simulation, including
 	removing variables from the result list.
@@ -514,18 +511,18 @@
 	results and the set of conditions for each.  Currently, ".dat" is in
 	octave format, but should support JSON format for python scripts.
 	The output of the "evaluate" tool is a single list of results that
 	replaces (in order) the result list passed to the tool.  Currently,
 	the output is passed in stdout, and is a list of "result" values
 	that replaces the existing "result" values in the testbench.
 
-4.13
-Internal calculations
---------------
+### Internal calculations
+
 Internal calculation (measurement) methods:
+
 	time:
 	remove:
 	rebase:
 	abs:
 	negate:
 	add:
 	subtract:
@@ -533,23 +530,29 @@
 	clip:
 	mean:
 	risingedge:
 	fallingedge:
 	stabletime:
 	inside:
 	
-4.14
-Plots
---------------
+### Plots
+
 "plot" dictionary:
+
 	filename: <string>
 	Name of a graphic format and filename to use for graph output.
 	Plots are done with python matplotlib, so it must be a format
 	known to matplotlib.
 
+	type: <string>
+	The type of plot to make.  If this record is missing from the
+	dictionary, then plot type "xyplot" is assumed by default.
+	Otherwise, the value should be one of "xyplot", "histogram",
+	"semilogx", "semilogy", or "loglog".
+
 	xaxis: <name>
 	Condition to be plotted on the graph X axis, as determined
 	from the condition related to <name> in the "variables"
 	section.  The X-axis label is taken from the variable entry
 	as well.
 
 	yaxis: <name>
@@ -564,17 +567,16 @@
 Plots are made from measured columnar data which may be from a "wrdata"
 command in ngspice, an "echo" statement directed to a file, or a raw file;
 regardless, each column will be either a condition or a result.  Conditions
 produced by plot-generating tools may contain vectors not in the listed
 conditions for the electrical parameter, such as TIME for time or TRACE for
 the result.
 	
-4.15
-Testbenches
---------------
+### Testbenches
+
 "testbenches" dictionary:
 
 	filename: <string>
 	The name of the filename passed to the simulator.
 
 	conditions: <list>
 	The value of all fixed conditions for this simulation.
@@ -592,17 +594,16 @@
 	is itself a list of which the first item should always be
 	"result", referring to the electrical parameter itself, and
 	optionally followed by one or more variable names.  Each item
 	in the "results" list must have the same number of entries as
 	the format, and entries must match the order of the entries
 	in the format.
 
-4.16
-Physical parameters
---------------
+### Physical parameters
+
 "physical_parameters" list:
 
 	The physical parameters list has the same keywords as the
 	electrical parameters, except that the parameters are
 	physical measurements of the layout such as area, width,
 	height, max metal layer, and may include number of DRC
 	or LVS errors.
@@ -610,18 +611,18 @@
 	Dictionary keys that are shared with "electrical_parameters"
 	are: name, status, description, display, unit, and spec.
 
 	The "evaluate" dictionary is unique to physical parameters
 	and takes the place of "simulate" and "measure" for electrical
 	parameters (see below).
 
-4.17
-Evaluation information
---------------
+### Evaluation information
+
 "evaluate" dictionary:
+
 	The "evaluate" dictionary is unique to the physical_parameters
 	dictionaries.  It describes how to obtain a specific physical
 	or other non-electrical parameter, such as cell size or number
 	of DRC or LVS errors.  Running the tool must produce a single
 	value as output, which is then checked against the spec to
 	provide a pass/fail result.
 
@@ -633,107 +634,24 @@
 	Any options to pass to the tool should be included in the string.
 
 	filename:	<name>
 	The name of a script or filename to pass to the tool specified
 	by "tool", if the tool is not an internal procedure.  The file
 	<name> should exist in the testbench directory.
 
-4.18
-Internal physical parameter tools
---------------
+### Internal physical parameter tools
+
 Internal physical parameter (evaluation) tools:
+
 	cace_drc:	Returns the number of DRC errors found in the design.
 			The result is generally useful only as being zero or
 			non-zero.
 
 	cace_lvs:	Returns the number of LVS errors found in the design.
 			The result is generally useful only as being zero or
 			non-zero.
 
 	cace_area:	Returns the area of the layout.
 
 	cace_width:	Returns the width of the layout.
 
 	cace_length:	Returns the length of the layout.
-.
-5.
-The CACE version 4.0 schematic description
------------------------------------------------------------------
-
-Schematics are drawn normally but statements can have special syntax
-that is substituted by CACE.  The syntax follows three essential rules:
-
-(1) Condition and variable names in the project specification file
-    are written in the schematic in braces, so "temperature" in the
-    project file is "{temperature}" in the schematic.
-
-(2) Expressions involving equations using condition and variable
-    names are written in the schematic in brackets, so, for example,
-    half of condition vdd would be written "[{vdd} / 2]".  These
-    expressions are evaluated in python, so any python expression
-    that evaluates to a valid result may appear inside the brackets.
-
-(3) There are a handful of reserved variable names that are automatically
-    substituted by CACE if they appear in the schematic:
-
-	{PIN|pin_name|net_name}
-		Used in symbol descriptions.  Indicates a pin of a subcircuit
-		including both the pin name in the subcircuit and the name
-		of the net connecting to the pin.  This allows a subcircuit
-		call to be made without any specific pin order.  CACE will
-		determine the pin order and output the correct syntax.
-
-	{FUNCTIONAL|ip_name}
-		Indicates that the subcircuit ip_name will be replaced with
-		its functional view (xspice or verilog) for simulation.
-
-	{cond=value}
-		For any condition cond, this form indicates that "value" is
-		to be subsituted for the condition if the condition is not
-		declared in the CACE project file.
-	
-	{cond|minimum}
-	{cond|maximum}
-	{cond|stepsize}
-	{cond|steps}
-		Instead of substituting one value for a condition, a value
-		over all conditions is substituted, including the maximum
-		over all conditions, minimum over all conditions, the
-		step size between neighboring condition values, or the
-		number of steps over all values of the condition.
-		This is used most often in cases where a condition is handled
-		entirely inside a testbench netlist (such as in a sweep), and
-		not iterated over multiple netlists.
-
-    	{N}
-		This is substituted with the simulation index.  Most often
-		used as a filename suffix for the output data file.
-
-	{filename}
-		The root name of the schematic file.
-
-	{simpath}
-		The name of the path to simulation files.
-
-	{random}
-		A random integer number.
-
-	{DUT_path}
-		The full path to the DUT subcircuit definition netlist.
-
-	{include_DUT}
-		A shorthand that inserts a ".include" statement with the
-		DUT path, or else in the case of a functional block,
-		in-lines the functional definition of the block. 
-
-	{DUT_call}
-		The pin list from the DUT schematic
-
-	{DUT_name}
-		The name of the DUT subcircuit
-
-	{PDK_ROOT}
-		The path to the directory containing the PDK
-
-	{PDK}
-		The name of the PDK
-.
```

### Comparing `cace-2.1.9/cace/gui/consoletext.py` & `cace-2.2.0/cace/gui/consoletext.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
     class StdoutRedirector(IORedirector):
         """A class for redirecting stdout to this Text widget."""
 
         def write(self, str):
             self.text_area.write(str, False)
 
+        def flush(self):
+            pass
+
     class StderrRedirector(IORedirector):
         """A class for redirecting stderr to this Text widget."""
 
         def write(self, str):
             self.text_area.write(str, True)
 
     def __init__(self, master=None, cnf={}, **kw):
```

### Comparing `cace-2.1.9/cace/gui/editparam.py` & `cace-2.2.0/cace/gui/editparam.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,14 @@
 class EditParam(tkinter.Toplevel):
     """Characterization tool electrical parameter editor."""
 
     def __init__(self, parent=None, fontsize=11, *args, **kwargs):
         """See the __init__ for Tkinter.Toplevel."""
         tkinter.Toplevel.__init__(self, parent, *args, **kwargs)
 
-        s = ttk.Style()
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
-        s.configure('bg.TFrame', background='gray40')
         self.parent = parent
         self.withdraw()
         self.title('Electrical parameter editor')
         self.sframe = tkinter.Frame(self)
         self.sframe.grid(column=0, row=0, sticky='news')
 
         # Keep current parameter
@@ -155,20 +147,22 @@
         frame3.canvas.bind_all('<Button-4>', self.on_mousewheel)
         frame3.canvas.bind_all('<Button-5>', self.on_mousewheel)
 
         # Set up configure callback
         frame3.canvas.dframe.bind('<Configure>', self.frame_configure)
 
         # Get the parent's datasheet
-        dsheet = self.parent.datasheet
+        dsheet = self.parent.simulation_manager.get_datasheet()
 
         # Get list of methods from testbench folder
-        dspath = os.path.split(self.parent.filename)[0]
+        # ("dspath" should be the same as "tbpath"---is there any case
+        # where it would not be?
+        # dspath = os.path.split(self.parent.filename)[0]
         paths = dsheet['paths']
-        tbpath = os.path.join(dspath, paths['root'], paths['testbench'])
+        tbpath = os.path.join(paths['root'], paths['testbench'])
         tbfiles = os.listdir(tbpath)
         methods = []
         for spicefile in tbfiles:
             if os.path.splitext(spicefile)[1] == '.spice':
                 methods.append(os.path.splitext(spicefile))
 
         # Get list of pins from parent datasheet
@@ -699,57 +693,62 @@
         if not (description == '(none)' or description == ''):
             self.param['description'] = description
 
         spec = self.param['spec']
 
         targmin = self.minrec.target.get()
         if not (targmin == '(none)' or targmin == ''):
-            pmin = []
-            pmin.append(targmin)
+            pmin = targmin
             pen = self.minrec.penalty.get()
             if not (pen == '(none)' or pen == ''):
+                pmin = []
+                pmin.append(targmin)
                 pmin.append(pen)
             cmin = self.minrec.calc.get()
             if not (cmin == '(none)' or cmin == ''):
                 lmin = self.minrec.limit.get()
                 if not (lmin == '(none)' or lmin == ''):
                     pmin.append(cmin + '-' + lmin)
                 else:
                     pmin.append(cmin)
-            self.param['minimum'] = pmin
+            spec['minimum'] = pmin
+
         targtyp = self.typrec.target.get()
         if not (targtyp == '(none)' or targtyp == ''):
-            ptyp = []
-            ptyp.append(targtyp)
+            ptyp = targtyp
             pen = self.typrec.penalty.get()
             if not (pen == '(none)' or pen == ''):
+                ptyp = []
+                ptyp.append(targtyp)
                 ptyp.append(pen)
             ctyp = self.typrec.calc.get()
             if not (ctyp == '(none)' or ctyp == ''):
                 ltyp = self.typrec.limit.get()
                 if not (ltyp == '(none)' or ltyp == ''):
                     ptyp.append(ctyp + '-' + ltyp)
                 else:
                     ptyp.append(ctyp)
-            self.param['typical'] = ptyp
+            spec['typical'] = ptyp
+
         targmax = self.maxrec.target.get()
         if not (targmax == '(none)' or targmax == ''):
-            pmax = []
-            pmax.append(targmax)
+            pmax = targmax
             pen = self.maxrec.penalty.get()
             if not (pen == '(none)' or pen == ''):
+                pmax = []
+                pmax.append(targmax)
                 pmax.append(pen)
             cmax = self.maxrec.calc.get()
             if not (cmax == '(none)' or cmax == ''):
                 lmax = self.maxrec.limit.get()
                 if not (lmax == '(none)' or lmax == ''):
                     pmax.append(cmax + '-' + lmax)
                 else:
                     pmax.append(cmax)
-            self.param['maximum'] = pmax
+            spec['maximum'] = pmax
 
         condlist = []
         for crec in self.cond:
             cond = {}
             cname = crec.condition.get()
             if cname == '(none)' or cname == '':
                 continue
```

### Comparing `cace-2.1.9/cace/gui/failreport.py` & `cace-2.2.0/cace/gui/failreport.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,71 +25,15 @@
 class FailReport(tkinter.Toplevel):
     """failure report window."""
 
     def __init__(self, parent=None, fontsize=11, *args, **kwargs):
         """See the __init__ for Tkinter.Toplevel."""
         tkinter.Toplevel.__init__(self, parent, *args, **kwargs)
 
-        s = ttk.Style()
-        s.configure('bg.TFrame', background='gray40')
-        s.configure(
-            'italic.TLabel',
-            font=('Helvetica', fontsize, 'italic'),
-            anchor='west',
-        )
-        s.configure(
-            'title.TLabel',
-            font=('Helvetica', fontsize, 'bold italic'),
-            foreground='brown',
-            anchor='center',
-        )
-        s.configure('normal.TLabel', font=('Helvetica', fontsize))
-        s.configure(
-            'red.TLabel', font=('Helvetica', fontsize), foreground='red'
-        )
-        s.configure(
-            'green.TLabel', font=('Helvetica', fontsize), foreground='green4'
-        )
-        s.configure(
-            'blue.TLabel', font=('Helvetica', fontsize), foreground='blue'
-        )
-        s.configure(
-            'brown.TLabel',
-            font=('Helvetica', fontsize, 'italic'),
-            foreground='brown',
-            anchor='center',
-        )
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'red.TButton',
-            font=('Helvetica', fontsize),
-            foreground='red',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'green.TButton',
-            font=('Helvetica', fontsize),
-            foreground='green4',
-            border=3,
-            relief='raised',
-        )
-        s.configure(
-            'title.TButton',
-            font=('Helvetica', fontsize, 'bold italic'),
-            foreground='brown',
-            border=0,
-            relief='groove',
-        )
-
+        self.parent = parent
         self.withdraw()
         self.title('Local Characterization Report')
         self.root = parent.root
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
 
         # Scrolled frame:  Need frame, then canvas and scrollbars;  finally, the
@@ -272,23 +216,35 @@
                 self.plotframe, text=param['display'], style='title.TLabel'
             ).grid(row=1, column=0)
         canvas.draw()
         canvas.get_tk_widget().grid(row=0, column=0, sticky='nsew')
         # Finally, open the window if it was not already open.
         self.open()
 
-    def table_to_plot(self, condition, dsheet, filename):
+    def table_to_plot(self, condition, pname):
         # Switch from a table view to a plot view, using the condname as
         # the X axis variable.
 
         # Destroy existing contents.
         for widget in self.plotframe.winfo_children():
             widget.destroy()
 
-        param = self.data
+        dsheet = self.parent.simulation_manager.get_datasheet()
+
+        # Find parameter
+        if pname:
+            param = self.parent.simulation_manager.find_parameter(pname)
+        # Reuse the last parameter
+        else:
+            param = self.data
+
+        filename = self.parent.simulation_manager.get_runtime_options(
+            'filename'
+        )
+
         plotrec = {}
         plotrec['xaxis'] = condition
         plotrec['xlabel'] = condition
         # Note: cace_makeplot adds text for units, if available
         plotrec['ylabel'] = param['name']
         plotrec['type'] = 'xyplot'
 
@@ -311,36 +267,44 @@
             canvas.get_tk_widget().grid(row=0, column=0, sticky='nsew')
 
             # Display the button to return to the table view
             # except for transient and Monte Carlo simulations which are too large to tabulate.
             if not condition == 'time':
                 self.bbar.table_button.grid(column=1, row=0, padx=5)
                 self.bbar.table_button.configure(
-                    command=lambda param=param, dsheet=dsheet, filename=filename: self.display(
-                        param, dsheet, filename
-                    )
+                    command=lambda pname=pname: self.display(pname)
                 )
 
             # Finally, open the window if it was not already open.
             self.open()
         else:
             # Plot failed;  revert to the table view
             self.display(param, dsheet, filename)
 
-    def display(self, param=None, dsheet=None, filename=None):
+    def display(self, pname=None):
         # (Diagnostic)
         # print('failure report:  passed parameter ' + str(param))
 
+        dsheet = self.parent.simulation_manager.get_datasheet()
+
+        # Find parameter
+        if pname:
+            param = self.parent.simulation_manager.find_parameter(pname)
+        # Reuse the last parameter
+        else:
+            param = self.data
+
+        filename = self.parent.simulation_manager.get_runtime_options(
+            'filename'
+        )
+
         # Destroy existing contents.
         for widget in self.mainarea.faildisplay.winfo_children():
             widget.destroy()
 
-        if not param:
-            param = self.data
-
         # 'param' is a dictionary pulled in from the annotate datasheet.
         # If the failure display was called, then 'param' should contain
         # record called 'results'.  If the parameter has no results, then
         # there is nothing to do.
 
         if 'plot' in param:
             self.failframe.grid_forget()
@@ -430,15 +394,15 @@
                 # Add the testbench filename as the last entry
                 tresult.append(os.path.split(testbench['filename'])[1])
                 results.append(tresult)
 
             # Check for transient simulation
             if 'time' in names:
                 # Transient data are (usually) too numerous to tabulate, so go straight to plot
-                self.table_to_plot('time', dsheet, filename)
+                self.table_to_plot('time', pname)
                 return
 
             # Check for Monte Carlo simulation
             if 'iterations' in names:
                 # Monte Carlo data are too numerous to tabulate, so go straight to plot
                 self.table_to_histogram(dsheet, filename)
                 return
@@ -585,26 +549,30 @@
                 if j == 0:
                     # Add unicode arrow up/down depending on sort direction
                     labtext += ' \u21e9' if self.sortdir else ' \u21e7'
                     header = ttk.Button(
                         body,
                         text=labtext,
                         style='title.TButton',
-                        command=lambda param=param, dsheet=dsheet: self.changesort(
-                            param, dsheet
-                        ),
+                        command=lambda pname=pname: self.changesort(pname),
                     )
                     ToolTip(header, text='Reverse order of results')
+                elif labtext == 'testbench':
+                    header = ttk.Label(
+                        body,
+                        text=labtext,
+                        style='title.TLabel',
+                    )
                 else:
                     header = ttk.Button(
                         body,
                         text=labtext,
                         style='title.TLabel',
-                        command=lambda plottext=plottext, dsheet=dsheet, filename=filename: self.table_to_plot(
-                            plottext, dsheet, filename
+                        command=lambda plottext=plottext, pname=pname: self.table_to_plot(
+                            plottext, pname
                         ),
                     )
                     ToolTip(
                         header,
                         text='Plot results with this condition on the X axis',
                     )
                 header.grid(row=0, column=j, sticky='ewns')
@@ -703,17 +671,17 @@
             self.size_failreport()
 
         # Don't put the button at the bottom to return to table view.
         self.bbar.table_button.grid_forget()
         # Finally, open the window if it was not already open.
         self.open()
 
-    def changesort(self, param, dsheet):
+    def changesort(self, pname):
         self.sortdir = False if self.sortdir == True else True
-        self.display(param, dsheet)
+        self.display(pname)
 
     def close(self):
         # pop down failure report window
         self.withdraw()
 
     def open(self):
         # pop up failure report window
```

### Comparing `cace-2.1.9/cace/gui/settings.py` & `cace-2.2.0/cace/gui/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 
     def __init__(
         self, parent=None, fontsize=11, callback=None, *args, **kwargs
     ):
         """See the __init__ for Tkinter.Toplevel."""
         tkinter.Toplevel.__init__(self, parent, *args, **kwargs)
 
-        s = ttk.Style()
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
         self.protocol('WM_DELETE_WINDOW', self.close)
         self.parent = parent
         self.withdraw()
         self.title('Characterization Tool Settings')
         self.sframe = tkinter.Frame(self)
         self.sframe.grid(column=0, row=0, sticky='news')
 
@@ -105,26 +98,79 @@
         self.dolog = tkinter.IntVar(self.sframe)
         self.dolog.set(0)
         self.sframe.log = ttk.Checkbutton(
             self.sframe, text='Log simulation output', variable=self.dolog
         )
         self.sframe.log.pack(side='top', anchor='w')
 
+        parallel_parameters = (
+            self.parent.simulation_manager.get_runtime_options(
+                'parallel_parameters'
+            )
+        )
+        self.sframe.ppframe = ttk.Frame(self.sframe)
+        vcmd = (
+            self.register(self.validate),
+            '%d',
+            '%i',
+            '%P',
+            '%s',
+            '%S',
+            '%v',
+            '%V',
+            '%W',
+        )
+        self.ppframe_entry = ttk.Entry(
+            self.sframe.ppframe, width=2, validate='key', validatecommand=vcmd
+        )
+        self.ppframe_entry.insert(0, parallel_parameters)
+        self.ppframe_label = ttk.Label(
+            self.sframe.ppframe, text='Max parallel parameters'
+        )
+
+        self.ppframe_entry.grid(column=0, row=0)
+        self.ppframe_label.grid(column=1, row=0)
+
+        self.sframe.ppframe.pack(side='top', anchor='w')
+
         # self.sframe.sdisplay.sopts(side = 'top', fill = 'x', expand = 'true')
 
         self.bbar = ttk.Frame(self)
         self.bbar.grid(column=0, row=1, sticky='news')
         self.bbar.close_button = ttk.Button(
             self.bbar, text='Close', command=self.close, style='normal.TButton'
         )
         self.bbar.close_button.grid(column=0, row=0, padx=5)
 
         # Callback-on-close
         self.callback = callback
 
+    def validate(
+        self,
+        action,
+        index,
+        value_if_allowed,
+        prior_value,
+        text,
+        validation_type,
+        trigger_type,
+        widget_name,
+    ):
+        # action=1 -> insert
+        if action == '1':
+            if text in '0123456789':
+                try:
+                    return int(value_if_allowed) > 0
+                except ValueError:
+                    return False
+            else:
+                return False
+        else:
+            return True
+
     def grid_configure(self, padx, pady):
         pass
 
     def redisplay(self):
         pass
 
     def get_force(self):
@@ -155,14 +201,21 @@
         # return the state of the "characterize as schematic" checkbox
         return False if self.doschem.get() == 0 else True
 
     def get_log(self):
         # return the state of the "log simulation output" checkbox
         return False if self.dolog.get() == 0 else True
 
+    def get_parallel_parameters(self):
+        # return the maximum number of parallel parameters
+        if self.ppframe_entry.get():
+            return int(self.ppframe_entry.get())
+        else:
+            return 1
+
     def close(self):
         # pop down settings window
         self.withdraw()
         # execute the callback function, if one is given
         if self.callback:
             self.callback()
```

### Comparing `cace-2.1.9/cace/gui/simhints.py` & `cace-2.2.0/cace/gui/simhints.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,14 @@
 class SimHints(tkinter.Toplevel):
     """Characterization tool simulation hints management."""
 
     def __init__(self, parent=None, fontsize=11, *args, **kwargs):
         """See the __init__ for Tkinter.Toplevel."""
         tkinter.Toplevel.__init__(self, parent, *args, **kwargs)
 
-        s = ttk.Style()
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
         self.protocol('WM_DELETE_WINDOW', self.close)
         self.parent = parent
         self.withdraw()
         self.title('Simulation hints management')
         self.sframe = tkinter.Frame(self)
         self.sframe.grid(column=0, row=0, sticky='news')
```

### Comparing `cace-2.1.9/cace/gui/textreport.py` & `cace-2.2.0/cace/gui/textreport.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 class TextReport(tkinter.Toplevel):
     """Open Galaxy text report window."""
 
     def __init__(self, parent=None, fontsize=11, *args, **kwargs):
         """See the __init__ for Tkinter.Toplevel."""
         tkinter.Toplevel.__init__(self, parent, *args, **kwargs)
 
-        s = ttk.Style()
-        s.configure(
-            'normal.TButton',
-            font=('Helvetica', fontsize),
-            border=3,
-            relief='raised',
-        )
         self.protocol('WM_DELETE_WINDOW', self.close)
 
         self.withdraw()
         self.title('Open Galaxy Text Report')
 
         self.texttitle = ttk.Label(
             self, style='title.TLabel', text='(no text)'
@@ -95,15 +88,15 @@
                     self.timestamp = statbuf.st_mtime
             else:
                 self.add_text_from_file(filename)
 
         # Remove and replace contents
         self.hframe.textdisplay.page.delete('1.0', 'end')
         self.hframe.textdisplay.page.insert('end', self.text)
-        self.textttitle.configure(text=self.title)
+        self.texttitle.configure(text=self.title)
         self.open()
 
     # Fill the text report from a file.
 
     def add_text_from_file(self, filename):
         print('Loading text from file ' + filename)
         with open(filename, 'r') as f:
```

### Comparing `cace-2.1.9/cace/gui/tksimpledialog.py` & `cace-2.2.0/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace/gui/tooltip.py` & `cace-2.2.0/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/cace.egg-info/PKG-INFO` & `cace-2.2.0/cace.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.1.9
+Version: 2.2.0
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -42,14 +42,18 @@
 	$ python3 -m pip install --upgrade cace
 Prerequisite design tools:
 
 - xschem:  [https://github.com/stefanschippers/xschem](https://github.com/stefanschippers/xschem)
 - ngspice: git://git.code.sf.net/p/ngspice/ngspice
 - magic:	 [https://github.com/RTimothyEdwards/magic](https://github.com/RTimothyEdwards/magic)
 
+Some of the measurements require:
+
+- octave: [https://octave.org/](https://octave.org/)
+
 ## Usage
 
 If installed as Python package, CACE can be started from the command line using:
 
 ```
 $ cace
 ```
@@ -100,21 +104,21 @@
 ```
 $ make docs
 ```
 
 To host the docs, run:
 
 ```
-make host-docs
+$ make host-docs
 ```
 
 To automatically refresh the docs upon changes, run:
 
 ```
-make auto-docs
+$ make auto-docs
 ```
 
 > [!NOTE]
 > The latest documentation can be viewed online at [cace.readthedocs.io](https://cace.readthedocs.io/). 
 
 ## Examples
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.1.9 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.0 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
@@ -17,26 +17,27 @@
 testbenches and analysis scripts to characterize a circuit and to produce a
 datasheet showing the circuit performance. ## Installation You'll need the
 following: - Python 3.8 or higher with PIP and Tkinter CACE can be installed
 directly from PyPI: $ python3 -m pip install --upgrade cace Prerequisite design
 tools: - xschem: [https://github.com/stefanschippers/xschem](https://
 github.com/stefanschippers/xschem) - ngspice: git://git.code.sf.net/p/ngspice/
 ngspice - magic: [https://github.com/RTimothyEdwards/magic](https://github.com/
-RTimothyEdwards/magic) ## Usage If installed as Python package, CACE can be
-started from the command line using: ``` $ cace ``` Or to start the GUI: ``` $
-cace-gui ``` Information on how to use CACE can be found in the documentation
-at [cace.readthedocs.io](https://cace.readthedocs.io/). ## Development ###
-Dependencies > [!IMPORTANT] > You may need to set up a Python [virtual
-environment](https://docs.python.org/3/library/venv.html). To install the
-dependencies for CACE, run: $ make dependencies ### Python Package To build the
-Python package, run: ``` $ make build ``` To install the package, run: ``` $
-make install ``` To install the package in editable mode, run: ``` $ make
+RTimothyEdwards/magic) Some of the measurements require: - octave: [https://
+octave.org/](https://octave.org/) ## Usage If installed as Python package, CACE
+can be started from the command line using: ``` $ cace ``` Or to start the GUI:
+``` $ cace-gui ``` Information on how to use CACE can be found in the
+documentation at [cace.readthedocs.io](https://cace.readthedocs.io/). ##
+Development ### Dependencies > [!IMPORTANT] > You may need to set up a Python
+[virtual environment](https://docs.python.org/3/library/venv.html). To install
+the dependencies for CACE, run: $ make dependencies ### Python Package To build
+the Python package, run: ``` $ make build ``` To install the package, run: ```
+$ make install ``` To install the package in editable mode, run: ``` $ make
 editable ``` ### Documentation To build the documentation, run: ``` $ make docs
-``` To host the docs, run: ``` make host-docs ``` To automatically refresh the
-docs upon changes, run: ``` make auto-docs ``` > [!NOTE] > The latest
+``` To host the docs, run: ``` $ make host-docs ``` To automatically refresh
+the docs upon changes, run: ``` $ make auto-docs ``` > [!NOTE] > The latest
 documentation can be viewed online at [cace.readthedocs.io](https://
 cace.readthedocs.io/). ## Examples The following repositories contain example
 circuit designs, each having a "cace/" subdirectory with a specification input
 file in the format described below, and a set of testbench schematics which are
 used by CACE to measure all specified electrical and physical parameters,
 generate results, and analyze them to determine circuit performance over
 corners. > [!NOTE] > Example repositories, like CACE itself, are currently a
```

### Comparing `cace-2.1.9/cace.egg-info/SOURCES.txt` & `cace-2.2.0/cace.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .readthedocs.yaml
+Changelog.md
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 requirements_docs.txt
@@ -30,27 +31,31 @@
 cace/common/cace_makeplot.py
 cace/common/cace_measure.py
 cace/common/cace_read.py
 cace/common/cace_regenerate.py
 cace/common/cace_simulate.py
 cace/common/cace_unused.txt
 cace/common/cace_write.py
+cace/common/electrical_parameter.py
 cace/common/layout_estimate.py
 cace/common/netlist_precheck.py
+cace/common/physical_parameter.py
 cace/common/safe_eval.py
+cace/common/simulation_job.py
+cace/common/simulation_manager.py
 cace/common/spiceunits.py
-cace/doc/characterize_help.txt
-cace/doc/format.txt
 cace/gui/__init__.py
 cace/gui/consoletext.py
 cace/gui/editparam.py
 cace/gui/failreport.py
 cace/gui/helpwindow.py
+cace/gui/rowwidget.py
 cace/gui/settings.py
 cace/gui/simhints.py
+cace/gui/style.py
 cace/gui/textreport.py
 cace/gui/tksimpledialog.py
 cace/gui/tooltip.py
 docs/Makefile
 docs/make.bat
 docs/source/characterization.md
 docs/source/conf.py
```

### Comparing `cace-2.1.9/docs/Makefile` & `cace-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/make.bat` & `cace-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/_static/cace_screenshot.png` & `cace-2.2.0/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/conf.py` & `cace-2.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/formats/schematic_description.md` & `cace-2.2.0/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/index.md` & `cace-2.2.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/usage/cace_gui.md` & `cace-2.2.0/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.9/docs/source/usage/getting_started.md` & `cace-2.2.0/docs/source/usage/getting_started.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,21 @@
 ```
 $ make docs
 ```
 
 To host the docs, run:
 
 ```
-make host-docs
+$ make host-docs
+```
+
+To automatically refresh the docs upon changes, run:
+
+```
+$ make auto-docs
 ```
 
 > [!NOTE]
 > The latest documentation can be viewed online at [cace.readthedocs.io](https://cace.readthedocs.io/). 
 
 ## Examples
```

### Comparing `cace-2.1.9/pyproject.toml` & `cace-2.2.0/pyproject.toml`

 * *Files identical despite different names*

