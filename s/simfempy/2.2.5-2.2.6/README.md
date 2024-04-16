# Comparing `tmp/simfempy-2.2.5.tar.gz` & `tmp/simfempy-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfempy-2.2.5.tar", last modified: Tue Apr 16 14:54:12 2024, max compression
+gzip compressed data, was "simfempy-2.2.6.tar", last modified: Tue Apr 16 14:56:05 2024, max compression
```

## Comparing `simfempy-2.2.5.tar` & `simfempy-2.2.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.127207 simfempy-2.2.5/
--rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.2.5/LICENSE
--rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:54:12.126588 simfempy-2.2.5/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     2679 2024-04-16 14:54:12.000000 simfempy-2.2.5/README.md
--rw-r--r--   0 becker     (501) staff       (20)       38 2024-04-16 14:54:12.127393 simfempy-2.2.5/setup.cfg
--rw-r--r--   0 becker     (501) staff       (20)     1332 2024-04-16 14:54:05.000000 simfempy-2.2.5/setup.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.098497 simfempy-2.2.5/simfempy/
--rw-r--r--   0 becker     (501) staff       (20)      153 2024-04-13 14:16:18.000000 simfempy-2.2.5/simfempy/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.102105 simfempy-2.2.5/simfempy/applications/
--rw-r--r--   0 becker     (501) staff       (20)       40 2024-04-14 11:38:13.000000 simfempy-2.2.5/simfempy/applications/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     4907 2024-04-15 15:48:55.000000 simfempy-2.2.5/simfempy/applications/application.py
--rw-r--r--   0 becker     (501) staff       (20)    15260 2024-04-14 11:38:49.000000 simfempy-2.2.5/simfempy/applications/navierstokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.104474 simfempy-2.2.5/simfempy/examples/
--rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.2.5/simfempy/examples/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     3266 2024-04-16 14:20:46.000000 simfempy-2.2.5/simfempy/examples/flow_static.py
--rw-r--r--   0 becker     (501) staff       (20)     3048 2024-04-14 11:36:23.000000 simfempy-2.2.5/simfempy/examples/heat_dynamic.py
--rw-r--r--   0 becker     (501) staff       (20)     2623 2024-04-14 16:50:50.000000 simfempy-2.2.5/simfempy/examples/heat_static.py
--rw-r--r--   0 becker     (501) staff       (20)     3950 2024-04-14 11:36:23.000000 simfempy-2.2.5/simfempy/examples/interface.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.108240 simfempy-2.2.5/simfempy/fems/
--rw-r--r--   0 becker     (501) staff       (20)       48 2024-04-14 08:58:57.000000 simfempy-2.2.5/simfempy/fems/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    27607 2024-04-16 13:11:08.000000 simfempy-2.2.5/simfempy/fems/cr1.py
--rw-r--r--   0 becker     (501) staff       (20)     2740 2024-04-14 11:13:29.000000 simfempy-2.2.5/simfempy/fems/d0.py
--rw-r--r--   0 becker     (501) staff       (20)      819 2024-04-14 14:58:27.000000 simfempy-2.2.5/simfempy/fems/data.py
--rw-r--r--   0 becker     (501) staff       (20)     2707 2024-04-14 14:40:31.000000 simfempy-2.2.5/simfempy/fems/femvector.py
--rw-r--r--   0 becker     (501) staff       (20)    29792 2024-04-16 12:20:49.000000 simfempy-2.2.5/simfempy/fems/p1.py
--rw-r--r--   0 becker     (501) staff       (20)     7757 2024-04-16 12:56:57.000000 simfempy-2.2.5/simfempy/fems/p1general.py
--rw-r--r--   0 becker     (501) staff       (20)    16154 2024-04-14 14:34:37.000000 simfempy-2.2.5/simfempy/fems/rt0.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.110933 simfempy-2.2.5/simfempy/linalg/
--rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.2.5/simfempy/linalg/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    14665 2024-04-14 16:43:13.000000 simfempy-2.2.5/simfempy/linalg/linalg.py
--rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.2.5/simfempy/linalg/matrixsystem.py
--rw-r--r--   0 becker     (501) staff       (20)    11014 2024-04-13 17:37:20.000000 simfempy-2.2.5/simfempy/linalg/saddle_point.py
--rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.2.5/simfempy/linalg/vectorview.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.113181 simfempy-2.2.5/simfempy/meshes/
--rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.2.5/simfempy/meshes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.2.5/simfempy/meshes/plotmesh.py
--rw-r--r--   0 becker     (501) staff       (20)    20506 2024-04-16 14:53:28.000000 simfempy-2.2.5/simfempy/meshes/simplexmesh.py
--rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.2.5/simfempy/meshes/testmeshes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.116063 simfempy-2.2.5/simfempy/models/
--rw-r--r--   0 becker     (501) staff       (20)       52 2024-04-14 11:36:23.000000 simfempy-2.2.5/simfempy/models/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)    29397 2024-04-16 14:04:25.000000 simfempy-2.2.5/simfempy/models/elliptic.py
--rw-r--r--   0 becker     (501) staff       (20)    29087 2024-04-16 13:36:02.000000 simfempy-2.2.5/simfempy/models/model.py
--rw-r--r--   0 becker     (501) staff       (20)     5358 2024-04-14 15:38:59.000000 simfempy-2.2.5/simfempy/models/navierstokes.py
--rw-r--r--   0 becker     (501) staff       (20)    10227 2024-04-14 12:02:52.000000 simfempy-2.2.5/simfempy/models/problemdata.py
--rw-r--r--   0 becker     (501) staff       (20)    39284 2024-04-14 15:43:35.000000 simfempy-2.2.5/simfempy/models/stokes.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.117531 simfempy-2.2.5/simfempy/solvers/
--rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.2.5/simfempy/solvers/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     8650 2024-04-13 22:01:19.000000 simfempy-2.2.5/simfempy/solvers/newton.py
--rw-r--r--   0 becker     (501) staff       (20)     2454 2024-04-13 21:39:49.000000 simfempy-2.2.5/simfempy/solvers/newtondata.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.118378 simfempy-2.2.5/simfempy/tests/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.5/simfempy/tests/__init__.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.119657 simfempy-2.2.5/simfempy/tests/navierstokes/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-04-14 09:41:29.000000 simfempy-2.2.5/simfempy/tests/navierstokes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     3881 2024-04-14 15:24:05.000000 simfempy-2.2.5/simfempy/tests/navierstokes/flow_static.py
--rw-r--r--   0 becker     (501) staff       (20)     4372 2024-04-13 14:20:43.000000 simfempy-2.2.5/simfempy/tests/navierstokes/incompflow.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.121044 simfempy-2.2.5/simfempy/tests/stokes/
--rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.5/simfempy/tests/stokes/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5012 2024-04-14 11:36:23.000000 simfempy-2.2.5/simfempy/tests/stokes/stokes_analytic.py
--rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.2.5/simfempy/tests/stokes/test_stokes.py
--rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.2.5/simfempy/tests/testcaseanalytical.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.125335 simfempy-2.2.5/simfempy/tools/
--rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.2.5/simfempy/tools/__init__.py
--rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.2.5/simfempy/tools/analyticalfunction.py
--rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.2.5/simfempy/tools/barycentric.py
--rw-r--r--   0 becker     (501) staff       (20)    14940 2024-04-15 15:48:55.000000 simfempy-2.2.5/simfempy/tools/comparemethods.py
--rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.2.5/simfempy/tools/file_explorer.py
--rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.2.5/simfempy/tools/iterationcounter.py
--rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.2.5/simfempy/tools/latexwriter.py
--rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.2.5/simfempy/tools/timer.py
-drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:54:12.125907 simfempy-2.2.5/simfempy.egg-info/
--rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:54:12.000000 simfempy-2.2.5/simfempy.egg-info/PKG-INFO
--rw-r--r--   0 becker     (501) staff       (20)     1731 2024-04-16 14:54:12.000000 simfempy-2.2.5/simfempy.egg-info/SOURCES.txt
--rw-r--r--   0 becker     (501) staff       (20)        1 2024-04-16 14:54:12.000000 simfempy-2.2.5/simfempy.egg-info/dependency_links.txt
--rw-r--r--   0 becker     (501) staff       (20)       47 2024-04-16 14:54:12.000000 simfempy-2.2.5/simfempy.egg-info/requires.txt
--rw-r--r--   0 becker     (501) staff       (20)        9 2024-04-16 14:54:12.000000 simfempy-2.2.5/simfempy.egg-info/top_level.txt
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.154505 simfempy-2.2.6/
+-rw-r--r--   0 becker     (501) staff       (20)     1065 2019-01-29 18:41:12.000000 simfempy-2.2.6/LICENSE
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:56:05.153682 simfempy-2.2.6/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     2679 2024-04-16 14:56:05.000000 simfempy-2.2.6/README.md
+-rw-r--r--   0 becker     (501) staff       (20)       38 2024-04-16 14:56:05.154652 simfempy-2.2.6/setup.cfg
+-rw-r--r--   0 becker     (501) staff       (20)     1332 2024-04-16 14:55:53.000000 simfempy-2.2.6/setup.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.125364 simfempy-2.2.6/simfempy/
+-rw-r--r--   0 becker     (501) staff       (20)      153 2024-04-13 14:16:18.000000 simfempy-2.2.6/simfempy/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.128995 simfempy-2.2.6/simfempy/applications/
+-rw-r--r--   0 becker     (501) staff       (20)       40 2024-04-14 11:38:13.000000 simfempy-2.2.6/simfempy/applications/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     4907 2024-04-15 15:48:55.000000 simfempy-2.2.6/simfempy/applications/application.py
+-rw-r--r--   0 becker     (501) staff       (20)    15260 2024-04-14 11:38:49.000000 simfempy-2.2.6/simfempy/applications/navierstokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.131258 simfempy-2.2.6/simfempy/examples/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2023-04-22 15:00:13.000000 simfempy-2.2.6/simfempy/examples/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3266 2024-04-16 14:20:46.000000 simfempy-2.2.6/simfempy/examples/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3048 2024-04-14 11:36:23.000000 simfempy-2.2.6/simfempy/examples/heat_dynamic.py
+-rw-r--r--   0 becker     (501) staff       (20)     2623 2024-04-14 16:50:50.000000 simfempy-2.2.6/simfempy/examples/heat_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     3950 2024-04-14 11:36:23.000000 simfempy-2.2.6/simfempy/examples/interface.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.135107 simfempy-2.2.6/simfempy/fems/
+-rw-r--r--   0 becker     (501) staff       (20)       48 2024-04-14 08:58:57.000000 simfempy-2.2.6/simfempy/fems/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    27607 2024-04-16 13:11:08.000000 simfempy-2.2.6/simfempy/fems/cr1.py
+-rw-r--r--   0 becker     (501) staff       (20)     2740 2024-04-14 11:13:29.000000 simfempy-2.2.6/simfempy/fems/d0.py
+-rw-r--r--   0 becker     (501) staff       (20)      819 2024-04-14 14:58:27.000000 simfempy-2.2.6/simfempy/fems/data.py
+-rw-r--r--   0 becker     (501) staff       (20)     2707 2024-04-14 14:40:31.000000 simfempy-2.2.6/simfempy/fems/femvector.py
+-rw-r--r--   0 becker     (501) staff       (20)    29792 2024-04-16 12:20:49.000000 simfempy-2.2.6/simfempy/fems/p1.py
+-rw-r--r--   0 becker     (501) staff       (20)     7757 2024-04-16 12:56:57.000000 simfempy-2.2.6/simfempy/fems/p1general.py
+-rw-r--r--   0 becker     (501) staff       (20)    16154 2024-04-14 14:34:37.000000 simfempy-2.2.6/simfempy/fems/rt0.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.138035 simfempy-2.2.6/simfempy/linalg/
+-rw-r--r--   0 becker     (501) staff       (20)       60 2024-02-18 09:07:24.000000 simfempy-2.2.6/simfempy/linalg/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    14665 2024-04-14 16:43:13.000000 simfempy-2.2.6/simfempy/linalg/linalg.py
+-rw-r--r--   0 becker     (501) staff       (20)     2218 2024-02-18 09:25:48.000000 simfempy-2.2.6/simfempy/linalg/matrixsystem.py
+-rw-r--r--   0 becker     (501) staff       (20)    11014 2024-04-13 17:37:20.000000 simfempy-2.2.6/simfempy/linalg/saddle_point.py
+-rw-r--r--   0 becker     (501) staff       (20)     2243 2024-02-10 23:29:14.000000 simfempy-2.2.6/simfempy/linalg/vectorview.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.139847 simfempy-2.2.6/simfempy/meshes/
+-rw-r--r--   0 becker     (501) staff       (20)       49 2024-02-15 12:46:23.000000 simfempy-2.2.6/simfempy/meshes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     7064 2024-02-15 13:04:52.000000 simfempy-2.2.6/simfempy/meshes/plotmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)    20496 2024-04-16 14:55:36.000000 simfempy-2.2.6/simfempy/meshes/simplexmesh.py
+-rw-r--r--   0 becker     (501) staff       (20)     4280 2024-02-10 17:30:04.000000 simfempy-2.2.6/simfempy/meshes/testmeshes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.143418 simfempy-2.2.6/simfempy/models/
+-rw-r--r--   0 becker     (501) staff       (20)       52 2024-04-14 11:36:23.000000 simfempy-2.2.6/simfempy/models/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)    29397 2024-04-16 14:04:25.000000 simfempy-2.2.6/simfempy/models/elliptic.py
+-rw-r--r--   0 becker     (501) staff       (20)    29087 2024-04-16 13:36:02.000000 simfempy-2.2.6/simfempy/models/model.py
+-rw-r--r--   0 becker     (501) staff       (20)     5358 2024-04-14 15:38:59.000000 simfempy-2.2.6/simfempy/models/navierstokes.py
+-rw-r--r--   0 becker     (501) staff       (20)    10227 2024-04-14 12:02:52.000000 simfempy-2.2.6/simfempy/models/problemdata.py
+-rw-r--r--   0 becker     (501) staff       (20)    39284 2024-04-14 15:43:35.000000 simfempy-2.2.6/simfempy/models/stokes.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.144899 simfempy-2.2.6/simfempy/solvers/
+-rw-r--r--   0 becker     (501) staff       (20)       33 2023-05-31 09:09:01.000000 simfempy-2.2.6/simfempy/solvers/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     8650 2024-04-13 22:01:19.000000 simfempy-2.2.6/simfempy/solvers/newton.py
+-rw-r--r--   0 becker     (501) staff       (20)     2454 2024-04-13 21:39:49.000000 simfempy-2.2.6/simfempy/solvers/newtondata.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.145855 simfempy-2.2.6/simfempy/tests/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.6/simfempy/tests/__init__.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.147070 simfempy-2.2.6/simfempy/tests/navierstokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-04-14 09:41:29.000000 simfempy-2.2.6/simfempy/tests/navierstokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     3881 2024-04-14 15:24:05.000000 simfempy-2.2.6/simfempy/tests/navierstokes/flow_static.py
+-rw-r--r--   0 becker     (501) staff       (20)     4372 2024-04-13 14:20:43.000000 simfempy-2.2.6/simfempy/tests/navierstokes/incompflow.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.148413 simfempy-2.2.6/simfempy/tests/stokes/
+-rw-r--r--   0 becker     (501) staff       (20)        0 2024-02-11 15:12:39.000000 simfempy-2.2.6/simfempy/tests/stokes/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5012 2024-04-14 11:36:23.000000 simfempy-2.2.6/simfempy/tests/stokes/stokes_analytic.py
+-rw-r--r--   0 becker     (501) staff       (20)     1037 2024-02-14 13:20:12.000000 simfempy-2.2.6/simfempy/tests/stokes/test_stokes.py
+-rw-r--r--   0 becker     (501) staff       (20)     1533 2024-02-11 15:08:51.000000 simfempy-2.2.6/simfempy/tests/testcaseanalytical.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.152336 simfempy-2.2.6/simfempy/tools/
+-rw-r--r--   0 becker     (501) staff       (20)       41 2023-05-13 13:35:56.000000 simfempy-2.2.6/simfempy/tools/__init__.py
+-rw-r--r--   0 becker     (501) staff       (20)     5356 2023-06-19 14:07:03.000000 simfempy-2.2.6/simfempy/tools/analyticalfunction.py
+-rw-r--r--   0 becker     (501) staff       (20)      718 2021-03-26 16:54:29.000000 simfempy-2.2.6/simfempy/tools/barycentric.py
+-rw-r--r--   0 becker     (501) staff       (20)    14940 2024-04-15 15:48:55.000000 simfempy-2.2.6/simfempy/tools/comparemethods.py
+-rw-r--r--   0 becker     (501) staff       (20)     3244 2023-05-11 21:05:40.000000 simfempy-2.2.6/simfempy/tools/file_explorer.py
+-rw-r--r--   0 becker     (501) staff       (20)     1493 2021-06-25 14:00:57.000000 simfempy-2.2.6/simfempy/tools/iterationcounter.py
+-rw-r--r--   0 becker     (501) staff       (20)    12086 2023-06-01 13:45:23.000000 simfempy-2.2.6/simfempy/tools/latexwriter.py
+-rw-r--r--   0 becker     (501) staff       (20)     1252 2023-06-12 15:33:34.000000 simfempy-2.2.6/simfempy/tools/timer.py
+drwxr-xr-x   0 becker     (501) staff       (20)        0 2024-04-16 14:56:05.152932 simfempy-2.2.6/simfempy.egg-info/
+-rw-r--r--   0 becker     (501) staff       (20)     3412 2024-04-16 14:56:05.000000 simfempy-2.2.6/simfempy.egg-info/PKG-INFO
+-rw-r--r--   0 becker     (501) staff       (20)     1731 2024-04-16 14:56:05.000000 simfempy-2.2.6/simfempy.egg-info/SOURCES.txt
+-rw-r--r--   0 becker     (501) staff       (20)        1 2024-04-16 14:56:05.000000 simfempy-2.2.6/simfempy.egg-info/dependency_links.txt
+-rw-r--r--   0 becker     (501) staff       (20)       47 2024-04-16 14:56:05.000000 simfempy-2.2.6/simfempy.egg-info/requires.txt
+-rw-r--r--   0 becker     (501) staff       (20)        9 2024-04-16 14:56:05.000000 simfempy-2.2.6/simfempy.egg-info/top_level.txt
```

### Comparing `simfempy-2.2.5/LICENSE` & `simfempy-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/PKG-INFO` & `simfempy-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfempy
-Version: 2.2.5
+Version: 2.2.6
 Summary: A small package for fem
 Home-page: https://github.com/beckerrh/simfempy
 Author: Roland Becker
 Author-email: beckerrolandh@gmail.com
 License: License :: OSI Approved :: MIT License
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simfempy-2.2.5/README.md` & `simfempy-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/setup.py` & `simfempy-2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 from setuptools import setup, find_packages
 
