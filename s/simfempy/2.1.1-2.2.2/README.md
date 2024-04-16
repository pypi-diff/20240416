# Comparing `tmp/simfempy-2.1.1.tar.gz` & `tmp/simfempy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfempy-2.1.1.tar", last modified: Tue Mar  5 17:08:55 2024, max compression
+gzip compressed data, was "simfempy-2.2.2.tar", last modified: Tue Apr 16 13:37:24 2024, max compression
```

## Comparing `simfempy-2.1.1.tar` & `simfempy-2.2.2.tar`

### file list

```diff
@@ -1,68 +1,75 @@
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.862179 simfempy-2.1.1/
--rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.1.1/LICENSE
--rw-r--r--   0 becker     (501) staff       (20)     3630 2024-03-05 17:08:55.861673 simfempy-2.1.1/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     2923 2024-03-05 17:08:55.000000 simfempy-2.1.1/README.md
--rw-r--r--   0 becker     (501) staff       (20)       38 2024-03-05 17:08:55.862338 simfempy-2.1.1/setup.cfg
--rw-r--r--   0 becker     (501) staff       (20)     1291 2024-03-05 17:06:16.000000 simfempy-2.1.1/setup.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.812759 simfempy-2.1.1/simfempy/
--rw-r--r--   0 becker     (501) staff       (20)      139 2023-04-15 10:39:45.000000 simfempy-2.1.1/simfempy/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.819939 simfempy-2.1.1/simfempy/examples/
--rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.1.1/simfempy/examples/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     3353 2024-03-01 13:08:04.000000 simfempy-2.1.1/simfempy/examples/heat_dynamic.py
--rw-r--r--   0 becker     (501) staff       (20)     2867 2024-03-01 20:05:36.000000 simfempy-2.1.1/simfempy/examples/heat_static.py
--rw-r--r--   0 becker     (501) staff       (20)     4368 2024-02-14 13:17:36.000000 simfempy-2.1.1/simfempy/examples/incompflow.py
--rw-r--r--   0 becker     (501) staff       (20)     3984 2024-03-04 18:58:03.000000 simfempy-2.1.1/simfempy/examples/interface.py
--rw-r--r--   0 becker     (501) staff       (20)    15261 2024-02-14 11:45:06.000000 simfempy-2.1.1/simfempy/examples/navier_stokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.827672 simfempy-2.1.1/simfempy/fems/
--rw-r--r--   0 becker     (501) staff       (20)       37 2024-02-14 13:27:20.000000 simfempy-2.1.1/simfempy/fems/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    38795 2024-02-18 13:26:53.000000 simfempy-2.1.1/simfempy/fems/cr1.py
--rw-r--r--   0 becker     (501) staff       (20)     2706 2024-02-11 15:15:59.000000 simfempy-2.1.1/simfempy/fems/d0.py
--rw-r--r--   0 becker     (501) staff       (20)      658 2022-03-09 17:02:11.000000 simfempy-2.1.1/simfempy/fems/data.py
--rw-r--r--   0 becker     (501) staff       (20)    29546 2024-02-18 13:26:53.000000 simfempy-2.1.1/simfempy/fems/p1.py
--rw-r--r--   0 becker     (501) staff       (20)     3156 2024-02-10 17:29:33.000000 simfempy-2.1.1/simfempy/fems/p1general.py
--rw-r--r--   0 becker     (501) staff       (20)    16280 2024-02-10 17:30:04.000000 simfempy-2.1.1/simfempy/fems/rt0.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.832709 simfempy-2.1.1/simfempy/linalg/
--rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.1.1/simfempy/linalg/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    14161 2024-03-03 16:02:08.000000 simfempy-2.1.1/simfempy/linalg/linalg.py
--rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.1.1/simfempy/linalg/matrixsystem.py
--rw-r--r--   0 becker     (501) staff       (20)    10899 2024-03-01 19:42:30.000000 simfempy-2.1.1/simfempy/linalg/saddle_point.py
--rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.1.1/simfempy/linalg/vectorview.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.837675 simfempy-2.1.1/simfempy/meshes/
--rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.1.1/simfempy/meshes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.1.1/simfempy/meshes/plotmesh.py
--rw-r--r--   0 becker     (501) staff       (20)    20440 2024-03-04 18:57:02.000000 simfempy-2.1.1/simfempy/meshes/simplexmesh.py
--rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.1.1/simfempy/meshes/testmeshes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.845945 simfempy-2.1.1/simfempy/models/
--rw-r--r--   0 becker     (501) staff       (20)       55 2023-05-13 13:38:12.000000 simfempy-2.1.1/simfempy/models/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     4256 2024-03-03 15:47:24.000000 simfempy-2.1.1/simfempy/models/application.py
--rw-r--r--   0 becker     (501) staff       (20)    28710 2024-03-03 11:38:38.000000 simfempy-2.1.1/simfempy/models/elliptic.py
--rw-r--r--   0 becker     (501) staff       (20)    29642 2024-03-03 15:49:11.000000 simfempy-2.1.1/simfempy/models/model.py
--rw-r--r--   0 becker     (501) staff       (20)     4812 2024-02-10 17:30:04.000000 simfempy-2.1.1/simfempy/models/navierstokes.py
--rw-r--r--   0 becker     (501) staff       (20)    10204 2024-03-02 13:14:26.000000 simfempy-2.1.1/simfempy/models/problemdata.py
--rw-r--r--   0 becker     (501) staff       (20)    38772 2024-03-02 13:18:37.000000 simfempy-2.1.1/simfempy/models/stokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.849582 simfempy-2.1.1/simfempy/solvers/
--rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.1.1/simfempy/solvers/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     8377 2024-03-03 15:47:24.000000 simfempy-2.1.1/simfempy/solvers/newton.py
--rw-r--r--   0 becker     (501) staff       (20)     2453 2024-03-03 14:16:45.000000 simfempy-2.1.1/simfempy/solvers/newtondata.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.851081 simfempy-2.1.1/simfempy/tests/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.1.1/simfempy/tests/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.853386 simfempy-2.1.1/simfempy/tests/stokes/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.1.1/simfempy/tests/stokes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5000 2024-03-02 13:34:00.000000 simfempy-2.1.1/simfempy/tests/stokes/stokes_analytic.py
--rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.1.1/simfempy/tests/stokes/test_stokes.py
--rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.1.1/simfempy/tests/testcaseanalytical.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.860191 simfempy-2.1.1/simfempy/tools/
--rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.1.1/simfempy/tools/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.1.1/simfempy/tools/analyticalfunction.py
--rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.1.1/simfempy/tools/barycentric.py
--rw-r--r--   0 becker     (501) staff       (20)    14825 2024-03-03 13:37:30.000000 simfempy-2.1.1/simfempy/tools/comparemethods.py
--rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.1.1/simfempy/tools/file_explorer.py
--rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.1.1/simfempy/tools/iterationcounter.py
--rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.1.1/simfempy/tools/latexwriter.py
--rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.1.1/simfempy/tools/timer.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-03-05 17:08:55.861028 simfempy-2.1.1/simfempy.egg-info/
--rw-r--r--   0 becker     (501) staff       (20)     3630 2024-03-05 17:08:55.000000 simfempy-2.1.1/simfempy.egg-info/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     1535 2024-03-05 17:08:55.000000 simfempy-2.1.1/simfempy.egg-info/SOURCES.txt
--rw-r--r--   0 becker     (501) staff       (20)        1 2024-03-05 17:08:55.000000 simfempy-2.1.1/simfempy.egg-info/dependency_links.txt
--rw-r--r--   0 becker     (501) staff       (20)       36 2024-03-05 17:08:55.000000 simfempy-2.1.1/simfempy.egg-info/requires.txt
--rw-r--r--   0 becker     (501) staff       (20)        9 2024-03-05 17:08:55.000000 simfempy-2.1.1/simfempy.egg-info/top_level.txt
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.747329 simfempy-2.2.2/
+-rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.2.2/LICENSE
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 13:37:24.746742 simfempy-2.2.2/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     2679 2024-04-16 13:37:24.000000 simfempy-2.2.2/README.md
+-rw-r--r--   0 becker     (501) staff       (20)       38 2024-04-16 13:37:24.747452 simfempy-2.2.2/setup.cfg
+-rw-r--r--   0 becker     (501) staff       (20)     1332 2024-04-16 13:36:33.000000 simfempy-2.2.2/setup.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.695540 simfempy-2.2.2/simfempy/
+-rw-r--r--   0 becker     (501) staff       (20)      153 2024-04-13 14:16:18.000000 simfempy-2.2.2/simfempy/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.700636 simfempy-2.2.2/simfempy/applications/
+-rw-r--r--   0 becker     (501) staff       (20)       40 2024-04-14 11:38:13.000000 simfempy-2.2.2/simfempy/applications/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     4907 2024-04-15 15:48:55.000000 simfempy-2.2.2/simfempy/applications/application.py
+-rw-r--r--   0 becker     (501) staff       (20)    15260 2024-04-14 11:38:49.000000 simfempy-2.2.2/simfempy/applications/navierstokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.703729 simfempy-2.2.2/simfempy/examples/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.2.2/simfempy/examples/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3266 2024-04-16 13:17:35.000000 simfempy-2.2.2/simfempy/examples/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3048 2024-04-14 11:36:23.000000 simfempy-2.2.2/simfempy/examples/heat_dynamic.py
+-rw-r--r--   0 becker     (501) staff       (20)     2623 2024-04-14 16:50:50.000000 simfempy-2.2.2/simfempy/examples/heat_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3950 2024-04-14 11:36:23.000000 simfempy-2.2.2/simfempy/examples/interface.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.712480 simfempy-2.2.2/simfempy/fems/
+-rw-r--r--   0 becker     (501) staff       (20)       48 2024-04-14 08:58:57.000000 simfempy-2.2.2/simfempy/fems/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    27607 2024-04-16 13:11:08.000000 simfempy-2.2.2/simfempy/fems/cr1.py
+-rw-r--r--   0 becker     (501) staff       (20)     2740 2024-04-14 11:13:29.000000 simfempy-2.2.2/simfempy/fems/d0.py
+-rw-r--r--   0 becker     (501) staff       (20)      819 2024-04-14 14:58:27.000000 simfempy-2.2.2/simfempy/fems/data.py
+-rw-r--r--   0 becker     (501) staff       (20)     2707 2024-04-14 14:40:31.000000 simfempy-2.2.2/simfempy/fems/femvector.py
+-rw-r--r--   0 becker     (501) staff       (20)    29792 2024-04-16 12:20:49.000000 simfempy-2.2.2/simfempy/fems/p1.py
+-rw-r--r--   0 becker     (501) staff       (20)     7757 2024-04-16 12:56:57.000000 simfempy-2.2.2/simfempy/fems/p1general.py
+-rw-r--r--   0 becker     (501) staff       (20)    16154 2024-04-14 14:34:37.000000 simfempy-2.2.2/simfempy/fems/rt0.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.717408 simfempy-2.2.2/simfempy/linalg/
+-rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.2.2/simfempy/linalg/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    14665 2024-04-14 16:43:13.000000 simfempy-2.2.2/simfempy/linalg/linalg.py
+-rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.2.2/simfempy/linalg/matrixsystem.py
+-rw-r--r--   0 becker     (501) staff       (20)    11014 2024-04-13 17:37:20.000000 simfempy-2.2.2/simfempy/linalg/saddle_point.py
+-rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.2.2/simfempy/linalg/vectorview.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.721846 simfempy-2.2.2/simfempy/meshes/
+-rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.2.2/simfempy/meshes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.2.2/simfempy/meshes/plotmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)    21709 2024-04-14 09:50:54.000000 simfempy-2.2.2/simfempy/meshes/simplexmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.2.2/simfempy/meshes/testmeshes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.727621 simfempy-2.2.2/simfempy/models/
+-rw-r--r--   0 becker     (501) staff       (20)       52 2024-04-14 11:36:23.000000 simfempy-2.2.2/simfempy/models/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    29395 2024-04-16 13:16:00.000000 simfempy-2.2.2/simfempy/models/elliptic.py
+-rw-r--r--   0 becker     (501) staff       (20)    29087 2024-04-16 13:36:02.000000 simfempy-2.2.2/simfempy/models/model.py
+-rw-r--r--   0 becker     (501) staff       (20)     5358 2024-04-14 15:38:59.000000 simfempy-2.2.2/simfempy/models/navierstokes.py
+-rw-r--r--   0 becker     (501) staff       (20)    10227 2024-04-14 12:02:52.000000 simfempy-2.2.2/simfempy/models/problemdata.py
+-rw-r--r--   0 becker     (501) staff       (20)    39284 2024-04-14 15:43:35.000000 simfempy-2.2.2/simfempy/models/stokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.731689 simfempy-2.2.2/simfempy/solvers/
+-rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.2.2/simfempy/solvers/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     8650 2024-04-13 22:01:19.000000 simfempy-2.2.2/simfempy/solvers/newton.py
+-rw-r--r--   0 becker     (501) staff       (20)     2454 2024-04-13 21:39:49.000000 simfempy-2.2.2/simfempy/solvers/newtondata.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.733175 simfempy-2.2.2/simfempy/tests/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.2/simfempy/tests/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.735705 simfempy-2.2.2/simfempy/tests/navierstokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-04-14 09:41:29.000000 simfempy-2.2.2/simfempy/tests/navierstokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3881 2024-04-14 15:24:05.000000 simfempy-2.2.2/simfempy/tests/navierstokes/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     4372 2024-04-13 14:20:43.000000 simfempy-2.2.2/simfempy/tests/navierstokes/incompflow.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.737886 simfempy-2.2.2/simfempy/tests/stokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.2/simfempy/tests/stokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5012 2024-04-14 11:36:23.000000 simfempy-2.2.2/simfempy/tests/stokes/stokes_analytic.py
+-rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.2.2/simfempy/tests/stokes/test_stokes.py
+-rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.2.2/simfempy/tests/testcaseanalytical.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.745191 simfempy-2.2.2/simfempy/tools/
+-rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.2.2/simfempy/tools/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.2.2/simfempy/tools/analyticalfunction.py
+-rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.2.2/simfempy/tools/barycentric.py
+-rw-r--r--   0 becker     (501) staff       (20)    14940 2024-04-15 15:48:55.000000 simfempy-2.2.2/simfempy/tools/comparemethods.py
+-rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.2.2/simfempy/tools/file_explorer.py
+-rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.2.2/simfempy/tools/iterationcounter.py
+-rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.2.2/simfempy/tools/latexwriter.py
+-rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.2.2/simfempy/tools/timer.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 13:37:24.746025 simfempy-2.2.2/simfempy.egg-info/
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 13:37:24.000000 simfempy-2.2.2/simfempy.egg-info/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     1731 2024-04-16 13:37:24.000000 simfempy-2.2.2/simfempy.egg-info/SOURCES.txt
+-rw-r--r--   0 becker     (501) staff       (20)        1 2024-04-16 13:37:24.000000 simfempy-2.2.2/simfempy.egg-info/dependency_links.txt
+-rw-r--r--   0 becker     (501) staff       (20)       47 2024-04-16 13:37:24.000000 simfempy-2.2.2/simfempy.egg-info/requires.txt
+-rw-r--r--   0 becker     (501) staff       (20)        9 2024-04-16 13:37:24.000000 simfempy-2.2.2/simfempy.egg-info/top_level.txt
```

### Comparing `simfempy-2.1.1/LICENSE` & `simfempy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/PKG-INFO` & `simfempy-2.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfempy
-Version: 2.1.1
+Version: 2.2.2
 Summary: A small package for fem
 Home-page: https://github.com/beckerrh/simfempy
 Author: Roland Becker
 Author-email: beckerrolandh@gmail.com
 License: License :: OSI Approved :: MIT License
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -16,67 +16,66 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygmsh
 Requires-Dist: pyamg
 Requires-Dist: scipy
 Requires-Dist: sympy
 Requires-Dist: matplotlib
+Requires-Dist: setuptools
 
 SIMple Finite Element Methods in PYthon
 
 ```python
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import pathlib, sys
 simfempypath = str(pathlib.Path(__file__).parent.parent.parent)
 sys.path.insert(0,simfempypath)
 
 from simfempy.models.elliptic import Elliptic
-from simfempy.models.application import Application
-from simfempy.meshes import plotmesh
+from simfempy.applications.application import Application
 
-# define Application class
+#--------------------------------------------------------------
 class HeatExample(Application):
-    def __init__(self):
-        super().__init__(h=0.1)
-        # fill problem data
+    # nomen est omen
+    def defineProblemData(self, problemdata):
         # boundary conditions
-        self.problemdata.bdrycond.set("Dirichlet", [1000, 3000])
-        self.problemdata.bdrycond.set("Neumann", [1001, 1002, 1003])
-        self.problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
-        self.problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
+        problemdata.bdrycond.set(type="Dirichlet", colors=[1000, 3000])
+        problemdata.bdrycond.set(type="Neumann", colors=[1001, 1002, 1003])
+        problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
+        problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
         # postprocess
-        self.problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
-        self.problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
-        self.problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
-        self.problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
+        problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
+        problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
+        problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
+        problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
         # paramaters in equation
-        self.problemdata.params.set_scal_cells("kheat", [100], 0.001)
-        self.problemdata.params.set_scal_cells("kheat", [200], 10.0)
-        # data.params.fct_glob["convection"] = ["0", "0.001"]
+        problemdata.params.set_scal_cells("kheat", [100], 0.001)
+        problemdata.params.set_scal_cells("kheat", [200], 10.0)
+    # nomen est omen
     def defineGeometry(self, geom, h):
+        h=0.2
         holes = []
         rectangle = geom.add_rectangle(xmin=-1.5, xmax=-0.5, ymin=-1.5, ymax=-0.5, z=0, mesh_size=h)
         geom.add_physical(rectangle.surface, label="200")
         geom.add_physical(rectangle.lines, label="20")  # required for correct boundary labels (!?)
         holes.append(rectangle)
         circle = geom.add_circle(x0=[0, 0], radius=0.5, mesh_size=h, num_sections=6, make_surface=False)
         geom.add_physical(circle.curve_loop.curves, label="3000")
         holes.append(circle)
         p = geom.add_rectangle(xmin=-2, xmax=2, ymin=-2, ymax=2, z=0, mesh_size=h, holes=holes)
         geom.add_physical(p.surface, label="100")
         for i in range(len(p.lines)): geom.add_physical(p.lines[i], label=f"{1000 + i}")
 
-disc_params={'dirichletmethod':'nitsche'}
-heat = Elliptic(application=HeatExample(), fem='p1', disc_params=disc_params, linearsolver={'method':'pyamg', 'disp':0, 'smoother':'schwarz'})
-result, u = heat.static(mode="newton")
+#--------------------------------------------------------------
+heat = Elliptic(application=HeatExample(), fem='cr1')
+result, u = heat.static()
 print(f"{result=}")
-# for p, v in result.data['scalar'].items(): print(f"{p}: {v}")
 fig = plt.figure(figsize=(10, 8))
 fig.suptitle(f"{heat.application.__class__.__name__} (static)", fontsize=16)
 outer = gridspec.GridSpec(1, 2, wspace=0.2, hspace=0.2)
-plotmesh.meshWithBoundaries(heat.mesh, fig=fig, outer=outer[0])
-data = heat.sol_to_data(u)
+heat.mesh.plot(fig=fig, outer=outer[0], bdry=True)
+data = u.tovisudata()
 data.update({'cell': {'k': heat.kheatcell}})
-plotmesh.meshWithData(heat.mesh, data=data, alpha=0.5, fig=fig, outer=outer[1])
+heat.mesh.plot(data=data, alpha=0.5, fig=fig, outer=outer[1])
 plt.show()
 ```
