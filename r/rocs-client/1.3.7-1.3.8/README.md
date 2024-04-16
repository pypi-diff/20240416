# Comparing `tmp/rocs_client-1.3.7.tar.gz` & `tmp/rocs_client-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocs_client-1.3.7.tar", last modified: Tue Apr 16 09:23:56 2024, max compression
+gzip compressed data, was "rocs_client-1.3.8.tar", last modified: Tue Apr 16 09:43:36 2024, max compression
```

## Comparing `rocs_client-1.3.7.tar` & `rocs_client-1.3.8.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.370538 rocs_client-1.3.7/
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.328560 rocs_client-1.3.7/.github/
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.332219 rocs_client-1.3.7/.github/workflows/
--rw-r--r--   0 jax        (501) staff       (20)     1250 2023-12-05 04:31:02.000000 rocs_client-1.3.7/.github/workflows/static.yml
--rw-r--r--   0 jax        (501) staff       (20)      497 2023-12-05 03:43:04.000000 rocs_client-1.3.7/.gitignore
--rw-r--r--   0 jax        (501) staff       (20)     1073 2023-12-05 03:43:04.000000 rocs_client-1.3.7/LICENSE
--rw-r--r--   0 jax        (501) staff       (20)    14004 2024-04-16 09:23:56.370210 rocs_client-1.3.7/PKG-INFO
--rw-r--r--   0 jax        (501) staff       (20)    13350 2024-01-16 09:36:24.000000 rocs_client-1.3.7/README.md
--rw-r--r--   0 jax        (501) staff       (20)      105 2024-01-16 07:23:48.000000 rocs_client-1.3.7/deploy_pypi.sh
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.334578 rocs_client-1.3.7/doc/
--rw-r--r--   0 jax        (501) staff       (20)      638 2023-12-05 03:43:04.000000 rocs_client-1.3.7/doc/Makefile
--rw-r--r--   0 jax        (501) staff       (20)      246 2024-01-16 03:34:29.000000 rocs_client-1.3.7/doc/build_doc.sh
--rw-r--r--   0 jax        (501) staff       (20)      484 2024-01-04 09:33:19.000000 rocs_client-1.3.7/doc/conf.py
--rw-r--r--   0 jax        (501) staff       (20)    57336 2023-12-05 03:43:04.000000 rocs_client-1.3.7/doc/ico.jpg
--rw-r--r--   0 jax        (501) staff       (20)      785 2024-01-16 03:34:29.000000 rocs_client-1.3.7/doc/index.rst
--rw-r--r--   0 jax        (501) staff       (20)      769 2023-12-05 03:43:04.000000 rocs_client-1.3.7/doc/make.bat
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.336010 rocs_client-1.3.7/docs/
--rw-r--r--   0 jax        (501) staff       (20)      230 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/.buildinfo
--rw-r--r--   0 jax        (501) staff       (20)        0 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/.nojekyll
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.338578 rocs_client-1.3.7/docs/_sources/
--rw-r--r--   0 jax        (501) staff       (20)      887 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_sources/index.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)       76 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_sources/modules.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)      460 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_sources/rocs_client.common.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)      428 2024-01-16 03:34:29.000000 rocs_client-1.3.7/docs/_sources/rocs_client.end_effector.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)      306 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_sources/rocs_client.motor.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)      592 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_sources/rocs_client.robot.rst.txt
--rw-r--r--   0 jax        (501) staff       (20)      278 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_sources/rocs_client.rst.txt
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.344036 rocs_client-1.3.7/docs/_static/
--rw-r--r--   0 jax        (501) staff       (20)     4289 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 jax        (501) staff       (20)    15094 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/basic.css
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.344741 rocs_client-1.3.7/docs/_static/css/
--rw-r--r--   0 jax        (501) staff       (20)     3229 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/badge_only.css
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.356854 rocs_client-1.3.7/docs/_static/css/fonts/
--rw-r--r--   0 jax        (501) staff       (20)    87624 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 jax        (501) staff       (20)    67312 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 jax        (501) staff       (20)    86288 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 jax        (501) staff       (20)    66444 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 jax        (501) staff       (20)   165742 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 jax        (501) staff       (20)   444379 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 jax        (501) staff       (20)   165548 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 jax        (501) staff       (20)    98024 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 jax        (501) staff       (20)    77160 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 jax        (501) staff       (20)   323344 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 jax        (501) staff       (20)   193308 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 jax        (501) staff       (20)   309728 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 jax        (501) staff       (20)   184912 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 jax        (501) staff       (20)   328412 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 jax        (501) staff       (20)   195704 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 jax        (501) staff       (20)   309192 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 jax        (501) staff       (20)   182708 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 jax        (501) staff       (20)   135314 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/css/theme.css
--rw-r--r--   0 jax        (501) staff       (20)     4472 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/doctools.js
--rw-r--r--   0 jax        (501) staff       (20)      329 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_static/documentation_options.js
--rw-r--r--   0 jax        (501) staff       (20)      286 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/file.png
--rw-r--r--   0 jax        (501) staff       (20)    57336 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/ico.jpg
--rw-r--r--   0 jax        (501) staff       (20)    18313 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_static/icon.svg
--rw-r--r--   0 jax        (501) staff       (20)    89501 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/jquery.js
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.358295 rocs_client-1.3.7/docs/_static/js/
--rw-r--r--   0 jax        (501) staff       (20)      934 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/js/badge_only.js
--rw-r--r--   0 jax        (501) staff       (20)     4370 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 jax        (501) staff       (20)     2734 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 jax        (501) staff       (20)     5023 2024-01-08 09:51:47.000000 rocs_client-1.3.7/docs/_static/js/theme.js
--rw-r--r--   0 jax        (501) staff       (20)     4758 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/language_data.js
--rw-r--r--   0 jax        (501) staff       (20)       90 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/minus.png
--rw-r--r--   0 jax        (501) staff       (20)       68 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/_static/my_theme.css
--rw-r--r--   0 jax        (501) staff       (20)       90 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/plus.png
--rw-r--r--   0 jax        (501) staff       (20)     4902 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/pygments.css
--rw-r--r--   0 jax        (501) staff       (20)    18732 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/searchtools.js
--rw-r--r--   0 jax        (501) staff       (20)     5123 2024-01-16 07:26:13.000000 rocs_client-1.3.7/docs/_static/sphinx_highlight.js
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.358627 rocs_client-1.3.7/docs/genindex/
--rw-r--r--   0 jax        (501) staff       (20)    18224 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/genindex/index.html
--rw-r--r--   0 jax        (501) staff       (20)     6607 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.359055 rocs_client-1.3.7/docs/modules/
--rw-r--r--   0 jax        (501) staff       (20)     5672 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/modules/index.html
--rw-r--r--   0 jax        (501) staff       (20)      873 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/objects.inv
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.359346 rocs_client-1.3.7/docs/py-modindex/
--rw-r--r--   0 jax        (501) staff       (20)     6147 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/py-modindex/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.359637 rocs_client-1.3.7/docs/rocs_client/
--rw-r--r--   0 jax        (501) staff       (20)     7968 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/rocs_client/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.360160 rocs_client-1.3.7/docs/rocs_client.common/
--rw-r--r--   0 jax        (501) staff       (20)    11153 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/rocs_client.common/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.360533 rocs_client-1.3.7/docs/rocs_client.end_effector/
--rw-r--r--   0 jax        (501) staff       (20)    22750 2024-01-16 03:34:29.000000 rocs_client-1.3.7/docs/rocs_client.end_effector/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.360935 rocs_client-1.3.7/docs/rocs_client.motor/
--rw-r--r--   0 jax        (501) staff       (20)    26813 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/rocs_client.motor/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.361317 rocs_client-1.3.7/docs/rocs_client.robot/
--rw-r--r--   0 jax        (501) staff       (20)    86720 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/rocs_client.robot/index.html
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.363730 rocs_client-1.3.7/docs/search/
--rw-r--r--   0 jax        (501) staff       (20)     3922 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/search/index.html
--rw-r--r--   0 jax        (501) staff       (20)    20164 2024-01-22 03:11:33.000000 rocs_client-1.3.7/docs/searchindex.js
--rw-r--r--   0 jax        (501) staff       (20)      765 2024-02-22 11:05:12.000000 rocs_client-1.3.7/pyproject.toml
--rw-r--r--   0 jax        (501) staff       (20)      188 2023-12-28 11:00:45.000000 rocs_client-1.3.7/requirements.txt
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.365228 rocs_client-1.3.7/rocs_client/
--rw-r--r--   0 jax        (501) staff       (20)     1878 2024-01-16 03:34:29.000000 rocs_client-1.3.7/rocs_client/__init__.py
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.366883 rocs_client-1.3.7/rocs_client/common/
--rw-r--r--   0 jax        (501) staff       (20)      247 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/common/__init__.py
--rw-r--r--   0 jax        (501) staff       (20)     1551 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/common/camera.py
--rw-r--r--   0 jax        (501) staff       (20)      244 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/common/system.py
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.367351 rocs_client-1.3.7/rocs_client/end_effector/
--rw-r--r--   0 jax        (501) staff       (20)       57 2024-01-16 03:34:29.000000 rocs_client-1.3.7/rocs_client/end_effector/__init__.py
--rw-r--r--   0 jax        (501) staff       (20)     3166 2024-04-16 09:23:08.000000 rocs_client-1.3.7/rocs_client/end_effector/end_effector.py
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.367637 rocs_client-1.3.7/rocs_client/motor/
--rw-r--r--   0 jax        (501) staff       (20)      383 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/motor/__init__.py
--rw-r--r--   0 jax        (501) staff       (20)     8246 2023-12-14 02:00:49.000000 rocs_client-1.3.7/rocs_client/motor/motor.py
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.368682 rocs_client-1.3.7/rocs_client/robot/
--rw-r--r--   0 jax        (501) staff       (20)     1468 2024-01-08 04:56:54.000000 rocs_client-1.3.7/rocs_client/robot/__init__.py
--rw-r--r--   0 jax        (501) staff       (20)     3288 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/robot/car.py
--rw-r--r--   0 jax        (501) staff       (20)    22492 2024-02-19 02:54:09.000000 rocs_client-1.3.7/rocs_client/robot/human.py
--rw-r--r--   0 jax        (501) staff       (20)    10151 2024-01-08 09:05:41.000000 rocs_client-1.3.7/rocs_client/robot/robot_base.py
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.369870 rocs_client-1.3.7/rocs_client.egg-info/
--rw-r--r--   0 jax        (501) staff       (20)    14004 2024-04-16 09:23:56.000000 rocs_client-1.3.7/rocs_client.egg-info/PKG-INFO
--rw-r--r--   0 jax        (501) staff       (20)     2793 2024-04-16 09:23:56.000000 rocs_client-1.3.7/rocs_client.egg-info/SOURCES.txt
--rw-r--r--   0 jax        (501) staff       (20)        1 2024-04-16 09:23:56.000000 rocs_client-1.3.7/rocs_client.egg-info/dependency_links.txt
--rw-r--r--   0 jax        (501) staff       (20)       41 2024-04-16 09:23:56.000000 rocs_client-1.3.7/rocs_client.egg-info/requires.txt
--rw-r--r--   0 jax        (501) staff       (20)       12 2024-04-16 09:23:56.000000 rocs_client-1.3.7/rocs_client.egg-info/top_level.txt
--rw-r--r--   0 jax        (501) staff       (20)       38 2024-04-16 09:23:56.370600 rocs_client-1.3.7/setup.cfg
-drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:23:56.369661 rocs_client-1.3.7/test/
--rw-r--r--   0 jax        (501) staff       (20)      520 2023-12-05 04:31:02.000000 rocs_client-1.3.7/test/test_car.py
--rw-r--r--   0 jax        (501) staff       (20)     2148 2024-01-16 09:18:32.000000 rocs_client-1.3.7/test/test_end_effector.py
--rw-r--r--   0 jax        (501) staff       (20)     3342 2024-03-12 08:57:20.000000 rocs_client-1.3.7/test/test_human.py
--rw-r--r--   0 jax        (501) staff       (20)     8529 2024-03-12 08:57:30.000000 rocs_client-1.3.7/test/test_motor.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.323107 rocs_client-1.3.8/
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.303627 rocs_client-1.3.8/.github/
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.306530 rocs_client-1.3.8/.github/workflows/
+-rw-r--r--   0 jax        (501) staff       (20)     1250 2023-12-05 04:31:02.000000 rocs_client-1.3.8/.github/workflows/static.yml
+-rw-r--r--   0 jax        (501) staff       (20)      497 2023-12-05 03:43:04.000000 rocs_client-1.3.8/.gitignore
+-rw-r--r--   0 jax        (501) staff       (20)     1073 2023-12-05 03:43:04.000000 rocs_client-1.3.8/LICENSE
+-rw-r--r--   0 jax        (501) staff       (20)    14004 2024-04-16 09:43:36.322805 rocs_client-1.3.8/PKG-INFO
+-rw-r--r--   0 jax        (501) staff       (20)    13350 2024-01-16 09:36:24.000000 rocs_client-1.3.8/README.md
+-rw-r--r--   0 jax        (501) staff       (20)      105 2024-01-16 07:23:48.000000 rocs_client-1.3.8/deploy_pypi.sh
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.307326 rocs_client-1.3.8/doc/
+-rw-r--r--   0 jax        (501) staff       (20)      638 2023-12-05 03:43:04.000000 rocs_client-1.3.8/doc/Makefile
+-rw-r--r--   0 jax        (501) staff       (20)      246 2024-01-16 03:34:29.000000 rocs_client-1.3.8/doc/build_doc.sh
+-rw-r--r--   0 jax        (501) staff       (20)      484 2024-01-04 09:33:19.000000 rocs_client-1.3.8/doc/conf.py
+-rw-r--r--   0 jax        (501) staff       (20)    57336 2023-12-05 03:43:04.000000 rocs_client-1.3.8/doc/ico.jpg
+-rw-r--r--   0 jax        (501) staff       (20)      785 2024-01-16 03:34:29.000000 rocs_client-1.3.8/doc/index.rst
+-rw-r--r--   0 jax        (501) staff       (20)      769 2023-12-05 03:43:04.000000 rocs_client-1.3.8/doc/make.bat
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.307939 rocs_client-1.3.8/docs/
+-rw-r--r--   0 jax        (501) staff       (20)      230 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/.buildinfo
+-rw-r--r--   0 jax        (501) staff       (20)        0 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/.nojekyll
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.308791 rocs_client-1.3.8/docs/_sources/
+-rw-r--r--   0 jax        (501) staff       (20)      887 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_sources/index.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)       76 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_sources/modules.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)      460 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_sources/rocs_client.common.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)      428 2024-01-16 03:34:29.000000 rocs_client-1.3.8/docs/_sources/rocs_client.end_effector.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)      306 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_sources/rocs_client.motor.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)      592 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_sources/rocs_client.robot.rst.txt
+-rw-r--r--   0 jax        (501) staff       (20)      278 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_sources/rocs_client.rst.txt
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.310806 rocs_client-1.3.8/docs/_static/
+-rw-r--r--   0 jax        (501) staff       (20)     4289 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 jax        (501) staff       (20)    15094 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/basic.css
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.311062 rocs_client-1.3.8/docs/_static/css/
+-rw-r--r--   0 jax        (501) staff       (20)     3229 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/badge_only.css
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.317314 rocs_client-1.3.8/docs/_static/css/fonts/
+-rw-r--r--   0 jax        (501) staff       (20)    87624 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 jax        (501) staff       (20)    67312 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 jax        (501) staff       (20)    86288 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 jax        (501) staff       (20)    66444 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   165742 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 jax        (501) staff       (20)   444379 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 jax        (501) staff       (20)   165548 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 jax        (501) staff       (20)    98024 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 jax        (501) staff       (20)    77160 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   323344 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 jax        (501) staff       (20)   193308 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   309728 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 jax        (501) staff       (20)   184912 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   328412 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 jax        (501) staff       (20)   195704 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   309192 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 jax        (501) staff       (20)   182708 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 jax        (501) staff       (20)   135314 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/css/theme.css
+-rw-r--r--   0 jax        (501) staff       (20)     4472 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/doctools.js
+-rw-r--r--   0 jax        (501) staff       (20)      329 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_static/documentation_options.js
+-rw-r--r--   0 jax        (501) staff       (20)      286 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/file.png
+-rw-r--r--   0 jax        (501) staff       (20)    57336 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/ico.jpg
+-rw-r--r--   0 jax        (501) staff       (20)    18313 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_static/icon.svg
+-rw-r--r--   0 jax        (501) staff       (20)    89501 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/jquery.js
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.317976 rocs_client-1.3.8/docs/_static/js/
+-rw-r--r--   0 jax        (501) staff       (20)      934 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/js/badge_only.js
+-rw-r--r--   0 jax        (501) staff       (20)     4370 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 jax        (501) staff       (20)     2734 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 jax        (501) staff       (20)     5023 2024-01-08 09:51:47.000000 rocs_client-1.3.8/docs/_static/js/theme.js
+-rw-r--r--   0 jax        (501) staff       (20)     4758 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/language_data.js
+-rw-r--r--   0 jax        (501) staff       (20)       90 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/minus.png
+-rw-r--r--   0 jax        (501) staff       (20)       68 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/_static/my_theme.css
+-rw-r--r--   0 jax        (501) staff       (20)       90 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/plus.png
+-rw-r--r--   0 jax        (501) staff       (20)     4902 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/pygments.css
+-rw-r--r--   0 jax        (501) staff       (20)    18732 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/searchtools.js
+-rw-r--r--   0 jax        (501) staff       (20)     5123 2024-01-16 07:26:13.000000 rocs_client-1.3.8/docs/_static/sphinx_highlight.js
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318126 rocs_client-1.3.8/docs/genindex/
+-rw-r--r--   0 jax        (501) staff       (20)    18224 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/genindex/index.html
+-rw-r--r--   0 jax        (501) staff       (20)     6607 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318274 rocs_client-1.3.8/docs/modules/
+-rw-r--r--   0 jax        (501) staff       (20)     5672 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/modules/index.html
+-rw-r--r--   0 jax        (501) staff       (20)      873 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/objects.inv
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318424 rocs_client-1.3.8/docs/py-modindex/
+-rw-r--r--   0 jax        (501) staff       (20)     6147 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/py-modindex/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318566 rocs_client-1.3.8/docs/rocs_client/
+-rw-r--r--   0 jax        (501) staff       (20)     7968 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/rocs_client/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318709 rocs_client-1.3.8/docs/rocs_client.common/
+-rw-r--r--   0 jax        (501) staff       (20)    11153 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/rocs_client.common/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.318973 rocs_client-1.3.8/docs/rocs_client.end_effector/
+-rw-r--r--   0 jax        (501) staff       (20)    22750 2024-01-16 03:34:29.000000 rocs_client-1.3.8/docs/rocs_client.end_effector/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.319120 rocs_client-1.3.8/docs/rocs_client.motor/
+-rw-r--r--   0 jax        (501) staff       (20)    26813 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/rocs_client.motor/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.319282 rocs_client-1.3.8/docs/rocs_client.robot/
+-rw-r--r--   0 jax        (501) staff       (20)    86720 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/rocs_client.robot/index.html
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.319494 rocs_client-1.3.8/docs/search/
+-rw-r--r--   0 jax        (501) staff       (20)     3922 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/search/index.html
+-rw-r--r--   0 jax        (501) staff       (20)    20164 2024-01-22 03:11:33.000000 rocs_client-1.3.8/docs/searchindex.js
+-rw-r--r--   0 jax        (501) staff       (20)      765 2024-04-16 09:36:08.000000 rocs_client-1.3.8/pyproject.toml
+-rw-r--r--   0 jax        (501) staff       (20)      188 2023-12-28 11:00:45.000000 rocs_client-1.3.8/requirements.txt
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.319634 rocs_client-1.3.8/rocs_client/
+-rw-r--r--   0 jax        (501) staff       (20)     1878 2024-01-16 03:34:29.000000 rocs_client-1.3.8/rocs_client/__init__.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.320675 rocs_client-1.3.8/rocs_client/common/
+-rw-r--r--   0 jax        (501) staff       (20)      247 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/common/__init__.py
+-rw-r--r--   0 jax        (501) staff       (20)     1551 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/common/camera.py
+-rw-r--r--   0 jax        (501) staff       (20)      244 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/common/system.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.320935 rocs_client-1.3.8/rocs_client/end_effector/
+-rw-r--r--   0 jax        (501) staff       (20)       57 2024-01-16 03:34:29.000000 rocs_client-1.3.8/rocs_client/end_effector/__init__.py
+-rw-r--r--   0 jax        (501) staff       (20)     3191 2024-04-16 09:40:08.000000 rocs_client-1.3.8/rocs_client/end_effector/end_effector.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.321215 rocs_client-1.3.8/rocs_client/motor/
+-rw-r--r--   0 jax        (501) staff       (20)      383 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/motor/__init__.py
+-rw-r--r--   0 jax        (501) staff       (20)     8246 2023-12-14 02:00:49.000000 rocs_client-1.3.8/rocs_client/motor/motor.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.321761 rocs_client-1.3.8/rocs_client/robot/
+-rw-r--r--   0 jax        (501) staff       (20)     1468 2024-01-08 04:56:54.000000 rocs_client-1.3.8/rocs_client/robot/__init__.py
+-rw-r--r--   0 jax        (501) staff       (20)     3288 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/robot/car.py
+-rw-r--r--   0 jax        (501) staff       (20)    22492 2024-02-19 02:54:09.000000 rocs_client-1.3.8/rocs_client/robot/human.py
+-rw-r--r--   0 jax        (501) staff       (20)    10151 2024-01-08 09:05:41.000000 rocs_client-1.3.8/rocs_client/robot/robot_base.py
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.322476 rocs_client-1.3.8/rocs_client.egg-info/
+-rw-r--r--   0 jax        (501) staff       (20)    14004 2024-04-16 09:43:36.000000 rocs_client-1.3.8/rocs_client.egg-info/PKG-INFO
+-rw-r--r--   0 jax        (501) staff       (20)     2793 2024-04-16 09:43:36.000000 rocs_client-1.3.8/rocs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jax        (501) staff       (20)        1 2024-04-16 09:43:36.000000 rocs_client-1.3.8/rocs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jax        (501) staff       (20)       41 2024-04-16 09:43:36.000000 rocs_client-1.3.8/rocs_client.egg-info/requires.txt
+-rw-r--r--   0 jax        (501) staff       (20)       12 2024-04-16 09:43:36.000000 rocs_client-1.3.8/rocs_client.egg-info/top_level.txt
+-rw-r--r--   0 jax        (501) staff       (20)       38 2024-04-16 09:43:36.323149 rocs_client-1.3.8/setup.cfg
+drwxr-xr-x   0 jax        (501) staff       (20)        0 2024-04-16 09:43:36.322280 rocs_client-1.3.8/test/
+-rw-r--r--   0 jax        (501) staff       (20)      520 2023-12-05 04:31:02.000000 rocs_client-1.3.8/test/test_car.py
+-rw-r--r--   0 jax        (501) staff       (20)     2152 2024-04-16 09:39:12.000000 rocs_client-1.3.8/test/test_end_effector.py
+-rw-r--r--   0 jax        (501) staff       (20)     3211 2024-04-16 09:36:20.000000 rocs_client-1.3.8/test/test_human.py
+-rw-r--r--   0 jax        (501) staff       (20)     8529 2024-03-12 08:57:30.000000 rocs_client-1.3.8/test/test_motor.py
```

### Comparing `rocs_client-1.3.7/.github/workflows/static.yml` & `rocs_client-1.3.8/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/LICENSE` & `rocs_client-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/PKG-INFO` & `rocs_client-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocs_client
-Version: 1.3.7
+Version: 1.3.8
 Summary: Fourier General Robotics OS - Client Library (python)
 Author-email: jax <ming.li@fftai.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FFTAI/rocs_client_py
 Project-URL: Bug Tracker, https://github.com/FFTAI/rocs_client_py/issues
 Project-URL: Blog, https://fftai.github.io/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rocs_client-1.3.7/README.md` & `rocs_client-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/doc/Makefile` & `rocs_client-1.3.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/doc/ico.jpg` & `rocs_client-1.3.8/doc/ico.jpg`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/doc/index.rst` & `rocs_client-1.3.8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/doc/make.bat` & `rocs_client-1.3.8/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_sources/index.rst.txt` & `rocs_client-1.3.8/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_sources/rocs_client.robot.rst.txt` & `rocs_client-1.3.8/docs/_sources/rocs_client.robot.rst.txt`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/_sphinx_javascript_frameworks_compat.js` & `rocs_client-1.3.8/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/basic.css` & `rocs_client-1.3.8/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/badge_only.css` & `rocs_client-1.3.8/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.eot` & `rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.svg` & `rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.ttf` & `rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/fontawesome-webfont.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-bold-italic.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-bold-italic.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-bold.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-bold.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-normal-italic.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-normal-italic.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-normal.woff` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/fonts/lato-normal.woff2` & `rocs_client-1.3.8/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/css/theme.css` & `rocs_client-1.3.8/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/doctools.js` & `rocs_client-1.3.8/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/ico.jpg` & `rocs_client-1.3.8/docs/_static/ico.jpg`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/icon.svg` & `rocs_client-1.3.8/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/jquery.js` & `rocs_client-1.3.8/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/js/badge_only.js` & `rocs_client-1.3.8/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/js/html5shiv-printshiv.min.js` & `rocs_client-1.3.8/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/js/html5shiv.min.js` & `rocs_client-1.3.8/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/js/theme.js` & `rocs_client-1.3.8/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/language_data.js` & `rocs_client-1.3.8/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/pygments.css` & `rocs_client-1.3.8/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/searchtools.js` & `rocs_client-1.3.8/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/_static/sphinx_highlight.js` & `rocs_client-1.3.8/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/genindex/index.html` & `rocs_client-1.3.8/docs/genindex/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/index.html` & `rocs_client-1.3.8/docs/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/modules/index.html` & `rocs_client-1.3.8/docs/modules/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/objects.inv` & `rocs_client-1.3.8/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/py-modindex/index.html` & `rocs_client-1.3.8/docs/py-modindex/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/rocs_client/index.html` & `rocs_client-1.3.8/docs/rocs_client/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/rocs_client.common/index.html` & `rocs_client-1.3.8/docs/rocs_client.common/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/rocs_client.end_effector/index.html` & `rocs_client-1.3.8/docs/rocs_client.end_effector/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/rocs_client.motor/index.html` & `rocs_client-1.3.8/docs/rocs_client.motor/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/rocs_client.robot/index.html` & `rocs_client-1.3.8/docs/rocs_client.robot/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/search/index.html` & `rocs_client-1.3.8/docs/search/index.html`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/docs/searchindex.js` & `rocs_client-1.3.8/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/pyproject.toml` & `rocs_client-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "setuptools_scm",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rocs_client"
