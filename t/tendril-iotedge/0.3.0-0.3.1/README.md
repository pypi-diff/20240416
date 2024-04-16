# Comparing `tmp/tendril-iotedge-0.3.0.tar.gz` & `tmp/tendril_iotedge-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-iotedge-0.3.0.tar", last modified: Sat Mar 30 00:17:20 2024, max compression
+gzip compressed data, was "tendril_iotedge-0.3.1.tar", last modified: Tue Apr 16 18:44:32 2024, max compression
```

## Comparing `tendril-iotedge-0.3.0.tar` & `tendril_iotedge-0.3.1.tar`

### file list

```diff
@@ -1,78 +1,83 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.592032 tendril-iotedge-0.3.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2024-03-30 00:17:20.592032 tendril-iotedge-0.3.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.580032 tendril-iotedge-0.3.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-03-30 00:17:20.592032 tendril-iotedge-0.3.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-08-29 06:16:15.000000 tendril-iotedge-0.3.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.576032 tendril-iotedge-0.3.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2024-03-30 00:00:45.000000 tendril-iotedge-0.3.0/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2909 2023-09-01 12:23:47.000000 tendril-iotedge-0.3.0/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.584032 tendril-iotedge-0.3.0/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril-iotedge-0.3.0/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril-iotedge-0.3.0/src/tendril/common/iotcore/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.3.0/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril-iotedge-0.3.0/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.3.0/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-03-29 23:49:43.000000 tendril-iotedge-0.3.0/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.3.0/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.3.0/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      487 2023-08-05 17:25:22.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/heartbeat.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.588032 tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1916 2023-08-12 07:56:01.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril-iotedge-0.3.0/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.592032 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2024-03-30 00:17:20.000000 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1575 2024-03-30 00:17:20.000000 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-03-30 00:17:20.000000 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2024-03-30 00:17:20.000000 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-03-30 00:17:20.000000 tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 00:17:20.592032 tendril-iotedge-0.3.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.3.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.535465 tendril_iotedge-0.3.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.539465 tendril_iotedge-0.3.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-08-29 06:16:15.000000 tendril_iotedge-0.3.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.531465 tendril_iotedge-0.3.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2024-04-05 13:17:24.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2909 2023-09-01 12:23:47.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril_iotedge-0.3.1/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.1/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.1/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      341 2024-04-16 18:36:14.000000 tendril_iotedge-0.3.1/src/tendril/core/topology/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.1/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.1/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril_iotedge-0.3.1/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      487 2023-08-05 17:25:22.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/heartbeat.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1916 2023-08-12 07:56:01.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1679 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tox.ini
```

### Comparing `tendril-iotedge-0.3.0/.gitignore` & `tendril_iotedge-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/.readthedocs.yml` & `tendril_iotedge-0.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/.travis.yml` & `tendril_iotedge-0.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/LICENSE` & `tendril_iotedge-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/README.rst` & `tendril_iotedge-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/Makefile` & `tendril_iotedge-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/_static/custom.css` & `tendril_iotedge-0.3.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/_static/favicon.ico` & `tendril_iotedge-0.3.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/_static/logo.png` & `tendril_iotedge-0.3.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/_static/logo_packed.png` & `tendril_iotedge-0.3.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/_templates/about.html` & `tendril_iotedge-0.3.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/conf.py` & `tendril_iotedge-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/index.rst` & `tendril_iotedge-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/docs/installation.rst` & `tendril_iotedge-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/setup.py` & `tendril_iotedge-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/apiserver/routers/iotcore.py` & `tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotcore.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/apiserver/routers/iotedge.py` & `tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/common/iotedge/exceptions.py` & `tendril_iotedge-0.3.1/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/common/iotedge/formats.py` & `tendril_iotedge-0.3.1/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/config/__init__.py` & `tendril_iotedge-0.3.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/config/iotedge.py` & `tendril_iotedge-0.3.1/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/db/models/deviceconfig.py` & `tendril_iotedge-0.3.1/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/iotcore/settings.py` & `tendril_iotedge-0.3.1/src/tendril/iotcore/settings.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/iotedge/announce.py` & `tendril_iotedge-0.3.1/src/tendril/iotedge/announce.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/base.py` & `tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/base.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/iotedge/profiles/manager.py` & `tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril/iotedge/registration.py` & `tendril_iotedge-0.3.1/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 src/tendril/common/iotcore/exceptions.py
 src/tendril/common/iotcore/formats.py
 src/tendril/common/iotedge/__init__.py
 src/tendril/common/iotedge/exceptions.py
 src/tendril/common/iotedge/formats.py
 src/tendril/config/__init__.py
 src/tendril/config/iotedge.py
+src/tendril/core/__init__.py
+src/tendril/core/topology/__init__.py
+src/tendril/core/topology/iotedge.py
 src/tendril/db/__init__.py
 src/tendril/db/models/__init__.py
 src/tendril/db/models/deviceconfig.py
 src/tendril/iotcore/__init__.py
 src/tendril/iotcore/settings.py
 src/tendril/iotedge/__init__.py
 src/tendril/iotedge/announce.py
```

### Comparing `tendril-iotedge-0.3.0/src/tendril_iotedge.egg-info/requires.txt` & `tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/tests/coveralls.py` & `tendril_iotedge-0.3.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.3.0/tox.ini` & `tendril_iotedge-0.3.1/tox.ini`

 * *Files identical despite different names*