```

### Comparing `simfempy-2.1.1/README.md` & `simfempy-2.2.2/simfempy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,81 @@
+Metadata-Version: 2.1
+Name: simfempy
+Version: 2.2.2
+Summary: A small package for fem
+Home-page: https://github.com/beckerrh/simfempy
+Author: Roland Becker
+Author-email: beckerrolandh@gmail.com
+License: License :: OSI Approved :: MIT License
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pygmsh
+Requires-Dist: pyamg
+Requires-Dist: scipy
+Requires-Dist: sympy
+Requires-Dist: matplotlib
+Requires-Dist: setuptools
+
 SIMple Finite Element Methods in PYthon
 
 ```python
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import pathlib, sys
 simfempypath = str(pathlib.Path(__file__).parent.parent.parent)
 sys.path.insert(0,simfempypath)
 
 from simfempy.models.elliptic import Elliptic
-from simfempy.models.application import Application
-from simfempy.meshes import plotmesh
+from simfempy.applications.application import Application
 
-# define Application class
+#--------------------------------------------------------------
 class HeatExample(Application):
-    def __init__(self):
-        super().__init__(h=0.1)
-        # fill problem data
+    # nomen est omen
+    def defineProblemData(self, problemdata):
         # boundary conditions
-        self.problemdata.bdrycond.set("Dirichlet", [1000, 3000])
-        self.problemdata.bdrycond.set("Neumann", [1001, 1002, 1003])
-        self.problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
-        self.problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
+        problemdata.bdrycond.set(type="Dirichlet", colors=[1000, 3000])
+        problemdata.bdrycond.set(type="Neumann", colors=[1001, 1002, 1003])
+        problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
+        problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
         # postprocess
-        self.problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
-        self.problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
-        self.problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
-        self.problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
+        problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
+        problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
+        problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
+        problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
         # paramaters in equation
-        self.problemdata.params.set_scal_cells("kheat", [100], 0.001)
-        self.problemdata.params.set_scal_cells("kheat", [200], 10.0)
-        # data.params.fct_glob["convection"] = ["0", "0.001"]
+        problemdata.params.set_scal_cells("kheat", [100], 0.001)
+        problemdata.params.set_scal_cells("kheat", [200], 10.0)
+    # nomen est omen
     def defineGeometry(self, geom, h):
+        h=0.2
         holes = []
         rectangle = geom.add_rectangle(xmin=-1.5, xmax=-0.5, ymin=-1.5, ymax=-0.5, z=0, mesh_size=h)
         geom.add_physical(rectangle.surface, label="200")
         geom.add_physical(rectangle.lines, label="20")  # required for correct boundary labels (!?)
         holes.append(rectangle)
         circle = geom.add_circle(x0=[0, 0], radius=0.5, mesh_size=h, num_sections=6, make_surface=False)
         geom.add_physical(circle.curve_loop.curves, label="3000")
         holes.append(circle)
         p = geom.add_rectangle(xmin=-2, xmax=2, ymin=-2, ymax=2, z=0, mesh_size=h, holes=holes)
         geom.add_physical(p.surface, label="100")
         for i in range(len(p.lines)): geom.add_physical(p.lines[i], label=f"{1000 + i}")
 
-disc_params={'dirichletmethod':'nitsche'}
-heat = Elliptic(application=HeatExample(), fem='p1', disc_params=disc_params, linearsolver={'method':'pyamg', 'disp':0, 'smoother':'schwarz'})
-result, u = heat.static(mode="newton")
+#--------------------------------------------------------------
+heat = Elliptic(application=HeatExample(), fem='cr1')
+result, u = heat.static()
 print(f"{result=}")
-# for p, v in result.data['scalar'].items(): print(f"{p}: {v}")
 fig = plt.figure(figsize=(10, 8))
 fig.suptitle(f"{heat.application.__class__.__name__} (static)", fontsize=16)
 outer = gridspec.GridSpec(1, 2, wspace=0.2, hspace=0.2)
-plotmesh.meshWithBoundaries(heat.mesh, fig=fig, outer=outer[0])
-data = heat.sol_to_data(u)
+heat.mesh.plot(fig=fig, outer=outer[0], bdry=True)
+data = u.tovisudata()
 data.update({'cell': {'k': heat.kheatcell}})
-plotmesh.meshWithData(heat.mesh, data=data, alpha=0.5, fig=fig, outer=outer[1])
+heat.mesh.plot(data=data, alpha=0.5, fig=fig, outer=outer[1])
 plt.show()
 ```
```

### Comparing `simfempy-2.1.1/setup.py` & `simfempy-2.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 from setuptools import setup, find_packages
 
-VERSION = "2.1.1"
+VERSION = "2.2.2"
 
 with open("simfempy/examples/heat_static.py", "r") as heat:
     example = heat.read()
 with open("README.md", "w") as readme:
     readme.write("SIMple Finite Element Methods in PYthon\n\n```python\n")
     readme.write(example)
     readme.write("\n```\n")
@@ -21,15 +21,16 @@
     url="https://github.com/beckerrh/simfempy",
     license="License :: OSI Approved :: MIT License",
     description="A small package for fem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms="any",
     # install_requires=['gmsh', 'pygmsh', 'meshio', 'scipy', 'sympy', 'matplotlib'],
-    install_requires=['pygmsh', 'pyamg', 'scipy', 'sympy', 'matplotlib'],
+    # setuptools for pyamg
+    install_requires=['pygmsh', 'pyamg', 'scipy', 'sympy', 'matplotlib', 'setuptools'],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Mathematics",
     ],
```

### Comparing `simfempy-2.1.1/simfempy/examples/heat_dynamic.py` & `simfempy-2.2.2/simfempy/examples/heat_dynamic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 import matplotlib.pyplot as plt
-import matplotlib.gridspec as gridspec
-import pygmsh
 # in shell
 import os, sys
 simfempypath = os.path.abspath(os.path.join(__file__, os.path.pardir, os.path.pardir, os.path.pardir, os.path.pardir,'simfempy'))
 sys.path.insert(0,simfempypath)
 
 from simfempy.models.elliptic import Elliptic
-from simfempy.models.application import Application
-from simfempy.models.problemdata import ProblemData
-from simfempy.meshes.simplexmesh import SimplexMesh
-from simfempy.meshes import plotmesh
+from simfempy.applications.application import Application
+
 
 # define Application class
 class HeatExample(Application):
-    def __init__(self):
-        super().__init__(h=0.1)
-        # fill problem data
-        # boundary conditions
-        self.problemdata.bdrycond.set("Dirichlet", [1000, 3000])
-        self.problemdata.bdrycond.set("Neumann", [1001, 1002, 1003])
-        self.problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
-        self.problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
+    def defineProblemData(self, problemdata):
+        problemdata.bdrycond.set("Dirichlet", [1000, 3000])
+        problemdata.bdrycond.set("Neumann", [1001, 1002, 1003])
+        problemdata.bdrycond.fct[1000] = lambda x, y, z: 200
+        problemdata.bdrycond.fct[3000] = lambda x, y, z: 320
         # postprocess
-        self.problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
-        self.problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
-        self.problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
-        self.problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
+        problemdata.postproc.set(name='bdrymean_right', type='bdry_mean', colors=1001)
+        problemdata.postproc.set(name='bdrymean_left', type='bdry_mean', colors=1003)
+        problemdata.postproc.set(name='bdrymean_up', type='bdry_mean', colors=1002)
+        problemdata.postproc.set(name='bdrynflux', type='bdry_nflux', colors=[3000])
         # paramaters in equation
-        self.problemdata.params.set_scal_cells("kheat", [100], 0.001)
-        self.problemdata.params.set_scal_cells("kheat", [200], 10.0)
+        problemdata.params.set_scal_cells("kheat", [100], 0.001)
+        problemdata.params.set_scal_cells("kheat", [200], 10.0)
         # data.params.fct_glob["convection"] = ["0", "0.001"]
     def defineGeometry(self, geom, h):
         holes = []
         rectangle = geom.add_rectangle(xmin=-1.5, xmax=-0.5, ymin=-1.5, ymax=-0.5, z=0, mesh_size=h)
         geom.add_physical(rectangle.surface, label="200")
         geom.add_physical(rectangle.lines, label="20")  # required for correct boundary labels (!?)
         holes.append(rectangle)
```

### Comparing `simfempy-2.1.1/simfempy/examples/incompflow.py` & `simfempy-2.2.2/simfempy/tests/navierstokes/incompflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import matplotlib.pyplot as plt
 import pathlib, sys
 simfempypath = str(pathlib.Path(__file__).parent.parent.parent)
 sys.path.insert(0,simfempypath)
 from simfempy.models.navierstokes import NavierStokes
 from simfempy.models.stokes import Stokes
-from simfempy.examples import navier_stokes
+from simfempy.applications import navierstokes
+
 
 # ================================================================c#
 def getModel(**kwargs):
     disc_params = kwargs.pop('disc_params', {})
     application = kwargs.pop('application', {})
     model = kwargs.pop('model', 'NavierStokes')
     if model == "Stokes":
```

### Comparing `simfempy-2.1.1/simfempy/examples/interface.py` & `simfempy-2.2.2/simfempy/examples/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pathlib, sys
 simfempypath = str(pathlib.Path(__file__).parent.parent.parent)
 sys.path.insert(0,simfempypath)
 
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from matplotlib import cm
-from mpl_toolkits.mplot3d import axes3d
 import numpy as np
 from simfempy.models.elliptic import Elliptic
-from simfempy.models.application import Application
+from simfempy.applications.application import Application
 from simfempy.meshes import plotmesh
 from simfempy.tools.comparemethods import CompareMethods
 
 class InterfaceAnalyticalSolution(Application):
     def __init__(self, h=0.1):
         self.k1, self.k2, self.r02 = 1, 100, 0.75**2
         self.u = self.ExactSolution(self)
```

### Comparing `simfempy-2.1.1/simfempy/examples/navier_stokes.py` & `simfempy-2.2.2/simfempy/applications/navierstokes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
-import simfempy.models.application
+from . import  application
 
 # ================================================================ #
-class Application(simfempy.models.application.Application):
-    def __init__(self, ncomp=2, h=None, mu=0.1):
-        super().__init__(ncomp=ncomp, h=h, scal_glob={'mu':mu})
+class Application(application.Application):
+    def __init__(self, h=None, **kwargs):
+        if 'mu' in kwargs: scal_glob={'mu':kwargs.pop('mu')}
+        else: scal_glob={}
+        super().__init__(h=h, scal_glob=scal_glob)
     def plot(self, mesh, data, **kwargs):
         import matplotlib.pyplot as plt
         fig = kwargs.pop('fig', None)
         gs = kwargs.pop('gs', None)
         if fig is None:
             if gs is not None:
                 raise ValueError(f"got gs but no fig")
@@ -27,15 +29,15 @@
         import matplotlib.pyplot as plt
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         import matplotlib.gridspec as gridspec
         nplots = 4
         inner = gridspec.GridSpecFromSubplotSpec(nrows=nplots, ncols=1, subplot_spec=gs, wspace=0.3, hspace=0.3)
         x, y, tris = mesh.points[:, 0], mesh.points[:, 1], mesh.simplices
         iplot = 0
-        p = data['cell']['P']
+        p = data['cell']['p']
         ax = fig.add_subplot(inner[iplot])
         ax.get_xaxis().set_visible(False)
         ax.get_yaxis().set_visible(False)
         ax.triplot(x, y, tris, color='gray', lw=1, alpha=0.1)
         cnt = ax.tripcolor(x, y, tris, facecolors=p, edgecolors='k', cmap='jet')
         divider = make_axes_locatable(ax)
         cax = divider.append_axes('right', size='3%', pad=0.4)
@@ -49,15 +51,15 @@
             ax.triplot(x, y, tris, color='gray', lw=1, alpha=0.3)
             cnt = ax.tricontourf(x, y, tris, values, levels=16, cmap='jet', alpha=1.)
             divider = make_axes_locatable(ax)
             cax = divider.append_axes('right', size='3%', pad=0.4)
             clb = plt.colorbar(cnt, cax=cax, orientation='vertical')
             clb.ax.set_title(name)
             iplot += 1
-        v0,v1 = data['point']['V_0'], data['point']['V_1']
+        v0,v1 = data['point']['v_1'], data['point']['v_2']
         ax = fig.add_subplot(inner[iplot])
         ax.get_xaxis().set_visible(False)
         ax.get_yaxis().set_visible(False)
         ax.triplot(x, y, tris, color='gray', lw=1, alpha=0.1)
         qv = ax.quiver(x, y, v0, v1, units='xy')
     def plot3d(self, mesh, data, fig, gs, **kwargs):
         try:
@@ -67,19 +69,19 @@
             celltypes = pyvista.CellType.TETRA * np.ones(ntets, dtype=int)
             cells = np.insert(tets, 0, 4, axis=1).ravel()
             pyvistamesh = pyvista.UnstructuredGrid(cells, celltypes, mesh.points)
             import matplotlib.pyplot as plt
             import matplotlib.gridspec as gridspec
             inner = gridspec.GridSpecFromSubplotSpec(nrows=2, ncols=2, subplot_spec=gs, wspace=0.3, hspace=0.3)
             alpha = kwargs.pop('alpha', 0.6)
-            p = data['cell']['P']
+            p = data['cell']['p']
             v = np.zeros(shape=(mesh.nnodes, 3))
-            v[:,0] = data['point']['V_0']
-            v[:,1] = data['point']['V_1']
-            v[:,2] = data['point']['V_2']
+            v[:,0] = data['point']['v_0']
+            v[:,1] = data['point']['v_1']
+            v[:,2] = data['point']['v_2']
             vnorm = np.linalg.norm(v, axis=1)
             pyvistamesh["V"] = v
             pyvistamesh["vn"] = vnorm
             pyvistamesh.cell_data['P'] = p
             plotter = pyvista.Plotter(off_screen=kwargs.pop('off_screen',True))
             plotter.renderer.SetBackground(255, 255, 255)
             plotter.add_mesh(pyvistamesh, opacity=alpha, color='gray', show_edges=True)
@@ -129,15 +131,15 @@
     def defineGeometry(self, geom, h):
         p = geom.add_rectangle(xmin=0, xmax=4, ymin=0, ymax=1, z=0, mesh_size=h)
         geom.add_physical(p.surface, label="100")
         for i in range(len(p.lines)): geom.add_physical(p.lines[i], label=f"{1000 + i}")
 # ================================================================ #
 class Poiseuille3d(Application):
     def __init__(self, mu=0.01, h=0.5):
-        super().__init__(mu=mu, h=h, ncomp=3)
+        super().__init__(mu=mu, h=h)
         data = self.problemdata
         # boundary conditions
         data.bdrycond.set("Dirichlet", [100, 103])
         data.bdrycond.set("Neumann", [101])
         data.bdrycond.fct[103] = [lambda x, y, z: 16 * y * (1 - y) * z * (1 - z), lambda x, y, z: 0, lambda x, y, z: 0]
     def defineGeometry(self, geom, h):
         p = geom.add_rectangle(xmin=0, xmax=4, ymin=0, ymax=1, z=0, mesh_size=h)
@@ -146,15 +148,15 @@
         geom.add_physical([top, p.surface, lat[0], lat[2]], label="100")
         geom.add_physical(lat[1], label="101")
         geom.add_physical(lat[3], label="103")
         geom.add_physical(vol, label="10")
 # ================================================================ #
 class DrivenCavity2d(Application):
     def __init__(self, h=0.1, mu=0.003):
-        super().__init__(mu=mu, h=h, ncomp=2)
+        super().__init__(mu=mu, h=h)
         data = self.problemdata
         # boundary conditions
         data.bdrycond.set("Dirichlet", [1000, 1002])
         data.bdrycond.fct[1002] = [lambda x, y, z: 1, lambda x, y, z: 0]
         # parameters
         data.params.scal_glob["mu"] = mu
     #
@@ -163,15 +165,15 @@
         p = geom.add_rectangle(xmin=0, xmax=1, ymin=0, ymax=1, z=0, mesh_size=ms)
         geom.add_physical(p.surface, label="100")
         geom.add_physical(p.lines[2], label="1002")
         geom.add_physical([p.lines[0], p.lines[1], p.lines[3]], label="1000")
 # ================================================================ #
 class DrivenCavity3d(Application):
     def __init__(self, h=0.1, mu=0.003):
-        super().__init__(mu=mu, h=h, ncomp=3)
+        super().__init__(mu=mu, h=h)
         data = self.problemdata
         data.bdrycond.set("Dirichlet", [100, 102])
         data.bdrycond.fct[102] = [lambda x, y, z: 1, lambda x, y, z: 0, lambda x, y, z: 0]
         # parameters
         data.params.scal_glob["mu"] = mu
     def defineGeometry(self, geom, h):
         ms = [h*v for v in [1.,1.,0.1,0.1]]
@@ -206,15 +208,15 @@
         dirlines = [p for i,p in enumerate(p.lines) if i != 0 and i != 4]
         geom.add_physical(dirlines, "1002")
         geom.add_physical(p.lines[0], "1000")
         geom.add_physical(p.lines[4], "1004")
 # ================================================================ #
 class BackwardFacingStep3d(Application):
     def __init__(self, h=0.2, mu=0.02):
-        super().__init__(mu=mu, h=h, ncomp=3)
+        super().__init__(mu=mu, h=h)
         # boundary conditions
         self.problemdata.bdrycond.set("Dirichlet", [100, 102])
         self.problemdata.bdrycond.set("Neumann", [104])
         self.problemdata.bdrycond.fct[102] = [lambda x, y, z: y*(1-y)*z*(1-z), lambda x, y, z: 0, lambda x, y, z: 0]
     def defineGeometry(self, geom, h):
         X = []
         X.append([-1.0, 1.0])
@@ -267,15 +269,15 @@
         geom.add_physical(circle.curve_loop.curves, label="3000")
         p = geom.add_rectangle(xmin=0, xmax=11, ymin=0, ymax=4.1, z=0, mesh_size=h, holes=[circle])
         geom.add_physical(p.surface, label="100")
         for i in range(len(p.lines)): geom.add_physical(p.lines[i], label=f"{1000 + i}")
 # ================================================================ #
 class SchaeferTurek3d(Application):
     def __init__(self, hcircle=None, mu=0.01, h=0.5, errordrag=True):
-        super().__init__(mu=mu, h=h, ncomp=3)
+        super().__init__(mu=mu, h=h)
         self.hcircle, self.errordrag = hcircle, errordrag
         # boundary conditions
         self.problemdata.bdrycond.set("Dirichlet", [100, 103, 300])
         self.problemdata.bdrycond.set("Neumann", [101])
         self.problemdata.bdrycond.fct[103] = [lambda x, y, z: 0.45 * y * (4.1 - y) * z * (4.1 - z) / 2.05 ** 4, lambda x, y, z: 0,
                                   lambda x, y, z: 0]
         self.problemdata.params.scal_glob["mu"] = mu
