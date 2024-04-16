# Comparing `tmp/auto_archiver-0.9.8.tar.gz` & `tmp/auto_archiver-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.9.8.tar", last modified: Fri Feb 23 14:10:44 2024, max compression
+gzip compressed data, was "auto_archiver-0.9.9.tar", last modified: Fri Feb 23 15:39:56 2024, max compression
```

## Comparing `auto_archiver-0.9.8.tar` & `auto_archiver-0.9.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.063917 auto_archiver-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.067916 auto_archiver-0.9.8/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.071917 auto_archiver-0.9.8/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/archivers/youtubedl_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.071917 auto_archiver-0.9.8/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.071917 auto_archiver-0.9.8/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/api_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.075917 auto_archiver-0.9.8/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/meta_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/metadata_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/pdq_hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/ssl_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/timestamping_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.075917 auto_archiver-0.9.8/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.075917 auto_archiver-0.9.8/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 14:09:14.000000 auto_archiver-0.9.8/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:10:44.079917 auto_archiver-0.9.8/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-23 14:10:44.000000 auto_archiver-0.9.8/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.972440 auto_archiver-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-02-23 15:39:56.972440 auto_archiver-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-23 15:39:56.972440 auto_archiver-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.952440 auto_archiver-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.956440 auto_archiver-0.9.9/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.960440 auto_archiver-0.9.9/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14640 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/archivers/youtubedl_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.960440 auto_archiver-0.9.9/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.964440 auto_archiver-0.9.9/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/api_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.964440 auto_archiver-0.9.9/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/meta_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/metadata_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/pdq_hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/ssl_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/timestamping_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.964440 auto_archiver-0.9.9/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.968440 auto_archiver-0.9.9/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.968440 auto_archiver-0.9.9/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.968440 auto_archiver-0.9.9/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.968440 auto_archiver-0.9.9/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 15:38:25.000000 auto_archiver-0.9.9/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:39:56.968440 auto_archiver-0.9.9/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-23 15:39:56.000000 auto_archiver-0.9.9/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.9.8/LICENSE` & `auto_archiver-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/PKG-INFO` & `auto_archiver-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.9.8/README.md` & `auto_archiver-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/setup.cfg` & `auto_archiver-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/__init__.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_api_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_api_archiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,18 +98,26 @@
                 stories = self._download_stories_reusable(result, username)
                 result.set("#stories", len(stories))
             except Exception as e:
                 result.append("errors", f"Error downloading stories for {username}")
                 logger.error(f"Error downloading stories for {username}: {e}")
 
             # download all posts
-            self.download_all_posts(result, user_id)
+            try:
+                self.download_all_posts(result, user_id)
+            except Exception as e:
+                result.append("errors", f"Error downloading posts for {username}")
+                logger.error(f"Error downloading posts for {username}: {e}")
 
             # download all tagged
-            self.download_all_tagged(result, user_id)
+            try:
+                self.download_all_tagged(result, user_id)
+            except Exception as e:
+                result.append("errors", f"Error downloading tagged posts for {username}")
+                logger.error(f"Error downloading tagged posts for {username}: {e}")
 
             # download all highlights
             try:
                 count_highlights = 0
                 highlights = self.call_api(f"v1/user/highlights", {"user_id": user_id})
                 for h in highlights:
                     try: 
@@ -239,16 +247,16 @@
         """
         if "clips_metadata" in item:
             if reusable_text := item.get("clips_metadata", {}).get("reusable_text_attribute_string"):
                 item["clips_metadata_text"] = reusable_text
             if self.minimize_json_output: 
                 del item["clips_metadata"]
 
-        if code := item.get("code"): 
-            result.set("url", f"https://www.instagram.com/p/{code}/")
+        if code := item.get("code") and not result.get("url"): 
+            result.set_url(f"https://www.instagram.com/p/{code}/")
             
         resources = item.get("resources", item.get("carousel_media", []))
         item, media, media_id = self.scrape_media(item, context)
         # if resources are present take the main media from the first resource
         if not media and len(resources):
             _, media, media_id = self.scrape_media(resources[0], context)
             resources = resources[1:]
```

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.9.9/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/config.py` & `auto_archiver-0.9.9/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/context.py` & `auto_archiver-0.9.9/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/media.py` & `auto_archiver-0.9.9/src/auto_archiver/core/media.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/metadata.py` & `auto_archiver-0.9.9/src/auto_archiver/core/metadata.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.9.9/src/auto_archiver/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/core/step.py` & `auto_archiver-0.9.9/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/databases/api_db.py` & `auto_archiver-0.9.9/src/auto_archiver/databases/api_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.9.9/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.9.9/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/databases/database.py` & `auto_archiver-0.9.9/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.9.9/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/__init__.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/meta_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/meta_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/metadata_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/metadata_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/pdq_hash_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/pdq_hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/ssl_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/ssl_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/timestamping_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/timestamping_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.9.9/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.9.9/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.9.9/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.9.9/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.9.9/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.9.9/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.9.9/src/auto_archiver/formatters/templates/html_template.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.9.9/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/storages/gd.py` & `auto_archiver-0.9.9/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/storages/local.py` & `auto_archiver-0.9.9/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/storages/s3.py` & `auto_archiver-0.9.9/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/storages/storage.py` & `auto_archiver-0.9.9/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.9.9/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.9.9/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/utils/misc.py` & `auto_archiver-0.9.9/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/utils/url.py` & `auto_archiver-0.9.9/src/auto_archiver/utils/url.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.9.9/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.9.8/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.9.9/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.9.8/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.9.9/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

