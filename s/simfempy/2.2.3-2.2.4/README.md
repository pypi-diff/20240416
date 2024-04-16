# Comparing `tmp/simfempy-2.2.3.tar.gz` & `tmp/simfempy-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfempy-2.2.3.tar", last modified: Tue Apr 16 14:23:56 2024, max compression
+gzip compressed data, was "simfempy-2.2.4.tar", last modified: Tue Apr 16 14:27:03 2024, max compression
```

## Comparing `simfempy-2.2.3.tar` & `simfempy-2.2.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.082609 simfempy-2.2.3/
--rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.2.3/LICENSE
--rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:23:56.081822 simfempy-2.2.3/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     2679 2024-04-16 14:23:55.000000 simfempy-2.2.3/README.md
--rw-r--r--   0 becker     (501) staff       (20)       38 2024-04-16 14:23:56.082758 simfempy-2.2.3/setup.cfg
--rw-r--r--   0 becker     (501) staff       (20)     1332 2024-04-16 14:23:48.000000 simfempy-2.2.3/setup.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.053926 simfempy-2.2.3/simfempy/
--rw-r--r--   0 becker     (501) staff       (20)      153 2024-04-13 14:16:18.000000 simfempy-2.2.3/simfempy/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.057756 simfempy-2.2.3/simfempy/applications/
--rw-r--r--   0 becker     (501) staff       (20)       40 2024-04-14 11:38:13.000000 simfempy-2.2.3/simfempy/applications/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     4907 2024-04-15 15:48:55.000000 simfempy-2.2.3/simfempy/applications/application.py
--rw-r--r--   0 becker     (501) staff       (20)    15260 2024-04-14 11:38:49.000000 simfempy-2.2.3/simfempy/applications/navierstokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.060102 simfempy-2.2.3/simfempy/examples/
--rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.2.3/simfempy/examples/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     3266 2024-04-16 14:20:46.000000 simfempy-2.2.3/simfempy/examples/flow_static.py
--rw-r--r--   0 becker     (501) staff       (20)     3048 2024-04-14 11:36:23.000000 simfempy-2.2.3/simfempy/examples/heat_dynamic.py
--rw-r--r--   0 becker     (501) staff       (20)     2623 2024-04-14 16:50:50.000000 simfempy-2.2.3/simfempy/examples/heat_static.py
--rw-r--r--   0 becker     (501) staff       (20)     3950 2024-04-14 11:36:23.000000 simfempy-2.2.3/simfempy/examples/interface.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.063842 simfempy-2.2.3/simfempy/fems/
--rw-r--r--   0 becker     (501) staff       (20)       48 2024-04-14 08:58:57.000000 simfempy-2.2.3/simfempy/fems/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    27607 2024-04-16 13:11:08.000000 simfempy-2.2.3/simfempy/fems/cr1.py
--rw-r--r--   0 becker     (501) staff       (20)     2740 2024-04-14 11:13:29.000000 simfempy-2.2.3/simfempy/fems/d0.py
--rw-r--r--   0 becker     (501) staff       (20)      819 2024-04-14 14:58:27.000000 simfempy-2.2.3/simfempy/fems/data.py
--rw-r--r--   0 becker     (501) staff       (20)     2707 2024-04-14 14:40:31.000000 simfempy-2.2.3/simfempy/fems/femvector.py
--rw-r--r--   0 becker     (501) staff       (20)    29792 2024-04-16 12:20:49.000000 simfempy-2.2.3/simfempy/fems/p1.py
--rw-r--r--   0 becker     (501) staff       (20)     7757 2024-04-16 12:56:57.000000 simfempy-2.2.3/simfempy/fems/p1general.py
--rw-r--r--   0 becker     (501) staff       (20)    16154 2024-04-14 14:34:37.000000 simfempy-2.2.3/simfempy/fems/rt0.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.066446 simfempy-2.2.3/simfempy/linalg/
--rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.2.3/simfempy/linalg/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    14665 2024-04-14 16:43:13.000000 simfempy-2.2.3/simfempy/linalg/linalg.py
--rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.2.3/simfempy/linalg/matrixsystem.py
--rw-r--r--   0 becker     (501) staff       (20)    11014 2024-04-13 17:37:20.000000 simfempy-2.2.3/simfempy/linalg/saddle_point.py
--rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.2.3/simfempy/linalg/vectorview.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.068390 simfempy-2.2.3/simfempy/meshes/
--rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.2.3/simfempy/meshes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.2.3/simfempy/meshes/plotmesh.py
--rw-r--r--   0 becker     (501) staff       (20)    20421 2024-04-16 14:20:18.000000 simfempy-2.2.3/simfempy/meshes/simplexmesh.py
--rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.2.3/simfempy/meshes/testmeshes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.071336 simfempy-2.2.3/simfempy/models/
--rw-r--r--   0 becker     (501) staff       (20)       52 2024-04-14 11:36:23.000000 simfempy-2.2.3/simfempy/models/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    29397 2024-04-16 14:04:25.000000 simfempy-2.2.3/simfempy/models/elliptic.py
--rw-r--r--   0 becker     (501) staff       (20)    29087 2024-04-16 13:36:02.000000 simfempy-2.2.3/simfempy/models/model.py
--rw-r--r--   0 becker     (501) staff       (20)     5358 2024-04-14 15:38:59.000000 simfempy-2.2.3/simfempy/models/navierstokes.py
--rw-r--r--   0 becker     (501) staff       (20)    10227 2024-04-14 12:02:52.000000 simfempy-2.2.3/simfempy/models/problemdata.py
--rw-r--r--   0 becker     (501) staff       (20)    39284 2024-04-14 15:43:35.000000 simfempy-2.2.3/simfempy/models/stokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.073050 simfempy-2.2.3/simfempy/solvers/
--rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.2.3/simfempy/solvers/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     8650 2024-04-13 22:01:19.000000 simfempy-2.2.3/simfempy/solvers/newton.py
--rw-r--r--   0 becker     (501) staff       (20)     2454 2024-04-13 21:39:49.000000 simfempy-2.2.3/simfempy/solvers/newtondata.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.074008 simfempy-2.2.3/simfempy/tests/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.3/simfempy/tests/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.075440 simfempy-2.2.3/simfempy/tests/navierstokes/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-04-14 09:41:29.000000 simfempy-2.2.3/simfempy/tests/navierstokes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     3881 2024-04-14 15:24:05.000000 simfempy-2.2.3/simfempy/tests/navierstokes/flow_static.py
--rw-r--r--   0 becker     (501) staff       (20)     4372 2024-04-13 14:20:43.000000 simfempy-2.2.3/simfempy/tests/navierstokes/incompflow.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.076730 simfempy-2.2.3/simfempy/tests/stokes/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.3/simfempy/tests/stokes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5012 2024-04-14 11:36:23.000000 simfempy-2.2.3/simfempy/tests/stokes/stokes_analytic.py
--rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.2.3/simfempy/tests/stokes/test_stokes.py
--rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.2.3/simfempy/tests/testcaseanalytical.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.080624 simfempy-2.2.3/simfempy/tools/
--rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.2.3/simfempy/tools/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.2.3/simfempy/tools/analyticalfunction.py
--rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.2.3/simfempy/tools/barycentric.py
--rw-r--r--   0 becker     (501) staff       (20)    14940 2024-04-15 15:48:55.000000 simfempy-2.2.3/simfempy/tools/comparemethods.py
--rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.2.3/simfempy/tools/file_explorer.py
--rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.2.3/simfempy/tools/iterationcounter.py
--rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.2.3/simfempy/tools/latexwriter.py
--rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.2.3/simfempy/tools/timer.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:23:56.081178 simfempy-2.2.3/simfempy.egg-info/
--rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:23:56.000000 simfempy-2.2.3/simfempy.egg-info/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     1731 2024-04-16 14:23:56.000000 simfempy-2.2.3/simfempy.egg-info/SOURCES.txt
--rw-r--r--   0 becker     (501) staff       (20)        1 2024-04-16 14:23:56.000000 simfempy-2.2.3/simfempy.egg-info/dependency_links.txt
--rw-r--r--   0 becker     (501) staff       (20)       47 2024-04-16 14:23:56.000000 simfempy-2.2.3/simfempy.egg-info/requires.txt
--rw-r--r--   0 becker     (501) staff       (20)        9 2024-04-16 14:23:56.000000 simfempy-2.2.3/simfempy.egg-info/top_level.txt
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.607526 simfempy-2.2.4/
+-rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.2.4/LICENSE
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:27:03.606857 simfempy-2.2.4/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     2679 2024-04-16 14:27:03.000000 simfempy-2.2.4/README.md
+-rw-r--r--   0 becker     (501) staff       (20)       38 2024-04-16 14:27:03.607668 simfempy-2.2.4/setup.cfg
+-rw-r--r--   0 becker     (501) staff       (20)     1332 2024-04-16 14:26:54.000000 simfempy-2.2.4/setup.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.577686 simfempy-2.2.4/simfempy/
+-rw-r--r--   0 becker     (501) staff       (20)      153 2024-04-13 14:16:18.000000 simfempy-2.2.4/simfempy/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.581511 simfempy-2.2.4/simfempy/applications/
+-rw-r--r--   0 becker     (501) staff       (20)       40 2024-04-14 11:38:13.000000 simfempy-2.2.4/simfempy/applications/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     4907 2024-04-15 15:48:55.000000 simfempy-2.2.4/simfempy/applications/application.py
+-rw-r--r--   0 becker     (501) staff       (20)    15260 2024-04-14 11:38:49.000000 simfempy-2.2.4/simfempy/applications/navierstokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.584112 simfempy-2.2.4/simfempy/examples/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.2.4/simfempy/examples/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3266 2024-04-16 14:20:46.000000 simfempy-2.2.4/simfempy/examples/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3048 2024-04-14 11:36:23.000000 simfempy-2.2.4/simfempy/examples/heat_dynamic.py
+-rw-r--r--   0 becker     (501) staff       (20)     2623 2024-04-14 16:50:50.000000 simfempy-2.2.4/simfempy/examples/heat_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3950 2024-04-14 11:36:23.000000 simfempy-2.2.4/simfempy/examples/interface.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.588079 simfempy-2.2.4/simfempy/fems/
+-rw-r--r--   0 becker     (501) staff       (20)       48 2024-04-14 08:58:57.000000 simfempy-2.2.4/simfempy/fems/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    27607 2024-04-16 13:11:08.000000 simfempy-2.2.4/simfempy/fems/cr1.py
+-rw-r--r--   0 becker     (501) staff       (20)     2740 2024-04-14 11:13:29.000000 simfempy-2.2.4/simfempy/fems/d0.py
+-rw-r--r--   0 becker     (501) staff       (20)      819 2024-04-14 14:58:27.000000 simfempy-2.2.4/simfempy/fems/data.py
+-rw-r--r--   0 becker     (501) staff       (20)     2707 2024-04-14 14:40:31.000000 simfempy-2.2.4/simfempy/fems/femvector.py
+-rw-r--r--   0 becker     (501) staff       (20)    29792 2024-04-16 12:20:49.000000 simfempy-2.2.4/simfempy/fems/p1.py
+-rw-r--r--   0 becker     (501) staff       (20)     7757 2024-04-16 12:56:57.000000 simfempy-2.2.4/simfempy/fems/p1general.py
+-rw-r--r--   0 becker     (501) staff       (20)    16154 2024-04-14 14:34:37.000000 simfempy-2.2.4/simfempy/fems/rt0.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.590726 simfempy-2.2.4/simfempy/linalg/
+-rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.2.4/simfempy/linalg/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    14665 2024-04-14 16:43:13.000000 simfempy-2.2.4/simfempy/linalg/linalg.py
+-rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.2.4/simfempy/linalg/matrixsystem.py
+-rw-r--r--   0 becker     (501) staff       (20)    11014 2024-04-13 17:37:20.000000 simfempy-2.2.4/simfempy/linalg/saddle_point.py
+-rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.2.4/simfempy/linalg/vectorview.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.592707 simfempy-2.2.4/simfempy/meshes/
+-rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.2.4/simfempy/meshes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.2.4/simfempy/meshes/plotmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)    20433 2024-04-16 14:25:56.000000 simfempy-2.2.4/simfempy/meshes/simplexmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.2.4/simfempy/meshes/testmeshes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.595878 simfempy-2.2.4/simfempy/models/
+-rw-r--r--   0 becker     (501) staff       (20)       52 2024-04-14 11:36:23.000000 simfempy-2.2.4/simfempy/models/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    29397 2024-04-16 14:04:25.000000 simfempy-2.2.4/simfempy/models/elliptic.py
+-rw-r--r--   0 becker     (501) staff       (20)    29087 2024-04-16 13:36:02.000000 simfempy-2.2.4/simfempy/models/model.py
+-rw-r--r--   0 becker     (501) staff       (20)     5358 2024-04-14 15:38:59.000000 simfempy-2.2.4/simfempy/models/navierstokes.py
+-rw-r--r--   0 becker     (501) staff       (20)    10227 2024-04-14 12:02:52.000000 simfempy-2.2.4/simfempy/models/problemdata.py
+-rw-r--r--   0 becker     (501) staff       (20)    39284 2024-04-14 15:43:35.000000 simfempy-2.2.4/simfempy/models/stokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.597607 simfempy-2.2.4/simfempy/solvers/
+-rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.2.4/simfempy/solvers/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     8650 2024-04-13 22:01:19.000000 simfempy-2.2.4/simfempy/solvers/newton.py
+-rw-r--r--   0 becker     (501) staff       (20)     2454 2024-04-13 21:39:49.000000 simfempy-2.2.4/simfempy/solvers/newtondata.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.598451 simfempy-2.2.4/simfempy/tests/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.4/simfempy/tests/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.599952 simfempy-2.2.4/simfempy/tests/navierstokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-04-14 09:41:29.000000 simfempy-2.2.4/simfempy/tests/navierstokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3881 2024-04-14 15:24:05.000000 simfempy-2.2.4/simfempy/tests/navierstokes/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     4372 2024-04-13 14:20:43.000000 simfempy-2.2.4/simfempy/tests/navierstokes/incompflow.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.601280 simfempy-2.2.4/simfempy/tests/stokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.4/simfempy/tests/stokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5012 2024-04-14 11:36:23.000000 simfempy-2.2.4/simfempy/tests/stokes/stokes_analytic.py
+-rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.2.4/simfempy/tests/stokes/test_stokes.py
+-rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.2.4/simfempy/tests/testcaseanalytical.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.605416 simfempy-2.2.4/simfempy/tools/
+-rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.2.4/simfempy/tools/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.2.4/simfempy/tools/analyticalfunction.py
+-rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.2.4/simfempy/tools/barycentric.py
+-rw-r--r--   0 becker     (501) staff       (20)    14940 2024-04-15 15:48:55.000000 simfempy-2.2.4/simfempy/tools/comparemethods.py
+-rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.2.4/simfempy/tools/file_explorer.py
+-rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.2.4/simfempy/tools/iterationcounter.py
+-rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.2.4/simfempy/tools/latexwriter.py
+-rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.2.4/simfempy/tools/timer.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:27:03.606078 simfempy-2.2.4/simfempy.egg-info/
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:27:03.000000 simfempy-2.2.4/simfempy.egg-info/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     1731 2024-04-16 14:27:03.000000 simfempy-2.2.4/simfempy.egg-info/SOURCES.txt
+-rw-r--r--   0 becker     (501) staff       (20)        1 2024-04-16 14:27:03.000000 simfempy-2.2.4/simfempy.egg-info/dependency_links.txt
+-rw-r--r--   0 becker     (501) staff       (20)       47 2024-04-16 14:27:03.000000 simfempy-2.2.4/simfempy.egg-info/requires.txt
+-rw-r--r--   0 becker     (501) staff       (20)        9 2024-04-16 14:27:03.000000 simfempy-2.2.4/simfempy.egg-info/top_level.txt
```

### Comparing `simfempy-2.2.3/LICENSE` & `simfempy-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/PKG-INFO` & `simfempy-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfempy
-Version: 2.2.3
+Version: 2.2.4
 Summary: A small package for fem
 Home-page: https://github.com/beckerrh/simfempy
 Author: Roland Becker
 Author-email: beckerrolandh@gmail.com
 License: License :: OSI Approved :: MIT License
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simfempy-2.2.3/README.md` & `simfempy-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/setup.py` & `simfempy-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 from setuptools import setup, find_packages
 