```

### Comparing `simfempy-2.1.1/simfempy/fems/cr1.py` & `simfempy-2.2.2/simfempy/fems/cr1.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 @author: becker
 """
 
 from matplotlib import colors
 import numpy as np
 import scipy.linalg as linalg
 import scipy.sparse as sparse
-# from simfempy.tools import barycentric, npext, checkmmatrix
 from simfempy.tools import barycentric
-# from simfempy.meshes import move, plotmesh
 from simfempy.fems import p1general
 import simfempy.fems.data, simfempy.fems.rt0
 
 #=================================================================#
 class CR1(p1general.P1general):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -291,16 +289,14 @@
             # print(f"{mask=}")
             fi = foc[mask].reshape(foc.shape[0], foc.shape[1] - 1)
             # print(f"{massloc=}")
             cols = np.tile(fi, dim).ravel()
             rows = np.repeat(fi, dim).ravel()
             mat = np.einsum('n,kl->nkl', dS, massloc).ravel()
             return AD + sparse.coo_matrix((mat, (rows, cols)), shape=(nfaces, nfaces))
-
-
         assert(isinstance(coeff, dict))
         rows = np.empty(shape=(0), dtype=int)
         cols = np.empty(shape=(0), dtype=int)
         mat = np.empty(shape=(0), dtype=float)
         for color in colors:
             faces = self.mesh.bdrylabels[color]
             normalsS = self.mesh.normals[faces]
@@ -324,14 +320,15 @@
         # assert np.all(faces == foc[:,-1])
         if colors is None: colors = self.mesh.bdrylabels.keys()
         massloc = barycentric.crbdryothers(self.mesh.dimension)
         if not isinstance(coeff, dict):
             faces = self.mesh.bdryFaces(colors)
             normalsS = self.mesh.normals[faces]
             dS = linalg.norm(normalsS, axis=1)
+            # print(f"{coeff.shape=} {dS.shape=} {self.mesh=}")
             if isinstance(coeff, (int,float)): dS *= coeff
             elif coeff.shape[0]==self.mesh.nfaces: dS *= coeff[faces]
             else: dS *= coeff
             if b is None: bsum = np.sum(dS*f[faces])
             else: b[faces] += dS*f[faces]
             ci = self.mesh.cellsOfFaces[faces][:, 0]
             foc = self.mesh.facesOfCells[ci]
@@ -354,40 +351,14 @@
             foc = self.mesh.facesOfCells[ci]
             mask = foc!=faces[:,np.newaxis]
             fi = foc[mask].reshape(foc.shape[0],foc.shape[1]-1)
             r = np.einsum('n,kl,nl->nk', dS, massloc, f[fi])
             # print(f"{np.linalg.norm(f[fi])=}")
             np.add.at(b, fi, r)
         return b
-    def computeFormTransportCellWise(self, du, u, data, type):
-        beta, betart = data.beta, data.betart
-        nfaces, dim, dV, foc = self.mesh.nfaces, self.mesh.dimension, self.mesh.dV, self.mesh.facesOfCells
-        cellgrads = self.cellgrads[:,:,:dim]
-        if type=='centered':
-            mat = np.einsum('n,njk,nk,i,nj -> ni', dV, cellgrads, beta, 1/(dim+1)*np.ones(dim+1),u[foc])
-        elif type=='supg':
-            mus = data.md.mus
-            mat = np.einsum('n,njk,nk,ni,nj -> ni', dV, cellgrads, beta, 1-dim*mus,u[foc])
-        else: raise ValueError(f"unknown type {type=}")
-        np.add.at(du, foc, mat)
-        self.massDotBoundary(du, u, coeff=-np.minimum(betart, 0))
-    def computeMatrixTransportCellWise(self, data, type):
-        beta, betart = data.beta, data.betart
-        nfaces, dim, dV = self.mesh.nfaces, self.mesh.dimension, self.mesh.dV
-        cellgrads = self.cellgrads[:,:,:dim]
-        if type=='centered':
-            # betagrad = np.einsum('njk,nk -> nj', cellgrads, beta)
-            mat = np.einsum('n,njk,nk,i -> nij', dV, cellgrads, beta, 1/(dim+1)*np.ones(dim+1))
-            # mat += np.einsum('n,nj,ni -> nij', dV*deltas, betagrad, betagrad)
-        elif type=='supg':
-            mus = data.md.mus
-            mat = np.einsum('n,njk,nk,ni -> nij', dV, cellgrads, beta, 1-dim*mus)
-        else: raise ValueError(f"unknown type {type=}")
-        A = sparse.coo_matrix((mat.ravel(), (self.rows, self.cols)), shape=(nfaces, nfaces))
-        return A - self.computeBdryMassMatrix(coeff=np.minimum(betart, 0), lumped=False)
     def computeMatrixJump(self, betart, mode='primal', monotone=False):
         dim, dV, nfaces, ndofs = self.mesh.dimension, self.mesh.dV, self.mesh.nfaces, self.nunknowns()
         nloc, dofspercell = self.nlocal(), self.dofspercell()
         if not hasattr(self.mesh,'innerfaces'): self.mesh.constructInnerFaces()
         innerfaces = self.mesh.innerfaces
         ci0 = self.mesh.cellsOfInteriorFaces[:,0]
         ci1 = self.mesh.cellsOfInteriorFaces[:,1]
@@ -459,193 +430,14 @@
             assert 0
         elif mode =='centered':
             assert 0
         else:
             raise ValueError(f"unknown {mode=}")
     def computeMassMatrixSupg(self, xd, coeff=1):
         raise NotImplemented(f"computeMassMatrixSupg")
-    def computeMatrixTransportUpwindAlg(self, data):
-        A = self.computeMatrixTransportCellWise(data, type='centered')
-        # moins bon en L2, mais meilleur en H1
-        # A += self.computeMatrixJump(betart)
-        self.diffalg = checkmmatrix.diffusionForMMatrix(A)
-        return A + self.diffalg
-    def computeMatrixTransportUpwind(self, data, method):
-        return self.computeMatrixTransportUpwindAlg(data)
-
-        beta, betart, mus = data.beta, data.betart, data.md.mus
-        nfaces, ncells, dim, dV = self.mesh.nfaces, self.mesh.ncells, self.mesh.dimension, self.mesh.dV
-        normalsS, foc, cof = self.mesh.normals, self.mesh.facesOfCells, self.mesh.cellsOfFaces
-        dbS = linalg.norm(normalsS, axis=1)*betart
-
-        innerfaces = self.mesh.innerfaces
-        infaces = np.arange(nfaces)[innerfaces]
-        ci0 = self.mesh.cellsOfInteriorFaces[:, 0]
-        ci1 = self.mesh.cellsOfInteriorFaces[:, 1]
-        matloc = np.ones(shape=(dim+1))/(dim+1)
-        cols = np.repeat(infaces, dim + 1).ravel()
-        #centered
-        # rows0 = foc[ci0].ravel()
-        # rows1 = foc[ci1].ravel()
-        # mat = np.einsum('n,i->ni', dbS[infaces], matloc).ravel()
-        # A = sparse.coo_matrix((mat, (rows0, cols)), shape=(nfaces, nfaces))
-        # A -= sparse.coo_matrix((mat, (rows1, cols)), shape=(nfaces, nfaces))
-
-        if method=='upw2':
-            rows0 = foc[ci0].ravel()
-            rows1 = foc[ci1].ravel()
-            mat = np.einsum('n,ni->ni', dbS[infaces], 1-dim*mus[ci0]).ravel()
-            A = -sparse.coo_matrix((mat, (cols, rows0)), shape=(nfaces, nfaces))
-            mat = np.einsum('n,ni->ni', dbS[infaces], 1-dim*mus[ci1]).ravel()
-            A += sparse.coo_matrix((mat, (cols, rows1)), shape=(nfaces, nfaces))
-            faces = self.mesh.bdryFaces()
-            ci0 = self.mesh.cellsOfFaces[faces, 0]
-            rows0 = foc[ci0].ravel()
-            cols = np.repeat(faces, dim + 1).ravel()
-            # mat = np.einsum('n,ni->ni', dbS[faces], 1-dim*mus[ci0]).ravel()
-            mat = np.einsum('n,i->ni', dbS[faces], matloc).ravel()
-            A -= sparse.coo_matrix((mat, (cols,rows0)), shape=(nfaces, nfaces))
-            A += self.computeMatrixJump(betart, mode='dual')
-            A += self.computeBdryMassMatrix(coeff=np.maximum(betart, 0), lumped=False)
-            # B = self.computeMatrixTransportCellWise(type='centered')
-            # if not np.allclose(A.tocsr().A,B.tocsr().A):
-            #     raise ValueError(f"{A.diagonal()=}\n{B.diagonal()=}")
-            return A
-
-        #supg
-        rows0 = foc[ci0].ravel()
-        rows1 = foc[ci1].ravel()
-        mat = np.einsum('n,ni->ni', dbS[infaces], 1-dim*mus[ci0]).ravel()
-        A = sparse.coo_matrix((mat, (rows0, cols)), shape=(nfaces, nfaces))
-        mat = np.einsum('n,ni->ni', dbS[infaces], 1-dim*mus[ci1]).ravel()
-        A -= sparse.coo_matrix((mat, (rows1, cols)), shape=(nfaces, nfaces))
-        faces = self.mesh.bdryFaces()
-        ci0 = self.mesh.cellsOfFaces[faces, 0]
-        rows0 = foc[ci0].ravel()
-        cols = np.repeat(faces, dim + 1).ravel()
-        mat = np.einsum('n,ni->ni', dbS[faces], 1-dim*mus[ci0]).ravel()
-        A += sparse.coo_matrix((mat, (rows0,cols)), shape=(nfaces, nfaces))
-        A += self.computeMatrixJump(betart, mode='primal')
-        A -= self.computeBdryMassMatrix(coeff=np.minimum(betart, 0), lumped=False)
-        # B = self.computeMatrixTransportSupg(bdrylumped=False, method='supg')
-        # if not np.allclose(A.tocsr().A,B.tocsr().A):
-        #     raise ValueError(f"{A.diagonal()=}\n{B.diagonal()=}")
-
-        # A += self.computeMatrixJump(betart, mode='primal')
-        #upwind
-
-        # mat0 = np.einsum('n,ni->ni', np.minimum(dbS[infaces],0), 1-dim*self.md.mus[self.md.cells[ci0]]).ravel()
-        # mat1 = np.einsum('n,i->ni', np.minimum(dbS[infaces],0), matloc).ravel()
-        # rows0 = foc[self.md.cells[ci0]].ravel()
-        # rows1 = foc[ci1].ravel()
-        # A = sparse.coo_matrix((mat0, (rows0, cols)), shape=(nfaces, nfaces))
-        # A -= sparse.coo_matrix((mat1, (rows1, cols)), shape=(nfaces, nfaces))
-        #
-        # mat0 = np.einsum('n,i->ni', np.maximum(dbS[infaces],0), matloc).ravel()
-        # mat1 = np.einsum('n,ni->ni', np.maximum(dbS[infaces],0), 1-dim*self.md.mus[self.md.cells[ci1]]).ravel()
-        # rows0 = foc[ci0].ravel()
-        # rows1 = foc[self.md.cells[ci1]].ravel()
-        # A = sparse.coo_matrix((mat0, (rows0, cols)), shape=(nfaces, nfaces))
-        # A -= sparse.coo_matrix((mat1, (rows1, cols)), shape=(nfaces, nfaces))
-
-
-        # faces = self.mesh.bdryFaces()
-        # ci0 = self.mesh.cellsOfFaces[faces, 0]
-        # rows0 = foc[ci0].ravel()
-        # cols = np.repeat(faces, dim + 1).ravel()
-        # mat = np.einsum('n,i->ni', dbS[faces], matloc).ravel()
-        # A += sparse.coo_matrix((mat, (rows0,cols)), shape=(nfaces, nfaces))
-        #
-        # A -= self.computeBdryMassMatrix(coeff=np.minimum(betart, 0), lumped=False)
-        # A += self.computeMatrixJump(betart, mode='primal')
-
-        # B = self.computeMatrixTransportCellWise(type='centered')
-        #
-        # A = A.tocsr()
-        # B = B.tocsr()
-        # if not np.allclose(A.A,B.A):
-        #     raise ValueError(f"{A.diagonal()=}\n{B.diagonal()=}\n{A.todense()=}\n{B.todense()=}")
-
-        return A.tocsr()
-
-        # ind = np.arange(nfaces)[dbS>0]
-        # # ind = np.arange(nfaces)[np.logical_and(self.mesh.innerfaces,dbS>0)]
-        # ci = self.mesh.cellsOfFaces[ind,0].ravel()
-        # faces = self.mesh.faces[ind]
-        # ind0 = npext.positionin(faces, self.mesh.simplices[ci])
-        # fi0 = np.take_along_axis(self.mesh.facesOfCells[ci], ind0, axis=1)
-        # rows = fi0.ravel()
-        # mat = dbS[ind].repeat(dim)
-        # A += sparse.coo_matrix((mat.ravel(), (rows, rows)), shape=(nfaces, nfaces))
-        # cols = ind.repeat(dim)
-        # A -= sparse.coo_matrix((mat.ravel(), (rows, cols)), shape=(nfaces, nfaces))
-        #
-        # ind = np.arange(nfaces)[np.logical_and(self.mesh.innerfaces,dbS<0)]
-        # ci = self.mesh.cellsOfFaces[ind,1].ravel()
-        # faces = self.mesh.faces[ind]
-        # ind0 = npext.positionin(faces, self.mesh.simplices[ci])
-        # fi0 = np.take_along_axis(self.mesh.facesOfCells[ci], ind0, axis=1)
-        # rows = fi0.ravel()
-        # mat = dbS[ind].repeat(dim)
-        # A -= sparse.coo_matrix((mat.ravel(), (rows, rows)), shape=(nfaces, nfaces))
-        # cols = ind.repeat(dim)
-        # A += sparse.coo_matrix((mat.ravel(), (rows, cols)), shape=(nfaces, nfaces))
-        # sigma = self.mesh.sigma
-        # mat = np.einsum('nj,i -> nij', dbS[foc] * sigma, np.ones(dim + 1)).ravel()
-        # cols = np.array(self.cols)
-        # m = np.where(mat > 0)
-        # cols[m] = self.rows[m]
-        # A = sparse.coo_matrix((mat, (self.rows, cols)), shape=(nfaces, nfaces))
-        # # A += self.computeMatrixJump(betart, mode='primal')
-        # A -= self.computeBdryMassMatrix(coeff=np.minimum(betart, 0))
-    def computeMatrixTransportSupg(self, data, method):
-        beta, betart, mus = data.beta, data.betart, data.md.mus
-        if method=='supg2':
-            beta, mus, deltas = beta, self.md.mus, self.md.deltas
-            nfaces, dim, dV = self.mesh.nfaces, self.mesh.dimension, self.mesh.dV
-            cellgrads = self.cellgrads[:,:,:dim]
-            mat = np.einsum('n,njk,nk,ni -> nij', dV, cellgrads, beta, 1-dim*mus)
-            print(f"{self.mesh.facesOfCells[self.md.cells]=}")
-            rows = np.repeat(self.mesh.facesOfCells[self.md.cells], self.nloc).ravel()
-            A = sparse.coo_matrix((mat.ravel(), (rows, self.cols)), shape=(nfaces, nfaces))
-            A -= self.computeBdryMassMatrix(coeff=np.minimum(betart, 0), lumped=False)
-            print(f"{A.diagonal()=}")
-            return A
-        A = self.computeMatrixTransportCellWise(data, type='supg')
-        A += self.computeMatrixJump(betart)
-        return A
-    def computeMatrixTransportLps(self, data, **kwargs):
-        A = self.computeMatrixTransportCellWise(data, type='centered')
-        A += self.computeMatrixJump(data.betart)
-        A += self.computeMatrixLps(data.betart, **kwargs)
-        return A
-    def computeFormTransportUpwind(self, du, u, data, method):
-        return self.computeFormTransportUpwindAlg(du, u, data)
-    def computeFormTransportUpwindAlg(self, du, u, data):
-        self.computeFormTransportCellWise(du, u, data, type='centered')
-        if hasattr(self,'diffalg'):
-            du += self.diffalg@u
-    def computeFormTransportSupg(self, du, u, data, method):
-        self.computeFormTransportCellWise(du, u, data, type='supg')
-        self.computeFormJump(du, u, data.betart)
-    def computeFormTransportLps(self, du, u, data, **kwargs):
-        self.computeFormTransportCellWise(du, u, data, type='centered')
-        self.computeFormJump(du, u, data.betart)
-        self.computeFormLps(du, u, data.betart, **kwargs)
-    # def massDotSupg(self, b, f, data, coeff=1):
-    #     if self.params_str['convmethod'][:4] != 'supg': return
-    #     dim, facesOfCells, dV = self.mesh.dimension, self.mesh.facesOfCells, self.mesh.dV
-    #     # beta, mus, deltas = beta, self.md.mus, self.md.deltas
-    #     # cellgrads = self.cellgrads[:,:,:dim]
-    #     # betagrad = np.einsum('njk,nk -> nj', cellgrads, beta)
-    #     # r = np.einsum('n,ni->ni', deltas*dV*f[facesOfCells].mean(axis=1), betagrad)
-    #     r = np.einsum('n,nk->nk', coeff*dV*f[facesOfCells].mean(axis=1), dim/(dim+1)-dim*data.md.mus)
-    #     np.add.at(b, facesOfCells, r)
-    #     return b
-    # dotmat
     def massDotCell(self, b, f, coeff=1):
         assert f.shape[0] == self.mesh.ncells
         dimension, facesOfCells, dV = self.mesh.dimension, self.mesh.facesOfCells, self.mesh.dV
         massloc = 1/(dimension+1)
         np.add.at(b, facesOfCells, (massloc*coeff*dV*f)[:, np.newaxis])
         return b
     def massDot(self, b, f, coeff=1):
```

### Comparing `simfempy-2.1.1/simfempy/fems/d0.py` & `simfempy-2.2.2/simfempy/fems/d0.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     def __init__(self, mesh=None):
         pass
         # super().__init__(mesh=mesh)
     def setMesh(self, mesh):
         self.mesh = mesh
     def nlocal(self): return 1
     def nunknowns(self): return self.mesh.ncells
+    def tocell(self, u): return u
     def tonode(self, u):
         unodes = np.zeros(self.mesh.nnodes)
         if u.shape[0] != self.mesh.ncells: raise ValueError(f"{u.shape=} {self.mesh.ncells=}")
         np.add.at(unodes, self.mesh.simplices.T, u.T)
         countnodes = np.zeros(self.mesh.nnodes, dtype=int)
         np.add.at(countnodes, self.mesh.simplices.T, 1)
         unodes /= countnodes
```

### Comparing `simfempy-2.1.1/simfempy/fems/data.py` & `simfempy-2.2.2/simfempy/fems/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 #=================================================================#
 class ConvectionData(object):
     """
     Information for boundary conditions
     """
     def __init__(self, **kwargs):
         self.betacell, self.betart, self.md = kwargs.pop('betacell',None), kwargs.pop('betart',None), kwargs.pop('md',None)
+    def __repr__(self):
+        return ", ".join("'{}': {}".format(attr, value.shape if value is not None else "None") for attr, value in self.__dict__.items())
```

### Comparing `simfempy-2.1.1/simfempy/fems/p1.py` & `simfempy-2.2.2/simfempy/fems/p1.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,46 +15,46 @@
 class P1(p1general.P1general):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
     def setMesh(self, mesh):
         super().setMesh(mesh)
         self.computeStencilCell(self.mesh.simplices)
         self.cellgrads = self.computeCellGrads()
-    def prepareAdvection(self, beta, scale):
-        method = self.params_str['convmethod']
-        rt = simfempy.fems.rt0.RT0(mesh=self.mesh)
-        betart = scale*rt.interpolate(beta)
-        betacell = rt.toCell(betart)
-        convdata = simfempy.fems.data.ConvectionData(betacell=betacell, betart=betart)
-        if method == 'upwalg':
-             return convdata 
-        elif method == 'lps':
-            self.mesh.constructInnerFaces()
-            return convdata 
-        elif method == 'supg':
-            md = meshes.move.move_midpoints(self.mesh, betacell)
-            # self.md.plot(self.mesh, beta, type='midpoints')
-        elif method == 'supg2':
-            md = meshes.move.move_midpoints(self.mesh, betacell, extreme=True)
-            # self.md.plot(self.mesh, beta, type='midpoints')
-        elif method == 'upwalg':
-            pass
-        elif method == 'upw':
-            md = meshes.move.move_nodes(self.mesh, -betacell)
-            # self.md.plot(self.mesh, beta)
-        elif method == 'upw2':
-            md = meshes.move.move_nodes(self.mesh, -betacell, second=True)
-            # self.md.plot(self.mesh, beta)
-        elif method == 'upwsides':
-            self.mesh.constructInnerFaces()
-            md = meshes.move.move_midpoints(self.mesh, -betacell)
-        else:
-            raise ValueError(f"don't know {method=}")
-        convdata.md = md
-        return convdata
+    # def prepareAdvection(self, beta, scale):
+    #     method = self.params_str['convmethod']
+    #     rt = simfempy.fems.rt0.RT0(mesh=self.mesh)
+    #     betart = scale*rt.interpolate(beta)
+    #     betacell = rt.toCell(betart)
+    #     convdata = simfempy.fems.data.ConvectionData(betacell=betacell, betart=betart)
+    #     if method == 'upwalg':
+    #          return convdata
+    #     elif method == 'lps':
+    #         self.mesh.constructInnerFaces()
+    #         return convdata
+    #     elif method == 'supg':
+    #         md = meshes.move.move_midpoints(self.mesh, betacell)
+    #         # self.md.plot(self.mesh, beta, type='midpoints')
+    #     elif method == 'supg2':
+    #         md = meshes.move.move_midpoints(self.mesh, betacell, extreme=True)
+    #         # self.md.plot(self.mesh, beta, type='midpoints')
+    #     elif method == 'upwalg':
+    #         pass
+    #     elif method == 'upw':
+    #         md = meshes.move.move_nodes(self.mesh, -betacell)
+    #         # self.md.plot(self.mesh, beta)
+    #     elif method == 'upw2':
+    #         md = meshes.move.move_nodes(self.mesh, -betacell, second=True)
+    #         # self.md.plot(self.mesh, beta)
+    #     elif method == 'upwsides':
+    #         self.mesh.constructInnerFaces()
+    #         md = meshes.move.move_midpoints(self.mesh, -betacell)
+    #     else:
+    #         raise ValueError(f"don't know {method=}")
+    #     convdata.md = md
+    #     return convdata
     def nlocal(self): return self.mesh.dimension+1
     def nunknowns(self): return self.mesh.nnodes
     def dofspercell(self): return self.mesh.simplices
     def computeCellGrads(self):
         ncells, normals, cellsOfFaces, facesOfCells, dV = self.mesh.ncells, self.mesh.normals, self.mesh.cellsOfFaces, self.mesh.facesOfCells, self.mesh.dV
         scale = -1/self.mesh.dimension
         return scale*(normals[facesOfCells].T * self.mesh.sigma.T / dV.T).T
@@ -221,14 +221,17 @@
     def interpolateBoundary(self, colors, f, lumped=False):
         """
         :param colors: set of colors to interpolate
         :param f: ditct of functions
         :return:
         """
         b = np.zeros(self.mesh.nnodes)
+        # print(f"{type(f)=} {colors=} {len(f)=}")
+        # if len(f) < len(colors):
+        #     raise ValueError(f"{type(f)=} {colors=} {len(f)=}")
         for color in colors:
             if not color in f or not f[color]: continue
             faces = self.mesh.bdrylabels[color]
             normalsS = self.mesh.normals[faces]
             dS = linalg.norm(normalsS,axis=1)
             normalsS = normalsS/dS[:,np.newaxis]
             nx, ny, nz = normalsS.T
@@ -357,14 +360,15 @@
         A = self.computeMatrixTransportCellWise(data, type='centered')
         A += self.computeMatrixLps(data.betart)
         return A
     def computeMatrixTransportCellWise(self, data, type):
         nnodes, ncells, nfaces, dim = self.mesh.nnodes, self.mesh.ncells, self.mesh.nfaces, self.mesh.dimension
         if type=='centered':
             beta, mus = data.betacell, np.full(dim+1,1.0/(dim+1))
+            # print(f"{beta=} {data=}")
             mat = np.einsum('n,njk,nk,i -> nij', self.mesh.dV, self.cellgrads[:,:,:dim], beta, mus)
             A =  sparse.coo_matrix((mat.ravel(), (self.rows, self.cols)), shape=(nnodes, nnodes)).tocsr()
         elif type=='supg':
             beta, mus = data.betacell, data.md.mus
             mat = np.einsum('n,njk,nk,ni -> nij', self.mesh.dV, self.cellgrads[:,:,:dim], beta, mus)
             A =  sparse.coo_matrix((mat.ravel(), (self.rows, self.cols)), shape=(nnodes, nnodes)).tocsr()
         else: raise ValueError(f"unknown type {type=}")
@@ -401,24 +405,24 @@
     def massDotSupg(self, b, f, data, coeff=1):
         if self.params_str['convmethod'][:4] != 'supg': return
         dim, simplices, dV = self.mesh.dimension, self.mesh.simplices, self.mesh.dV
         r = np.einsum('n,nk,n->nk', coeff*dV, data.md.mus-1/(dim+1), f[simplices].mean(axis=1))
         np.add.at(b, simplices, r)
         return b
     def massDotBoundary(self, b=None, f=None, colors=None, coeff=1, lumped=False):
-        # if lumped is None: lumped=self.params_bool['masslumpedbdry']
         if colors is None: colors = self.mesh.bdrylabels.keys()
         for color in colors:
             faces = self.mesh.bdrylabels[color]
             normalsS = self.mesh.normals[faces]
             dS = linalg.norm(normalsS, axis=1)
             nodes = self.mesh.faces[faces]
             if isinstance(coeff, (int,float)): dS *= coeff
             elif isinstance(coeff, dict): dS *= coeff[color]
             else:
+                # print(f"{coeff.shape=} {self.mesh.nfaces=}")
                 assert coeff.shape[0]==self.mesh.nfaces
                 dS *= coeff[faces]
             # print(f"{scalemass=}")
             if lumped:
                 np.add.at(b, nodes, f[nodes]*dS[:,np.newaxis]/self.mesh.dimension)
             else:
                 massloc = tools.barycentric.tensor(d=self.mesh.dimension-1, k=2)
```

### Comparing `simfempy-2.1.1/simfempy/fems/rt0.py` & `simfempy-2.2.2/simfempy/fems/rt0.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,32 +15,29 @@
 class RT0():
     """
     on suppose que  self.mesh.edgesOfCell[ic, kk] et oppose à elem[ic,kk] !!!
     """
     def __init__(self, mesh=None):
         if mesh is not None:
             self.setMesh(mesh)
-        pass
-        # super().__init__(mesh=mesh)
-        # for p, v in zip(['massproj', 'convmethod'], ['standard', 'supg']):
-        #     self.params_str[p] = kwargs.pop(p, v)
     def setMesh(self, mesh):
         self.mesh = mesh
         self.Mtocell = self.toCellMatrix()
     def nunknowns(self): return self.mesh.nfaces
     def nlocal(self): return self.mesh.dimension+1
     def interpolate(self, f):
         dim = self.mesh.dimension
         nfaces, normals = self.mesh.nfaces, self.mesh.normals[:,:dim]
         nnormals = normals/linalg.norm(normals, axis=1)[:,np.newaxis]
         if len(f) != self.mesh.dimension: raise TypeError(f"f needs {dim} components")
         xf, yf, zf = self.mesh.pointsf.T
         fa = np.array([f[i](xf,yf,zf) for i in range(dim)])
         return np.einsum('ni, in -> n', nnormals, fa)
-    def interpolateCR1(self, v, stack_storage):
+    def interpolateFromFem(self, v, fem, stack_storage):
+        assert isinstance(fem, fems.cr1.CR1)
         dim = self.mesh.dimension
         nfaces, normals = self.mesh.nfaces, self.mesh.normals[:,:dim]
         assert v.shape[0] == dim*nfaces
         nnormals = normals/linalg.norm(normals, axis=1)[:,np.newaxis]
         if stack_storage:
             return np.einsum('ni, in -> n', nnormals, v.reshape(dim, nfaces))
         return np.einsum('ni, ni -> n', nnormals, v.reshape(nfaces,dim))
```

### Comparing `simfempy-2.1.1/simfempy/linalg/linalg.py` & `simfempy-2.2.2/simfempy/linalg/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         else:
             return ScipySolve(method=method, **kwargs)
     elif method == "spsolve":
         return ScipySpSolve(matrix=matrix)
     elif method == "pyamg":
         return Pyamg(matrix, **kwargs)
     else:
-        raise ValueError(f"unknwown {method=} not in ['spsolve', 'pyamg', {pyamgsolvers}]")
+        raise ValueError(f"unknwown {method=} not in ['spsolve', 'pyamg', {pyamgsolvers}] nor {scipysolvers=}")
     if len(kwargs.keys()):
         raise ValueError(f"*** unused arguments {kwargs=}")
 
 #-------------------------------------------------------------------#
 def getLinearSolversAndTest(**kwargs):
     """
     :param kwargs: if args is dict build the correspong solver