-version = "1.3.7"
+version = "1.3.8"
 authors = [{name = "jax", email = "ming.li@fftai.com"}]
 license = {text = "MIT"}
 requires-python = ">=3.8"
 description = "Fourier General Robotics OS - Client Library (python)"
 readme="README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
```

### Comparing `rocs_client-1.3.7/rocs_client/__init__.py` & `rocs_client-1.3.8/rocs_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/common/camera.py` & `rocs_client-1.3.8/rocs_client/common/camera.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/end_effector/end_effector.py` & `rocs_client-1.3.8/rocs_client/end_effector/end_effector.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 "qy": param.qy,
                 "qz": param.qz,
                 "qw": param.qw,
                 "vx": param.vx,
                 "vy": param.vy,
                 "vz": param.vz
             },
-            "system": 0
+            "system": 1
         }
         self._send_websocket_msg({'command': 'left_hand_pr', 'data': data})
 
     def control_right(self, param: EndEffectorScheme):
         """ Controlling right hand """
         data = {
             "param": {
@@ -92,10 +92,11 @@
                 "qx": param.qx,
                 "qy": param.qy,
                 "qz": param.qz,
                 "qw": param.qw,
                 "vx": param.vx,
                 "vy": param.vy,
                 "vz": param.vz
-            }
+            },
+            "system": 1
         }
         self._send_websocket_msg({'command': 'right_hand_pr', 'data': data})