-VERSION = "2.2.3"
+VERSION = "2.2.4"
 
 with open("simfempy/examples/heat_static.py", "r") as heat:
     example = heat.read()
 with open("README.md", "w") as readme:
     readme.write("SIMple Finite Element Methods in PYthon\n\n```python\n")
     readme.write(example)
     readme.write("\n```\n")
```

### Comparing `simfempy-2.2.3/simfempy/applications/application.py` & `simfempy-2.2.4/simfempy/applications/application.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/applications/navierstokes.py` & `simfempy-2.2.4/simfempy/applications/navierstokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/examples/flow_static.py` & `simfempy-2.2.4/simfempy/examples/flow_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/examples/heat_dynamic.py` & `simfempy-2.2.4/simfempy/examples/heat_dynamic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/examples/heat_static.py` & `simfempy-2.2.4/simfempy/examples/heat_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/examples/interface.py` & `simfempy-2.2.4/simfempy/examples/interface.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/cr1.py` & `simfempy-2.2.4/simfempy/fems/cr1.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/d0.py` & `simfempy-2.2.4/simfempy/fems/d0.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/data.py` & `simfempy-2.2.4/simfempy/fems/data.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/femvector.py` & `simfempy-2.2.4/simfempy/fems/femvector.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/p1.py` & `simfempy-2.2.4/simfempy/fems/p1.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/p1general.py` & `simfempy-2.2.4/simfempy/fems/p1general.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/fems/rt0.py` & `simfempy-2.2.4/simfempy/fems/rt0.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/linalg/linalg.py` & `simfempy-2.2.4/simfempy/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/linalg/matrixsystem.py` & `simfempy-2.2.4/simfempy/linalg/matrixsystem.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/linalg/saddle_point.py` & `simfempy-2.2.4/simfempy/linalg/saddle_point.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/linalg/vectorview.py` & `simfempy-2.2.4/simfempy/linalg/vectorview.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/meshes/plotmesh.py` & `simfempy-2.2.4/simfempy/meshes/plotmesh.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/meshes/simplexmesh.py` & `simfempy-2.2.4/simfempy/meshes/simplexmesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             raise ValueError(f"{len(np.unique(self.simplices))=} BUT {self.nnodes=}")
     def getBdryPoints(self, colors):
         if not isinstance(colors, (list,tuple)): colors = [colors]
         bdrypoints = []
         for color in colors:
             if not isinstance(color, int): color = self.labeldict_s2i[color]
             bdrypoints.append(self.bdrylabels[color])
