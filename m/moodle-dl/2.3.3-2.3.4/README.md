# Comparing `tmp/moodle_dl-2.3.3.tar.gz` & `tmp/moodle_dl-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle_dl-2.3.3.tar", last modified: Mon Apr 15 13:20:33 2024, max compression
+gzip compressed data, was "moodle_dl-2.3.4.tar", last modified: Mon Apr 15 13:48:05 2024, max compression
```

## Comparing `moodle_dl-2.3.3.tar` & `moodle_dl-2.3.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.670647 moodle_dl-2.3.3/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.670647 moodle_dl-2.3.3/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41220 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/book.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.291313 moodle_dl-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.275313 moodle_dl-2.3.4/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.279312 moodle_dl-2.3.4/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.279312 moodle_dl-2.3.4/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:48:05.291313 moodle_dl-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/setup.py
```

### Comparing `moodle_dl-2.3.3/LICENSE` & `moodle_dl-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/PKG-INFO` & `moodle_dl-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.3
+Version: 2.3.4
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.3/README.md` & `moodle_dl-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/cli/__init__.py` & `moodle_dl-2.3.4/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/cli/config_wizard.py` & `moodle_dl-2.3.4/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/cli/database_manager.py` & `moodle_dl-2.3.4/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/cli/moodle_wizard.py` & `moodle_dl-2.3.4/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/cli/notifications_wizard.py` & `moodle_dl-2.3.4/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/config.py` & `moodle_dl-2.3.4/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/database.py` & `moodle_dl-2.3.4/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/download_service.py` & `moodle_dl-2.3.4/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/__init__.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/echo360.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/googledrive.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/owncloud.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepoint.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/fake_download_service.py` & `moodle_dl-2.3.4/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/downloader/task.py` & `moodle_dl-2.3.4/moodle_dl/downloader/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,17 @@
         # if a flat path is requested
         if not course.create_directory_structure:
             return PT.flat_path_of_file(storage_path, course_name, file.content_filepath)
 
         # TODO: Get mod names automated; all mods should be in a sub-folder
         # If the file is located in a folder or in an assignment,
         # it should be saved in a sub-folder (with the name of the module).
-        if file.module_modname.endswith(('assign', 'book', 'data', 'folder', 'forum', 'lesson', 'page', 'quiz', 'workshop')):
+        if file.module_modname.endswith(
+            ('assign', 'book', 'data', 'folder', 'forum', 'lesson', 'page', 'quiz', 'workshop')
+        ):
             return PT.path_of_file_in_module(
                 storage_path, course_name, file.section_name, file.module_name, file.content_filepath
             )
         return PT.path_of_file(storage_path, course_name, file.section_name, file.content_filepath)
 
     def add_token_to_url(self, url: str) -> str:
         """
```

### Comparing `moodle_dl-2.3.3/moodle_dl/main.py` & `moodle_dl-2.3.4/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/cookie_handler.py` & `moodle_dl-2.3.4/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/core_handler.py` & `moodle_dl-2.3.4/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/__init__.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/assign.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/assign.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/book.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/book.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,28 +51,48 @@
             if len(book_contents) > 1:
                 book_files += book_contents[1:]
 
             if len(book_contents) > 0:
                 # Generate Table of Contents
                 book_toc = json.loads(book_contents[0].get('content', ''))
 
-                toc_html = '<ul>'
-                for entry in book_toc:
-                    chapter_title = html.escape(entry.get("title", "untitled"))
-                    chapter_href = urllib.parse.quote(entry.get("href", "#failed"))
-                    toc_html += f'<li><a title="{chapter_title}" href="{chapter_href}">{chapter_title}</a></li>'
-                toc_html += '</ul>'
+                toc_html = '''
+<!DOCTYPE html>
+<html>
+    <head>
+        <style>
+            ol {
+                counter-reset: item
+            }
+            li {
+                display: block
+            }
+            li:before {
+                content: counters(item, ".")" ";
+                counter-increment: item
+            }
+        </style>
+    </head>
+    <body>
+        '''
+                toc_html += self.create_ordered_index(book_toc)
+                toc_html += '''
+    </body>
+</html>
+                '''
+
                 book_files.append(
                     {
                         'filename': 'Table of Contents',
                         'filepath': '/',
                         'timemodified': book.get('timemodified', 0),
                         'html': toc_html,
                         'type': 'html',
                         'no_search_for_urls': True,
+                        'filesize': len(toc_html),
                     }
                 )
 
             self.add_module(
                 result,
                 course_id,
                 module_id,
@@ -80,7 +100,21 @@
                     'id': book.get('id', 0),
                     'name': book_name,
                     'files': book_files,
                 },
             )
 
         return result
+
+    @staticmethod
+    def create_ordered_index(items: List[Dict]) -> str:
+        result = '<ol>\n'
+        for entry in items:
+            chapter_title = html.escape(entry.get("title", "untitled"))
+            chapter_href = urllib.parse.quote(entry.get("href", "#failed"))
+            result += f'<li><a title="{chapter_title}" href="{chapter_href}">{chapter_title}</a></li>\n'
+            subitems = entry.get('subitems', [])
+            if len(subitems) > 0:
+                result += BookMod.create_ordered_index(subitems)
+
+        result += '</ol>'
+        return result
```

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/common.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/common.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/data.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/folder.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/forum.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/lesson.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/page.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/quiz.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/mods/workshop.py` & `moodle_dl-2.3.4/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/moodle_constants.py` & `moodle_dl-2.3.4/moodle_dl/moodle/moodle_constants.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/moodle_service.py` & `moodle_dl-2.3.4/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/request_helper.py` & `moodle_dl-2.3.4/moodle_dl/moodle/request_helper.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/moodle/result_builder.py` & `moodle_dl-2.3.4/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/__init__.py` & `moodle_dl-2.3.4/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/console/console_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_formatter.py` & `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_formatter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_shooter.py` & `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/mail/header.png` & `moodle_dl-2.3.4/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/mail/header_extender.png` & `moodle_dl-2.3.4/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_formater.py` & `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_shooter.py` & `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/notification_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/types.py` & `moodle_dl-2.3.4/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl/utils.py` & `moodle_dl-2.3.4/moodle_dl/utils.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/moodle_dl.egg-info/PKG-INFO` & `moodle_dl-2.3.4/moodle_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.3
+Version: 2.3.4
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.3/moodle_dl.egg-info/SOURCES.txt` & `moodle_dl-2.3.4/moodle_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.3/setup.py` & `moodle_dl-2.3.4/setup.py`

 * *Files identical despite different names*