@@ -234,34 +234,41 @@
 #=================================================================#
 class ScipySolve(IterativeSolver):
     def __init__(self, **kwargs):
         self.method = kwargs.pop('method')
         super().__init__(kwargs)
         # if self.method in strangesolvers: raise ValueError(f"method '{self.method}' is i strange scipy solver")
         self.n = kwargs.pop('n', None)
-        if "prec" in kwargs:
-            self.M = kwargs.pop("prec")
+        if "preconditioner" in kwargs:
+            # n = kwargs.pop('n')
+            self.preconditioner = kwargs.pop('preconditioner')
+            self.M = splinalg.LinearOperator(shape=(self.n, self.n), matvec=self.preconditioner.solve)
+        # else:
+        # self.M = None
+        # if "prec" in kwargs:
+        #     self.M = kwargs.pop("prec")
         if "matrix" in kwargs:
             self.matvec = kwargs.pop('matrix')
             if not "matvecprec" in kwargs:
                 fill_factor = kwargs.pop("fill_factor", 2)
                 drop_tol = kwargs.pop("fill_factor", 0.01)
                 spilu = splinalg.spilu(self.matvec.tocsc(), drop_tol=drop_tol, fill_factor=fill_factor)
-                self.M = splinalg.LinearOperator(self.matvec.shape, lambda x: spilu.solve(x))
+                if not hasattr(self, "M"): self.M = splinalg.LinearOperator(self.matvec.shape, lambda x: spilu.solve(x))
         else:
             if self.n is None: raise ValueError(f"need 'n' if no matrix given")
             # n = kwargs.pop('n')
             # raise ValueError(f"@@@@{n=}")
             self.matvec = splinalg.LinearOperator(shape=(self.n, self.n), matvec=kwargs.pop('matvec'))
-        if "preconditioner" in kwargs:
-            # n = kwargs.pop('n')
-            self.preconditioner = kwargs.pop('preconditioner')
-            self.M = splinalg.LinearOperator(shape=(self.n, self.n), matvec=self.preconditioner.solve)
-        else:
-            self.M = None
+        # if "preconditioner" in kwargs:
+        #     # n = kwargs.pop('n')
+        #     if kwargs.pop('preconditioner') == "scipy.sparse.linalg.spilu":
+        #         self.preconditioner = sparse.linalg.spilu()
+        #         self.M = splinalg.LinearOperator(shape=(self.n, self.n), matvec=self.preconditioner.solve)
+        # else:
+        #     self.M = None
         # self.args = {"A": self.matvec, "M":self.M, "atol":self.atol}
         self.args['A'] = self.matvec
         self.args['M'] = self.M
         name = self.method
         if self.method=='scipy_gcrotmk':
             self.args['m'] = kwargs.pop('m', 5)
             self.args['truncate'] = kwargs.pop('truncate', 'smallest')
@@ -304,14 +311,16 @@
             raise ImportError(f"*** pyamg not found ***")
         assert A is not None
         self.method = 'pyamg'
         nsmooth = kwargs.pop('nsmooth', 1)
         symmetric = kwargs.pop('symmetric', False)
         self.smoother = kwargs.pop('smoother', 'gauss_seidel')
         # pyamgargs = {'B': pyamg.solver_configuration(A, verb=False)['B']}
+        # pyamgargs = kwargs.pop("pyamgargs", {})
+        # print(f"{pyamgargs=}")
         pyamgargs = {}
         smoother = (self.smoother, {'sweep': 'symmetric', 'iterations': nsmooth})
         if symmetric:
             smooth = ('energy', {'krylov': 'cg'})
         else:
             smooth = ('energy', {'krylov': 'fgmres'})
             pyamgargs['symmetry'] = 'nonsymmetric'
```

### Comparing `simfempy-2.1.1/simfempy/linalg/matrixsystem.py` & `simfempy-2.2.2/simfempy/linalg/matrixsystem.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/linalg/saddle_point.py` & `simfempy-2.2.2/simfempy/linalg/saddle_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 n = self.A.shape[0]
                 for i in range(self.ncompA): w[i*n:(i+1)*n] = self.A.dot(b[i*n:(i+1)*n])
             else:
                 for i in range(self.ncompA): w[i::self.ncompA] = self.A.dot(b[i::self.ncompA])
             return w
         return self.A.dot(b)
     def scale_matrix(self):
+        print(f"** SaddlePointSystem scale_matrix {hasattr(self,'scalings')=}")
         DA = self.A.diagonal()
         assert np.all(DA>0)
         if self.singleA:
             AD = linalg.linalg.diagmatrix2systemdiagmatrix(1 / DA, self.ncompA, self.stack_storage)
         else:
             AD = sparse.diags(1/DA, offsets=(0), shape=self.A.shape)
         vs = sparse.diags(np.power(AD.diagonal(), 0.5), offsets=(0), shape=AD.shape)
@@ -58,14 +59,15 @@
             self.A = vss @ self.A @ vss
         else:
             self.A = vs@self.A@vs
         nb = self.B.shape[0]
         ps = sparse.diags(np.power((self.B@vs**2@self.B.T).diagonal(), -0.5), offsets=(0), shape=(nb,nb))
         self.B = ps@self.B@vs
         self.scalings = [vs, ps]
+        print(f"{self.scalings=}")
         if self.C is None: return
         nc = self.C.shape[0]
         ls = sparse.diags(np.power((self.C@ps**2@self.C.T).diagonal(), -0.5), offsets=(0), shape=(nc,nc))
         self.C = ls@self.C@ps
         self.scalings.append(ls)
     def scale_vec(self, b):
         self.vectorview.scale(b, self.scalings)
```

### Comparing `simfempy-2.1.1/simfempy/linalg/vectorview.py` & `simfempy-2.2.2/simfempy/linalg/vectorview.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/meshes/plotmesh.py` & `simfempy-2.2.2/simfempy/meshes/plotmesh.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/meshes/simplexmesh.py` & `simfempy-2.2.2/simfempy/meshes/simplexmesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Sun Dec  4 18:14:29 2016
 
 @author: becker
 """
 import os
 import meshio
 import numpy as np
-from numpy.lib.shape_base import take_along_axis
+# from numpy.lib.shape_base import take_along_axis
 from scipy import sparse
 # from simfempy.tools import npext, timer
 from simfempy.tools import timer
 
 #=================================================================#
 class SimplexMesh(object):
     """
