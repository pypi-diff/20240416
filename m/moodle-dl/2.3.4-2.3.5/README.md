# Comparing `tmp/moodle_dl-2.3.4.tar.gz` & `tmp/moodle_dl-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle_dl-2.3.4.tar", last modified: Mon Apr 15 13:48:05 2024, max compression
+gzip compressed data, was "moodle_dl-2.3.5.tar", last modified: Tue Apr 16 11:48:25 2024, max compression
```

## Comparing `moodle_dl-2.3.4.tar` & `moodle_dl-2.3.5.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.291313 moodle_dl-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.275313 moodle_dl-2.3.4/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.279312 moodle_dl-2.3.4/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.279312 moodle_dl-2.3.4/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/book.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.283313 moodle_dl-2.3.4/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:05.287313 moodle_dl-2.3.4/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:48:05.000000 moodle_dl-2.3.4/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:48:05.291313 moodle_dl-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-15 13:47:53.000000 moodle_dl-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.793054 moodle_dl-2.3.5/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.797054 moodle_dl-2.3.5/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27074 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27735 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.797054 moodle_dl-2.3.5/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.797054 moodle_dl-2.3.5/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.797054 moodle_dl-2.3.5/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.801054 moodle_dl-2.3.5/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30307 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.801054 moodle_dl-2.3.5/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.801054 moodle_dl-2.3.5/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.801054 moodle_dl-2.3.5/moodle_dl/notifications/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.801054 moodle_dl-2.3.5/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 11:48:25.000000 moodle_dl-2.3.5/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:48:25.805054 moodle_dl-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 11:48:18.000000 moodle_dl-2.3.5/setup.py
```

### Comparing `moodle_dl-2.3.4/LICENSE` & `moodle_dl-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/PKG-INFO` & `moodle_dl-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.4
+Version: 2.3.5
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
@@ -46,15 +46,15 @@
 </div>
 
 ---
 
 
 `moodle-dl` is a console application that can download all the files from your Moodle courses that are necessary for your daily study routine. Furthermore, moodle-dl can notify you about various activities on your Moodle server. Notifications can be sent to Telegram, Discord, XMPP and Mail. The current implementation includes: 
 
