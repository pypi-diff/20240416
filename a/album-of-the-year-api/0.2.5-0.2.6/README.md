# Comparing `tmp/album-of-the-year-api-0.2.5.tar.gz` & `tmp/album-of-the-year-api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "album-of-the-year-api-0.2.5.tar", last modified: Thu Mar 24 20:25:04 2022, max compression
+gzip compressed data, was "dist/album-of-the-year-api-0.2.6.tar", last modified: Tue Apr 16 04:30:39 2024, max compression
```

## Comparing `album-of-the-year-api-0.2.5.tar` & `album-of-the-year-api-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-03-24 20:25:04.523112 album-of-the-year-api-0.2.5/
--rw-rw-rw-   0        0        0     4811 2022-03-24 20:25:04.523112 album-of-the-year-api-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3359 2022-03-24 20:24:08.000000 album-of-the-year-api-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2022-03-24 20:25:04.521111 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/
--rw-rw-rw-   0        0        0     4811 2022-03-24 20:25:04.000000 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2022-03-24 20:25:04.000000 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-24 20:25:04.000000 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-03-24 20:25:04.000000 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2022-03-24 20:25:04.000000 album-of-the-year-api-0.2.5/album_of_the_year_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-03-24 20:25:04.526110 album-of-the-year-api-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      828 2022-03-24 20:24:22.000000 album-of-the-year-api-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/album_of_the_year_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/albumoftheyearapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/albumoftheyearapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/albumoftheyearapi/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/albumoftheyearapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/albumoftheyearapi/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 04:30:39.000000 album-of-the-year-api-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-16 04:30:26.000000 album-of-the-year-api-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

