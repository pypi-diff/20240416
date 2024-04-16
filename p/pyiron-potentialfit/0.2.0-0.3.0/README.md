# Comparing `tmp/pyiron_potentialfit-0.2.0.tar.gz` & `tmp/pyiron_potentialfit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_potentialfit-0.2.0.tar", last modified: Wed Apr 10 09:12:40 2024, max compression
+gzip compressed data, was "pyiron_potentialfit-0.3.0.tar", last modified: Tue Apr 16 05:40:13 2024, max compression
```

## Comparing `pyiron_potentialfit-0.2.0.tar` & `pyiron_potentialfit-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/pyiron_potentialfit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/atomicrex_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/function_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/general_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/potential_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    33964 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/structure_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/meamfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/potentialfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/cfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/masters.py
--rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlipdescriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/storageclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.435933 pyiron_potentialfit-0.3.0/pyiron_potentialfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/atomicrex_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/function_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/general_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/potential_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33964 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/structure_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/meamfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/potentialfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/masters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlipdescriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/storageclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/projectflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/versioneer.py
```

### Comparing `pyiron_potentialfit-0.2.0/LICENSE` & `pyiron_potentialfit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/PKG-INFO` & `pyiron_potentialfit-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.2.0
+Version: 0.3.0
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
-Requires-Dist: pyiron_atomistics>=0.4.16
+Requires-Dist: pyiron_atomistics>=0.5.1
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyiron_base>=0.7.9
+Requires-Dist: pyiron_base>=0.8.1
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: runnerase>=0.3.3
+Requires-Dist: seaborn
+Requires-Dist: dill
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/__init__.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/base.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/fit_properties.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/fit_properties.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/function_factory.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/function_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/general_input.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/general_input.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/interactive.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/parameter_constraints.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/potential_factory.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/potential_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/structure_list.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/structure_list.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/utility_functions.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/meamfit.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/meamfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/potentialfit.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/potentialfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/cfgs.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/cfgs.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/lammps.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/masters.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/masters.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlip.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlip.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlipdescriptors.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlipdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/parser.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/potential.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/job.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/job.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/storageclasses.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/storageclasses.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/utils.py` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/PKG-INFO` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.2.0
+Version: 0.3.0
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
-Requires-Dist: pyiron_atomistics>=0.4.16
+Requires-Dist: pyiron_atomistics>=0.5.1
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyiron_base>=0.7.9
+Requires-Dist: pyiron_base>=0.8.1
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: runnerase>=0.3.3
+Requires-Dist: seaborn
+Requires-Dist: dill
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/SOURCES.txt` & `pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 versioneer.py
 pyiron_potentialfit/__init__.py
 pyiron_potentialfit/_version.py
 pyiron_potentialfit.egg-info/PKG-INFO
 pyiron_potentialfit.egg-info/SOURCES.txt
 pyiron_potentialfit.egg-info/dependency_links.txt
+pyiron_potentialfit.egg-info/entry_points.txt
 pyiron_potentialfit.egg-info/requires.txt
 pyiron_potentialfit.egg-info/top_level.txt
 pyiron_potentialfit/atomicrex/__init__.py
 pyiron_potentialfit/atomicrex/atomicrex_job.py
 pyiron_potentialfit/atomicrex/base.py
 pyiron_potentialfit/atomicrex/fit_properties.py
 pyiron_potentialfit/atomicrex/function_factory.py
@@ -40,8 +41,14 @@
 pyiron_potentialfit/mlip/parser.py
 pyiron_potentialfit/mlip/potential.py
 pyiron_potentialfit/pacemaker/__init__.py
 pyiron_potentialfit/pacemaker/job.py
 pyiron_potentialfit/runner/__init__.py
 pyiron_potentialfit/runner/job.py
 pyiron_potentialfit/runner/storageclasses.py
-pyiron_potentialfit/runner/utils.py
+pyiron_potentialfit/runner/utils.py
+pyiron_potentialfit/spgfit/__init__.py
+pyiron_potentialfit/spgfit/calculations.py
+pyiron_potentialfit/spgfit/learn.py
+pyiron_potentialfit/spgfit/projectflow.py
+pyiron_potentialfit/spgfit/structures.py
+pyiron_potentialfit/spgfit/util.py
```

### Comparing `pyiron_potentialfit-0.2.0/setup.py` & `pyiron_potentialfit-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,16 +27,26 @@
         'Programming Language :: Python :: 3.11',
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
         'ase>=3.22.1',
-        'pyiron_atomistics>=0.4.16',
+        'pyiron_atomistics>=0.5.1',
         'matplotlib>=3.8.3',
         'numpy>=1.26.4',
-        'pyiron_base>=0.7.9',
+        'pyiron_base>=0.8.1',
         'scipy>=1.11.4',
         'runnerase>=0.3.3',
+        # spgfit
+        'seaborn',
+        'dill'
     ],
     cmdclass=versioneer.get_cmdclass(),
+    entry_points={
+        "console_scripts": [
+            "spgfit-structures = pyiron_potentialfit.spgfit.structures:main",
+            "spgfit-calculations = pyiron_potentialfit.spgfit.calculations:main",
+            "spgfit-learn = pyiron_potentialfit.spgfit.learn:main"
+        ]
+    }
 )
```

### Comparing `pyiron_potentialfit-0.2.0/versioneer.py` & `pyiron_potentialfit-0.3.0/versioneer.py`

 * *Files identical despite different names*