```

### Comparing `rocs_client-1.3.7/rocs_client/motor/motor.py` & `rocs_client-1.3.8/rocs_client/motor/motor.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/robot/__init__.py` & `rocs_client-1.3.8/rocs_client/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/robot/car.py` & `rocs_client-1.3.8/rocs_client/robot/car.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/robot/human.py` & `rocs_client-1.3.8/rocs_client/robot/human.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client/robot/robot_base.py` & `rocs_client-1.3.8/rocs_client/robot/robot_base.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/rocs_client.egg-info/PKG-INFO` & `rocs_client-1.3.8/rocs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocs_client
-Version: 1.3.7
+Version: 1.3.8
 Summary: Fourier General Robotics OS - Client Library (python)
 Author-email: jax <ming.li@fftai.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FFTAI/rocs_client_py
 Project-URL: Bug Tracker, https://github.com/FFTAI/rocs_client_py/issues
 Project-URL: Blog, https://fftai.github.io/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rocs_client-1.3.7/rocs_client.egg-info/SOURCES.txt` & `rocs_client-1.3.8/rocs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/test/test_car.py` & `rocs_client-1.3.8/test/test_car.py`

 * *Files identical despite different names*

### Comparing `rocs_client-1.3.7/test/test_end_effector.py` & `rocs_client-1.3.8/test/test_end_effector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     print("WebSocket closed")
 
 
 async def on_error(error: Exception):
     print("WebSocket error:", error)
 
 
-end_effector = EndEffector(host="127.0.0.1",
+end_effector = EndEffector(host="192.168.9.168",
                            on_connected=on_connected, on_message=on_message, on_close=on_close, on_error=on_error)
 
 
 class TestEndEffector(unittest.TestCase):
 
     def test_enable(self):
         """ Enable the end control service.
```

### Comparing `rocs_client-1.3.7/test/test_motor.py` & `rocs_client-1.3.8/test/test_motor.py`

 * *Files identical despite different names*