@@ -39,17 +39,23 @@
     dV: shape (ncells), volumes of simplices
     bdrylabels: dictionary(keys: colors, values: id's of boundary faces)
     cellsoflabel: dictionary(keys: colors, values: id's of cells)
     """
 
     def __repr__(self):
         s = f"dim/nnodes/nfaces/ncells: {self.dimension}/{self.nnodes}/{self.nfaces}/{self.ncells}"
-        s += f"\nbdrylabels={list(self.bdrylabels.keys())}"
-        s += f"\ncellsoflabel={list(self.cellsoflabel.keys())}"
+        if hasattr(self, "labeldict_i2s"):
+            s += f"\nbdrylabels={[self.labeldict_i2s[k] for k in self.bdrylabels.keys()]}"
+            s += f"\ncellsoflabel={[self.labeldict_i2s[k] for k in self.cellsoflabel.keys()]}"
+        else:
+            s += f"\nbdrylabels={list(self.bdrylabels.keys())}"
+            s += f"\ncellsoflabel={list(self.cellsoflabel.keys())}"
         return s
+    def __str__(self):
+        return f"dim/nnodes/nfaces/ncells: {self.dimension}/{self.nnodes}/{self.nfaces}/{self.ncells}"
     def __init__(self, mesh, **kwargs):
         # if not isinstance(mesh, meshio.Mesh):
         #     raise KeyError(f"Needs a meshio.Mesh, got {type(mesh)}")
         self.timer = timer.Timer(name="SimplexMesh")
         celltypes = [c.type for c in mesh.cells]
         # celltypes = [key for key, cellblock in mesh.cells]
         self._initMeshPyGmsh(mesh, celltypes)
@@ -156,28 +162,40 @@
         # the indices of the np.array are not the cellids !
         # ???
         # print(f"{cell_sets=}")
         typesoflabel = {}
         sizes = {key:0 for key in celltypes}
         cellsoflabel = {key:{} for key in celltypes}
         ctorderd = []
+        labeldict_s2i, labeldict_i2s, labind = {}, {}, 0
         for label, cb in cell_sets.items():
             if label=='gmsh:bounding_entities': continue
             # print(f"{label=} {cb=}")
             if len(cb) != len(celltypes): raise KeyError(f"mismatch {label=}")
             for celltype, info in zip(celltypes, cb):
                 # only one is supposed to be not None
                 if info is not None:
-                    try: ilabel=int(label)
-                    except: raise ValueError(f"cannot convert to int {label=} {cell_sets=}")
+                    try:
+                        ilabel=int(label)
+                    except:
+                        if label in labeldict_s2i.keys():
+                            ilabel = labeldict_s2i[label]
+                        else:
+                            labind -= 1
+                            ilabel = labind
+                            labeldict_s2i[label] = ilabel
+                            labeldict_i2s[ilabel] = label
+                            # raise ValueError(f"cannot convert to int {label=} {cell_sets=}")
                     cellsoflabel[celltype][ilabel] = info
                     # print(f"{label=} {celltype=} {info=}")
                     sizes[celltype] += info.shape[0]
                     typesoflabel[ilabel] = celltype
                     ctorderd.append(celltype)
+        if labind:
+            self.labeldict_s2i, self.labeldict_i2s = labeldict_s2i, labeldict_i2s
         # print(f"{celltypes=}\n{cellsoflabel=}")
         #correcting the numbering in cell_sets
         n = 0
         for ct in list(dict.fromkeys(ctorderd)):
             #eliminates duplicates
             for l, cb in cellsoflabel[ct].items(): cb -= n
             n += sizes[ct]
@@ -394,14 +412,23 @@
             # print("S=",S)
             from . import plotmesh
             import matplotlib.pyplot as plt
             simps, xc, yc = self.simplices, self.pointsc[:,0], self.pointsc[:,1]
             meshdata =  self.x, self.y, simps, xc, yc
             plotmesh.meshWithNodesAndTriangles(meshdata)
             plt.show()
+    # ----------------------------------------------------------------#
+    def plot(self, **kwargs):
+        from . import plotmesh
+        import matplotlib.pyplot as plt
+        if kwargs.pop("bdry", False):
+            plotmesh.meshWithBoundaries(self, **kwargs)
+        else:
+            plotmesh.meshWithData(self, **kwargs)
+
 
 #=================================================================#
 if __name__ == '__main__':
     import pygmsh
     rect = [-2, 2, -2, 2]
     with pygmsh.geo.Geometry() as geom:
         z=0
```

### Comparing `simfempy-2.1.1/simfempy/meshes/testmeshes.py` & `simfempy-2.2.2/simfempy/meshes/testmeshes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/models/application.py` & `simfempy-2.2.2/simfempy/applications/application.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,46 +3,60 @@
 from simfempy.meshes.simplexmesh import SimplexMesh
 # import simfempy.tools.analyticalfunction
 from simfempy.tools.analyticalfunction import analyticalSolution
 
 # ================================================================ #
 class Application:
     def __init__(self, **kwargs):
-        self.h = kwargs.pop('h', None)
+        self.h = kwargs.pop('h', 0.5)
         self.exactsolution = kwargs.pop('exactsolution', None)
         self.random_exactsolution = kwargs.pop('random_exactsolution', None)
         self.generatePDforES = kwargs.pop('generatePDforES', None)
         if self.generatePDforES is None and self.exactsolution:
             self.generatePDforES = True
         self.problemdata = ProblemData()
-        self.problemdata.ncomp = kwargs.pop('ncomp', 1)
+        self.defineProblemData(self.problemdata)
+        # print(f"{self.problemdata=}")
         scal_glob = kwargs.pop('scal_glob', {})
         for k,v in scal_glob.items():
             self.problemdata.params.scal_glob[k] = v
         if len(kwargs.keys()):
             raise ValueError(f"*** unused arguments {kwargs=}")
-    def createExactSolution(self, mesh):
-        dim, ncomp, ran = mesh.dimension, self.problemdata.ncomp, self.random_exactsolution
-        # print(f"****** createExactSolution: {dim=} {ncomp=} {self.exactsolution=}")
-        if isinstance(ncomp, (list,tuple)) or isinstance(self.exactsolution,(list,tuple)):
-            assert len(ncomp)==len(self.exactsolution)
-            es= []
-            for i in range(len(ncomp)):
-                es.append(analyticalSolution(self.exactsolution[i], dim, ncomp[i], ran))
-            self.exactsolution = es
-        else:
-            if isinstance(self.exactsolution, str):
-                self.exactsolution = analyticalSolution(self.exactsolution, dim, ncomp, ran)
 
-    def createMesh(self, h=None):
+    def defineGeometry(self, geom, h): raise ValueError(f"not written")
+    def createExactSolution(self, mesh, ncomps):
+        dim, ran = mesh.dimension, self.random_exactsolution
+        assert isinstance(ncomps, (list,tuple))
+        if isinstance(self.exactsolution, str): names=[self.exactsolution]
+        else: names = self.exactsolution
+        # print(f"***{ncomps=} {names=} {self.exactsolution=}")
+        assert len(ncomps) == len(names)
+        self.exactsolution = []
+        for i in range(len(ncomps)):
+            print(f"{i=} {names[i]=} {ncomps[i]=}")
+            self.exactsolution.append(analyticalSolution(names[i], dim, ncomps[i], ran))
+        return
+        # print(f"****** createExactSolution: {dim=} {ncomp=} {self.exactsolution=}")
+        # if isinstance(ncomp, (list,tuple)) or isinstance(self.exactsolution,(list,tuple)):
+        #     assert len(ncomp)==len(self.exactsolution)
+        #     es= []
+        #     for i in range(len(ncomp)):
+        #         es.append(analyticalSolution(self.exactsolution[i], dim, ncomp[i], ran))
+        #     self.exactsolution = es
+        # else:
+        #     if isinstance(self.exactsolution, str):
+        #         self.exactsolution = analyticalSolution(self.exactsolution, dim, ncomp, ran)
+    def createMesh(self, h=0.5):
         if h is None: h = self.h
         with pygmsh.geo.Geometry() as geom:
             self.defineGeometry(geom, h)
             mesh = geom.generate_mesh()
         return SimplexMesh(mesh)
+    def defineProblemData(self, problemdata):
+        pass
     def plot(self, mesh, data, **kwargs):
         if mesh.dimension != 2:
             raise ValueError("not written")
         import matplotlib.pyplot as plt
         from matplotlib.figure import figaspect
         import matplotlib.gridspec as gridspec
         from mpl_toolkits.axes_grid1 import make_axes_locatable
```

### Comparing `simfempy-2.1.1/simfempy/models/elliptic.py` & `simfempy-2.2.2/simfempy/models/elliptic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import numpy as np
 from simfempy import fems
 from simfempy.models.model import Model
 from simfempy.tools.analyticalfunction import AnalyticalFunction
 import scipy
 import scipy.sparse.linalg as splinalg
-import simfempy.tools.iterationcounter
+# import simfempy.tools.iterationcounter
 from simfempy.linalg import saddle_point, matrixsystem
 
 # ================================================================= #
 def Elliptic(**kwargs):
-    if kwargs['fem'] == 'rt0': return EllipticMixed(**kwargs)
-    elif kwargs['fem'] in ['p1', 'cr1']: return EllipticPrimal(**kwargs)
-    else: raise NotImplementedError(f"unknown {kwargs['fem']=}")
+    fem = kwargs.pop("fem", "cr1")
+    kwargs["fem"] = fem
+    if fem == 'rt0': return EllipticMixed(**kwargs)
+    else: return EllipticPrimal(**kwargs)
+    # if kwargs['fem'] == 'rt0':
+    #     return EllipticMixed(**kwargs)
+    # elif kwargs['fem'] in ['p1', 'cr1']:
+    #     return EllipticPrimal(**kwargs)
+    # else:
+    #     raise NotImplementedError(f"unknown {kwargs['fem']=}")
+
+
 # ================================================================= #
 class EllipticBase(Model):
     """
     Class for the elliptic equation
     $$
     -\div(A \nabla T) + b\cdot\nabla u + c u= f         domain
     A\nabla\cdot n + alpha T = g  bdry
@@ -48,94 +57,118 @@
         return self.__repr__()
     def __repr__(self):
         repr = super().__repr__()
         repr += f"\nfem={self.fem}"
         return repr
     def __init__(self, **kwargs):
         # print(f"{kwargs=}")
-        self.fem = kwargs.pop('fem','p1')
+        # print(f"{kwargs.keys()=}")
+        self.fem = kwargs.pop('fem','cr1')
+        self.linearsolver = kwargs.pop('linearsolver', 'pyamg')
         super().__init__(**kwargs)
     def createFem(self):
-        self.convection = 'convection' in self.disc_params
+        self.hasconvection = 'convection' in self.disc_params \
+                          or 'convection' in self.problemdata.params.data.keys()\
+                          or 'convection' in self.problemdata.params.fct_glob.keys()
+        if self.hasconvection:
+            print(f"{self.disc_params=}")
+            self.convectionmethod = self.disc_params.pop('convmethod', 'lps')
+            if self.convectionmethod == 'lps':
+                self.lpsparam = self.disc_params.pop('lpsparam', 0.1)
         self.dirichletmethod = self.disc_params.pop('dirichletmethod','nitsche')
         if self.dirichletmethod=='nitsche':
             self.nitscheparam = self.disc_params.pop('nitscheparam', 10)
         if self.fem == 'p1': self.fem = fems.p1.P1()
         elif self.fem == 'cr1': self.fem = fems.cr1.CR1()
         else:
             self.rt = fems.rt0.RT0()
             self.d0 = fems.d0.D0()
             self.fem = "RT0-D0"
     def meshSet(self):
         if hasattr(self, 'A'):
             del self.A
         self._checkProblemData()
         self.kheatcell = self.compute_cell_vector_from_params('kheat', self.problemdata.params)
-        if self.convection:
-            convectionfct = self.problemdata.params.fct_glob['convection']
-            self.convdata = self.fem.prepareAdvection(convectionfct, 1)
+        if self.hasconvection:
+            if not hasattr(self, 'convdata'):
+                self.convdata = fems.data.ConvectionData()
+            rt = fems.rt0.RT0(mesh=self.mesh)
+            if 'convection' in self.problemdata.params.fct_glob:
+                convection_given = self.problemdata.params.fct_glob['convection']
+                if not isinstance(convection_given, list):
+                    p = "problemdata.params.fct_glob['convection']"
+                    raise ValueError(f"need '{p}' as a list of length dim of str or AnalyticalSolution")
+                elif isinstance(convection_given[0],str):
+                    self.convection_fct = [AnalyticalFunction(expr=e) for e in convection_given]
+                else:
+                    self.convection_fct = convection_given
+                    if not isinstance(convection_given[0], AnalyticalFunction):
+                        raise ValueError(f"convection should be given as 'str' and not '{type(convection_given[0])}'")
+                if len(self.convection_fct) != self.mesh.dimension:
+                    raise ValueError(f"{self.mesh.dimension=} {self.problemdata.params.fct_glob['convection']=}")
+                # print(f"{convection_given=}")
+                self.convdata.betart = rt.interpolate(self.convection_fct)
+            else:
+                data, fem, stack_storage = self.problemdata.params.data['convection']
+                self.convdata.betart = rt.interpolateFromFem(data, fem, stack_storage)
+            self.convdata.betacell = rt.toCell(self.convdata.betart)
             colorsinflow = self.findInflowColors()
             colorsdir = self.problemdata.bdrycond.colorsOfType("Dirichlet")
             if not set(colorsinflow).issubset(set(colorsdir)):
                 raise ValueError(f"Inflow boundaries need to be subset of Dirichlet boundaries {colorsinflow=} {colorsdir=}")
     def findInflowColors(self):
         colors=[]
         for color in self.mesh.bdrylabels.keys():
             faces = self.mesh.bdrylabels[color]
             if np.any(self.convdata.betart[faces]<-1e-10): colors.append(color)
         return colors
     def _checkProblemData(self):
         if self.verbose: print(f"checking problem data {self.problemdata=}")
-        if self.convection:
-            convection_given = self.problemdata.params.fct_glob['convection']
-            if not isinstance(convection_given, list):
-                p = "problemdata.params.fct_glob['convection']"
-                raise ValueError(f"need '{p}' as a list of length dim of str or AnalyticalSolution")
-            elif isinstance(convection_given[0],str):
-                self.problemdata.params.fct_glob['convection'] = [AnalyticalFunction(expr=e) for e in convection_given]
-            else:
-                if not isinstance(convection_given[0], AnalyticalFunction):
-                    raise ValueError(f"convection should be given as 'str' and not '{type(convection_given[0])}'")
-            if len(self.problemdata.params.fct_glob['convection']) != self.mesh.dimension:
-                raise ValueError(f"{self.mesh.dimension=} {self.problemdata.params.fct_glob['convection']=}")
         bdrycond = self.problemdata.bdrycond
         for color in self.mesh.bdrylabels:
             if not color in bdrycond.type: raise ValueError(f"color={color} not in bdrycond={bdrycond}")
             if bdrycond.type[color] in ["Robin"]:
                 if not color in bdrycond.param:
                     raise ValueError(f"Robin condition needs paral 'alpha' color={color} bdrycond={bdrycond}")
-    def defineRhsAnalyticalSolution(self, solexact):
+        if bdrycond.type[color] == "Dirichlet":
+            if not color in bdrycond.fct:
+                bdrycond.fct[color] = lambda x,y,z: 0
+                # raise ValueError(f"Dirichlet condition needs fct for color={color} bdrycond={bdrycond}")
+    def defineRhsAnalyticalSolution(self, solexact_list):
+        solexact = solexact_list[0]
         def _fctu(x, y, z):
             kheat = self.problemdata.params.scal_glob['kheat']
-            beta = self.problemdata.params.fct_glob['convection']
+            beta = self.convection_fct
             rhs = np.zeros(x.shape)
             for i in range(self.mesh.dimension):
                 rhs += beta[i](x,y,z) * solexact.d(i, x, y, z)
                 rhs -= kheat * solexact.dd(i, i, x, y, z)
             return rhs
         def _fctu2(x, y, z):
             kheat = self.problemdata.params.scal_glob['kheat']
             rhs = np.zeros(x.shape)
             for i in range(self.mesh.dimension):
                 rhs -= kheat * solexact.dd(i, i, x, y, z)
             return rhs
-        if self.convection: return _fctu
+        if self.hasconvection: return _fctu
         return _fctu2
-    def defineNeumannAnalyticalSolution(self, problemdata, color):
-        solexact = problemdata.solexact
+    def defineNeumannAnalyticalSolution(self, problemdata, color, solexact):
+        solexact = solexact[0]
+        # solexact = problemdata.solexact
         def _fctneumann(x, y, z, nx, ny, nz):
             kheat = self.problemdata.params.scal_glob['kheat']
             rhs = np.zeros(x.shape)
             normals = nx, ny, nz
             for i in range(self.mesh.dimension):
                 rhs += kheat * solexact.d(i, x, y, z) * normals[i]
             return rhs
         return _fctneumann
-    def defineRobinAnalyticalSolution(self, problemdata, color):
-        solexact = problemdata.solexact
+    def defineRobinAnalyticalSolution(self, problemdata, color, solexact):
+        solexact = solexact[0]
+        # solexact = problemdata.solexact
         alpha = problemdata.bdrycond.param[color]
         kheat = self.problemdata.params.scal_glob['kheat']
         def _fctrobin(x, y, z, nx, ny, nz):
             rhs = np.zeros(x.shape)
             normals = nx, ny, nz
             rhs += alpha*solexact(x, y, z)
             for i in range(self.mesh.dimension):
@@ -148,116 +181,125 @@
             if not hasattr(self, self.paramname):
                 raise NotImplementedError("{} has no paramater '{}'".format(self, self.paramname))
             cmd = "self.{} = {}".format(self.paramname, param)
             eval(cmd)
 # ================================================================= #
 class EllipticPrimal(EllipticBase):
     def __init__(self, **kwargs):
+        # print(f"{kwargs.keys()=}")
         super().__init__(**kwargs)
     def meshSet(self):
         super().meshSet()
         self.fem.setMesh(self.mesh)
         colorsdirichlet = self.problemdata.bdrycond.colorsOfType("Dirichlet")
         colorsflux = self.problemdata.postproc.colorsOfType("bdry_nflux")
         if self.dirichletmethod!="nitsche":
             self.bdrydata = self.fem.prepareBoundary(colorsdirichlet, colorsflux)
+    def getNcomps(self, mesh):
+        return [1]
     def getSystemSize(self):
-        ncomps = [1]
         ns = [self.fem.nunknowns()]
-        return ncomps, ns
+        return ns
     def computeMassMatrix(self):
         lumped = self.disc_params.get('masslumped', False)
         return self.fem.computeMassMatrix(lumped=lumped)
-    def computeForm(self, u):
+    def computeForm(self, u, coeffmass=None):
         if not hasattr(self, 'A'):
             self.A = self.computeMatrix()
         # du2 = self.A@u
         du = np.zeros_like(u)
         bdrycond = self.problemdata.bdrycond
         colorsrobin = bdrycond.colorsOfType("Robin")
         colorsdir = bdrycond.colorsOfType("Dirichlet")
         self.fem.computeFormDiffusion(du, u, self.kheatcell)
-        if self.convection:
-            self.fem.computeFormConvection(du, u, self.convdata)
-        # if coeffmass is not None:
-        #     self.fem.massDot(du, u, coeff=coeffmass)
+        if self.hasconvection:
+            self.fem.computeFormTransportCellWise(du, u, self.convdata, type='centered')
+            if hasattr(self.fem, "computeFormJump"):
+                self.fem.computeFormJump(du, u, self.convdata.betart)
+            if self.convectionmethod == 'lps':
+                self.fem.computeFormLps(du, u, self.convdata.betart, lpsparam=self.lpsparam)
+        if coeffmass is not None:
+            self.fem.massDot(du, u, coeff=coeffmass)
         self.fem.massDotBoundary(du, u, colorsrobin, bdrycond.param, lumped=True)
         if self.dirichletmethod!="nitsche":
             self.fem.vectorBoundaryStrongEqual(du, u, self.bdrydata)
         else:
             self.fem.computeFormNitscheDiffusion(self.nitscheparam, du, u, self.kheatcell, colorsdir)
         # if not np.allclose(du,du2):
         #     # f = (f"\n{du[self.bdrydata.facesdirall]}\n{du2[self.bdrydata.facesdirall]}")
         #     raise ValueError(f"{np.linalg.norm(du-du2)}\n{du=}\n{du2=}")
         return du
     def computeMatrix(self, u=None, coeffmass=None):
         bdrycond = self.problemdata.bdrycond
         colorsrobin = bdrycond.colorsOfType("Robin")
         colorsdir = bdrycond.colorsOfType("Dirichlet")
         A = self.fem.computeMatrixDiffusion(self.kheatcell)
-        if self.dirichletmethod=="nitsche":
-            A += self.fem.computeMatrixNitscheDiffusion(self.nitscheparam, diffcoff=self.kheatcell, colors=colorsdir)
+        # if self.dirichletmethod=="nitsche":
+        #     A += self.fem.computeMatrixNitscheDiffusion(self.nitscheparam, diffcoff=self.kheatcell, colors=colorsdir)
         A += self.fem.computeBdryMassMatrix(colorsrobin, bdrycond.param, lumped=True)
-        if self.convection:
-            A += self.fem.computeMatrixConvection(self.convdata)
+        if self.hasconvection:
+            A += self.fem.computeMatrixTransportCellWise(self.convdata, type='centered')
+            if hasattr(self.fem, 'computeMatrixJump'):
+                A += self.fem.computeMatrixJump(self.convdata.betart)
+            if self.convectionmethod == 'lps':
+                A += self.fem.computeMatrixLps(self.convdata.betart, lpsparam=self.lpsparam)
         if coeffmass is not None:
             A += self.fem.computeMassMatrix(coeff=coeffmass)
         # if hasattr(self, 'bdrydata'):
-        if hasattr(self, 'bdrydata'):
+        if self.dirichletmethod!="nitsche":
+        # if hasattr(self, 'bdrydata') and self.dirichletmethod=="strong":
             # print(f"{self.bdrydata=}")
-            assert self.dirichletmethod!="nitsche"
+            # assert self.dirichletmethod!="nitsche"
             A = self.fem.matrixBoundaryStrong(A, self.bdrydata)
+        else:
+            A += self.fem.computeMatrixNitscheDiffusion(self.nitscheparam, diffcoff=self.kheatcell, colors=colorsdir)
         return A
     def computeRhs(self, b=None, coeffmass=None, u=None):
         if b is None:
             b = np.zeros(self.fem.nunknowns())
         else:
             if b.shape[0] != self.fem.nunknowns(): raise ValueError(f"{b.shape=} {self.fem.nunknowns()=}")
         bdrycond = self.problemdata.bdrycond
         colorsrobin = bdrycond.colorsOfType("Robin")
         colorsdir = bdrycond.colorsOfType("Dirichlet")
         colorsneu = bdrycond.colorsOfType("Neumann")
         if 'rhs' in self.problemdata.params.fct_glob:
             fp1 = self.fem.interpolate(self.problemdata.params.fct_glob['rhs'])
             self.fem.massDot(b, fp1)
-            if hasattr(self, 'convdata'): self.fem.massDotSupg(b, fp1, self.convdata)
+            # if hasattr(self, 'convdata'): self.fem.massDotSupg(b, fp1, self.convdata)
         if 'rhscell' in self.problemdata.params.fct_glob:
             fp1 = self.fem.interpolateCell(self.problemdata.params.fct_glob['rhscell'])
             self.fem.massDotCell(b, fp1)
         if 'rhspoint' in self.problemdata.params.fct_glob:
             self.fem.computeRhsPoint(b, self.problemdata.params.fct_glob['rhspoint'])
         if self.dirichletmethod=="nitsche":
             self.fem.computeRhsNitscheDiffusion(self.nitscheparam, b, self.kheatcell, colorsdir, udir=None, bdrycondfct=bdrycond.fct)
         else:
             self.fem.vectorBoundaryStrong(b, bdrycond, self.bdrydata)
-        if self.convection:
-            fp1 = self.fem.interpolateBoundary(self.mesh.bdrylabels.keys(), bdrycond.fct)
+        if self.hasconvection:
+            # fp1 = self.fem.interpolateBoundary(self.mesh.bdrylabels.keys(), bdrycond.fct)
+            fp1 = self.fem.interpolateBoundary(colorsdir, bdrycond.fct)
             self.fem.massDotBoundary(b, fp1, coeff=-np.minimum(self.convdata.betart, 0))
         #Fourier-Robin
         fp1 = self.fem.interpolateBoundary(colorsrobin, bdrycond.fct, lumped=True)
         # self.fem.massDotBoundary(b, fp1, colors=colorsrobin, lumped=True, coeff=bdrycond.param)
         self.fem.massDotBoundary(b, fp1, colors=colorsrobin, lumped=True, coeff=1)
         #Neumann
         fp1 = self.fem.interpolateBoundary(colorsneu, bdrycond.fct)
         self.fem.massDotBoundary(b, fp1, colorsneu)
         if coeffmass is not None:
             assert u is not None
             self.fem.massDot(b, u, coeff=coeffmass)
         if hasattr(self, 'bdrydata'):
             self.fem.vectorBoundaryStrong(b, bdrycond, self.bdrydata)
         return b
-    def sol_to_data(self, u):
-        data = {'point': {}, 'cell': {}, 'global': {}}
-        # point_data, side_data, cell_data, global_data = {}, {}, {}, {}
-        data['point']['U'] = self.fem.tonode(u)
-        return data
     def postProcess(self, u):
         data = {'scalar':{}}
-        solexact = self.application.exactsolution
-        if solexact:
+        if self.application.exactsolution:
+            solexact = self.application.exactsolution[0]
             data['scalar']['err_L2c'], ec = self.fem.computeErrorL2Cell(solexact, u)
             data['scalar']['err_L2n'], en = self.fem.computeErrorL2 (solexact, u)
             data['scalar']['err_H1'] = self.fem.computeErrorFluxL2  (solexact, u)
             data['scalar']['err_Flux'] = self.fem.computeErrorFluxL2(solexact, u, self.kheatcell)
             data['cell'] = {}
             data['cell']['err'] = ec
         if self.problemdata.postproc:
@@ -279,88 +321,68 @@
                 elif type == types[4]:
                     data['scalar'][name] = self.fem.computeMeanValues(u, colors)
                 elif type == types[5]:
                     data['scalar'][name] = self.fem.computeLineValues(u, colors)
                 else:
                     raise ValueError(f"unknown postprocess type '{type}' for key '{name}'\nknown types={types=}")
         return data
-    def pyamg_solver_args(self, maxiter):
-        if self.convection:
-            return {'cycle': 'V', 'maxiter': maxiter, 'tol': 1e-10, 'accel': 'bicgstab'}
-        return {'cycle': 'V', 'maxiter': maxiter, 'tol': 1e-10, 'accel': 'cg'}
-    def build_pyamg(self, A):
-        try:
-            import pyamg
-        except:
-            raise ImportError(f"*** pyamg not found {self.linearsolver=} ***")
-        # return pyamg.smoothed_aggregation_solver(A)
-        B = np.ones((A.shape[0], 1))
-        B = pyamg.solver_configuration(A, verb=False)['B']
-        if self.convection:
-            symmetry = 'nonsymmetric'
-            # smoother = 'gauss_seidel_nr'
-            smoother = 'gauss_seidel'
-            smoother = 'block_gauss_seidel'
-            smoother = 'strength_based_schwarz'
-            smoother = 'schwarz'
-            # smooth = ('energy', {'krylov': 'fgmres'})
-            smooth = ('energy', {'krylov': 'bicgstab'})
-            # improve_candidates =[ (smoother, {'sweep': 'symmetric', 'iterations': 4}), None]
-            improve_candidates = None
+    def pyamg_solver_args(self, args):
+        if self.hasconvection:
+            args['symmetric'] = False
+            args['smoother'] = 'schwarz'
         else:
-            symmetry = 'hermitian'
-            smooth = ('energy', {'krylov': 'cg'})
-            smoother = 'gauss_seidel'
-            # improve_candidates =[ ('gauss_seidel', {'sweep': 'symmetric', 'iterations': 4}), None]
-            improve_candidates = None
-        # strength = [('evolution', {'k': 2, 'epsilon': 10.0})]
-        strength = [('symmetric', {'theta': 0.05})]
-        psmoother = (smoother, {'sweep': 'symmetric', 'iterations': 1})
-        # psmoother = (smoother, {'maxiter': 10})
-        SA_build_args = {
-            'max_levels': 10,
-            'max_coarse': 25,
-            'coarse_solver': 'pinv2',
-            'symmetry': symmetry,
-            'smooth': smooth,
-            'strength': strength,
-            'presmoother': psmoother,
-            'presmoother': psmoother,
-            'improve_candidates': improve_candidates,
-            'diagonal_dominance': False
-        }
-        # return pyamg.smoothed_aggregation_solver(A, B, **SA_build_args)
-        return pyamg.rootnode_solver(A, B, **SA_build_args)
+            args['symmetric'] = True
 # ================================================================= #
 class EllipticMixed(EllipticBase):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
     def meshSet(self):
         super().meshSet()
         self.pureneumann = not ('Dirichlet' in self.problemdata.bdrycond.type.values() or 'Robin' in self.problemdata.bdrycond.type.values())
         # print(f"{self.pureneumann=} {self.dirichletmethod=}")
         self.rt.setMesh(self.mesh)
         self.d0.setMesh(self.mesh)
         colorsneumann = self.problemdata.bdrycond.colorsOfType("Neumann")
         self.bdrydata = self.rt.prepareBoundary(colorsneumann)
         self.divcoeffinv = 1/self.kheatcell
+    def tofemvector(self, u):
+        assert 0
+
+        # def sol_to_data(self, u):
+        #     nfaces, dim = self.mesh.nfaces, self.mesh.dimension
+        #     v = self.vectorview.get_part(0, u)
+        #     p = self.vectorview.get_part(1, u)
+        #     # sigma, u = uin[0], uin[1]
+        #     # sigma, u = u[:nfaces], u[nfaces:]
+        #     data = {'point': {}, 'cell': {}, 'global': {}}
+        #     # point_data, side_data, cell_data, global_data = {}, {}, {}, {}
+        #     data['cell']['p'] = p
+        #     vc = self.rt.toCell(v)
+        #     pn = self.rt.reconstruct(p, vc, self.divcoeffinv)
+        #     data['point']['pn'] = pn
+        #     for i in range(dim):
+        #         data['cell']['v{:1d}'.format(i)] = vc[:, i]
+        #     return data
+
+        return fems.femvector.FemVector(data = u, vectorview=self.vectorview, fems=[self.fem])
+    def getNcomps(self, mesh):
+        return [1, 1]
     def getSystemSize(self):
-        ncomps = [1, 1]
         ns = [self.rt.nunknowns(), self.d0.nunknowns()]
-        return ncomps, ns
+        return ns
     # def computeForm(self, u, coeffmass=None):
     #     raise NotImplementedError(f"computeForm for rt")
     def computeMatrix(self, u=None, coeffmass=None):
         # print("Hallo computeMatrix")
         bdrycond = self.problemdata.bdrycond
         colorsrobin = bdrycond.colorsOfType("Robin")
         A = self.rt.constructMass(diffinvcell=self.divcoeffinv)
         B = self.rt.constructDiv()
         A += self.rt.computeBdryMassMatrix(colorsrobin, bdrycond.param)
-        if self.convection:
+        if self.hasconvection:
             raise NotImplementedError(f"convection for rt")
         if coeffmass is not None:
             raise NotImplementedError(f"recation for rt")
         if self.pureneumann:
             A, B, self.bdrydata = self.rt.matrixNeumann(A, B, self.bdrydata)
         positions = [[{'pos':(0,0)}], [{'pos':(1,0)}, {'pos':(0,1), 'trp':True, 'scl':1}]]
         return matrixsystem.MatrixSystem(self.vectorview, [A,B], positions)
@@ -390,28 +412,30 @@
             nx, ny, nz = normalsS.T
             try:
                 ud = bdrycond.fct[color](xf, yf, zf, nx, ny, nz)
             except:
                 ud = bdrycond.fct[color](xf, yf, zf)
             if color in colorsrobin: dS /= bdrycond.param[color]
             bsides[faces] += dS * ud
-            if self.convection:
+            if self.hasconvection:
                 faces = self.mesh.bdrylabels[color]
-                normalsS = self.mesh.normals[faces]
-                dS = np.linalg.norm(normalsS, axis=1)
-                normalsS = normalsS / dS[:, np.newaxis]
-                xf, yf, zf = self.mesh.pointsf[faces].T
-                beta = np.array(self.convection(xf, yf, zf))
-                # print("beta", beta)
-                # print("normalsS", normalsS.T)
-                bn = np.einsum("ij,ij->j", beta, normalsS.T)
-                # print("bn", bn)
-                bn[bn<=0] = 0
+                # normalsS = self.mesh.normals[faces]
+                # dS = np.linalg.norm(normalsS, axis=1)
+                # normalsS = normalsS / dS[:, np.newaxis]
+                # xf, yf, zf = self.mesh.pointsf[faces].T
+                # beta = np.array(self.convection(xf, yf, zf))
+                # bn = np.einsum("ij,ij->j", beta, normalsS.T)
+                # # print("bn", bn)
+                # bn[bn<=0] = 0
                 cells = self.mesh.cellsOfFaces[faces,0]
-                bcells[cells] += bn*ud*dS
+                # bcells[cells] += bn*ud*dS
+
+                bn = self.convdata.betart[faces]
+                bcells[cells] += bn*ud
+
         help = np.zeros(self.mesh.nfaces)
         for color in colorsneu:
             if not color in bdrycond.fct or not bdrycond.fct[color]: continue
             faces = self.mesh.bdrylabels[color]
             normalsS = self.mesh.normals[faces]
             dS = np.linalg.norm(normalsS, axis=1)
             normalsS = normalsS / dS[:, np.newaxis]
@@ -422,29 +446,14 @@
         # print(f"{type(self.bdrydata.A_inner_neum)=}")
         if self.pureneumann:
             bsides[self.bdrydata.facesinner] -= self.bdrydata.A_inner_neum*help[self.bdrydata.facesneumann]
             bsides[self.bdrydata.facesneumann] += self.bdrydata.A_neum_neum*help[self.bdrydata.facesneumann]
             bcells -= self.bdrydata.B_inner_neum*help[self.bdrydata.facesneumann]
         return b
         # return bsides, bcells
-    def sol_to_data(self, u):
-        nfaces, dim =  self.mesh.nfaces, self.mesh.dimension
-        v = self.vectorview.get_part(0, u)
-        p = self.vectorview.get_part(1, u)
-        # sigma, u = uin[0], uin[1]
-        # sigma, u = u[:nfaces], u[nfaces:]
-        data = {'point':{}, 'cell':{}, 'global':{}}
-        # point_data, side_data, cell_data, global_data = {}, {}, {}, {}
-        data['cell']['p'] = p
-        vc = self.rt.toCell(v)
-        pn = self.rt.reconstruct(p, vc, self.divcoeffinv)
-        data['point']['pn'] = pn
-        for i in range(dim):
-            data['cell']['v{:1d}'.format(i)] = vc[:, i]
-        return data
     def postProcess(self, u):
         nfaces, dim =  self.mesh.nfaces, self.mesh.dimension
         v = self.vectorview.get_part(0, u)
         p = self.vectorview.get_part(1, u)
         vc = self.rt.toCell(v)
         pn = self.rt.reconstruct(p, vc, self.divcoeffinv)
         data = {}
```

### Comparing `simfempy-2.1.1/simfempy/models/model.py` & `simfempy-2.2.2/simfempy/models/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # import simfempy.tools.analyticalfunction
 import simfempy.tools.timer
 import simfempy.tools.iterationcounter
 import simfempy.models.problemdata
 from simfempy.tools.analyticalfunction import AnalyticalFunction
 import simfempy.solvers
 from simfempy.linalg import vectorview
+from simfempy import fems
 
 # import warnings
 # warnings.filterwarnings("error")
 
 #=================================================================#
 class Model(object):
     def __format__(self, spec):
@@ -44,32 +45,24 @@
         self.mode = kwargs.pop('mode', 'linear')
         self.verbose = kwargs.pop('verbose', 0)
         self.timer = simfempy.tools.timer.Timer(verbose=self.verbose)
         self.application = kwargs.pop('application', None)
         if self.application is None:
             raise ValueError(f"Model needs application (since 22/04/23)")
         self.problemdata = self.application.problemdata
-        self.ncomp = self.problemdata.ncomp
+        # self._setMeshCalled = True
         if not hasattr(self,'linearsolver'):
             self.linearsolver = kwargs.pop('linearsolver', 'spsolve')
         self.disc_params = kwargs.pop('disc_params', {})
-        print(f"Model {self.disc_params=}")
-        self.createFem()
-        self.setMesh(self.application.createMesh())
-        self.application.createExactSolution(self.mesh)
-        if self.application.generatePDforES:
-            self.generatePoblemDataForAnalyticalSolution()
-        # print(f"{self.__class__.__name__} {self.stack_storage=} {self.singleA=} {self.mesh=} {self.linearsolver=}")
         if not hasattr(self,'scale_ls'):
-            self.scale_ls = kwargs.pop('scale_ls', True)
-        print(f"{self.scale_ls=}")
+            self.scale_ls = kwargs.pop('scale_ls', False)
         if 'newton_stopping_parameters' in kwargs:
             self.newton_stopping_parameters = kwargs.pop('newton_stopping_parameters')
         else:
-            maxiter = kwargs.pop('newton_maxiter', 10)
+            maxiter = kwargs.pop('newton_maxiter', 100)
             rtol = kwargs.pop('newton_rtol', 1e-6)
             self.newton_stopping_parameters = simfempy.solvers.newtondata.StoppingParamaters(maxiter=maxiter, rtol=rtol)
         if isinstance(self.linearsolver, str):
             self.newton_stopping_parameters.addname = self.linearsolver
         else:
             self.newton_stopping_parameters.addname = self.linearsolver['method']
         datadir_def_name = f"{self.__class__.__name__}"+f"_{self.application.__class__.__name__}"
@@ -80,79 +73,71 @@
         if kwargs.pop("clean_data",True):
             try: shutil.rmtree(self.datadir)
             except: pass
         pathlib.Path(self.datadir).mkdir(parents=True, exist_ok=True)
         with open(self.datadir / "model", "w") as file:
             file.write(str(self))
         # check for unused arguments
+        if 'mesh' in kwargs.keys():
+            self.mesh = kwargs.pop('mesh')
+        else:
+            self.mesh =self.application.createMesh()
+        # print(f"{kwargs.keys()=}")
         if len(kwargs.keys()):
             raise ValueError(f"*** unused arguments {kwargs=}")
-    def createFem(self):
-        raise NotImplementedError(f"createFem has to be overwritten")
+        self.createFem()
+        self.setMesh(self.mesh)
     def setMesh(self, mesh):
-        self._setMeshCalled = True
-        self.timer.reset_all()
-        self.problemdata.check(mesh)
         self.mesh = mesh
+        self.timer.reset_all()
+        self.problemdata.check(self.mesh)
         if self.verbose: print(f"{self.mesh=}")
         if hasattr(self, 'LS'):
             del self.LS
         if hasattr(self, 'A'):
             del self.A
-        # if hasattr(self,'_generatePDforES') and self._generatePDforES:
-        # if self.application.generatePDforES:
-        #     self.generatePoblemDataForAnalyticalSolution()
-            # self._generatePDforES = False
+        self.ncomps = self.getNcomps(self.mesh)
         self.meshSet()
-        ncomps, ns = self.getSystemSize()
-        # print(f"Model {self.stack_storage=} {ncomps=} {ns=}")
-        self.vectorview = vectorview.VectorView(ncomps=ncomps, ns=ns, stack_storage=self.stack_storage)
+        ns = self.getSystemSize()
+        self.vectorview = vectorview.VectorView(ncomps=self.ncomps, ns=ns, stack_storage=self.stack_storage)
+        if not hasattr(self, "exactsolution_created"):
+            if self.application.exactsolution is not None:
+                self.exactsolution_created=True
+                self.application.createExactSolution(self.mesh, self.ncomps)
+            if self.application.generatePDforES:
+                self.generatePoblemDataForAnalyticalSolution()
+    def tofemvector(self, u):
+        return fems.femvector.FemVector(data = u, vectorview=self.vectorview, fems=[self.fem])
+    def createFem(self):
+        raise NotImplementedError(f"createFem has to be overwritten")
     def solve(self):
         if self.mode=='dynamic':
             return self.dynamic()
         return self.static(method=self.mode)
-    # def setParameter(self, paramname, param):
-    #     assert 0
-    def dirichletfct(self):
-        if self.ncomp > 1:
-            # def _solexactdir(x, y, z):
-            #     return [self.application.exactsolution[icomp](x, y, z) for icomp in range(self.ncomp)]
-            # return _solexactdir
+    def defineDirichletAnalyticalSolution(self, problemdata, color, solexact):
+        ncomp = self.ncomps[0]
+        if ncomp==1:
+            return solexact[0]
+        else:
             from functools import partial
             solexact = self.application.exactsolution
             def _solexactdir(x, y, z, icomp):
                 return solexact[icomp](x, y, z)
-            return [partial(_solexactdir, icomp=icomp) for icomp in range(self.ncomp)]
-        else:
-            return self.application.exactsolution
-            def _solexactdir(x, y, z):
-                return self.application.exactsolution(x, y, z)
-        return _solexactdir
+            return [partial(_solexactdir, icomp=icomp) for icomp in range(ncomp)]
     def generatePoblemDataForAnalyticalSolution(self):
         bdrycond = self.problemdata.bdrycond
-        # self.application.exactsolution = self.defineAnalyticalSolution(exactsolution=self.application.exactsolution, random=self.application.random_exactsolution)
-        # print("self.application.exactsolution", self.application.exactsolution)
+        print(f"{self.application.exactsolution=} {self.mesh.bdrylabels=}")
         solexact = self.application.exactsolution
         self.problemdata.params.fct_glob['rhs'] = self.defineRhsAnalyticalSolution(solexact)
         if hasattr(self, 'time'):
             self.problemdata.params.fct_glob['initial_condition'] = self.defineInitialConditionAnalyticalSolution(solexact)
         for color in self.mesh.bdrylabels:
-            if color in bdrycond.type and bdrycond.type[color] in ["Dirichlet","dirichlet"]:
-                bdrycond.fct[color] = self.dirichletfct()
-            else:
-                if color in bdrycond.type:
-                    cmd = "self.define{}AnalyticalSolution(self.problemdata,{})".format(bdrycond.type[color], color)
-                    # print(f"cmd={cmd}")
-                    bdrycond.fct[color] = eval(cmd)
-                else:
-                    bdrycond.fct[color] = self.defineBdryFctAnalyticalSolution(color, solexact)
-    # def defineAnalyticalSolution(self, exactsolution, random=True):
-    #     dim = self.mesh.dimension
-    #     # print(f"defineAnalyticalSolution: {dim=} {self.ncomp=}")
-    #     return simfempy.tools.analyticalfunction.analyticalSolution(exactsolution, dim, self.ncomp, random)
+            cmd = f"self.define{bdrycond.type[color]}AnalyticalSolution(self.problemdata,{color},solexact)"
+            # print(f"cmd={cmd}")
+            bdrycond.fct[color] = eval(cmd)
     def compute_cell_vector_from_params(self, name, params):
         if name in params.fct_glob:
             fct = np.vectorize(params.fct_glob[name])
             arr = np.empty(self.mesh.ncells)
             for color, cells in self.mesh.cellsoflabel.items():
                 xc, yc, zc = self.mesh.pointsc[cells].T
                 arr[cells] = fct(color, xc, yc, zc)
@@ -168,43 +153,46 @@
         return arr
     def initsolution(self, b):
         if isinstance(b,tuple):
             # raise KeyError("i don't know how to handle {type(b)=}")
             return [np.copy(bi) for bi in b]
         return b.copy()
     def computelinearSolver(self, A):
-        print(f"{self.linearsolver=} {self.scale_ls=}")
+        # print(f"{self.linearsolver=} {self.scale_ls=}")
         if isinstance(self.linearsolver,str):
             args = {'method': self.linearsolver}
         else:
             args = self.linearsolver.copy()
         # args['matrix'] = A
         if args['method'] != 'spsolve':
             if self.scale_ls:
                 if hasattr(A, 'scale_matrix'):
                     A.scale_matrix()
                 args['scale'] = self.scale_ls
             args['matrix'] = A
             if args['method'] != 'pyamg':
                 if hasattr(A,'matvec'):
-                    args['matvec'] = A.matvec
+                    # args['matvec'] = A.matvec
                     args['n'] = A.nall
                 else:
-                    args['matvec'] = lambda x: np.matmul(A,x)
+                    # args['matvec'] = lambda x: np.matmul(A,x)
                     args['n'] = A.shape[0]
+            else:
+                self.pyamg_solver_args(args)
+        # print(f"{args=}")
         return simfempy.linalg.linalg.getLinearSolver(**args)
     def static(self, **kwargs):
         method = kwargs.pop('method','newton')
         # raise ValueError(f"{method=}")
         u = kwargs.pop('u',None)
         if 'maxiter' in kwargs: self.newton_stopping_parameters.maxiter = kwargs.pop('maxiter')
         if 'rtol' in kwargs: self.newton_stopping_parameters.rtol = kwargs.pop('rtol')
         self.timer.reset_all()
         result = simfempy.models.problemdata.Results()
-        if not self._setMeshCalled: self.setMesh(self.mesh)
+        # if not self._setMeshCalled: self.setMesh(self.mesh)
         self.timer.add('setMesh')
         self.b = kwargs.pop('b',self.computeRhs())
         # self.b = self.computeRhs()
         # raise ValueError(f"{self.b.shape=}")
         if u is None:
             u = self.initsolution(self.b)
         self.timer.add('rhs')
@@ -259,25 +247,26 @@
                 raise ValueError(f"unknwon {method=}")
         pp = self.postProcess(u)
         if hasattr(self.application, "changepostproc"):
             self.application.changepostproc(pp['scalar'])
         self.timer.add('postp')
         result.setData(pp, timer=self.timer, iter=iter)
         self.save(u=u)
-        return result, u
+        return result, self.tofemvector(u)
     def computeDefect(self, u):
+        # print(f"{np.linalg.norm(self.b)=} {np.linalg.norm(u)=}")
         return self.computeForm(u)-self.b
     def computeForm(self, u):
         print(f"{type(self.A)=} {type(u)=}")
         return self.A@u
     def initialCondition(self, interpolate=True):
         #TODO: higher order interpolation
         if not 'initial_condition' in self.problemdata.params.fct_glob:
             raise ValueError(f"missing 'initial_condition' in {self.problemdata.params.fct_glob=}")
-        if not self._setMeshCalled: self.setMesh(self.mesh)
+        # if not self._setMeshCalled: self.setMesh(self.mesh)
         ic = AnalyticalFunction(self.problemdata.params.fct_glob['initial_condition'])
         fp1 = self.fem.interpolate(ic)
         if interpolate:
             return fp1
         if not hasattr(self, 'Mass'):
             self.Mass = self.fem.computeMassMatrix()
         b = np.zeros(self.fem.nunknowns())
@@ -295,17 +284,19 @@
         rhs += (1 / theta) * self.computeRhs()
     def newMatrix(self, u):
         if not hasattr(self, 'timeiter'):
             coeffmass = None
         else:
             coeffmass = self.coeffmass
         self.A = self.computeMatrix(u=u, coeffmass=coeffmass)
-        # print(f"{self.A=}")
-        if hasattr(self.A, 'scale_matrix'):
+        if hasattr(self.A, 'scale_matrix') and self.scale_ls:
             self.A.scale_matrix()
+        # print(f"{self.A=}")
+        # if hasattr(self.A, 'scale_matrix'):
+        #     self.A.scale_matrix()
         if hasattr(self, 'LS'):
             # self.LS = self.computelinearSolver(self.A)
             self.LS.update(self.A)
         else:
             self.LS = self.computelinearSolver(self.A)
     def computeDx(self, b, u, info):
         computeMatrix = False
@@ -313,21 +304,23 @@
             computeMatrix=True
         if hasattr(self, 'timeiter') and self.timeiter==0 and info.iter==0:
             computeMatrix=True
         elif hasattr(self, 'timeiter') and info.bad_convergence:
             computeMatrix = True
         if computeMatrix:
             self.newMatrix(u)
+        # print(f"{computeMatrix=}")
+        # assert hasattr(self.LS, 'scalings')
         rtol = 1e-7
         if hasattr(info,'rhor'):
             rtol = min(0.01, info.rhor)
             rtol = max(rtol, info.tol_missing)
         try:
             # raise ValueError(f"{rtol=} {info=}")
-            print(f"{rtol=}")
+            # print(f"{rtol=}")
             du = self.LS.solve(A=self.A, b=b, rtol=rtol)
             niter = self.LS.niter
             if niter==self.LS.maxiter:
                 return du, niter, False
         except Warning:
             raise ValueError(f"matrix is singular {self.A.shape=} {self.A.diagonal()=}")
         self.timer.add('solve_linear')
@@ -361,15 +354,14 @@
         rtolnewton = kwargs.pop('rtolnewton', 1e-3)
         rtolsemi_imp = kwargs.pop('rtolsemi_imp', 1e-8)
         sdata = kwargs.pop('sdata', simfempy.solvers.newtondata.StoppingParamaters(maxiter=maxiternewton, rtol=rtolnewton))
         output_vtu = kwargs.pop('output_vtu', False)
         semi_implicit = kwargs.pop('semi_implicit', False)
         if len(kwargs):
             raise ValueError(f"unused arguments: {kwargs.keys()}")
-
         if not dt or dt<=0: raise NotImplementedError(f"needs constant positive 'dt")
         result = simfempy.models.problemdata.Results(nframes)
         # self.timer.add('init')
         # self.timer.add('matrix')
         u = u0
         self.time = t_span[0]
         # rhs=None
@@ -380,16 +372,21 @@
             sdata.addname = self.linearsolver['method']
         if not hasattr(self, 'Mass'):
             self.Mass = self.computeMassMatrix()
         self.coeffmass = 1 / dt / theta
         # print(f"dynamic {self.coeffmass=}")
         if not hasattr(self, 'Aconst'):
             Aconst = self.computeMatrixConstant(coeffmass=self.coeffmass)
-            if self.linearsolver=="pyamg":
-                self.pyamgml = self.build_pyamg(Aconst)
+            if hasattr(self, 'LS'):
+                # self.LS = self.computelinearSolver(self.A)
+                self.LS.update(Aconst)
+            else:
+                self.LS = self.computelinearSolver(Aconst)
+            # if self.linearsolver=="pyamg":
+            #     self.pyamgml = self.build_pyamg(Aconst)
         self.theta, self.dt = theta, dt
         times = np.linspace(t_span[0], t_span[1], nframes+1)
         count_smallres = 0
         self.timeiter = 0
         info_new = simfempy.solvers.newtondata.IterationData(rtolsemi_imp)
         if verbose:
             print(30*"*" + f" {theta=} "+30*"*")
@@ -450,15 +447,16 @@
                     if dt <= dtmin:
                         raise ValueError(f"giving up {dt=}")
                     self.dt = dt
                     coeffmassold = self.coeffmass
                     self.coeffmass = 1 / dt / theta
                     Aconst = self.computeMatrixConstant(coeffmass=self.coeffmass, coeffmassold=coeffmassold)
                     self.A = self.computeMatrix(u=u, coeffmass=self.coeffmass)
-                    self.A.scale_matrix()
+                    if hasattr(self.A, 'scale_matrix') and self.scale_ls:
+                        self.A.scale_matrix()
                     self.LS.update(self.A)
                     print(f"*** {info_new.failure=} {dtold=} {dt=}")
                     info_new.success = True
 
                 # self.timer.add('solve')
                 self.timeiter += 1
             if verbose:
@@ -484,15 +482,14 @@
         self.save(u=u, iter=iframe)
         if output_vtu:
             data = self.sol_to_data(u)
             filename = "sol" + f"_{iframe:05d}" + ".vtu"
             self.mesh.write(self.datadir / filename, data=data)
         result.save(self.datadir)
         return result
-
     def dynamic_linear(self, u0, t_span, nframes, dt=None, callback=None, method='CN', verbose=1):
         # TODO: passing time
         """
         u_t + A u = f, u(t_0) = u_0
         M(u^{n+1}-u^n)/dt + a Au^{n+1} + (1-a) A u^n = (f^{n+1}-f^n)/2
         (M/dt+aA) u^{n+1} =  f + (M/dt -(1-a)A)u^n
                           =  f + 1/a (M/dt) u^n - (1-a)/a (M/dt+aA)u^n
@@ -565,24 +562,20 @@
     def load(self, iter=None, datadir=None, name= "sol", add=''):
         if add: name += add
         if iter is not None: name += f"_{iter:05d}"
         if datadir is None: datadir=self.datadir
         name += ".npy"
         return np.load(datadir/name)
     def load_data(self, iter=None, datadir=None, name= "sol", add=''):
-        if add: name += add
-        if iter is not None: name += f"_{iter:05d}"
-        if datadir is None: datadir=self.datadir
-        name += ".npy"
-        return self.sol_to_data(np.load(datadir/name))
+        u = self.tofemvector(self.load(iter, datadir, name, add))
+        return u.tovisudata()
     def get_t(self, datadir=None):
         if datadir is None: datadir=self.datadir
         times = np.load(self.datadir / "time.npy")
         return times
-
     def get_postprocs_dynamic(self):
         data = {'time': np.load(self.datadir/"time.npy"), 'postproc':{}}
         from pathlib import Path
         p = Path(self.datadir)
         for q in p.glob('postproc*.npy'):
             pname = '_'.join(str(q.parts[-1]).split('.')[0].split('_')[1:])
             # print(f"{pname=} {q=}")
```

### Comparing `simfempy-2.1.1/simfempy/models/navierstokes.py` & `simfempy-2.2.2/simfempy/models/navierstokes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 import numpy as np
 from simfempy.models.stokes import Stokes
 from simfempy import fems, meshes, solvers
 from simfempy.linalg import linalg
 
+linearsolver_def = {'method': 'scipy_lgmres', 'maxiter': 20, 'prec': 'Chorin', 'disp': 0, 'rtol': 1e-3}
+
+#=================================================================#
 class NavierStokes(Stokes):
     def __format__(self, spec):
         if spec=='-':
             repr = super().__format__(spec)
-            repr += f"\tconvmethod={self.convmethod}"
+            # repr += f"\tconvmethod={self.convmethod}"
             return repr
         return self.__repr__()
     def __init__(self, **kwargs):
-        self.linearsolver_def = {'method': 'scipy_lgmres', 'maxiter': 10, 'prec': 'Chorin', 'disp':0, 'rtol':1e-3}
+        self.linearsolver_def = linearsolver_def
         self.mode='nonlinear'
         self.convdata = fems.data.ConvectionData()
         # self.convmethod = kwargs.pop('convmethod', 'lps')
-        self.convmethod = kwargs.get('convmethod', 'lps')
-        self.lpsparam = kwargs.pop('lpsparam', 0.)
-        self.newtontol = kwargs.pop('newtontol', 0)
+        # self.lpsparam = kwargs.pop('lpsparam', 0.1)
+        # self.newtontol = kwargs.pop('newtontol', 0)
         if not 'linearsolver' in kwargs: kwargs['linearsolver'] = self.linearsolver_def
         super().__init__(**kwargs)
-        self.newmatrix = 0
-    def new_params(self):
-        super().new_params()
+        # self.newmatrix = 0
         self.Astokes = super().computeMatrix()
+        if self.scale_ls:
+            raise ValueError(f"*** not working ")
+
+    # def new_params(self):
+    #     super().new_params()
+    #     # self.Astokes = super().computeMatrix()
     def solve(self):
         sdata = solvers.newtondata.StoppingParamaters(maxiter=200, steptype='bt', nbase=1, rtol=self.newtontol)
         return self.static(mode='newton',sdata=sdata)
     def computeForm(self, u):
-        d = self.Astokes.matvec(u)
+        d = super().computeForm(u)
+        np.allclose(d, self.Astokes.matvec(u))
+        # d = self.Astokes.matvec(u)
         v = self.vectorview.get_part(0,u)
         dv = self.vectorview.get_part(0,d)
+        # print(f"{np.linalg.norm(v)=} {np.linalg.norm(dv)=}")
         # v = self._split(u)[0]
         # dv = self._split(d)[0]
         self.computeFormConvection(dv, v)
         self.timer.add('form')
         return d
     def rhs_dynamic(self, rhs, u, Aconst, time, dt, theta, semi_implicit):
         super().rhs_dynamic(rhs, u, Aconst, time, dt, theta, semi_implicit)
         if semi_implicit:
             self.computeFormConvection(rhs, 0.5*u)
-
-
     def computeMatrix(self, u=None, coeffmass=None):
+        return self.Astokes
+        import copy
+        X = copy.deepcopy(self.Astokes)
         # X = self.Astokes.copy()
-        X = super().computeMatrix(u=u, coeffmass=coeffmass)
+        # X = super().computeMatrix(u=u, coeffmass=coeffmass)
         # v = self._split(u)[0]
         v = self.vectorview.get_part(0,u)
         theta = 1
         if hasattr(self,'uold'): theta = 0.5
         X.A += theta*self.computeMatrixConvection(v)
         self.timer.add('matrix')
         return X
@@ -60,16 +70,17 @@
         return y
     def computeMatrixConstant(self, coeffmass, coeffmassold=0):
         self.Astokes.A  =  self.Mass.addToStokes(coeffmass-coeffmassold, self.Astokes.A)
         return self.Astokes
         return super().computeMatrix(u, coeffmass)
     def _compute_conv_data(self, v):
         rt = fems.rt0.RT0(mesh=self.mesh)
-        self.convdata.betart = rt.interpolateCR1(v, self.stack_storage)
-        self.convdata.beta = rt.toCell(self.convdata.betart)
+        # self.convdata.betart = rt.interpolateCR1(v, self.stack_storage)
+        self.convdata.betart = rt.interpolateFromFem(v, self.femv, self.stack_storage)
+        self.convdata.betacell = rt.toCell(self.convdata.betart)
     def computeFormConvection(self, du, u):
         dim = self.mesh.dimension
         self._compute_conv_data(self.vectorview.get_part(0,u))
         colorsdirichlet = self.problemdata.bdrycond.colorsOfType("Dirichlet")
         for icomp in range(dim):
             dv, v = self.vectorview.get(0,icomp,du), self.vectorview.get(0,icomp,u)
             fdict = {col: self.problemdata.bdrycond.fct[col][icomp] for col in colorsdirichlet if col in self.problemdata.bdrycond.fct.keys()}
@@ -79,19 +90,19 @@
             self.femv.computeFormJump(dv, v, self.convdata.betart)
     def computeMatrixConvection(self, v):
         if not hasattr(self.convdata,'beta'): self._compute_conv_data(v)
         A = self.femv.computeMatrixTransportCellWise(self.convdata, type='centered')
         A += self.femv.computeMatrixJump(self.convdata.betart)
         if self.singleA:
             return A
-        return linalg.matrix2systemdiagonal(A, self.ncomp).tocsr()
+        return linalg.matrix2systemdiagonal(A, self.ncomps[0], self.stack_storage).tocsr()
     def computeBdryNormalFluxNitsche(self, u, colors):
         flux = super().computeBdryNormalFluxNitsche(u,colors)
         if self.convdata.betart is None : return flux
-        ncomp, bdryfct = self.ncomp, self.problemdata.bdrycond.fct
+        ncomp, bdryfct = self.ncomps[0], self.problemdata.bdrycond.fct
         for icomp in range(ncomp):
             fdict = {col: bdryfct[col][icomp] for col in colors if col in bdryfct.keys()}
             vdir = self.femv.interpolateBoundary(colors, fdict)
             v = self.vectorview.get(0, icomp, u)
             for i,color in enumerate(colors):
                 flux[icomp, i] -= self.femv.massDotBoundary(b=None, f=v - vdir, colors=[color],
                                                         coeff=np.minimum(self.convdata.betart, 0))
```

### Comparing `simfempy-2.1.1/simfempy/models/problemdata.py` & `simfempy-2.2.2/simfempy/models/problemdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,40 +29,42 @@
             self.param = {color: None for color in colors}
     def __repr__(self):
         return f"types={self.type}\nfct={self.fct}\nparam={self.param}"
     def clear(self):
         self.type = {}
         self.fct = {}
         self.param = {}
-    # def hasExactSolution(self):
-    #     return hasattr(self, 'fctexact')
+    def convert(self, mesh):
+        if not hasattr(mesh,'labeldict_i2s'): return
+        self.type = {mesh.labeldict_s2i[k]:v for k,v in self.type.items()}
+        self.fct = {mesh.labeldict_s2i[k]: v for k, v in self.fct.items()}
+        self.param = {mesh.labeldict_s2i[k]: v for k, v in self.param.items()}
+
     def colors(self):
         return self.type.keys()
     def types(self):
         return self.type.values()
     def set(self, type, colors, fcts=None):
-        if isinstance(colors, int): colors = [colors]
+        if isinstance(colors, (int,str)): colors = [colors]
+        assert isinstance(colors, (list,tuple))
         for i,color in enumerate(colors):
-            if color in self.type.keys(): raise ValueError(f"attempt to defone {type=}, butalready defined b.c {color} as {self.type[color]=}")
+            if color in self.type.keys(): raise ValueError(f"Attempt to define {color=} for {type=}, but already defined b.c {color} as {self.type[color]=}")
             self.type[color] = type
             if fcts: self.fct[color] = fcts[i]
-    # def colorsOfType(self, type):
-    #     colors = []
-    #     for color, typeofcolor in self.type.items():
-    #         if typeofcolor == type: colors.append(color)
-    #     return colors
     def colorsOfType(self, types):
         if isinstance(types, str): types = [types]
         colors = []
         for color, typeofcolor in self.type.items():
             if typeofcolor in types: colors.append(color)
         return colors
     def check(self, colors):
         colors = set(colors)
         typecolors = set(self.type.keys())
+        if not len(typecolors):
+            raise ValueError(f"*** application should write 'defineProblemData(self, problemdata)'")
         if colors != typecolors: 
             raise ValueError(f"*** problem in boundary conditions mesh {colors=} colors with b.c.={typecolors}")
         # _check2setsequal_(colors, typecolors, "mesh colors", "types")
 
 # ---------------------------------------------------------------- #
 class PostProcess(object):
     """
@@ -104,14 +106,15 @@
     - scal_glob: dictionary name -> float
     - scal_cells dictionary name -> color -> float
     """
     def __init__(self):
         self.fct_glob = {}
         self.scal_glob = {}
         self.scal_cells = {}
+        self.data = {}
     def __repr__(self):
         repr = ""
         if len(self.fct_glob): repr += f" fct_glob={self.fct_glob}"
         if len(self.scal_glob): repr += f" scal_glob={self.scal_glob}"
         if len(self.scal_cells): repr += f" scal_cells={self.scal_cells}"
         return repr[1:]
     def set_scal_cells(self, name, colors, value):
@@ -133,70 +136,64 @@
             if name in self.scal_glob: raise ValueError(f"key '{name}' given twice")
     def paramdefined(self, name):
         return name in self.scal_glob or name in self.scal_cells or name in self.fct_glob
     def update(self, p):
         for k,v in p.fct_glob.items(): self.fct_glob[k] = v
         for k,v in p.scal_glob.items(): self.scal_glob[k] = v
         for k,v in p.scal_cells.items(): self.scal_cells[k] = v
+        for k,v in p.data.items(): self.data[k] = v
 
 
 
 # ---------------------------------------------------------------- #
 class ProblemData(object):
     """
     Contains data for definition of a problem:
     - boundary conditions
     - right-hand sides
     - exact solution (if ever)
     - postprocess
     - params: class Params
     """
-    def __init__(self, bdrycond=None, rhs=None, rhscell=None, rhspoint = None, postproc=None, ncomp=1):
-        self.ncomp=ncomp
+    def __init__(self, bdrycond=None, rhs=None, rhscell=None, rhspoint = None, postproc=None):
         if bdrycond is None: self.bdrycond = BoundaryConditions()
         else: self.bdrycond = bdrycond
         if postproc is None: self.postproc = PostProcess()
         else: self.postproc = postproc
         self.solexact = None
         self.params = Params()
 
     def _split2string(self, string, sep='\n\t\t'):
         return sep+sep.join(str(string).split('\n'))
 
     def __repr__(self):
         repr = f"\n{self.__class__}:"
-        repr += f"\n\tncomp = {self.ncomp}"
         repr += f"\n\tbdrycond:{self._split2string(self.bdrycond)}"
         repr += f"\n\tpostproc:{self._split2string(self.postproc)}"
         # if self.rhs: repr += f"\n\trhs={self.rhs}"
         # if self.rhscell: repr += f"\n\trhscell={self.rhscell}"
         # if self.rhspoint: repr += f"\n\trhspoint={self.rhspoint}"
         if self.solexact: repr += f"\n\tsolexact={self.solexact}"
         repr += f"\n\tparams:{self._split2string(self.params)}"
         return repr
 
     def check(self, mesh):
         colors = mesh.bdrylabels.keys()
-        # colors = list(mesh.bdrylabels.keys())
-        # colors.extend(list(mesh.verticesoflabel.keys()))
-        # colors.extend(list(mesh.linesoflabel.keys()))
+        self.bdrycond.convert(mesh)
         self.bdrycond.check(colors)
         colors = list(colors)
         colors.extend(list(mesh.verticesoflabel.keys()))
         colors.extend(list(mesh.linesoflabel.keys()))
         if self.postproc: self.postproc.check(colors)
         self.params.check(mesh)
 
     def clear(self):
         """
         keeps the boundary condition types and parameters !
         """
-        # self.rhs = None
-        # self.rhscell = None
-        # self.rhspoint = None
         self.solexact = None
         self.postproc = None
         for color in self.bdrycond.fct:
             self.bdrycond.fct[color] = None
 
 # ---------------------------------------------------------------- #
 class Results(object):
```

### Comparing `simfempy-2.1.1/simfempy/models/stokes.py` & `simfempy-2.2.2/simfempy/models/stokes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,87 @@
 import copy
 
 import numpy as np
 import scipy.sparse as sparse
 from simfempy import fems
 from simfempy.models.model import Model
 # from simfempy.tools.analyticalfunction import analyticalSolution
-from simfempy.linalg import linalg, saddle_point, vectorview
+from simfempy.linalg import linalg, saddle_point
 from functools import partial
 
+linearsolver_def = {'method': 'scipy_lgmres', 'maxiter': 100, 'prec': 'Chorin', 'disp': 0, 'rtol': 1e-6}
+
+
 #=================================================================#
 class Stokes(Model):
     """
     """
     def __init__(self, **kwargs):
+        # binz for derived class !!
         if not hasattr(self,'linearsolver_def'):
             self.linearsolver_def = {'method': 'scipy_lgmres', 'maxiter': 100, 'prec': 'Chorin', 'disp':0, 'rtol':1e-6}
         if not hasattr(self,'linearsolver'):
             self.linearsolver = kwargs.pop('linearsolver', self.linearsolver_def)
-        print(f"{self.linearsolver=}")
         self.singleA = kwargs.pop('singleA', True)
         super().__init__(**kwargs)
-        # print(f"{self=}")
+        # print(f"Stokes {self.ncomps=} {self.singleA=} {self.stack_storage=} {self.scale_ls=} {self.linearsolver=}")
+        if not self.singleA and self.scale_ls:
+            raise ValueError(f"*** not working ")
+        if self.linearsolver == 'spsolve' and self.singleA:
+            raise ValueError(f"*** not working ")
+
+    def tofemvector(self, u):
+        femss, names, types = [self.femv, self.femp], ['v', 'p'], ['point', 'cell']
+        if self.pmean:
+            femss.append(None)
+            names.append('lam')
+            types.append('glob')
+        return fems.femvector.FemVector(data = u, vectorview=self.vectorview, fems=femss, names=names, visutypes=types)
+
     def createFem(self):
         self.dirichletmethod = self.disc_params.get('dirichletmethod','nitsche')
         if self.dirichletmethod=='nitsche':
             self.nitscheparam = self.disc_params.get('nitscheparam', 10)
         self.femv = fems.cr1.CR1()
         self.femp = fems.d0.D0()
     def new_params(self):
         self.mucell = self.compute_cell_vector_from_params('mu', self.problemdata.params)
+
     def meshSet(self):
         # super().setMesh(mesh)
         self._checkProblemData()
-        if not self.ncomp[0]==self.mesh.dimension: raise ValueError(f"{self.mesh.dimension=} {self.ncomp=}")
+        # if not self.ncomp[0]==self.mesh.dimension: raise ValueError(f"{self.mesh.dimension=} {self.ncomp=}")
         self.femv.setMesh(self.mesh)
         self.femp.setMesh(self.mesh)
-        self.pmean = not ('Neumann' in self.problemdata.bdrycond.type.values() or 'Pressure' in self.problemdata.bdrycond.type.values())
+        # self.pmean = not ('Neumann' in self.problemdata.bdrycond.type.values() or 'Pressure' in self.problemdata.bdrycond.type.values())
         if self.dirichletmethod=='strong':
             assert 'Navier' not in self.problemdata.bdrycond.type.values()
             assert 'Pressure' not in self.problemdata.bdrycond.type.values()
             colorsdirichlet = self.problemdata.bdrycond.colorsOfType("Dirichlet")
             colorsflux = self.problemdata.postproc.colorsOfType("bdry_nflux")
             self.bdrydata = self.femv.prepareBoundary(colorsdirichlet, colorsflux)
         if self.singleA:
             assert 'Navier' not in self.problemdata.bdrycond.type.values()
             assert 'Pressure' not in self.problemdata.bdrycond.type.values()
-        # ncomps, ns = self.getSystemSize()
-        # print(f"Stokes {self.stack_storage=} {ncomps=} {ns=}")
-        # self.vectorview = vectorview.VectorView(ncomps=ncomps, ns=ns, stack_storage=self.stack_storage)
         self.new_params()
+
+    def getNcomps(self, mesh):
+        self.pmean = not ('Neumann' in self.problemdata.bdrycond.type.values() or 'Pressure' in self.problemdata.bdrycond.type.values())
+        if self.pmean:
+            ncomps = [mesh.dimension, 1, 1]
+        else:
+            ncomps = [mesh.dimension, 1]
+        return ncomps
     def getSystemSize(self):
+        mesh = self.mesh
         if self.pmean:
-            ncomps = [self.mesh.dimension, 1, 1]
-            ns = [self.mesh.nfaces, self.mesh.ncells, 1]
+            ns = [mesh.nfaces, mesh.ncells, 1]
         else:
-            ncomps = [self.mesh.dimension, 1]
-            ns = [self.mesh.nfaces, self.mesh.ncells]
-        return ncomps, ns
+            ns = [mesh.nfaces, mesh.ncells]
+        return ns
     def _checkProblemData(self):
         # TODO checkProblemData() incomplete
         for col, fct in self.problemdata.bdrycond.fct.items():
             type = self.problemdata.bdrycond.type[col]
             if type == "Dirichlet":
                 if len(fct) != self.mesh.dimension: raise ValueError(f"*** {type=} {len(fct)=} {self.mesh.dimension=}")
     # def defineAnalyticalSolution(self, exactsolution, random=True):
@@ -88,15 +109,14 @@
         ncomp = self.ncomp[0]
         def _fcticv(x, y, z):
             rhsv = np.empty(shape=(ncomp, *x.shape))
             for i in range(ncomp):
                 rhsv[i] = v[i](x, y, z, 0)
             return rhsv
         return _fcticv
-
     def defineRhsAnalyticalSolution(self, solexact):
         v,p = solexact
         mu = self.problemdata.params.scal_glob['mu']
         ncomp = self.ncomp[0]
         def _fctrhsv(x, y, z):
             rhsv = np.zeros(shape=(ncomp, *x.shape))
             if v[0].has_time:
@@ -167,33 +187,27 @@
             v, p = solexact
             return v[icomp](x,y,z)
         return {'p':_fctpressure, 'v':[partial(_fctpressurevtang, icomp=icomp) for icomp in range(self.ncomp)]}
     def initialCondition(self, interpolate=True):
         #TODO: higher order interpolation
         if not 'initial_condition' in self.problemdata.params.fct_glob:
             raise ValueError(f"missing 'initial_condition' in {self.problemdata.params.fct_glob=}")
-        if not self._setMeshCalled: self.setMesh(self.mesh)
+        # if not self._setMeshCalled: self.setMesh(self.mesh)
         u0 = np.zeros(self.vectorview.n())
         assert interpolate
         for icomp in range(self.ncomp):
             ic = self.problemdata.params.fct_glob['initial_condition'][icomp]
             ui = self.femv.interpolate(ic)
             self.vectorview.set(0, icomp, u0, ui)
             # print(f"{icomp=} {ui=}")
         return u0
-    def sol_to_data(self, u):
-        data = {'point':{}, 'cell':{}, 'global':{}}
-        for icomp in range(self.ncomp[0]):
-            data['point'][f'V_{icomp:1d}'] = self.femv.tonode(self.vectorview.get(0,icomp,u))
-        data['cell']['P'] = self.vectorview.get_part(1,u)
-        return data
     def postProcess(self, u):
         p = self.vectorview.get_part(1,u)
         data = {'scalar':{}}
-        ncomp = self.ncomp[0]
+        ncomp = self.ncomps[0]
         if self.application.exactsolution:
             errall, ecall = [], []
             for icomp in range(ncomp):
                 err, ec = self.femv.computeErrorL2(self.application.exactsolution[0][icomp], self.vectorview.get(0,icomp,u))
                 errall.append(err)
                 ecall.append(ec)
             data['scalar']['error_V_L2'] = np.sum(errall)
@@ -216,21 +230,22 @@
                     assert pp.ndim == 2
                     for i, color in enumerate(colors):
                         data['scalar'][name + "_" + f"{color}"] = pp[:, i]
                 else:
                     raise ValueError(f"unknown postprocess type '{type}' for key '{name}'\nknown types={types=}")
         return data
     def computelinearSolver(self, A):
+        # print(f"@@@ computelinearSolver")
         if self.linearsolver == 'spsolve':
             args = {'method':'spsolve'}
         else:
             args = copy.deepcopy(self.linearsolver)
         if args['method'] != 'spsolve':
             if self.scale_ls:
-                A.scale_matrix()
+                # A.scale_matrix()
                 args['scale'] = self.scale_ls
             # args['counter'] = 'sys'
             args['matvec'] = A.matvec
             # args['n'] = A.nall
             args['n'] = self.vectorview.n()
             prec = args.pop('prec', 'full')
             solver_v = args.pop('solver_v', None)
@@ -269,15 +284,15 @@
                 bS = dS * self.problemdata.bdrycond.fct[color][icomp](xf, yf, zf, nx, ny, nz)
                 self.vectorview.get(0, icomp, b)[faces] += bS
 
         if self.dirichletmethod == 'strong':
             self.vectorBoundaryStrong(b, self.problemdata.bdrycond.fct, self.bdrydata)
         else:
             bdryfct = self.problemdata.bdrycond.fct
-            ncomp = self.ncomp[0]
+            ncomp = self.ncomps[0]
             faces = self.mesh.bdryFaces(colorsdir)
             cells = self.mesh.cellsOfFaces[faces, 0]
             normalsS = self.mesh.normals[faces][:, :ncomp]
             for icomp in range(ncomp):
                 fdict = {col: bdryfct[col][icomp] for col in colorsdir if col in bdryfct.keys()}
                 vdir = self.femv.interpolateBoundary(colorsdir, fdict)
                 np.add.at(bp, cells, -np.einsum('n,n->n', vdir[faces], normalsS[:,icomp]))
@@ -342,19 +357,19 @@
             p = self.application.exactsolution[1]
             bmean = self.femp.computeMean(p)
         else: bmean=0
         b[-1] = bmean
         return b
     # def computeForm(self, u, coeffmass=None):
     def computeForm(self, u):
-        self.A = self.computeMatrix(u)
-        return self.A.dot(u)
+        # self.A = self.computeMatrix(u)
+        # return self.A.dot(u)
         d = np.zeros_like(u)
         dp, p = self.vectorview.get_part(1,d), self.vectorview.get_part(1,u)
-        ncomp, dV, cellgrads, foc = self.ncomp, self.mesh.dV, self.femv.cellgrads, self.mesh.facesOfCells
+        ncomp, dV, cellgrads, foc = self.ncomps[0], self.mesh.dV, self.femv.cellgrads, self.mesh.facesOfCells
         for icomp in range(ncomp):
             r = np.einsum('n,nil,njl,nj->ni', dV*self.mucell, cellgrads, cellgrads, self.vectorview.get(0, icomp, u)[foc])
             np.add.at(self.vectorview.get(0, icomp, d
 ), foc, r)
         for icomp in range(ncomp):
             r = np.einsum('n,ni->ni', -dV*p, cellgrads[:,:,icomp])
             np.add.at(self.vectorview.get(0, icomp, d), foc, r)
@@ -390,17 +405,17 @@
         y = self.computeForm(u)-f
         self.Mass.dot(y, 1 / (self.theta * self.dt), u)
         return y
    #     return u, niter
     def computeMatrix(self, u=None, coeffmass=None):
         if coeffmass is None and 'alpha' in self.problemdata.params.scal_glob.keys():
             coeffmass = self.problemdata.params.scal_glob['alpha']
-        print(f"computeMatrix {coeffmass=}")
+        # print(f"computeMatrix {coeffmass=}")
         A = self.femv.computeMatrixDiffusion(self.mucell, coeffmass)
-        nfaces, ncells, ncomp, dV = self.mesh.nfaces, self.mesh.ncells, self.ncomp[0], self.mesh.dV
+        nfaces, ncells, ncomp, dV = self.mesh.nfaces, self.mesh.ncells, self.ncomps[0], self.mesh.dV
         if not self.singleA:
             A = linalg.matrix2systemdiagonal(A, ncomp, self.stack_storage)
         nloc, cellgrads, foc = self.femv.nloc, self.femv.cellgrads, self.mesh.facesOfCells
         rowsB = np.repeat(np.arange(ncells), ncomp * nloc)
         colsB = self.vectorview.col_indices(0, foc, ncells, nloc, nfaces)
         # if self.stack_storage:
         #     colsB = np.repeat(foc, ncomp).reshape(ncells * nloc, ncomp) + nfaces*np.arange(ncomp)
@@ -449,18 +464,18 @@
             for i,color in enumerate(colors):
                 faces = self.mesh.bdrylabels[color]
                 cells = self.mesh.cellsOfFaces[faces,0]
                 normalsS = self.mesh.normals[faces][:,:ncomp]
                 flux[icomp,i] -= p[cells].dot(normalsS[:,icomp])
         return flux
     def computeFormBdryNitscheDirichlet(self, d, u, colors, mu):
-        ncomp, dim  = self.ncomp, self.mesh.dimension
+        ncomp, dim  = self.ncomps[0], self.mesh.dimension
         faces = self.mesh.bdryFaces(colors)
         cells = self.mesh.cellsOfFaces[faces, 0]
-        normalsS = self.mesh.normals[faces][:, :self.ncomp]
+        normalsS = self.mesh.normals[faces][:, :ncomp]
         dp, p = self.vectorview.get_part(1,d), self.vectorview.get_part(1,u)
         for icomp in range(ncomp):
             dv, v = self.vectorview.get(0, icomp, d), self.vectorview.get(0, icomp,u)
             self.femv.computeFormNitscheDiffusion(self.nitscheparam, dv, v, mu, colors)
             # pression
             r = np.einsum('f,f->f', p[cells], normalsS[:,icomp])
             np.add.at(self.vectorview.get(0, icomp, d), faces, r)
@@ -479,15 +494,15 @@
             r = np.einsum('f,f->f', self.vectorview.get_part(1,u)[cells], normalsS[:,icomp])
             np.add.at(self.vectorview.get(0, icomp, d), faces, r)
             r = np.einsum('f,f->f', normalsS[:,icomp], self.vectorview.get(0, icomp,u)[faces])
             np.add.at(self.vectorview.get_part(1,d), cells, -r)
         raise NotImplementedError()
 
     def computeMatrixBdryNitscheDirichlet(self, A, B, colors, mucell, singleA):
-        nfaces, ncells, ncomp, dim  = self.mesh.nfaces, self.mesh.ncells, self.ncomp[0], self.mesh.dimension
+        nfaces, ncells, ncomp, dim  = self.mesh.nfaces, self.mesh.ncells, self.ncomps[0], self.mesh.dimension
         if singleA:
             A += self.femv.computeMatrixNitscheDiffusion(self.nitscheparam, mucell, colors)
         else:
             A0 = self.femv.computeMatrixNitscheDiffusion(self.nitscheparam, mucell, colors)
             A += linalg.matrix2systemdiagonal(A0, ncomp, self.stack_storage)
         #grad-div
         faces = self.mesh.bdryFaces(colors)
@@ -710,16 +725,16 @@
         #     # print(f"{flux=}")
         #     #TODO flux Stokes Dirichlet strong wrong
         # return flux
 
 #=================================================================#
 if __name__ == '__main__':
     import matplotlib.pyplot as plt
-    from simfempy.meshes import plotmesh, animdata
-    from simfempy.examples.incompflow import schaeferTurek2d
+    from simfempy.meshes import plotmesh
+    from simfempy.tests.navierstokes.incompflow import schaeferTurek2d
     mesh, data = schaeferTurek2d(h=0.4, mu=1)
     stokes = Stokes(mesh=mesh, problemdata=data, femparams={'dirichletmethod':'strong'}, linearsolver='spsolve')
     print(f"{stokes=}")
     # results = stokes.static(mode="linear")
     results = stokes.static(mode="newton")
     print(f"{results.data['scalar']=}")
     fig = plt.figure(1)
```

### Comparing `simfempy-2.1.1/simfempy/solvers/newton.py` & `simfempy-2.2.2/simfempy/solvers/newton.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         print(f"bt {it:3} {resnorm:10.3e} {resfirst:10.3e} {step:9.2e}")
     while resnorm > (1-c*step)*resfirst and it<maxiter:
         it += 1
         step *= omega
         x = x0 + step * dx
         res = f(x)
         resnorm = np.linalg.norm(res)
+        # res2 = f(x)
+        # if not np.allclose(res, res2): raise ValueError(f"{sdata.steptype=} {np.linalg.norm(res-res2)=} {resnorm=} {np.linalg.norm(res2)=}")
         if verbose:
             print(f"bt {it:3} {resnorm:10.3e} {resfirst:10.3e} {step:9.2e}")
     return x, res, resnorm, step
 
 #----------------------------------------------------------------------
 class Baseopt:
     def __init__(self, f, sdata, n, verbose=False):
@@ -137,16 +139,16 @@
         print("{:20} {:3} {:9.3e} {:^9} {:9.3e} {:^4} {:^4} {:^3} {:^4} {:^1}".format(name, 0, resnorm, 3*'-', xnorm, 3*'-', 3*'-', 3*'-', 2*'-', 3*'-', '-'))
     if sdata.steptype == 'rb':
         bt = Baseopt(f, sdata, x.shape[0], verbose)
     iterdata.bad_convergence = False
     iterdata.success = True
     while(resnorm>tol  and iterdata.iter < maxiter):
         if resnorm<atol:
-            iterdata.success = False
-            iterdata.failure = 'residual too small'
+            iterdata.success = True
+            # iterdata.failure = 'residual too small'
             return x, iterdata
         iterdata.tol_missing = tol/resnorm
         if not computedx:
             J = jac(x)
             dx, liniter, success = linalg.solve(J, -res), 1, True
         else:
             dx, liniter, success = computedx(-res, x, iterdata)
@@ -160,29 +162,29 @@
             iterdata.failure = 'correction too small'
             return x, iterdata
         resold[:] = res[:]
         if sdata.steptype == 'rb':
             x, res, resnorm, step = bt.step(x, dx, resnorm)
         else:
             x, res, resnorm, step = backtracking(f, x, dx, resnorm, sdata, verbose=False)
-        res2 = f(x)
-        assert np.allclose(res, res2)
+        # res2 = f(x)
+        # if not np.allclose(res, res2): raise ValueError(f"{sdata.steptype=} {np.linalg.norm(res-res2)=} {resnorm=} {np.linalg.norm(res)=}")
         iterdata.newstep(dx, liniter, resnorm, step)
         xnorm = linalg.norm(x)
         matsymb = ''
         iterdata.bad_convergence = False
         if iterdata.rhodx>sdata.rho_aimed:
             iterdata.bad_convergence = True
             iterdata.bad_convergence_count += 1
             matsymb = 'M'
         if verbose:
             print(f"{name:20s} {iterdata.iter:3d} {resnorm:9.3e} {iterdata.dxnorm[-1]:9.3e} {xnorm:9.3e} {iterdata.rhodx:4.2f} {iterdata.rhor:4.2f} {liniter:3d} {step:4.2f} {matsymb:1s}")
         if resnorm<atol:
-            iterdata.success = False
-            iterdata.failure = 'residual too small'
+            iterdata.success = True
+            # iterdata.failure = 'residual too small'
             return x, iterdata
         if iterdata.iter == sdata.maxiter:
             iterdata.success = False
             iterdata.failure = 'maxiter exceded'
             return x, iterdata
         if xnorm >= divx:
             iterdata.success = False
```

### Comparing `simfempy-2.1.1/simfempy/solvers/newtondata.py` & `simfempy-2.2.2/simfempy/solvers/newtondata.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.divx = kwargs.pop('divx',1e8)
         self.rho_aimed = kwargs.pop('rho_aimed',0.1)
         self.firststep = 1.0
         self.steptype = kwargs.pop('steptype','backtracking')
         if 'nbase' in kwargs: self.nbase = kwargs.pop('nbase')
         self.bt_maxiter = kwargs.pop('bt_maxiter',10)
         self.bt_omega = kwargs.pop('bt_omega',0.75)
-        self.bt_c = kwargs.pop('bt_c',0.1)
+        self.bt_c = kwargs.pop('bt_c',0.01)
         self.maxter_stepsize = 5
 
 class IterationData:
     def __repr__(self):
         all = [f"{k}: {v}" for k,v in self.__dict__.items()]
         return ' '.join(all)
     def __init__(self, resnorm, **kwargs):
```

### Comparing `simfempy-2.1.1/simfempy/tests/stokes/stokes_analytic.py` & `simfempy-2.2.2/simfempy/tests/stokes/stokes_analytic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pathlib, sys
 simfempypath = str(pathlib.Path(__file__).parent.parent.parent.parent)
 sys.path.insert(0,simfempypath)
 import simfempy.meshes.testmeshes as testmeshes
 from simfempy.models.stokes import Stokes
 import simfempy.models.problemdata
-import simfempy.models.application
+import simfempy.applications.application
 from simfempy.tools.comparemethods import CompareMethods
 
 #----------------------------------------------------------------#
 def test(dim, **kwargs):
-    class StokesApplicationWithExactSolution(simfempy.models.application.Application):
+    class StokesApplicationWithExactSolution(simfempy.applications.application.Application):
         def __init__(self, dim, exactsolution, bctype):
             super().__init__(exactsolution=exactsolution)
             # self.exactsolution = exactsolution
             data = self.problemdata
             if dim == 2:
                 data.ncomp = (2,1)
                 self.defineGeometry = testmeshes.unitsquare
```

### Comparing `simfempy-2.1.1/simfempy/tests/stokes/test_stokes.py` & `simfempy-2.2.2/simfempy/tests/stokes/test_stokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tests/testcaseanalytical.py` & `simfempy-2.2.2/simfempy/tests/testcaseanalytical.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/analyticalfunction.py` & `simfempy-2.2.2/simfempy/tools/analyticalfunction.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/barycentric.py` & `simfempy-2.2.2/simfempy/tools/barycentric.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/comparemethods.py` & `simfempy-2.2.2/simfempy/tools/comparemethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                     raise ValueError("need 'model' (class) and 'modelargs' (dict) and  'paramsdict' (dict)")
             model, modelargs = kwargs.pop("model"), kwargs.pop("modelargs")
             if len(kwargs.keys()):
                 raise ValueError(f"*** unused arguments {kwargs=}")
             self._definemethods(model, modelargs)
 
     def _definemethods(self, model, modelargs):
-        print(f" _definemethods {modelargs=}")
+        if self.verbose: print(f" _definemethods {modelargs=}")
         paramsdict = self.paramsdict
         if self.paramname in paramsdict: paramsdict.pop(self.paramname)
         for pname,params in paramsdict.items():
             if isinstance(params, str): paramsdict[pname] = [params]
         def dicttensorproduct(paramsdicts):
             import itertools
             paramslist = [[(name, param) for param in params] for name, params in paramsdicts.items()]
@@ -164,15 +164,16 @@
                 if self.paramname != "ncells": 
                     method.paramname = param
                     # method.setParameter(self.paramname, param)
                 result,u = method.solve()
                 if self.verbose>=2: print(f"{result=}")
                 if self.plotsolution:
                     suptitle = "{}={}".format(self.paramname, parameters[-1])
-                    method.application.plot(mesh, method.sol_to_data(u), fig=fig, gs=outer[plotcount])
+                    # method.application.plot(mesh, method.sol_to_data(u), fig=fig, gs=outer[plotcount])
+                    method.application.plot(mesh, u.tovisudata(), fig=fig, gs=outer[plotcount])
                     plotcount += 1
                 # if self.plotsolution:
                 #     method.application.plot(mesh, method.sol_to_data(u))
                 #     plt.suptitle(f"{self.paramname}={parameters[-1]}")
                 #     plt.show()
                 resdict = result.info.copy()
                 if self.postproc: self.postproc(result.data['scalar'])
```

### Comparing `simfempy-2.1.1/simfempy/tools/file_explorer.py` & `simfempy-2.2.2/simfempy/tools/file_explorer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/iterationcounter.py` & `simfempy-2.2.2/simfempy/tools/iterationcounter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/latexwriter.py` & `simfempy-2.2.2/simfempy/tools/latexwriter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy/tools/timer.py` & `simfempy-2.2.2/simfempy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.1.1/simfempy.egg-info/SOURCES.txt` & `simfempy-2.2.2/simfempy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,53 @@
 setup.py
 simfempy/__init__.py
 simfempy.egg-info/PKG-INFO
 simfempy.egg-info/SOURCES.txt
 simfempy.egg-info/dependency_links.txt
 simfempy.egg-info/requires.txt
 simfempy.egg-info/top_level.txt
+simfempy/applications/__init__.py
+simfempy/applications/application.py
+simfempy/applications/navierstokes.py
 simfempy/examples/__init__.py
+simfempy/examples/flow_static.py
 simfempy/examples/heat_dynamic.py
 simfempy/examples/heat_static.py
-simfempy/examples/incompflow.py
 simfempy/examples/interface.py
-simfempy/examples/navier_stokes.py
 simfempy/fems/__init__.py
 simfempy/fems/cr1.py
 simfempy/fems/d0.py
 simfempy/fems/data.py
+simfempy/fems/femvector.py
 simfempy/fems/p1.py
 simfempy/fems/p1general.py
 simfempy/fems/rt0.py
 simfempy/linalg/__init__.py
 simfempy/linalg/linalg.py
 simfempy/linalg/matrixsystem.py
 simfempy/linalg/saddle_point.py
 simfempy/linalg/vectorview.py
 simfempy/meshes/__init__.py
 simfempy/meshes/plotmesh.py
 simfempy/meshes/simplexmesh.py
 simfempy/meshes/testmeshes.py
 simfempy/models/__init__.py
-simfempy/models/application.py
 simfempy/models/elliptic.py
 simfempy/models/model.py
 simfempy/models/navierstokes.py
 simfempy/models/problemdata.py
 simfempy/models/stokes.py
 simfempy/solvers/__init__.py
 simfempy/solvers/newton.py
 simfempy/solvers/newtondata.py
 simfempy/tests/__init__.py
 simfempy/tests/testcaseanalytical.py
+simfempy/tests/navierstokes/__init__.py
+simfempy/tests/navierstokes/flow_static.py
+simfempy/tests/navierstokes/incompflow.py
 simfempy/tests/stokes/__init__.py
 simfempy/tests/stokes/stokes_analytic.py
 simfempy/tests/stokes/test_stokes.py
 simfempy/tools/__init__.py
 simfempy/tools/analyticalfunction.py
 simfempy/tools/barycentric.py
 simfempy/tools/comparemethods.py
```

