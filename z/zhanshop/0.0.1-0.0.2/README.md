# Comparing `tmp/zhanshop-0.0.1.tar.gz` & `tmp/zhanshop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhanshop-0.0.1.tar", last modified: Thu Apr 11 11:48:14 2024, max compression
+gzip compressed data, was "zhanshop-0.0.2.tar", last modified: Tue Apr 16 09:15:48 2024, max compression
```

## Comparing `zhanshop-0.0.1.tar` & `zhanshop-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:48:14.074377 zhanshop-0.0.1/
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)    11357 2024-04-11 11:35:11.000000 zhanshop-0.0.1/LICENSE
--rw-r--r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       74 2024-04-11 11:48:14.074377 zhanshop-0.0.1/PKG-INFO
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       44 2024-04-11 11:41:41.000000 zhanshop-0.0.1/README.md
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       46 2024-04-11 11:45:19.000000 zhanshop-0.0.1/pyproject.toml
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       82 2024-04-11 11:48:14.074377 zhanshop-0.0.1/setup.cfg
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       79 2024-04-11 11:47:23.000000 zhanshop-0.0.1/setup.py
-drwxrwxr-x   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:48:14.074377 zhanshop-0.0.1/src/
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/app.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/config.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/console.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/container.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/curl.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/database.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/env.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/helper.py
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:35:11.000000 zhanshop-0.0.1/src/log.py
-drwxrwxr-x   0 zhangqiquan  (1000) zhangqiquan  (1000)        0 2024-04-11 11:48:14.074377 zhanshop-0.0.1/src/zhanshop.egg-info/
--rw-r--r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       74 2024-04-11 11:48:14.000000 zhanshop-0.0.1/src/zhanshop.egg-info/PKG-INFO
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)      316 2024-04-11 11:48:14.000000 zhanshop-0.0.1/src/zhanshop.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)        1 2024-04-11 11:48:14.000000 zhanshop-0.0.1/src/zhanshop.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangqiquan  (1000) zhangqiquan  (1000)       58 2024-04-11 11:48:14.000000 zhanshop-0.0.1/src/zhanshop.egg-info/top_level.txt
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.362721 zhanshop-0.0.2/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)     1100 2024-04-16 02:30:09.000000 zhanshop-0.0.2/LICENSE
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-16 09:15:48.361842 zhanshop-0.0.2/PKG-INFO
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      440 2024-04-16 02:37:57.000000 zhanshop-0.0.2/README.md
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       46 2024-04-16 09:15:27.000000 zhanshop-0.0.2/pyproject.toml
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       82 2024-04-16 09:15:48.365747 zhanshop-0.0.2/setup.cfg
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      318 2024-04-16 09:15:21.000000 zhanshop-0.0.2/setup.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.340173 zhanshop-0.0.2/test/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      104 2024-04-16 02:30:09.000000 zhanshop-0.0.2/test/test_zhanshop.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.345425 zhanshop-0.0.2/zhanshop/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      170 2024-04-16 05:37:08.000000 zhanshop-0.0.2/zhanshop/app.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.354752 zhanshop-0.0.2/zhanshop/command/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       73 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/command/__init__.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      130 2024-04-16 07:09:51.000000 zhanshop-0.0.2/zhanshop/command/helper.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      658 2024-04-16 05:51:46.000000 zhanshop-0.0.2/zhanshop/command/server.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      889 2024-04-16 07:09:08.000000 zhanshop-0.0.2/zhanshop/console.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      397 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/container.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      373 2024-04-16 08:43:54.000000 zhanshop-0.0.2/zhanshop/controller.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      234 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/helper.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      459 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/log.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      455 2024-04-16 06:47:48.000000 zhanshop-0.0.2/zhanshop/webhandle.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.358830 zhanshop-0.0.2/zhanshop.egg-info/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/PKG-INFO
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      422 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)        1 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)        9 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/top_level.txt
```

