# Comparing `tmp/tendril-connector-rabbitmq-0.1.7.tar.gz` & `tmp/tendril_connector_rabbitmq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-connector-rabbitmq-0.1.7.tar", last modified: Tue Sep 12 19:13:25 2023, max compression
+gzip compressed data, was "tendril_connector_rabbitmq-0.2.0.tar", last modified: Tue Apr 16 18:38:39 2024, max compression
```

## Comparing `tendril-connector-rabbitmq-0.1.7.tar` & `tendril_connector_rabbitmq-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3708 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.412447 tendril-connector-rabbitmq-0.1.7/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-connector-rabbitmq-0.1.7/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril-connector-rabbitmq-0.1.7/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.408447 tendril-connector-rabbitmq-0.1.7/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/config/mq.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/config/mq_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.416447 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/rabbitmq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/rabbitmq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3958 2023-08-11 17:15:46.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/rabbitmq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/rabbitmq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2410 2023-09-12 19:07:57.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      546 2023-08-04 21:03:31.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/aio_base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3708 2023-09-12 19:13:25.000000 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2023-09-12 19:13:25.000000 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-09-12 19:13:25.000000 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2023-09-12 19:13:25.000000 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-09-12 19:13:25.000000 tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 19:13:25.420447 tendril-connector-rabbitmq-0.1.7/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril-connector-rabbitmq-0.1.7/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.197510 tendril_connector_rabbitmq-0.2.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-16 18:38:39.193510 tendril_connector_rabbitmq-0.2.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.181510 tendril_connector_rabbitmq-0.2.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_rabbitmq-0.2.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:38:39.197510 tendril_connector_rabbitmq-0.2.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril_connector_rabbitmq-0.2.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.177510 tendril_connector_rabbitmq-0.2.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5677 2024-04-16 18:27:08.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2716 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      816 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio_base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tox.ini
```

### Comparing `tendril-connector-rabbitmq-0.1.7/.gitignore` & `tendril_connector_rabbitmq-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/.readthedocs.yml` & `tendril_connector_rabbitmq-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/.travis.yml` & `tendril_connector_rabbitmq-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/LICENSE` & `tendril_connector_rabbitmq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/README.rst` & `tendril_connector_rabbitmq-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/Makefile` & `tendril_connector_rabbitmq-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/_static/custom.css` & `tendril_connector_rabbitmq-0.2.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/_static/favicon.ico` & `tendril_connector_rabbitmq-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/_static/logo.png` & `tendril_connector_rabbitmq-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/_static/logo_packed.png` & `tendril_connector_rabbitmq-0.2.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/_templates/about.html` & `tendril_connector_rabbitmq-0.2.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/conf.py` & `tendril_connector_rabbitmq-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/index.rst` & `tendril_connector_rabbitmq-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/docs/installation.rst` & `tendril_connector_rabbitmq-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/setup.py` & `tendril_connector_rabbitmq-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril/config/__init__.py` & `tendril_connector_rabbitmq-0.2.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril/config/mq.py` & `tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril/config/mq_core.py` & `tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq_core.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril/connectors/rabbitmq/tx.py` & `tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/tx.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril/core/mq/aio.py` & `tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,57 +2,62 @@
 
 import asyncio
 import importlib
 from functools import wraps
 from contextlib import asynccontextmanager
 
 from .aio_base import GenericMQAsyncClient
+from .aio_base import MQServerNotEnabled
 from tendril.config import MQ_ENABLED
 from tendril.config import APISERVER_ENABLED
 from tendril.utils.versions import get_namespace_package_names
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 if True:
     from tendril.connectors.rabbitmq import aio
     MQManager = aio.manager
     MQClientClass = aio.client_class
 
 
-def with_mq_client(func):
-    @wraps(func)
-    async def wrapper(*args, **kwargs):
-        if 'mq' in kwargs.keys() and kwargs['mq']:
-            result = await func(*args, **kwargs)
-            return result
-        manager = await MQManager.get_instance()
-        async with manager.get_channel() as channel:
-            mq = MQClientClass(channel)
-            kwargs['mq'] = mq
-            result = await func(*args, **kwargs)
-            return result
+def with_mq_client(code='default'):
+    def wrapper(func):
+        @wraps(func)
+        async def inner_wrapper(*args, **kwargs):
+            if 'mq' in kwargs.keys() and kwargs['mq']:
+                result = await func(*args, **kwargs)
+                return result
+            manager = await MQManager.get_instance()
+            async with manager.get_channel(code=code) as channel:
+                mq = MQClientClass(channel, code=code)
+                kwargs['mq'] = mq
+                result = await func(*args, **kwargs)
+                return result
+        return inner_wrapper
     return wrapper
 
 
-@with_mq_client  # Use the decorator to inject a client object
+@with_mq_client()  # Use the decorator to inject a client object
 async def example(mq: GenericMQAsyncClient):  # Accept a client object as an argument
     await mq.send_message("test", "Hello world")
     message = await mq.receive_message("test")
     print(message)
 
 
 async def install_topology(prefix='tendril.core.topology'):
     logger.info("Loading MQ Topologies from '{0}.*'".format(prefix))
     for modname in get_namespace_package_names(prefix):
         try:
             globals()[modname] = importlib.import_module(modname)
             if hasattr(globals()[modname], 'create_mq_topology'):
                 logger.debug(f"Installing MQ Topology from {modname}")
                 await globals()[modname].create_mq_topology()
+        except MQServerNotEnabled as e:
+            logger.debug(f"Skipping topology installation on disabled MQ Server {e.code}")
         except ImportError as e:
             logger.debug(e)
 
 
 async def startup():
     manager = await MQManager.get_instance()
     await manager.init(loop=asyncio.get_running_loop())
```

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt` & `tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/src/tendril_connector_rabbitmq.egg-info/requires.txt` & `tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/tests/coveralls.py` & `tendril_connector_rabbitmq-0.2.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-rabbitmq-0.1.7/tox.ini` & `tendril_connector_rabbitmq-0.2.0/tox.ini`

 * *Files identical despite different names*