-        return np.array(bdrypoints)
+        return np.array(bdrypoints).reshape(-1)
 
     def bdryFaces(self, colors=None):
         if colors is None: colors = self.bdrylabels.keys()
         pos = [0]
         for color in colors: pos.append(pos[-1]+len(self.bdrylabels[color]))
         faces = np.empty(pos[-1], dtype=np.uint32)
         for i,color in enumerate(colors): faces[pos[i]:pos[i+1]] = self.bdrylabels[color]
```

### Comparing `simfempy-2.2.3/simfempy/meshes/testmeshes.py` & `simfempy-2.2.4/simfempy/meshes/testmeshes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/models/elliptic.py` & `simfempy-2.2.4/simfempy/models/elliptic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/models/model.py` & `simfempy-2.2.4/simfempy/models/model.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/models/navierstokes.py` & `simfempy-2.2.4/simfempy/models/navierstokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/models/problemdata.py` & `simfempy-2.2.4/simfempy/models/problemdata.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/models/stokes.py` & `simfempy-2.2.4/simfempy/models/stokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/solvers/newton.py` & `simfempy-2.2.4/simfempy/solvers/newton.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/solvers/newtondata.py` & `simfempy-2.2.4/simfempy/solvers/newtondata.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tests/navierstokes/flow_static.py` & `simfempy-2.2.4/simfempy/tests/navierstokes/flow_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tests/navierstokes/incompflow.py` & `simfempy-2.2.4/simfempy/tests/navierstokes/incompflow.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tests/stokes/stokes_analytic.py` & `simfempy-2.2.4/simfempy/tests/stokes/stokes_analytic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tests/stokes/test_stokes.py` & `simfempy-2.2.4/simfempy/tests/stokes/test_stokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tests/testcaseanalytical.py` & `simfempy-2.2.4/simfempy/tests/testcaseanalytical.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/analyticalfunction.py` & `simfempy-2.2.4/simfempy/tools/analyticalfunction.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/barycentric.py` & `simfempy-2.2.4/simfempy/tools/barycentric.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/comparemethods.py` & `simfempy-2.2.4/simfempy/tools/comparemethods.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/file_explorer.py` & `simfempy-2.2.4/simfempy/tools/file_explorer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/iterationcounter.py` & `simfempy-2.2.4/simfempy/tools/iterationcounter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/latexwriter.py` & `simfempy-2.2.4/simfempy/tools/latexwriter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy/tools/timer.py` & `simfempy-2.2.4/simfempy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.3/simfempy.egg-info/PKG-INFO` & `simfempy-2.2.4/simfempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfempy
-Version: 2.2.3
+Version: 2.2.4
 Summary: A small package for fem
 Home-page: https://github.com/beckerrh/simfempy
 Author: Roland Becker
 Author-email: beckerrolandh@gmail.com
 License: License :: OSI Approved :: MIT License
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simfempy-2.2.3/simfempy.egg-info/SOURCES.txt` & `simfempy-2.2.4/simfempy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