-- Download files, assignments including submissions, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
+- Download files, assignments including submissions, books, calendar events, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
 - Notifications about all downloaded files
 - Text from your Moodle courses (like pages, descriptions or forum posts) will be directly attached to the notifications, so you can read them directly in your messaging app.
 - A configuration wizard is also included, allowing all settings to be made very easily.
 - Running moodle-dl again will only download files that have not been downloaded yet. Do not miss any files, if files are deleted online, they are still available offline.
 - It is possible to download Moodle courses you are enrolled in, as well as courses that are publicly visible to you.
 
 Discussions about the development take place mainly on [Github](https://github.com/C0D3D3V/Moodle-DL/issues), but also on [Discord](https://discord.gg/HNg7CsqEnZ).
```

### Comparing `moodle_dl-2.3.4/README.md` & `moodle_dl-2.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 </div>
 
 ---
 
 
 `moodle-dl` is a console application that can download all the files from your Moodle courses that are necessary for your daily study routine. Furthermore, moodle-dl can notify you about various activities on your Moodle server. Notifications can be sent to Telegram, Discord, XMPP and Mail. The current implementation includes: 
 
-- Download files, assignments including submissions, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
+- Download files, assignments including submissions, books, calendar events, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
 - Notifications about all downloaded files
 - Text from your Moodle courses (like pages, descriptions or forum posts) will be directly attached to the notifications, so you can read them directly in your messaging app.
 - A configuration wizard is also included, allowing all settings to be made very easily.
 - Running moodle-dl again will only download files that have not been downloaded yet. Do not miss any files, if files are deleted online, they are still available offline.
 - It is possible to download Moodle courses you are enrolled in, as well as courses that are publicly visible to you.
 
 Discussions about the development take place mainly on [Github](https://github.com/C0D3D3V/Moodle-DL/issues), but also on [Discord](https://discord.gg/HNg7CsqEnZ).
```

### Comparing `moodle_dl-2.3.4/moodle_dl/cli/__init__.py` & `moodle_dl-2.3.5/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/cli/config_wizard.py` & `moodle_dl-2.3.5/moodle_dl/cli/config_wizard.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self._select_should_download_descriptions()
         self._select_should_download_links_in_descriptions()
         self._select_should_download_databases()
         self._select_should_download_forums()
         self._select_should_download_quizzes()
         self._select_should_download_lessons()
         self._select_should_download_workshops()
+        self._select_should_download_books()
+        self._select_should_download_calendars()
         self._select_should_download_linked_files()
         self._select_should_download_also_with_cookie()
 
         Log.success('Configuration successfully updated!')
 
     def interactively_add_all_visible_courses(self):
         """
@@ -488,14 +490,46 @@
 
         download_workshops = Cutie.prompt_yes_or_no(
             Log.blue_str('Do you want to download workshops of your courses?'), default_is_yes=download_workshops
         )
 
         self.config.set_property('download_workshops', download_workshops)
 
+    def _select_should_download_books(self):
+        """
+        Asks the user if books should be downloaded
+        """
+        download_books = self.config.get_download_books()
+
+        self.section_seperator()
+        Log.info('Books are collections of pages. A table of contents is created for each book.')
+        print('')
+
+        download_books = Cutie.prompt_yes_or_no(
+            Log.blue_str('Do you want to download books of your courses?'), default_is_yes=download_books
+        )
+
+        self.config.set_property('download_books', download_books)
+
+    def _select_should_download_calendars(self):
+        """
+        Asks the user if calendars should be downloaded
+        """
+        download_calendars = self.config.get_download_calendars()
+
+        self.section_seperator()
+        Log.info('Calendars can be downloaded as individually generated HTML files for each event.')
+        print('')
+
+        download_calendars = Cutie.prompt_yes_or_no(
+            Log.blue_str('Do you want to download calendars of your courses?'), default_is_yes=download_calendars
+        )
+
+        self.config.set_property('download_calendars', download_calendars)
+
     def _select_should_download_descriptions(self):
         """
         Asks the user if descriptions should be downloaded
         """
         download_descriptions = self.config.get_download_descriptions()
 
         self.section_seperator()
```

### Comparing `moodle_dl-2.3.4/moodle_dl/cli/database_manager.py` & `moodle_dl-2.3.5/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/cli/moodle_wizard.py` & `moodle_dl-2.3.5/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/cli/notifications_wizard.py` & `moodle_dl-2.3.5/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/config.py` & `moodle_dl-2.3.5/moodle_dl/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,22 @@
         # return a stored boolean if lessons should be downloaded
         return self.get_property_or('download_lessons', False)
 
     def get_download_workshops(self) -> bool:
         # return a stored boolean if workshops should be downloaded
         return self.get_property_or('download_workshops', False)
 
+    def get_download_books(self) -> str:
+        # return a stored boolean if books should be downloaded
+        return self.get_property_or('download_books', False)
+
+    def get_download_calendars(self) -> str:
+        # return a stored boolean if calendars should be downloaded
+        return self.get_property_or('download_calendars', False)
+
     def get_userid_and_version(self) -> Tuple[str, int]:
         # return the userid and a version
         try:
             user_id = self.get_property('userid')
             version = int(self.get_property('version'))
             return user_id, version
         except ValueError:
```

### Comparing `moodle_dl-2.3.4/moodle_dl/database.py` & `moodle_dl-2.3.5/moodle_dl/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         ):
             return True
         return False
 
     @staticmethod
     def ignore_deleted(file: File):
         # Returns true if the deleted file should be ignored.
-        if file.module_modname.endswith('forum'):
+        if file.module_modname.endswith(('forum', 'calendar')):
             return True
 
         return False
 
     def get_stored_files(self) -> List[Course]:
         # get all stored files (that are not yet deleted)
         conn = sqlite3.connect(self.db_file)
@@ -523,29 +523,39 @@
         }
         """
 
         conn = sqlite3.connect(self.db_file)
         conn.row_factory = sqlite3.Row
         cursor = conn.cursor()
         mod_forum_dict = {}
+        mod_calendar_dict = {}
 
         cursor.execute(
             """SELECT module_id, max(content_timemodified) as content_timemodified
             FROM files WHERE module_modname = 'forum' AND content_type = 'description'
             GROUP BY module_id;"""
         )
 
         curse_rows = cursor.fetchall()
 
         for course_row in curse_rows:
             mod_forum_dict[course_row['module_id']] = course_row['content_timemodified']
 
+        cursor.execute(
+            """SELECT module_id, max(content_timemodified) as content_timemodified
+            FROM files WHERE module_modname = 'calendar' AND content_type = 'html'
+            GROUP BY module_id;"""
+        )
+
+        course_row = cursor.fetchone()
+        mod_calendar_dict[course_row['module_id']] = course_row['content_timemodified']
+
         conn.close()
 
-        return {'forum': mod_forum_dict}
+        return {'forum': mod_forum_dict, 'calendar': mod_calendar_dict}
 
     def changes_to_notify(self) -> List[Course]:
         changed_courses = []
 
         conn = sqlite3.connect(self.db_file)
         conn.row_factory = sqlite3.Row
         cursor = conn.cursor()
```

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/download_service.py` & `moodle_dl-2.3.5/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/__init__.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/echo360.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/googledrive.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/owncloud.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepoint.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle_dl-2.3.5/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/fake_download_service.py` & `moodle_dl-2.3.5/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/downloader/task.py` & `moodle_dl-2.3.5/moodle_dl/downloader/task.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/main.py` & `moodle_dl-2.3.5/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/cookie_handler.py` & `moodle_dl-2.3.5/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/core_handler.py` & `moodle_dl-2.3.5/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/__init__.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from moodle_dl.config import ConfigHelper
 from moodle_dl.moodle.mods.common import MoodleMod
 from moodle_dl.moodle.request_helper import RequestHelper
 from moodle_dl.types import Course
 
 from moodle_dl.moodle.mods.assign import AssignMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.book import BookMod  # noqa: F401 isort:skip
+from moodle_dl.moodle.mods.calendar import CalendarMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.data import DataMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.folder import FolderMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.forum import ForumMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.lesson import LessonMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.page import PageMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.quiz import QuizMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.workshop import WorkshopMod  # noqa: F401 isort:skip
```

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/assign.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/assign.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/book.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/book.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 class BookMod(MoodleMod):
     MOD_NAME = 'book'
     MOD_PLURAL_NAME = 'books'
     MOD_MIN_VERSION = 2015111600  # 3.0
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
-        # TODO: Add download condition
-        return True
+        return config.get_download_books() or (not (file.module_modname.endswith(cls.MOD_NAME) and file.deleted))
 
     async def real_fetch_mod_entries(
         self, courses: List[Course], core_contents: Dict[int, List[Dict]]
     ) -> Dict[int, Dict[int, Dict]]:
+
+        result = {}
+        if not self.config.get_download_books():
+            return result
+
         books = (
             await self.client.async_post(
                 'mod_book_get_books_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('books', [])
 
-        result = {}
         for book in books:
             course_id = book.get('course', 0)
             module_id = book.get('coursemodule', 0)
             book_name = book.get('name', 'unnamed book')
 
             book_files = book.get('introfiles', [])
             self.set_props_of_files(book_files, type='book_file')
```

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/common.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,9 +219,9 @@
         return {}
 
     @staticmethod
     def add_module(result: Dict, course_id: int, module_id: int, module: Dict):
         if course_id not in result:
             result[course_id] = {}
         if module_id in result[course_id]:
-            logging.debug('Got duplicated module %s in course %s', module_id, course_id)
+            logging.warning('Got duplicated module %s in course %s', module_id, course_id)
         result[course_id][module_id] = module
```

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/data.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/folder.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/forum.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/lesson.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/page.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/quiz.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/mods/workshop.py` & `moodle_dl-2.3.5/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/moodle_constants.py` & `moodle_dl-2.3.5/moodle_dl/moodle/moodle_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,56 @@
+course_events_section_id = -2
+course_events_module_id = -2
+moodle_event_header = '''
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Calendar Event</title>
+    <style>
+      body {
+        font-family: Arial, sans-serif;
+        background-color: #f4f4f4;
+        margin: 0;
+        padding: 20px;
+      }
+      .container {
+        max-width: 600px;
+        background-color: #fff;
+        border-radius: 8px;
+        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
+        padding: 20px;
+        margin: auto;
+      }
+      .event-title {
+        font-size: 24px;
+        font-weight: bold;
+        color: #333;
+      }
+      .icon {
+        margin-right: 5px;
+      }
+      .attribute {
+        margin-bottom: 10px;
+      }
+      .attribute span {
+        font-weight: bold;
+      }
+    </style>
+    </head>
+    <body>
+    
+    <div class="container">
+'''
+moodle_event_footer = '''
+    </div>
+    
+    </body>
+    </html>
+'''
+
 moodle_html_header = '''
 <!DOCTYPE html>
 
 <html dir="ltr" lang="de" xml:lang="de">
 
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
```

#### html2text {}

```diff
@@ -1,3 +1,6 @@
-moodle_html_header = '''
+course_events_section_id = -2 course_events_module_id = -2 moodle_event_header
+= '''
+''' moodle_event_footer = '''
+''' moodle_html_header = '''
 ''' moodle_html_footer = '''
 '''
```

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/moodle_service.py` & `moodle_dl-2.3.5/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/request_helper.py` & `moodle_dl-2.3.5/moodle_dl/moodle/request_helper.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/moodle/result_builder.py` & `moodle_dl-2.3.5/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/__init__.py` & `moodle_dl-2.3.5/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/console/console_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_formatter.py` & `moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_formatter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/discord/discord_shooter.py` & `moodle_dl-2.3.5/moodle_dl/notifications/discord/discord_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/mail/header.png` & `moodle_dl-2.3.5/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/mail/header_extender.png` & `moodle_dl-2.3.5/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_formater.py` & `moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/mail/mail_shooter.py` & `moodle_dl-2.3.5/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/notification_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle_dl-2.3.5/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle_dl-2.3.5/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/types.py` & `moodle_dl-2.3.5/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl/utils.py` & `moodle_dl-2.3.5/moodle_dl/utils.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.4/moodle_dl.egg-info/PKG-INFO` & `moodle_dl-2.3.5/moodle_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.4
+Version: 2.3.5
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
@@ -46,15 +46,15 @@
 </div>
 
 ---
 
 
 `moodle-dl` is a console application that can download all the files from your Moodle courses that are necessary for your daily study routine. Furthermore, moodle-dl can notify you about various activities on your Moodle server. Notifications can be sent to Telegram, Discord, XMPP and Mail. The current implementation includes: 
 
-- Download files, assignments including submissions, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
+- Download files, assignments including submissions, books, calendar events, forums, workshops, lessons, quizzes, descriptions, as well as external links (OpenCast, Youtube, Sciebo, Owncloud, Kaltura, Helixmedia, Google drive,... videos/files).
 - Notifications about all downloaded files
 - Text from your Moodle courses (like pages, descriptions or forum posts) will be directly attached to the notifications, so you can read them directly in your messaging app.
 - A configuration wizard is also included, allowing all settings to be made very easily.
 - Running moodle-dl again will only download files that have not been downloaded yet. Do not miss any files, if files are deleted online, they are still available offline.
 - It is possible to download Moodle courses you are enrolled in, as well as courses that are publicly visible to you.
 
 Discussions about the development take place mainly on [Github](https://github.com/C0D3D3V/Moodle-DL/issues), but also on [Discord](https://discord.gg/HNg7CsqEnZ).
```

### Comparing `moodle_dl-2.3.4/moodle_dl.egg-info/SOURCES.txt` & `moodle_dl-2.3.5/moodle_dl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 moodle_dl/moodle/moodle_constants.py
 moodle_dl/moodle/moodle_service.py
 moodle_dl/moodle/request_helper.py
 moodle_dl/moodle/result_builder.py
 moodle_dl/moodle/mods/__init__.py
 moodle_dl/moodle/mods/assign.py
 moodle_dl/moodle/mods/book.py
+moodle_dl/moodle/mods/calendar.py
 moodle_dl/moodle/mods/common.py
 moodle_dl/moodle/mods/data.py
 moodle_dl/moodle/mods/folder.py
 moodle_dl/moodle/mods/forum.py
 moodle_dl/moodle/mods/lesson.py
 moodle_dl/moodle/mods/page.py
 moodle_dl/moodle/mods/quiz.py
```

### Comparing `moodle_dl-2.3.4/setup.py` & `moodle_dl-2.3.5/setup.py`

 * *Files identical despite different names*