-VERSION = "2.2.5"
+VERSION = "2.2.6"
 
 with open("simfempy/examples/heat_static.py", "r") as heat:
     example = heat.read()
 with open("README.md", "w") as readme:
     readme.write("SIMple Finite Element Methods in PYthon\n\n```python\n")
     readme.write(example)
     readme.write("\n```\n")
```

### Comparing `simfempy-2.2.5/simfempy/applications/application.py` & `simfempy-2.2.6/simfempy/applications/application.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/applications/navierstokes.py` & `simfempy-2.2.6/simfempy/applications/navierstokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/examples/flow_static.py` & `simfempy-2.2.6/simfempy/examples/flow_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/examples/heat_dynamic.py` & `simfempy-2.2.6/simfempy/examples/heat_dynamic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/examples/heat_static.py` & `simfempy-2.2.6/simfempy/examples/heat_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/examples/interface.py` & `simfempy-2.2.6/simfempy/examples/interface.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/cr1.py` & `simfempy-2.2.6/simfempy/fems/cr1.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/d0.py` & `simfempy-2.2.6/simfempy/fems/d0.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/data.py` & `simfempy-2.2.6/simfempy/fems/data.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/femvector.py` & `simfempy-2.2.6/simfempy/fems/femvector.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/p1.py` & `simfempy-2.2.6/simfempy/fems/p1.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/p1general.py` & `simfempy-2.2.6/simfempy/fems/p1general.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/fems/rt0.py` & `simfempy-2.2.6/simfempy/fems/rt0.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/linalg/linalg.py` & `simfempy-2.2.6/simfempy/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/linalg/matrixsystem.py` & `simfempy-2.2.6/simfempy/linalg/matrixsystem.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/linalg/saddle_point.py` & `simfempy-2.2.6/simfempy/linalg/saddle_point.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/linalg/vectorview.py` & `simfempy-2.2.6/simfempy/linalg/vectorview.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/meshes/plotmesh.py` & `simfempy-2.2.6/simfempy/meshes/plotmesh.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/meshes/simplexmesh.py` & `simfempy-2.2.6/simfempy/meshes/simplexmesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
         if len(np.unique(self.simplices)) != self.nnodes:
             raise ValueError(f"{len(np.unique(self.simplices))=} BUT {self.nnodes=}")
     def getBdryPoints(self, colors):
         if not isinstance(colors, (list,tuple)): colors = [colors]
         bdrypoints = []
         for color in colors:
             if not isinstance(color, int): color = self.labeldict_s2i[color]
-            facesdir = self.mesh.bdrylabels[color]
-            bdrypoints.append(np.unique(self.mesh.faces[facesdir].flat[:]))
+            facesdir = self.bdrylabels[color]
+            bdrypoints.append(np.unique(self.faces[facesdir].flat[:]))
         return np.array(bdrypoints).reshape(-1)
 
     def bdryFaces(self, colors=None):
         if colors is None: colors = self.bdrylabels.keys()
         pos = [0]
         for color in colors: pos.append(pos[-1]+len(self.bdrylabels[color]))
         faces = np.empty(pos[-1], dtype=np.uint32)
```

### Comparing `simfempy-2.2.5/simfempy/meshes/testmeshes.py` & `simfempy-2.2.6/simfempy/meshes/testmeshes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/models/elliptic.py` & `simfempy-2.2.6/simfempy/models/elliptic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/models/model.py` & `simfempy-2.2.6/simfempy/models/model.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/models/navierstokes.py` & `simfempy-2.2.6/simfempy/models/navierstokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/models/problemdata.py` & `simfempy-2.2.6/simfempy/models/problemdata.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/models/stokes.py` & `simfempy-2.2.6/simfempy/models/stokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/solvers/newton.py` & `simfempy-2.2.6/simfempy/solvers/newton.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/solvers/newtondata.py` & `simfempy-2.2.6/simfempy/solvers/newtondata.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tests/navierstokes/flow_static.py` & `simfempy-2.2.6/simfempy/tests/navierstokes/flow_static.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tests/navierstokes/incompflow.py` & `simfempy-2.2.6/simfempy/tests/navierstokes/incompflow.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tests/stokes/stokes_analytic.py` & `simfempy-2.2.6/simfempy/tests/stokes/stokes_analytic.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tests/stokes/test_stokes.py` & `simfempy-2.2.6/simfempy/tests/stokes/test_stokes.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tests/testcaseanalytical.py` & `simfempy-2.2.6/simfempy/tests/testcaseanalytical.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/analyticalfunction.py` & `simfempy-2.2.6/simfempy/tools/analyticalfunction.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/barycentric.py` & `simfempy-2.2.6/simfempy/tools/barycentric.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/comparemethods.py` & `simfempy-2.2.6/simfempy/tools/comparemethods.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/file_explorer.py` & `simfempy-2.2.6/simfempy/tools/file_explorer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/iterationcounter.py` & `simfempy-2.2.6/simfempy/tools/iterationcounter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/latexwriter.py` & `simfempy-2.2.6/simfempy/tools/latexwriter.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy/tools/timer.py` & `simfempy-2.2.6/simfempy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `simfempy-2.2.5/simfempy.egg-info/PKG-INFO` & `simfempy-2.2.6/simfempy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfempy
-Version: 2.2.5
+Version: 2.2.6
 Summary: A small package for fem
 Home-page: https://github.com/beckerrh/simfempy
 Author: Roland Becker
 Author-email: beckerrolandh@gmail.com
 License: License :: OSI Approved :: MIT License
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simfempy-2.2.5/simfempy.egg-info/SOURCES.txt` & `simfempy-2.2.6/simfempy.egg-info/SOURCES.txt`

 * *Files identical despite different names*
