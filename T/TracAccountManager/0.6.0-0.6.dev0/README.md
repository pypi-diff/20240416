# Comparing `tmp/tracaccountmanager-0.6.0.tar.gz` & `tmp/TracAccountManager-0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracaccountmanager-0.6.0.tar", last modified: Tue Apr 16 09:35:21 2024, max compression
+gzip compressed data, was "dist/TracAccountManager-0.6.dev0.tar", last modified: Wed Apr 29 02:33:04 2020, max compression
```

## Comparing `tracaccountmanager-0.6.0.tar` & `TracAccountManager-0.6.dev0.tar`

### file list

```diff
@@ -1,217 +1,192 @@
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/.github/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/.github/workflows/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      788 2023-11-07 03:24:11.000000 tracaccountmanager-0.6.0/.github/workflows/build.yml
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)       51 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/.gitignore
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3418 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/COPYING
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      357 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/MANIFEST.in
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      895 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/PKG-INFO
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1465 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/README
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      696 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/README.hashes
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     7376 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/README.update
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/TracAccountManager.egg-info/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      895 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/PKG-INFO
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5437 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/SOURCES.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        1 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/dependency_links.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      741 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/entry_points.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      136 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/requires.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        9 2024-04-16 09:35:21.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/top_level.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        1 2023-03-21 06:05:26.000000 tracaccountmanager-0.6.0/TracAccountManager.egg-info/zip-safe
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.105565 tracaccountmanager-0.6.0/acct_mgr/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)       56 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    75072 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/admin.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    20452 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/api.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1249 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/compat.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4391 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/db.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    10545 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/guard.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.105565 tracaccountmanager-0.6.0/acct_mgr/htdocs/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4449 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/acctmgr.css
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3955 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/approval.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      773 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/arrow.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      997 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/delete.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3372 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/guard.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      629 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/info.png
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.105565 tracaccountmanager-0.6.0/acct_mgr/htdocs/js/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5503 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/js/acctmgr_admin.js
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      582 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/locked.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     6632 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/refresh.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      617 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/status_disabled.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      664 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/status_error.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      647 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/status_ok.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      616 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/status_unknown.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      748 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/time-locked.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5599 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htdocs/users.png
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     9583 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htfile.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1328 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/htfile.pyi
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3145 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/http.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      164 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/locale/.placeholder
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/cs/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/cs/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8793 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/cs/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    76381 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/cs/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/de/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/de/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    21462 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    95916 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/es/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/es/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5833 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/es/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    73879 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/es/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/et/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/et/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1562 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/et/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    67964 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/et/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/fi/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/fi/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1561 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/fi/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    67962 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/fi/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/fr/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5468 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/fr/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    71637 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/fr/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/he/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/he/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     9964 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/he/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    80427 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/he/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/id_ID/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/id_ID/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1368 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/id_ID/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    67969 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/id_ID/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/it/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/it/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     9766 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/it/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    78050 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/it/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/ja/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/ja/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    57918 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/ja/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    97529 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/ja/LC_MESSAGES/acct_mgr.po
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    68005 2023-06-05 12:24:30.000000 tracaccountmanager-0.6.0/acct_mgr/locale/messages.pot
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/nl/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/nl/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     6181 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/nl/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    73475 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/nl/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/pl/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.109565 tracaccountmanager-0.6.0/acct_mgr/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2398 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/pl/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    68986 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/pl/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/pt_BR/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8774 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/pt_BR/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    75407 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/pt_BR/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/ru/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    12181 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/ru/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    83399 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/ru/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/sv/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/sv/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     9360 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/sv/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    77497 2023-04-09 22:04:42.000000 tracaccountmanager-0.6.0/acct_mgr/locale/sv/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.097565 tracaccountmanager-0.6.0/acct_mgr/locale/te/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/te/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3659 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/te/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    70424 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/locale/te/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/acct_mgr/locale/tr/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/tr/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8736 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/tr/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    75514 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/locale/tr/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/acct_mgr/locale/uk/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/uk/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1625 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/uk/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    68194 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/locale/uk/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/acct_mgr/locale/zh_CN/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3489 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/zh_CN/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    69608 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/locale/zh_CN/LC_MESSAGES/acct_mgr.po
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/acct_mgr/locale/zh_TW/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1319 2023-04-06 23:41:17.000000 tracaccountmanager-0.6.0/acct_mgr/locale/zh_TW/LC_MESSAGES/acct_mgr.mo
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    67911 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/locale/zh_TW/LC_MESSAGES/acct_mgr.po
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     6119 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/macros.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    21392 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/model.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8256 2023-04-14 21:45:21.000000 tracaccountmanager-0.6.0/acct_mgr/notification.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        0 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/__init__.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/announcer/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        0 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/announcer/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1969 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/announcer/uid_chg.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4633 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/radius.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/tests/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1721 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tests/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1977 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tests/radius.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/tracforms/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        0 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracforms/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1882 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracforms/uid_chg.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/tracscreenshots/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        0 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracscreenshots/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      463 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracscreenshots/uid_chg.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.113565 tracaccountmanager-0.6.0/acct_mgr/opt/tracvote/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)        0 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracvote/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      468 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/opt/tracvote/uid_chg.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     6507 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/pwhash.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1257 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/pwhash.pyi
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    28719 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/register.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2825 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/svnserve.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.101565 tracaccountmanager-0.6.0/acct_mgr/templates/
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.117565 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    11568 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_admin.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    48899 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_config.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3589 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_db_cleanup.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2606 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_login.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2327 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_notification.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2176 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_prefs.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2520 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_register.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1421 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_reset_password.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      214 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_reset_password_email.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      105 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_user_changes_email.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2379 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_user_table.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8687 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_users.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1780 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_verify_email.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      219 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_verify_email.txt
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.117565 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    13435 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_admin.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    50908 2023-11-13 13:36:53.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_config.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2217 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_db_cleanup.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2857 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_login.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2447 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_notification.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1938 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_prefs.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2699 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_register.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1451 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_reset_password.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      214 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_reset_password_email.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      105 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_user_changes_email.txt
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2548 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_user_table.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8331 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_users.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1765 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_verify_email.html
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      219 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/templates/jinja2/account_verify_email.txt
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/acct_mgr/tests/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1763 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     7965 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/admin.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     7691 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/api.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3830 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/db.py
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/acct_mgr/tests/functional/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2997 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/functional/__init__.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5865 2024-04-16 03:10:37.000000 tracaccountmanager-0.6.0/acct_mgr/tests/functional/smtpd.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    15879 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/functional/testcases.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     7015 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/functional/testenv.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     2349 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/functional/tester.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     8440 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/guard.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    10357 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/htfile.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      905 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/http.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     7890 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/model.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4661 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/pwhash.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    16889 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/register.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4543 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/tests/svnserve.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     3493 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/tests/util.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     4760 2023-04-09 22:04:43.000000 tracaccountmanager-0.6.0/acct_mgr/util.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    36686 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/acct_mgr/web_ui.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    17533 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/changelog
-drwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)        0 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/contrib/
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     5989 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/contrib/approval.xcf.bz2
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1554 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/contrib/fix-session_attribute-failed_logins.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)    15186 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/contrib/refresh.xcf.bz2
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)     1490 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/contrib/sessionstore_convert.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      680 2023-04-06 14:21:19.000000 tracaccountmanager-0.6.0/contrib/style.css
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      756 2023-06-05 12:24:30.000000 tracaccountmanager-0.6.0/messages.cfg
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      659 2024-04-16 09:35:21.121565 tracaccountmanager-0.6.0/setup.cfg
--rwxr-xr-x   0 jun66j5   (1000) jun66j5   (1000)     2601 2024-04-16 09:30:20.000000 tracaccountmanager-0.6.0/setup.py
--rw-r--r--   0 jun66j5   (1000) jun66j5   (1000)      468 2024-04-16 03:07:09.000000 tracaccountmanager-0.6.0/tox.ini
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/
+-rw-r--r--   0 rjollos    (501) staff       (20)      522 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/PKG-INFO
+-rw-r--r--   0 rjollos    (501) staff       (20)    17533 2018-06-22 05:44:07.000000 TracAccountManager-0.6.dev0/changelog
+-rw-r--r--   0 rjollos    (501) staff       (20)      353 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/MANIFEST.in
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/contrib/
+-rw-r--r--   0 rjollos    (501) staff       (20)     5989 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/contrib/approval.xcf.bz2
+-rw-r--r--   0 rjollos    (501) staff       (20)     1554 2017-03-23 18:53:24.000000 TracAccountManager-0.6.dev0/contrib/fix-session_attribute-failed_logins.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    15186 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/contrib/refresh.xcf.bz2
+-rw-r--r--   0 rjollos    (501) staff       (20)     1490 2017-03-23 19:12:52.000000 TracAccountManager-0.6.dev0/contrib/sessionstore_convert.py
+-rw-r--r--   0 rjollos    (501) staff       (20)      680 2017-03-23 18:50:53.000000 TracAccountManager-0.6.dev0/contrib/style.css
+-rw-r--r--   0 rjollos    (501) staff       (20)     1465 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/README
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/
+-rw-r--r--   0 rjollos    (501) staff       (20)     4398 2017-03-23 18:46:21.000000 TracAccountManager-0.6.dev0/acct_mgr/db.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/
+-rw-r--r--   0 rjollos    (501) staff       (20)    53716 2018-06-22 05:46:15.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/messages.pot
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pl/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    25045 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pl/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21957 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pl/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/sv/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    31037 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/sv/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21806 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/sv/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/he/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/he/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    33605 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/he/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    23984 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/he/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/id_ID/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/id_ID/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    24403 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/id_ID/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21582 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/id_ID/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pt_BR/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    29751 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pt_BR/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22466 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/pt_BR/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ja/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    35371 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ja/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    23851 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ja/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/it/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    31594 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/it/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22276 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/it/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_TW/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    24345 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_TW/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21533 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_TW/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/cs/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    30603 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/cs/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22032 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/cs/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/te/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/te/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    26277 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/te/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22870 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/te/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ru/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    36044 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ru/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    26866 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/ru/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_CN/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    25507 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_CN/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21359 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/zh_CN/LC_MESSAGES/acct_mgr.mo
+-rw-r--r--   0 rjollos    (501) staff       (20)      164 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/.placeholder
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/uk/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    24562 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/uk/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21966 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/uk/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/nl/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    28421 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/nl/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22253 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/nl/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/de/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    37210 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    24678 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fi/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    24386 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fi/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21689 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fi/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fr/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    26829 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fr/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21995 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/fr/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/es/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    28655 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/es/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22306 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/es/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/et/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/et/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    24388 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/et/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    21690 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/et/LC_MESSAGES/acct_mgr.mo
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/tr/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)    30070 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/tr/LC_MESSAGES/acct_mgr.po
+-rw-r--r--   0 rjollos    (501) staff       (20)    22201 2018-06-22 06:02:20.000000 TracAccountManager-0.6.dev0/acct_mgr/locale/tr/LC_MESSAGES/acct_mgr.mo
+-rw-r--r--   0 rjollos    (501) staff       (20)      548 2018-03-04 16:49:31.000000 TracAccountManager-0.6.dev0/acct_mgr/compat.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    29285 2018-06-22 05:40:40.000000 TracAccountManager-0.6.dev0/acct_mgr/register.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    10015 2017-03-23 20:38:44.000000 TracAccountManager-0.6.dev0/acct_mgr/htfile.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     4980 2017-06-16 17:17:55.000000 TracAccountManager-0.6.dev0/acct_mgr/util.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     8530 2019-09-19 01:54:03.000000 TracAccountManager-0.6.dev0/acct_mgr/notification.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/
+-rw-r--r--   0 rjollos    (501) staff       (20)     3837 2017-03-23 20:04:40.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/db.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    17022 2020-01-31 18:59:49.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/register.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     8966 2017-03-23 20:04:27.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/htfile.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     2625 2017-06-16 17:21:26.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/util.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     1474 2019-02-13 15:16:10.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/__init__.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     8271 2020-01-31 18:48:14.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/model.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     7700 2020-01-31 18:47:55.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/api.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     8022 2018-06-22 05:31:43.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/admin.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     4550 2020-01-31 19:01:55.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/svnserve.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     8446 2020-01-31 18:48:05.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/guard.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/
+-rw-r--r--   0 rjollos    (501) staff       (20)     1694 2017-04-03 22:30:09.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/tester.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     4747 2017-03-23 19:09:01.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/testenv.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     2327 2017-04-03 22:30:09.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/__init__.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    12563 2017-04-03 22:30:09.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/testcases.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     3224 2016-11-27 19:23:00.000000 TracAccountManager-0.6.dev0/acct_mgr/tests/functional/smtpd.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     5207 2017-10-04 03:22:58.000000 TracAccountManager-0.6.dev0/acct_mgr/pwhash.py
+-rw-r--r--   0 rjollos    (501) staff       (20)       58 2019-09-12 00:42:04.000000 TracAccountManager-0.6.dev0/acct_mgr/__init__.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    21342 2018-06-27 03:40:49.000000 TracAccountManager-0.6.dev0/acct_mgr/model.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    20365 2018-06-22 05:39:17.000000 TracAccountManager-0.6.dev0/acct_mgr/api.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    75929 2019-09-11 05:08:40.000000 TracAccountManager-0.6.dev0/acct_mgr/admin.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     6210 2018-06-22 05:42:01.000000 TracAccountManager-0.6.dev0/acct_mgr/macros.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     2784 2017-03-23 19:09:56.000000 TracAccountManager-0.6.dev0/acct_mgr/http.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/
+-rw-r--r--   0 rjollos    (501) staff       (20)      629 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/info.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      748 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/time-locked.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      616 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_unknown.png
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/js/
+-rw-r--r--   0 rjollos    (501) staff       (20)     5503 2017-03-23 18:59:15.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/js/acctmgr_admin.js
+-rw-r--r--   0 rjollos    (501) staff       (20)     4449 2017-10-16 07:01:43.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/acctmgr.css
+-rw-r--r--   0 rjollos    (501) staff       (20)      773 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/arrow.png
+-rw-r--r--   0 rjollos    (501) staff       (20)     3955 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/approval.png
+-rw-r--r--   0 rjollos    (501) staff       (20)     3372 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/guard.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      647 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_ok.png
+-rw-r--r--   0 rjollos    (501) staff       (20)     5599 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/users.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      582 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/locked.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      617 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_disabled.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      997 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/delete.png
+-rw-r--r--   0 rjollos    (501) staff       (20)      664 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_error.png
+-rw-r--r--   0 rjollos    (501) staff       (20)     6632 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/htdocs/refresh.png
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/announcer/
+-rw-r--r--   0 rjollos    (501) staff       (20)     1981 2017-03-23 19:04:49.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/announcer/uid_chg.py
+-rw-r--r--   0 rjollos    (501) staff       (20)        0 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/announcer/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracforms/
+-rw-r--r--   0 rjollos    (501) staff       (20)     1894 2017-03-23 19:02:33.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracforms/uid_chg.py
+-rw-r--r--   0 rjollos    (501) staff       (20)        0 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracforms/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracvote/
+-rw-r--r--   0 rjollos    (501) staff       (20)      474 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracvote/uid_chg.py
+-rw-r--r--   0 rjollos    (501) staff       (20)        0 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracvote/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tests/
+-rw-r--r--   0 rjollos    (501) staff       (20)     1711 2016-07-09 05:17:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tests/__init__.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     1987 2017-03-23 19:03:29.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tests/radius.py
+-rw-r--r--   0 rjollos    (501) staff       (20)        0 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:03.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracscreenshots/
+-rw-r--r--   0 rjollos    (501) staff       (20)      469 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracscreenshots/uid_chg.py
+-rw-r--r--   0 rjollos    (501) staff       (20)        0 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/tracscreenshots/__init__.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     4637 2017-03-23 20:34:43.000000 TracAccountManager-0.6.dev0/acct_mgr/opt/radius.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     2835 2019-02-13 15:11:54.000000 TracAccountManager-0.6.dev0/acct_mgr/svnserve.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/
+-rw-r--r--   0 rjollos    (501) staff       (20)    46500 2017-10-04 04:16:50.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_config.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     2164 2019-09-12 00:18:00.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_notification.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     2960 2016-11-29 01:22:24.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_login.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     3662 2017-10-04 04:16:50.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_db_cleanup.html
+-rw-r--r--   0 rjollos    (501) staff       (20)    11801 2018-03-09 00:12:15.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_admin.html
+-rw-r--r--   0 rjollos    (501) staff       (20)      105 2019-09-11 23:41:02.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_user_changes_email.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)     2593 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_register.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     1679 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_verify_email.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     2389 2017-10-04 03:56:36.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_user_table.html
+-rw-r--r--   0 rjollos    (501) staff       (20)     2251 2018-06-22 05:44:46.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_prefs.html
+-rw-r--r--   0 rjollos    (501) staff       (20)      219 2019-09-11 23:52:23.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_verify_email.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)     8845 2018-06-22 05:42:52.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_users.html
+-rw-r--r--   0 rjollos    (501) staff       (20)      214 2019-09-11 04:12:26.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_reset_password_email.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)     1494 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/acct_mgr/templates/account_reset_password.html
+-rw-r--r--   0 rjollos    (501) staff       (20)    10513 2017-04-03 22:30:09.000000 TracAccountManager-0.6.dev0/acct_mgr/guard.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    36948 2018-06-27 04:22:49.000000 TracAccountManager-0.6.dev0/acct_mgr/web_ui.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     2830 2017-03-23 18:22:40.000000 TracAccountManager-0.6.dev0/acct_mgr/md5crypt.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     3418 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/COPYING
+-rwxr-xr-x   0 rjollos    (501) staff       (20)     2785 2020-04-29 02:32:52.000000 TracAccountManager-0.6.dev0/setup.py
+-rw-r--r--   0 rjollos    (501) staff       (20)     7376 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/README.update
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/
+-rw-r--r--   0 rjollos    (501) staff       (20)      522 2020-04-29 02:33:01.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/PKG-INFO
+-rw-r--r--   0 rjollos    (501) staff       (20)        1 2018-02-13 14:10:17.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/zip-safe
+-rw-r--r--   0 rjollos    (501) staff       (20)     4513 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/SOURCES.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)      747 2020-04-29 02:33:02.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/entry_points.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)      136 2020-04-29 02:33:01.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/requires.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)        9 2020-04-29 02:33:01.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/top_level.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)        1 2020-04-29 02:33:01.000000 TracAccountManager-0.6.dev0/TracAccountManager.egg-info/dependency_links.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)      696 2016-06-27 12:44:47.000000 TracAccountManager-0.6.dev0/README.hashes
+-rw-r--r--   0 rjollos    (501) staff       (20)      605 2020-04-29 02:33:04.000000 TracAccountManager-0.6.dev0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tracaccountmanager-0.6.0/COPYING` & `TracAccountManager-0.6.dev0/COPYING`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/README` & `TracAccountManager-0.6.dev0/README`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/README.hashes` & `TracAccountManager-0.6.dev0/README.hashes`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/README.update` & `TracAccountManager-0.6.dev0/README.update`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/TracAccountManager.egg-info/entry_points.txt` & `TracAccountManager-0.6.dev0/TracAccountManager.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 acct_mgr.admin = acct_mgr.admin
 acct_mgr.api = acct_mgr.api
 acct_mgr.db = acct_mgr.db
 acct_mgr.htfile = acct_mgr.htfile
 acct_mgr.http = acct_mgr.http
 acct_mgr.macros = acct_mgr.macros
 acct_mgr.notification = acct_mgr.notification
-acct_mgr.opt.announcer.uid_chg = acct_mgr.opt.announcer.uid_chg[announcer]
-acct_mgr.opt.radius = acct_mgr.opt.radius[pyrad]
-acct_mgr.opt.tracforms.uid_chg = acct_mgr.opt.tracforms.uid_chg[forms]
-acct_mgr.opt.tracscreenshots.uid_chg = acct_mgr.opt.tracscreenshots.uid_chg[screenshots]
-acct_mgr.opt.tracvote.uid_chg = acct_mgr.opt.tracvote.uid_chg[vote]
+acct_mgr.opt.announcer.uid_chg = acct_mgr.opt.announcer.uid_chg [announcer]
+acct_mgr.opt.radius = acct_mgr.opt.radius [pyrad]
+acct_mgr.opt.tracforms.uid_chg = acct_mgr.opt.tracforms.uid_chg [forms]
+acct_mgr.opt.tracscreenshots.uid_chg = acct_mgr.opt.tracscreenshots.uid_chg [screenshots]
+acct_mgr.opt.tracvote.uid_chg = acct_mgr.opt.tracvote.uid_chg [vote]
 acct_mgr.pwhash = acct_mgr.pwhash
 acct_mgr.register = acct_mgr.register
 acct_mgr.svnserve = acct_mgr.svnserve
 acct_mgr.web_ui = acct_mgr.web_ui
+
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/admin.py` & `TracAccountManager-0.6.dev0/acct_mgr/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,44 +5,45 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-from datetime import datetime
 import inspect
 import re
 
+from acct_mgr.api import AccountManager, CommonTemplateProvider
+from acct_mgr.api import IUserIdChanger
+from acct_mgr.api import _, dgettext, gettext, ngettext, tag_
+from acct_mgr.compat import genshi_template_args
+from acct_mgr.guard import AccountGuard
+from acct_mgr.model import (
+    change_uid, del_user_attribute, email_verification_token, email_verified)
+from acct_mgr.model import get_user_attribute, last_seen, set_user_attribute
+from acct_mgr.notification import NotificationError
+from acct_mgr.register import EmailVerificationModule, RegistrationError
+from acct_mgr.util import pretty_precise_timedelta
+from acct_mgr.web_ui import AccountModule
 from trac.admin import IAdminPanelProvider
 from trac.config import BoolOption, Option
 from trac.core import Component, ExtensionPoint, implements
 from trac.perm import PermissionCache, PermissionSystem
 from trac.util import as_int
+from trac.util.compat import cleandoc
 from trac.util.datefmt import format_datetime, to_datetime
 from trac.util.html import html as tag
 from trac.util.presentation import Paginator
-from trac.util.translation import dgettext, tagn_
-from trac.util.text import cleandoc, exception_to_unicode
+from trac.util.translation import tagn_
+from trac.util.text import exception_to_unicode
 from trac.web.api import IAuthenticator
 from trac.web.chrome import Chrome, add_ctxtnav, add_link, add_notice
 from trac.web.chrome import add_script, add_stylesheet, add_warning
 from trac.wiki.formatter import format_to_html
 
-from .api import AccountManager, IUserIdChanger, _, gettext, ngettext, tag_
-from .compat import iteritems, itervalues
-from .guard import AccountGuard
-from .model import (change_uid, del_user_attribute, email_verification_token,
-                    email_verified, get_user_attribute, last_seen,
-                    set_user_attribute)
-from .notification import NotificationError
-from .register import EmailVerificationModule, RegistrationError
-from .util import i18n_tag, format_timespan
-from .web_ui import AccountModule
-
 
 def fetch_user_data(env, req, filters=None):
     acctmgr = AccountManager(env)
     guard = AccountGuard(env)
     accounts = {}
     for username in acctmgr.get_users():
         if 'ACCTMGR_USER_ADMIN' in req.perm:
@@ -57,16 +58,16 @@
                 t_release = guard.pretty_release_time(req, username)
                 accounts[username]['release_hint'] = _(
                     "Locked until %(t_release)s",
                     t_release=t_release)
     verify_email = env.is_enabled(EmailVerificationModule) and \
                    EmailVerificationModule(env).email_enabled and \
                    EmailVerificationModule(env).verify_email
-    for acct, status in iteritems(get_user_attribute(env, username=None,
-                                                     authenticated=None)):
+    for acct, status in get_user_attribute(env, username=None,
+                                           authenticated=None).iteritems():
         account = accounts.get(acct)
         if account is not None and 1 in status:
             # Only use attributes related to authenticated
             # accounts.
             account['name'] = status[1].get('name')
             account['email'] = status[1].get('email')
             # Obfuscate email address if required.
@@ -96,15 +97,15 @@
                 inactive_accounts[username] = accounts[username]
         accounts = inactive_accounts
     ts_seen = last_seen(env)
     for username, last_visit in ts_seen:
         account = accounts.get(username)
         if account and last_visit:
             account['last_visit'] = to_datetime(last_visit)
-    return sorted(itervalues(accounts), key=lambda acct: acct['username'])
+    return sorted(accounts.itervalues(), key=lambda acct: acct['username'])
 
 
 def _getoptions(cls):
     opt_cls = isinstance(cls, Component) and cls.__class__ or cls
     options = [(name, value) for name, value in inspect.getmembers(opt_cls)
                if isinstance(value, Option)]
     index = 0
@@ -157,49 +158,49 @@
 
     def __setitem__(self, key, value):
         if isinstance(key, Component):
             order = self.d[key]
             self.d[key] = value
             self.d[order].remove(key)
             self[value] = key
-        elif isinstance(key, str):
+        elif isinstance(key, basestring):
             self.d[self.sxref[key]] = value
         elif isinstance(key, int):
             self.d.setdefault(key, [])
             self.d[key].append(value)
         else:
-            raise KeyError("Invalid key type (%s) for ExtensionOrder" %
-                           type(key))
+            raise KeyError(_("Invalid key type (%s) for ExtensionOrder")
+                           % str(type(key)))
         pass
 
     def get_enabled_components(self):
         """Return an ordered list of components.
 
         All components that are order 0 are dropped from the list.
         """
-        keys = sorted(k for k in self.d if isinstance(k, int))
+        keys = sorted([k for k in self.d.keys() if isinstance(k, int)])
         component_list = []
         for k in keys[1:]:
             component_list.extend(self.d[k])
             continue
         return component_list
 
     def get_enabled_component_names(self):
         """Returns the class names of the enabled components."""
         components = self.get_enabled_components()
         return [c.__class__.__name__ for c in components]
 
     def get_all_components(self):
-        return [k for k in self.d if isinstance(k, Component)]
+        return [k for k in self.d.keys() if isinstance(k, Component)]
 
     def component_count(self):
         return len(self.get_all_components())
 
 
-class UserAdminPanel(Component):
+class UserAdminPanel(CommonTemplateProvider):
     implements(IAdminPanelProvider)
 
     uid_changers = ExtensionPoint(IUserIdChanger)
 
     ACCTS_PER_PAGE = 20
 
     def __init__(self):
@@ -221,119 +222,125 @@
         """Add new user account on verified request."""
         return _add_user_account(self.env, req)
 
     def _do_db_cleanup(self, req):
         if 'ACCTMGR_ADMIN' in req.perm:
             env = self.env
             changed = False
-            # Get data for all authenticated users from 'session_attribute'.
+            # Get data for all authenticated users from 'session_attributes'.
             attr = get_user_attribute(self.env, username=None,
                                       authenticated=1)
             attrs = {}
             accounts = req.args.get('accounts')
             accounts = accounts and accounts.split(',') or []
             sel = req.args.getlist('sel')
             if req.args.get('purge') and sel:
                 sel_len = len(sel)
                 matched = []
-                for acct, states in iteritems(attr):
-                    for state in states['id']:
-                        for elem, id in iteritems(states[state]['id']):
+                for acct, states in attr.iteritems():
+                    for state in states['id'].keys():
+                        for elem, id in states[state]['id'].iteritems():
                             if id in sel:
-                                if acct in attrs:
-                                    if state in attrs[acct]:
-                                        attrs[acct][state].append(elem)
+                                if acct in attrs.keys():
+                                    if state in attrs[acct].keys():
+                                        attrs[acct][state] \
+                                            .append(elem)
                                     else:
                                         attrs[acct][state] = [elem]
                                 else:
                                     attrs[acct] = {state: [elem]}
                                 matched.append(id)
                                 if len(matched) == sel_len:
                                     break
                         if len(matched) == sel_len:
                             break
                     if len(matched) == sel_len:
                         break
                 for id in (frozenset(sel) - frozenset(matched)):
-                    for acct, states in iteritems(attr):
-                        for state, id_ in iteritems(states['id']):
+                    for acct, states in attr.iteritems():
+                        for state, id_ in states['id'].iteritems():
                             if id == id_:
                                 # Full account is marked, forget attributes.
-                                if acct in attrs:
-                                    attrs[acct][state] = []
+                                if acct in attrs.keys():
+                                    attrs[acct].update({state: []})
                                 else:
                                     attrs[acct] = {state: []}
                                 matched.append(id)
                                 if len(matched) == sel_len:
                                     break
                         if len(matched) == sel_len:
                             break
                 # DEVEL: For Python>2.4 better use defaultdict for counters.
                 del_count = {'acct': 0, 'attr': 0}
-                for account, states in iteritems(attrs):
-                    for state, elem in iteritems(states):
+                for account, states in attrs.iteritems():
+                    for state, elem in states.iteritems():
                         if len(elem) == 0:
                             del_user_attribute(env, account, state)
                             del_count['acct'] += 1
                         else:
                             for attribute in elem:
                                 del_user_attribute(env, account, state,
                                                    attribute)
                                 del_count['attr'] += 1
                     changed = True
 
             if changed:
                 accounts_ = attributes = ''
                 n_plural = del_count['acct']
                 if n_plural > 0:
-                    accounts_ = tag.li(ngettext("%(count)s account",
-                                                "%(count)s accounts",
-                                                n_plural, count=n_plural))
+                    accounts_ = tag.li(tag.span(tag(ngettext(
+                        "%(count)s account",
+                        "%(count)s accounts",
+                        n_plural, count=n_plural
+                    ))))
                 n_plural = del_count['attr']
                 if n_plural > 0:
-                    attributes = tag.li(ngettext(
+                    attributes = tag.li(tag.span(tag(ngettext(
                         "%(count)s account attribute",
                         "%(count)s account attributes",
-                        n_plural, count=n_plural))
+                        n_plural, count=n_plural
+                    ))))
                 add_notice(req, tag_("Successfully deleted: %(account)s",
                                      account=tag.ul(accounts_, attributes)))
                 # Update the dict after changes.
                 attr = get_user_attribute(env, username=None,
                                           authenticated=1)
             if not accounts and sel:
                 # Get initial account selection from account/user list.
                 accounts = sel
-            attr_sel = dict((account, states)
-                            for account, states in iteritems(attr)
-                            if account in accounts)
+            attr_sel = dict()
+            for account, states in attr.iteritems():
+                if account in accounts:
+                    attr_sel.update({account: states})
 
             if len(accounts) == 1:
                 back_label = _("Back to Account")
                 back_href = req.href.admin('accounts', 'users', accounts[0])
             else:
                 back_label = _("Back to Accounts")
                 back_href = req.href.admin('accounts', 'users')
             add_ctxtnav(req, back_label, href=back_href)
             add_stylesheet(req, 'acct_mgr/acctmgr.css')
-            data = dict(i18n_tag=i18n_tag, accounts=accounts, attr=attr_sel)
-            return 'account_db_cleanup.html', data
+            data = dict(_dgettext=dgettext, accounts=accounts, attr=attr_sel)
+            return genshi_template_args(self.env, 'account_db_cleanup.html',
+                                        data)
 
     def _do_acct_details(self, req, username):
         env = self.env
         acctmgr = self.acctmgr
         guard = self.guard
 
         if not (username and acctmgr.has_user(username)):
             add_warning(req, _(
                 "Please choose account by username from the list to proceed."
             ))
             req.redirect(req.href.admin('accounts', 'users'))
 
         change_uid_enabled = self.uid_changers and True or False
-        data = dict(i18n_tag=i18n_tag,
+        data = dict(_dgettext=dgettext,
                     attr_addonly=bool(req.args.get('attr_addonly')),
                     change_uid_enabled=change_uid_enabled,
                     skip_delete=bool(req.args.get('skip_delete')),
                     uid_exists=bool(req.args.get('uid_exists')),
                     url=req.href.admin('accounts', 'users', username),
                     user=username)
 
@@ -362,21 +369,23 @@
                 old_values = {}
                 if username in attributes:
                     old_values['name'] = attributes[username][1].get('name')
                     old_values['email'] = attributes[username][1].get('email')
                 success = []
 
                 # Delete a single user account attribute value.
-                if any(k.startswith('delete_email') for k in req.args):
+                if any([k.startswith('delete_email')
+                        for k in req.args.keys()]):
                     del_user_attribute(env, username, attribute='email')
                     add_notice(req, tag_(
                         "Deleted %(attribute)s for %(username)s.",
                         attribute=tag.b(labels.get('email')),
                         username=tag.b(username)))
-                elif any(k.startswith('delete_name') for k in req.args):
+                elif any([k.startswith('delete_name')
+                          for k in req.args.keys()]):
                     del_user_attribute(env, username, attribute='name')
                     add_notice(req, tag_(
                         "Deleted %(attribute)s for %(username)s.",
                         attribute=tag.b(labels.get('name')),
                         username=tag.b(username)))
 
                 password = req.args.get('password')
@@ -420,57 +429,58 @@
 
             # Change user ID of existing user account.
             elif action == 'uid':
                 new_uid = req.args.get('new_uid', '').strip()
                 results = None
                 if new_uid:
                     results = self._do_change_uid(req, username, new_uid)
-                if not results:
-                    pass
-                elif 'error' in results:
-                    for key, message in iteritems(results['error']):
+                if results:
+                    if 'error' in results:
                         add_warning(req, _(
                             "Update error in table %(table)s: %(message)s",
-                            table=key[0], message=message))
-                        break
-                else:
-                    add_notice(req, tag.ul(
-                        [tag.li(ngettext(
-                            "Table %(table)s column %(column)s%(constraint)s: "
-                            "%(result)s change",
-                            "Table %(table)s column %(column)s%(constraint)s: "
-                            "%(result)s changes",
-                            n_changes,
-                            table=tag.b(key[0]),
-                            column=tag.b(key[1]),
-                            constraint='(' + key[2] + ')' if key[2] else '',
-                            result=tag.b(n_changes)))
-                            for key, n_changes in sorted(iteritems(results))]
-                    ))
-                    # Switch to display information for new user ID.
-                    username = new_uid
-                    data.update({
-                        'url': req.href.admin('accounts', 'users', username),
-                        'user': username,
-                    })
+                            table=results['error'].keys()[0][0],
+                            message=results['error'].values()[0]))
+                    else:
+                        result_list = sorted([(k, v) for k, v in
+                                              results.iteritems()])
+                        add_notice(req, tag.ul(
+                            [tag.li(ngettext(
+                                "Table %(table)s column %(column)s"
+                                "%(constraint)s: %(result)s change",
+                                "Table %(table)s column %(column)s"
+                                "%(constraint)s: %(result)s changes",
+                                result[1], table=tag.b(result[0][0]),
+                                column=tag.b(result[0][1]),
+                                constraint=result[0][2] and
+                                           '(' + result[0][2] + ')' or '',
+                                result=tag.b(result[1])))
+                                for result in result_list]
+                        ))
+                        # Switch to display information for new user ID.
+                        username = new_uid
+                        data.update(
+                            dict(url=req.href.admin('accounts', 'users',
+                                                    username),
+                                 user=username)
+                        )
 
         # Get account attributes and account status information.
         stores = ExtensionOrder(components=acctmgr.stores,
                                 list=acctmgr.password_stores)
         user_store = acctmgr.find_user_store(username)
         if user_store:
             data['user_store'] = user_store.__class__.__name__
             data['store_order_num'] = stores[user_store]
             if hasattr(user_store, 'set_password'):
                 data['password_change_enabled'] = True
         data['ignore_auth_case'] = \
             self.config.getbool('trac', 'ignore_auth_case')
 
         approval = email = name = None
-        # Fetch data from 'session_attribute'.
+        # Fetch data from 'session_attributes'.
         attributes = get_user_attribute(self.env, username=username,
                                         authenticated=1)
         if username in attributes:
             name = attributes[username][1].get('name')
             email = attributes[username][1].get('email')
             if self.config.getbool('account-manager', 'require_approval'):
                 approval = attributes[username][1].get('approval')
@@ -499,25 +509,24 @@
                     "Failed login attempts for user %(user)s deleted",
                     user=tag.b(username)))
         data['approval'] = approval
 
         # Get access history.
         ts_seen = last_seen(env, username)
         if ts_seen and ts_seen[0][1]:
-            data['last_visit'] = datetime.fromtimestamp(ts_seen[0][1], req.tz)
+            data['last_visit'] = format_datetime(ts_seen[0][1], tzinfo=req.tz)
 
         if self.env.is_enabled(AccountGuard):
             attempts = []
             attempts_count = guard.failed_count(username, reset=None)
             if attempts_count > 0:
                 for attempt in guard.get_failed_log(username):
-                    attempt = attempt.copy()
-                    attempt['time'] = datetime.fromtimestamp(attempt['time'],
-                                                             req.tz)
-                    attempts.append(attempt)
+                    t = format_datetime(to_datetime(
+                        attempt['time']), tzinfo=req.tz)
+                    attempts.append({'ipnr': attempt['ipnr'], 'time': t})
                 data['attempts'] = attempts
                 data['pretty_lock_time'] = guard.pretty_lock_time(username,
                                                                   next=True)
             data['attempts_count'] = attempts_count
             data['lock_count'] = guard.lock_count(username)
             if guard.user_locked(username) is True:
                 data['user_locked'] = True
@@ -533,28 +542,28 @@
         data['active_form'] = req.args.get('action') or forms[0][0]
         add_ctxtnav(req, _("Account Attributes"),
                     href=req.href.admin('accounts', 'users', cleanup='1',
                                         accounts=username))
         add_ctxtnav(req, _("Back to Accounts"),
                     href=req.href.admin('accounts', 'users'))
         add_stylesheet(req, 'acct_mgr/acctmgr.css')
-        return 'account_admin.html', data
+        return genshi_template_args(self.env, 'account_admin.html', data)
 
     def _do_users(self, req):
         env = self.env
         acctmgr = self.acctmgr
         acctmod = AccountModule(env)
         listing_enabled = acctmgr.supports('get_users')
         password_change_enabled = acctmgr.supports('set_password')
         password_reset_enabled = acctmod.reset_password_enabled
         delete_enabled = acctmgr.supports('delete_user')
         verify_enabled = (EmailVerificationModule(env).email_enabled and
                           EmailVerificationModule(env).verify_email)
         data = {
-            'i18n_tag': i18n_tag,
+            '_dgettext': dgettext,
             'acctmgr': dict(), 'email_approved': True, 'filters': [],
             'listing_enabled': listing_enabled,
             'create_enabled': acctmgr.supports('set_password'),
             'delete_enabled': delete_enabled,
             'verify_enabled': verify_enabled,
             'ignore_auth_case': self.config.getbool('trac',
                                                     'ignore_auth_case'),
@@ -687,15 +696,15 @@
                 req.redirect(req.href.admin('accounts', 'users'))
 
             # Read account information.
             data.update(self._paginate(req, fetch_user_data(env, req,
                                                             filters)))
         add_stylesheet(req, 'acct_mgr/acctmgr.css')
         add_stylesheet(req, 'common/css/report.css')
-        return 'account_users.html', data
+        return genshi_template_args(self.env, 'account_users.html', data)
 
     def _do_change_uid(self, req, old_uid, new_uid):
         acctmgr = self.acctmgr
         acctmod = AccountModule(self.env)
         attr_overwrite = not bool(req.args.get('attr_addonly'))
         create_user = not bool(req.args.get('uid_exists'))
         delete_user = not bool(req.args.get('skip_delete'))
@@ -756,15 +765,15 @@
             name = old_uid in attributes and \
                    attributes[old_uid][1].get('name') or None
             if name:
                 req.args['name'] = name
 
             try:
                 acctmgr.validate_account(req)
-            except RegistrationError as e:
+            except RegistrationError, e:
                 add_warning(req, e)
                 if email:
                     set_user_attribute(self.env, old_uid, 'email', email)
                 return
             if not keep_passwd and \
                             self._set_password(req, new_uid,
                                                acctmod._random_password,
@@ -802,42 +811,42 @@
                 username=tag.b(new_uid)))
         if delete_user:
             # Finally delete old user ID.
             self._delete_user(req, old_uid)
         # Notify listeners about successful ID change.
         try:
             acctmgr._notify('id_changed', old_uid, new_uid)
-        except NotificationError as e:
+        except NotificationError, e:
             add_warning(req, _("Error raised while sending a change "
                                "notification.") +
                         _("You'll get details with TracLogging "
                           "enabled."))
             self.log.error('Unable to send user ID change notification: %s',
                            exception_to_unicode(e, traceback=True))
         return results
 
     def _set_password(self, req, username, password, overwrite=True):
         """Password saving with graceful handling of notification errors."""
         try:
             result = self.acctmgr.set_password(username, password,
                                                overwrite=overwrite)
-        except NotificationError as e:
+        except NotificationError, e:
             add_warning(req, _("Error raised while sending a change "
                                "notification.") +
                         _("You'll get details with TracLogging enabled."))
             self.log.error('Unable to send password change notification: %s',
                            exception_to_unicode(e, traceback=True))
             result = self.acctmgr.has_user(username) or None
         return result
 
     def _delete_user(self, req, username):
         """Delete method, that handles notification errors gracefully."""
         try:
             self.acctmgr.delete_user(username)
-        except NotificationError as e:
+        except NotificationError, e:
             add_warning(req, _("Error raised while sending a change "
                                "notification.") +
                         _("You'll get details with TracLogging "
                           "enabled."))
             self.log.error('Unable to send user delete notification: %s',
                            exception_to_unicode(e, traceback=True))
 
@@ -868,15 +877,15 @@
             prev_href = req.href.admin('accounts', 'users', page=page - 1)
             add_link(req, 'prev', prev_href, _('Previous Page'))
         page_href = req.href.admin('accounts', 'cleanup')
         return dict(accounts=pager, displayed_items=total,
                     page_href=page_href)
 
 
-class ConfigurationAdminPanel(Component):
+class ConfigurationAdminPanel(CommonTemplateProvider):
     implements(IAdminPanelProvider, IAuthenticator)
 
     auth_init = BoolOption('account-manager', 'auth_init', True,
                            doc="Launch an initial Trac authentication setup.")
 
     def __init__(self):
         self.acctmgr = AccountManager(self.env)
@@ -898,22 +907,22 @@
         cfg = self.config
         env = self.env
 
         def safe_wiki_to_html(context, text):
             """Convenience function from trac.admin.web_ui."""
             try:
                 return format_to_html(env, context, text)
-            except Exception as e:
+            except Exception, e:
                 self.log.error('Unable to render component documentation: %s',
                                exception_to_unicode(e, traceback=True))
             return tag.pre(text)
 
         data = {
-            'i18n_tag': i18n_tag,
-            'format_timespan': format_timespan,
+            '_dgettext': dgettext,
+            'pretty_precise_timedelta': pretty_precise_timedelta,
             'safe_wiki_to_html': safe_wiki_to_html,
         }
 
         # Prefer args from URL to make progress bar links work.
         step = req.args.get('step', 0)
         step = int(step and step or req.args.get('active', 0))
         stores = ExtensionOrder(components=self.acctmgr.stores,
@@ -991,43 +1000,44 @@
                     p = 'password_store'
                     # Set minimal required options, leaving most options out
                     # to keep them at - maybe changing - default values.
                     if init_store == 'db':
                         cfg.set(a, p, 'SessionStore')
                         cfg.set(c, 'acct_mgr.db.SessionStore', e)
                         cfg.set(c, 'acct_mgr.pwhash.HtDigestHashMethod', e)
-                        from .db import SessionStore
-                        from .pwhash import HtDigestHashMethod
+                        from acct_mgr.db import SessionStore
+                        from acct_mgr.pwhash import HtDigestHashMethod
                         assert env.is_enabled(HtDigestHashMethod)
                         assert env.is_enabled(SessionStore)
                     elif init_store == 'file':
                         if init_store_file == 'htdigest':
                             cfg.set(a, 'htdigest_file', 'trac.htdigest')
                             cfg.set(a, p, 'HtDigestStore')
                             cfg.set(c, 'acct_mgr.htfile.HtDigestStore', e)
-                            from .htfile import HtDigestStore
+                            from acct_mgr.htfile import HtDigestStore
                             assert env.is_enabled(HtDigestStore)
                         elif init_store_file == 'htpasswd':
                             cfg.set(a, 'htpasswd_file', 'trac.htpasswd')
                             cfg.set(a, 'htpasswd_hash_type', 'md5')
                             cfg.set(a, p, 'HtPasswdStore')
                             cfg.set(c, 'acct_mgr.htfile.HtPasswdStore', e)
-                            from .htfile import HtPasswdStore
+                            from acct_mgr.htfile import HtPasswdStore
                             assert env.is_enabled(HtPasswdStore)
                         elif init_store_file == 'svn_file':
                             cfg.set(a, p, 'SvnServePasswordStore')
                             cfg.set(c,
                                     'acct_mgr.svnserve.SvnServePasswordStore',
                                     e)
-                            from .svnserve import SvnServePasswordStore
+                            from acct_mgr.svnserve import \
+                                SvnServePasswordStore
                             assert env.is_enabled(SvnServePasswordStore)
                     elif init_store == 'http':
                         cfg.set(a, p, 'HttpAuthStore')
                         cfg.set(c, 'acct_mgr.http.HttpAuthStore', e)
-                        from .http import HttpAuthStore
+                        from acct_mgr.http import HttpAuthStore
                         assert env.is_enabled(HttpAuthStore)
                         # ToDo
                         # elif init_store == 'etc':
                         #    [account-manager]
                         #    password_store =
                         #    [components]
                 else:
@@ -1096,15 +1106,15 @@
                 verify_email = bool(req.args.get('verify_email', False))
                 cfg.set('account-manager', 'verify_email', verify_email)
                 cfg.set(
                     'components', 'acct_mgr.register.EmailVerificationModule',
                     verify_email and 'enabled' or 'disabled')
                 # Refresh object after changes.
                 register_checks = self.config.getlist('account-manager',
-                                                      'register_check')
+                                                      'register_checks')
                 checks = ExtensionOrder(components=self.acctmgr.checks,
                                         list=register_checks)
 
             elif step == 4:
                 acctmgr_guard = req.args.get('acctmgr_guard', False)
                 cfg.set('components', 'acct_mgr.guard.AccountGuard',
                         acctmgr_guard and 'enabled' or 'disabled')
@@ -1206,15 +1216,15 @@
                 options = []
                 for attr, option in _getoptions(store):
                     error = None
                     opt_val = None
                     value = None
                     try:
                         opt_val = option.__get__(store, store)
-                    except AttributeError as e:
+                    except AttributeError, e:
                         env.log.error(e)
                         regexp = r'^.* interface named \"(.*?)\".*$'
                         error = _("Error while reading configuration - Hint: "
                                   "Enable/install required component '%s'."
                                   % re.sub(regexp, r'\1', str(e)))
                         pass
                     if opt_val:
@@ -1334,15 +1344,15 @@
             options = []
             for attr, option in _getoptions(check):
                 error = None
                 opt_val = None
                 value = None
                 try:
                     opt_val = option.__get__(check, check)
-                except AttributeError as e:
+                except AttributeError, e:
                     env.log.error(e)
                     regexp = r'^.* interface named \"(.*?)\".*$'
                     error = _("Error while reading configuration - "
                               "Hint: Enable/install required component '%s'."
                               % re.sub(regexp, r'\1', str(e)))
                 if opt_val:
                     value = isinstance(opt_val, Component) and \
@@ -1444,15 +1454,15 @@
         details.append(dict(
             desc=_("Account Guard"),
             status=((not acctmgr_guard or login_attempt_max_count < 1) and
                     'disabled' or 'ok'),
             step=4)
         )
         admin_available = self.perms.get_users_with_permission('TRAC_ADMIN')
-        status = 'ok' if admin_available else 'error'
+        status = not admin_available and 'error' or 'ok'
         details.append(dict(desc=_("Admin user account"), status=status))
         # Require at least one admin account.
         ready = ready and status != 'error'
 
         details.append(dict(desc=_("Configuration Review"), status='unknown'))
         data.update({
             'admin_available': admin_available,
@@ -1494,15 +1504,16 @@
                     else:
                         roundup_defaults[section] = list((option[0],))
         data.update(dict(roundup=roundup, roundup_defaults=roundup_defaults))
 
         add_script(req, 'acct_mgr/js/acctmgr_admin.js')
         add_stylesheet(req, 'acct_mgr/acctmgr.css')
         add_stylesheet(req, 'common/css/report.css')
-        return 'account_config.html', data
+        return genshi_template_args(self.env, 'account_config.html',
+                                    data)
 
     # IAuthenticator methods
 
     def authenticate(self, req):
         """Launch an initial Trac authentication setup.
 
         This method authorizes the first login request after Trac environment
@@ -1550,22 +1561,22 @@
                 acctmgr.validate_account(req, True)
                 # Account email approval for authoritative action.
                 if verify_enabled and account['email'] and \
                         req.args.get('email_approved'):
                     set_user_attribute(env, account['username'],
                                        'email_verification_sent_to',
                                        account['email'])
-            except NotificationError as e:
+            except NotificationError, e:
                 add_warning(req, _("Error raised while sending a change "
                                    "notification.") +
                             _("You'll get details with TracLogging "
                               "enabled."))
                 env.log.error('Unable to send change notification: %s',
                               exception_to_unicode(e, traceback=True))
-            except RegistrationError as e:
+            except RegistrationError, e:
                 add_warning(req, e)
             else:
                 add_notice(req, tag_(
                     "Account %(username)s created.",
                     username=tag.b(account['username'])))
                 # User editor form clean-up.
                 account = {}
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/api.py` & `TracAccountManager-0.6.dev0/acct_mgr/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,30 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-from pkg_resources import resource_filename, resource_isdir
+from pkg_resources import resource_filename
 
-from trac.config import BoolOption, Option, OrderedExtensionsOption
+from trac.config import BoolOption
+from trac.config import Option, OrderedExtensionsOption
 from trac.core import Component, ExtensionPoint, Interface, TracError
 from trac.core import implements
 from trac.perm import IPermissionRequestor, PermissionCache
-from trac.util.text import cleandoc, exception_to_unicode
-from trac.util.translation import domain_functions
+from trac.util.compat import cleandoc
+from trac.util.text import exception_to_unicode
+from trac.util.translation import dgettext, domain_functions
 from trac.web.chrome import ITemplateProvider, add_warning
 from trac.web.main import IRequestFilter
 
-from .compat import use_jinja2
-
-DOMAIN = 'acct_mgr'
-
 add_domain, _, N_, gettext, ngettext, tag_ = \
-    domain_functions(DOMAIN, ('add_domain', '_', 'N_', 'gettext', 'ngettext',
-                              'tag_'))
+    domain_functions('acct_mgr', ('add_domain', '_', 'N_', 'gettext',
+                                  'ngettext', 'tag_'))
 
 cleandoc_ = cleandoc
 
 
 class IAccountChangeListener(Interface):
     """An interface for receiving account change events."""
 
@@ -99,15 +97,15 @@
     """An interface for Components that provide a storage method for users and
     passwords.
     """
 
     def config_key():
         """'''Deprecated''': New implementations should not use this method.
 
-        The preferred way to configure an `IPasswordStore` implementation is by
+        The prefered way to configure an `IPasswordStore` implemenation is by
         using its class name in the `password_store` option.
 
         Returns a string used to identify this implementation in the config.
         This password storage implementation will be used, if the value of
         config property "account-manager.password_format" matches.
         """
 
@@ -124,19 +122,19 @@
         Returns True, if a new account was created, False if an existing
         account was updated.
         """
 
     def check_password(user, password):
         """Checks if the password is valid for the user.
 
-        Returns True, if the correct user and password are specified.
+        Returns True, if the correct user and password are specfied.
         Returns False, if the incorrect password was specified.
         Returns None, if the user doesn't exist in this password store.
 
-        Note: Returning `False` is an active rejection of the login attempt.
+        Note: Returing `False` is an active rejection of the login attempt.
         Return None to let the authentication eventually fall through to
         next store in a chain.
         """
 
     def delete_user(user):
         """Deletes the user account.
 
@@ -168,16 +166,15 @@
     The methods will be handled by underlying password storage implementations
     set in trac.ini with the "account-manager.password_store" option.
 
     The "account-manager.password_store" may be an ordered list of password
     stores, and if so, then each password store is queried in turn.
     """
 
-    implements(IAccountChangeListener, IPermissionRequestor, IRequestFilter,
-               ITemplateProvider)
+    implements(IAccountChangeListener, IPermissionRequestor, IRequestFilter)
 
     change_listeners = ExtensionPoint(IAccountChangeListener)
 
     # All checks, not only the configured ones (see self.register_checks).
     checks = ExtensionPoint(IAccountRegistrationInspector)
 
     password_stores = OrderedExtensionsOption(
@@ -219,23 +216,18 @@
             but should be disabled/unset otherwise.""")
 
     username_char_blacklist = Option(
         'account-manager', 'username_char_blacklist', ':[]',
         doc="""Always exclude some special characters from usernames.
             This is enforced upon new user registration.""")
 
-    _htdocs_dir = resource_filename(__name__, 'htdocs')
-    _templates_dir = resource_filename(
-        __name__, 'templates/%s' % ('jinja2' if use_jinja2 else 'genshi'))
-
     def __init__(self):
         # Bind the 'acct_mgr' catalog to the specified locale directory.
-        if resource_isdir(__name__, 'locale'):
-            locale_dir = resource_filename(__name__, 'locale')
-            add_domain(self.env.path, locale_dir)
+        locale_dir = resource_filename(__name__, 'locale')
+        add_domain(self.env.path, locale_dir)
 
     # Public API
 
     def get_users(self):
         """Get usernames from all active stores.
 
         Because we allow concurrent active stores, and some stores even don't
@@ -274,22 +266,23 @@
                 # Support former method signature - overwrite unconditionally.
                 result = None
                 if overwrite or not store.has_user(user):
                     result = store.set_password(user, password, old_password)
             if result:
                 self._notify('created', user, password)
             elif not overwrite:
-                raise TracError(_("Password for user %(user)s existed, "
-                                  "couldn't create.", user=user))
+                raise TracError(_(
+                    "Password for user %s existed, couldn't create." % user))
             else:
                 self._notify('password_changed', user, password)
         else:
-            raise TracError(_("None of the IPasswordStore components listed "
-                              "in the trac.ini supports setting the password "
-                              "or creating users."))
+            raise TracError(_(
+                """None of the IPasswordStore components listed in the
+                trac.ini supports setting the password or creating users.
+                """))
         return result
 
     def check_password(self, user, password):
         valid = False
         user = self.handle_username_casing(user)
         for store in self.password_stores:
             valid = store.check_password(user, password)
@@ -306,15 +299,15 @@
         # Delete credentials from password store.
         store = self.find_user_store(user)
         del_method = getattr(store, 'delete_user', None)
         if callable(del_method):
             del_method(user)
         # Delete session attributes, session and any custom permissions
         # set for the user.
-        from .model import delete_user
+        from acct_mgr.model import delete_user
         delete_user(self.env, user)
         self._notify('deleted', user)
 
     def supports(self, operation):
         try:
             self.password_stores
         except AttributeError:
@@ -390,15 +383,15 @@
         """Set password and prime a new authenticated Trac session."""
         username = req.args.get('username', '').strip()
         username = self.handle_username_casing(username)
         # Result of a successful account creation request is a made-up
         # authenticated session, that a new user can refer to later on.
         # Strictly required to create a primary key for additional attributes,
         # perhaps even something as critical as the SessionStore password.
-        from .model import prime_auth_session, set_user_attribute
+        from acct_mgr.model import prime_auth_session, set_user_attribute
         try:
             prime_auth_session(self.env, username)
             # Save attributes for the user with reference to that session ID.
             # Done before writing to a password store to preserve attributes
             # in case of non-fatal errors (especially notification errors).
             for attribute in ('name', 'email'):
                 value = req.args.get(attribute)
@@ -407,19 +400,19 @@
                 set_user_attribute(self.env, username, attribute, value)
             # Create the user in the configured (primary) password store.
             self.set_password(username, req.args.get('password'),
                               overwrite=False)
         finally:
             if not self.has_user(username):
                 # Rollback.
-                from .model import delete_user
+                from acct_mgr.model import delete_user
                 delete_user(self.env, username)
 
     def _maybe_update_hash(self, user, password):
-        from .model import get_user_attribute, set_user_attribute
+        from acct_mgr.model import get_user_attribute, set_user_attribute
         if get_user_attribute(self.env, user, 1,
                               'password_refreshed', 1) == [0]:
             self.log.debug("Refresh password for user: %s", user)
             store = self.find_user_store(user)
             pwstore = self.get_supporting_store('set_password')
             if pwstore.set_password(user, password) is True:
                 # Account re-created according to current settings.
@@ -431,15 +424,15 @@
     def _notify(self, mod, *args):
         mod = '_'.join(['user', mod])
         for listener in self.change_listeners:
             # Support divergent account change listener implementations too.
             try:
                 self.log.debug("CHANGE_LISTENER: %s(%s)", repr(listener), mod)
                 getattr(listener, mod)(*args)
-            except AttributeError as e:
+            except AttributeError, e:
                 self.log.warning("IAccountChangeListener %s does not support "
                                  "method %s: %s", listener.__class__.__name__,
                                  mod, exception_to_unicode(e))
 
     # IAccountChangeListener methods
 
     def user_created(self, user, password):
@@ -488,27 +481,35 @@
     def get_permission_actions(self):
         action = ['ACCTMGR_CONFIG_ADMIN', 'ACCTMGR_USER_ADMIN', 'EMAIL_VIEW',
                   'USER_VIEW']
         actions = [('ACCTMGR_ADMIN', action), action[0],
                    (action[1], action[2:]), action[3]]
         return actions
 
+
+class CommonTemplateProvider(Component):
+    """Generic template provider."""
+
+    implements(ITemplateProvider)
+
+    abstract = True
+
     # ITemplateProvider methods
 
     def get_htdocs_dirs(self):
         """Return the absolute path of a directory containing additional
         static resources (such as images, style sheets, etc).
         """
-        yield 'acct_mgr', self._htdocs_dir
+        return [('acct_mgr', resource_filename(__name__, 'htdocs'))]
 
     def get_templates_dirs(self):
         """Return the absolute path of the directory containing the provided
         Genshi templates.
         """
-        yield self._templates_dir
+        return [resource_filename(__name__, 'templates')]
 
 
 class GenericUserIdChanger(Component):
     """Define common class attributes for IUserIdChanger components."""
 
     implements(IUserIdChanger)
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/db.py` & `TracAccountManager-0.6.dev0/acct_mgr/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-from trac.core import Component, implements
 from trac.config import ExtensionOption
+from trac.core import Component, implements
 
-from .api import IPasswordStore, N_
-from .pwhash import IPasswordHashMethod
+from acct_mgr.api import IPasswordStore
+from acct_mgr.pwhash import IPasswordHashMethod
 
 
 class SessionStore(Component):
-
     implements(IPasswordStore)
 
     hash_method = ExtensionOption('account-manager', 'hash_method',
         IPasswordHashMethod, 'HtDigestHashMethod',
-        doc=N_("IPasswordHashMethod used to create new/updated passwords"))
+        doc="IPasswordHashMethod used to create new/updated passwords")
 
     def __init__(self):
         self.key = 'password'
         # Check for valid hash method configuration.
         self.hash_method_enabled
 
     def get_users(self):
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/guard.py` & `TracAccountManager-0.6.dev0/acct_mgr/guard.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
 from datetime import timedelta
-import json
-import time
 
+from acct_mgr.model import del_user_attribute, get_user_attribute
+from acct_mgr.model import set_user_attribute, user_known
 from trac.config import IntOption, Option
 from trac.core import Component
 from trac.util.datefmt import format_datetime, pretty_timedelta
 from trac.util.datefmt import to_datetime, to_timestamp
 
-from .compat import unicode
-from .model import (del_user_attribute, get_user_attribute, set_user_attribute,
-                    user_known)
-
 
 class AccountGuard(Component):
     """The AccountGuard component protects against brute-force attacks
     on user passwords.
 
     It does so by adding logging of failed login attempts,
     account status tracking and administative user account locking.
@@ -98,19 +94,19 @@
         if not reset:
             # Trigger the failed attempt logger.
             attempts = self.get_failed_log(user)
             log_length = len(attempts)
             if log_length > self.login_attempt_max_count:
                 # Truncate attempts list preserving most recent events.
                 del attempts[:(log_length - self.login_attempt_max_count)]
-            attempts.append({'ipnr': ipnr, 'time': int(time.time())})
+            attempts.append({'ipnr': ipnr,
+                             'time': to_timestamp(to_datetime(None))})
             count += 1
             # Update or create attempts counter and list.
-            set_user_attribute(self.env, user, 'failed_logins',
-                               unicode(attempts))
+            set_user_attribute(self.env, user, 'failed_logins', str(attempts))
             set_user_attribute(self.env, user, key, count)
             self.log.debug("AccountGuard.failed_count(%s) = %s", user, count)
         else:
             # Delete existing attempts counter and list.
             del_user_attribute(self.env, user, 1, 'failed_logins')
             del_user_attribute(self.env, user, 1, key)
             # Delete the lock count too.
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/acctmgr.css` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/acctmgr.css`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/approval.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/approval.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/arrow.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/arrow.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/delete.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/delete.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/guard.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/guard.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/info.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/info.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/js/acctmgr_admin.js` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/js/acctmgr_admin.js`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/locked.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/locked.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/refresh.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/refresh.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/status_disabled.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_disabled.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/status_error.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_error.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/status_ok.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_ok.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/status_unknown.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/status_unknown.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/time-locked.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/time-locked.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htdocs/users.png` & `TracAccountManager-0.6.dev0/acct_mgr/htdocs/users.png`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/acct_mgr/htfile.py` & `TracAccountManager-0.6.dev0/acct_mgr/htfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,39 +6,22 @@
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
 import errno
-import io
 import os
 
+from acct_mgr.api import IPasswordStore, _
+from acct_mgr.pwhash import htpasswd, mkhtpasswd, htdigest
+from acct_mgr.util import EnvRelativePathOption
 from trac.config import Option
 from trac.core import Component, TracError, implements
 
-from .api import IPasswordStore, _, N_
-from .compat import compare_digest, unicode
-from .pwhash import check_hash, generate_hash, htdigest
-from .util import EnvRelativePathOption
-
-
-def _eachline(filename, encoding='utf-8'):
-    with io.open(filename, 'r', encoding=encoding) as f:
-        for line in f:
-            yield line
-
-
-def _writelines(filename, lines, encoding='utf-8'):
-    with io.open(filename, 'w', encoding=encoding) as f:
-        for line in lines:
-            if isinstance(line, bytes):
-                line = unicode(line, 'utf-8')
-            f.write(line)
-
 
 class AbstractPasswordFileStore(Component):
     """Base class for managing password files.
 
     Derived classes support different formats such as
     Apache's htpasswd and htdigest format.
     See these concrete sub-classes for usage information.
@@ -47,41 +30,47 @@
 
     # Note: 'filename' is a required, store-specific option.
 
     def has_user(self, user):
         return user in self.get_users()
 
     def get_users(self):
-        filename = self.filename
+        filename = str(self.filename)
         if not os.path.exists(filename):
             self.log.error('acct_mgr: get_users() -- '
                            'Can\'t locate password file "%s"', filename)
             return []
         return self._get_users(filename)
 
     def set_password(self, user, password, old_password=None, overwrite=True):
+        user = user.encode('utf-8')
+        password = password.encode('utf-8')
         return not self._update_file(self.prefix(user),
                                      self.userline(user, password),
                                      overwrite)
 
     def delete_user(self, user):
+        user = user.encode('utf-8')
         return self._update_file(self.prefix(user), None)
 
     def check_password(self, user, password):
-        filename = self.filename
+        filename = str(self.filename)
         if not os.path.exists(filename):
             self.log.error('acct_mgr: check_password() -- '
                            'Can\'t locate password file "%s"', filename)
             return False
+        user = user.encode('utf-8')
+        password = password.encode('utf-8')
         prefix = self.prefix(user)
         try:
-            for line in _eachline(filename):
-                if line.startswith(prefix):
-                    line = line[len(prefix):].rstrip('\n')
-                    return self._check_userline(user, password, line)
+            with open(filename, 'rU') as f:
+                for line in f:
+                    if line.startswith(prefix):
+                        line = line[len(prefix):].rstrip('\n')
+                        return self._check_userline(user, password, line)
         except (OSError, IOError):
             self.log.error('acct_mgr: check_password() -- '
                            'Can\'t read password file "%s"', filename)
         return None
 
     def _update_file(self, prefix, userline, overwrite=True):
         """Add or remove user and change password.
@@ -96,35 +85,27 @@
         """
         if not self.filename:
             option = self.__class__.filename
             raise TracError(
                 _("[%(section)s] %(name)s option for the password "
                   "file is not configured",
                   section=option.section, name=option.name))
-        filename = self.filename
+        filename = str(self.filename)
         matched = False
         new_lines = []
         eol = '\n'
         try:
             # Open existing file read-only to read old content.
-            lines = list(_eachline(filename))
-        except EnvironmentError as e:
-            if e.errno == errno.ENOENT:
-                # Ignore, when file doesn't exist and create it below.
-                pass
-            elif e.errno == errno.EACCES:
-                raise TracError(_(
-                    "The password file could not be read. Trac requires read "
-                    "and write access to both the password file and its "
-                    "parent directory."))
-            else:
-                raise
-        else:
+            # DEVEL: Use `with` statement available in Python >= 2.5
+            #   as soon as we don't need to support 2.4 anymore.
+            with open(filename) as f:
+                lines = f.readlines()
+
             # DEVEL: Beware, in shared use there is a race-condition,
-            #   since file changes by other programs that occur from now on
+            #   since file changes by other programs that occure from now on
             #   are currently not detected and will get overwritten.
             #   This could be fixed by file locking, but a cross-platform
             #   implementation is certainly non-trivial.
             if len(lines) > 0:
                 # predict eol style for lines without eol characters
                 if not os.linesep == '\n':
                     if lines[-1].endswith('\r') and os.linesep == '\r':
@@ -147,31 +128,49 @@
                     elif line.endswith(eol) and not \
                             (eol == '\n' and line.endswith('\r\n')):
                         new_lines.append(line)
                     # unify eol style using confirmed default and
                     # make sure the (last) line has a newline anyway
                     else:
                         new_lines.append(line.rstrip('\r\n') + eol)
+        except EnvironmentError, e:
+            if e.errno == errno.ENOENT:
+                # Ignore, when file doesn't exist and create it below.
+                pass
+            elif e.errno == errno.EACCES:
+                raise TracError(_(
+                    """The password file could not be read. Trac requires
+                    read and write access to both the password file
+                    and its parent directory."""))
+            else:
+                raise
 
         # Finally add the new line here, if it wasn't used before
         # to update or delete a line, creating content for a new file as well.
         if not matched and userline:
             new_lines.append(userline + eol)
 
         # Try to (re-)open file write-only now and save new content.
         try:
-            _writelines(filename, new_lines)
-        except EnvironmentError as e:
+            with open(filename, 'w') as f:
+                f.writelines(new_lines)
+        except EnvironmentError, e:
             if e.errno == errno.EACCES or e.errno == errno.EROFS:
                 raise TracError(_(
-                    "The password file could not be updated. Trac requires "
-                    "read and write access to both the password file and its "
-                    "parent directory."))
+                    """The password file could not be updated. Trac requires
+                    read and write access to both the password file
+                    and its parent directory."""))
             else:
                 raise
+        if f:
+            # Close open file now, even after exception raised.
+            f.close()
+            if not f.closed:
+                self.log.debug('acct_mgr: _update_file() -- '
+                               'Closing password file "%s" failed', filename)
         return matched
 
 
 class HtPasswdStore(AbstractPasswordFileStore):
     """Manages user accounts stored in Apache's htpasswd format.
 
     To use this implementation add the following configuration section to
@@ -186,36 +185,37 @@
     Default behaviour is to detect presence of 'crypt' and use it or
     fallback to generation of passwords with md5 hash otherwise.
     """
 
     implements(IPasswordStore)
 
     filename = EnvRelativePathOption('account-manager', 'htpasswd_file', '',
-        doc=N_("Path relative to Trac environment or full host machine path "
-               "to password file"))
+        doc="Path relative to Trac environment or full host machine path "
+            "to password file")
     hash_type = Option('account-manager', 'htpasswd_hash_type', 'crypt',
-        doc=N_("Default hash type of new/updated passwords"))
+        doc="Default hash type of new/updated passwords")
 
     def config_key(self):
         return 'htpasswd'
 
     def prefix(self, user):
         return user + ':'
 
     def userline(self, user, password):
-        return self.prefix(user) + generate_hash(password, self.hash_type)
+        return self.prefix(user) + mkhtpasswd(password, self.hash_type)
 
     def _check_userline(self, user, password, suffix):
-        return check_hash(password, suffix)
+        return suffix == htpasswd(password, suffix)
 
     def _get_users(self, filename):
-        for line in _eachline(filename):
-            user = line.split(':', 1)[0]
-            if user:
-                yield user
+        with open(filename, 'rU') as f:
+            for line in f:
+                user = line.split(':', 1)[0]
+                if user:
+                    yield user.decode('utf-8')
 
 
 class HtDigestStore(AbstractPasswordFileStore):
     """Manages user accounts stored in Apache's htdigest format.
 
     To use this implementation add the following configuration section to
     trac.ini:
@@ -226,33 +226,34 @@
     htdigest_realm = TracDigestRealm
     }}}
     """
 
     implements(IPasswordStore)
 
     filename = EnvRelativePathOption('account-manager', 'htdigest_file', '',
-        doc=N_("Path relative to Trac environment or full host machine path "
-               "to password file"))
+        doc="""Path relative to Trac environment or full host machine
+            path to password file""")
     realm = Option('account-manager', 'htdigest_realm', '',
-        doc=N_("Realm to select relevant htdigest file entries"))
+        doc="Realm to select relevant htdigest file entries")
 
     def config_key(self):
         return 'htdigest'
 
     def prefix(self, user):
-        return '%s:%s:' % (user, self.realm)
+        return '%s:%s:' % (user, self.realm.encode('utf-8'))
 
     def userline(self, user, password):
-        prefix = self.prefix(user)
-        return prefix + htdigest(user, self.realm, password)
+        return self.prefix(user) + htdigest(user, self.realm.encode('utf-8'),
+                                            password)
 
     def _check_userline(self, user, password, suffix):
-        hash_ = htdigest(user, self.realm, password)
-        return compare_digest(suffix, hash_)
+        return suffix == htdigest(user, self.realm.encode('utf-8'), password)
 
     def _get_users(self, filename):
-        for line in _eachline(filename):
-            args = line.split(':')[:2]
-            if len(args) == 2:
-                user, realm = args
-                if realm == self.realm and user:
-                    yield user
+        _realm = self.realm.encode('utf-8')
+        with open(filename) as f:
+            for line in f:
+                args = line.split(':')[:2]
+                if len(args) == 2:
+                    user, realm = args
+                    if realm == _realm and user:
+                        yield user.decode('utf-8')
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/http.py` & `TracAccountManager-0.6.dev0/acct_mgr/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,67 +5,58 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-import sys
-if sys.version_info[0] == 2:
-    from urlparse import urlparse
-    from urllib2 import (HTTPPasswordMgrWithDefaultRealm,
-                         HTTPBasicAuthHandler, HTTPDigestAuthHandler,
-                         build_opener)
-else:
-    from urllib.parse import urlparse
-    from urllib.request import (HTTPPasswordMgrWithDefaultRealm,
-                                HTTPBasicAuthHandler, HTTPDigestAuthHandler,
-                                build_opener)
+import urllib2
+import urlparse
 
 from trac.config import Option
 from trac.core import Component, implements
 from trac.web.href import Href
 
-from .api import IPasswordStore, N_
+from acct_mgr.api import IPasswordStore, N_
+from acct_mgr.util import HTTPBasicAuthHandler
 
 
 class HttpAuthStore(Component):
-
     implements(IPasswordStore)
 
     auth_url = Option('account-manager', 'authentication_url', '',
-        doc=N_("URL of the HTTP authentication service"))
+        doc="URL of the HTTP authentication service")
 
     def check_password(self, username, password):
         self.log.debug("Trac.ini authentication_url = '%s'", self.auth_url)
         # Nothing to do, if URL is absolute.
         if self.auth_url.startswith('http://') or \
                 self.auth_url.startswith('https://'):
             auth_url = self.auth_url
         # Handle server-relative URLs.
         elif self.auth_url.startswith('/'):
             # Prepend the Trac server component.
-            pr = urlparse(self.env.abs_href())
+            pr = urlparse.urlparse(self.env.abs_href())
             href = Href(pr[0] + '://' + pr[1])
             auth_url = href(self.auth_url)
         elif '/' in self.auth_url:
             # URLs with path like 'common/authFile' or 'site/authFile'.
             auth_url = self.env.abs_href.chrome(self.auth_url)
         else:
             # Bare file name option value like 'authFile'.
             auth_url = self.env.abs_href.chrome('common', self.auth_url)
         self.log.debug("Final auth_url = '%s'", auth_url)
 
-        acctmgr = HTTPPasswordMgrWithDefaultRealm()
+        acctmgr = urllib2.HTTPPasswordMgrWithDefaultRealm()
         acctmgr.add_password(None, auth_url, username, password)
         try:
-            build_opener(HTTPBasicAuthHandler(acctmgr),
-                                 HTTPDigestAuthHandler(acctmgr))\
+            urllib2.build_opener(HTTPBasicAuthHandler(acctmgr),
+                                 urllib2.HTTPDigestAuthHandler(acctmgr))\
                    .open(auth_url)
-        except IOError as e:
+        except IOError, e:
             if hasattr(e, 'code') and e.code == 404:
                 self.log.debug("HttpAuthStore page not found; we are "
                                "authenticated nonetheless")
                 return True
             if hasattr(e, 'code') and e.code == 401:
                 self.log.debug("HttpAuthStore authentication failed")
             return None
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.mo` & `TracAccountManager-0.6.dev0/acct_mgr/locale/de/LC_MESSAGES/acct_mgr.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,28 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: TracAccountManager 0.6\n"
+"Project-Id-Version: TracAccountManager 0.5\n"
 "Report-Msgid-Bugs-To: hoff.st@shaas.net\n"
-"POT-Creation-Date: 2023-04-06 13:05+0000\n"
+"POT-Creation-Date: 2012-12-22 23:08+0100\n"
 "PO-Revision-Date: 2012-09-16 19:07+0000\n"
 "Last-Translator: Steffen Hoffmann <hoff.st@web.de>\n"
 "Language: de\n"
 "Language-Team: German <trac-dev@googlegroups.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.6.0\n"
 
 msgid " Add "
 msgstr " Hinzufügen "
 
+msgid " Change "
+msgstr " Ändern "
+
 msgid "%(count)s account"
 msgid_plural "%(count)s accounts"
 msgstr[0] "%(count)s Benutzerkonto"
 msgstr[1] "%(count)s Benutzerkonten"
 
 msgid "%(count)s account attribute"
 msgid_plural "%(count)s account attributes"
@@ -32,649 +35,745 @@
 msgstr[1] "%(num)i Tage %%s"
 
 msgid "%(num)i second"
 msgid_plural "%(num)i seconds"
 msgstr[0] "%(num)i Sekunde"
 msgstr[1] "%(num)i Sekunden"
 
+msgid "%(relativetime)s ago"
+msgstr "vor %(relativetime)s"
+
 msgid "(required %(perm)s missing)"
 msgstr "(erforderliches %(perm)s fehlt)"
 
 msgid ""
-"A collection of basic checks.\n"
-"\n"
-"This includes checking for\n"
-" * emptiness (no user input for username and/or password)\n"
-" * some blacklisted username characters\n"
-" * upper-cased usernames (reserved for Trac permission actions)\n"
-" * some reserved usernames\n"
-" * a username duplicate in configured password stores\n"
-"\n"
-"''This check is bypassed for requests regarding user's own preferences.''"
-msgstr ""
-"Eine Sammlung grundlegender Überprüfungen.\n"
-"\n"
-"Dies beinhaltet die Überprüfung auf\n"
-" * Leerheit (keine Benutzereingabe für Benutzername und/oder Passwort)\n"
-" * einige Zeichen auf der schwarzen Liste des Benutzernamens\n"
-" * Benutzernamen in Großbuchstaben (reserviert für Trac-"
-"Berechtigungsaktionen)\n"
-" * einige reservierte Benutzernamen\n"
-" * ein Duplikat des Benutzernamens in konfigurierten Passwortspeichern\n"
-"\n"
-"''Diese Überprüfung wird bei Anfragen bezüglich der eigenen Präferenzen des "
-"Benutzers umgangen.''"
-
-msgid ""
-"A collection of checks based on regular expressions.\n"
-"\n"
-"''It depends on !EmailCheck being enabled too for using it's input field.\n"
-"Likewise email checking is bypassed, if account verification is\n"
-"disabled.''"
-msgstr ""
-"Eine Sammlung von Prüfungen basierend auf regulären Ausdrücken.\n"
-"\n"
-"''Es hängt davon ab, ob !EmailCheck auch für die Verwendung des Eingabefelds "
-"aktiviert ist.\n"
-"Ebenso wird die Email-Prüfung umgangen, wenn die Kontoverifizierung\n"
-"Behinderte.''"
-
-msgid ""
-"A collection of checks for email addresses.\n"
-"\n"
-"''This check is bypassed, if account verification is disabled.''"
-msgstr ""
-"Eine Sammlung von Prüfungen für Email-Adressen.\n"
-"\n"
-"''Diese Überprüfung wird umgangen, wenn die Kontoüberprüfung deaktiviert "
-"ist.''"
-
-msgid "A new password has been sent to you at <%(email)s>."
+"A new password\n"
+"        has been emailed to you at %(email)s ."
 msgstr ""
-"Ein neues Passwort ist Ihnen per Email zugeschickt worden an <%(email)s>."
+"Ein neues Kennwort ist Ihnen per E-Mail zugeschickt worden an %(email)s ."
+
+msgid "A notification email has been resent to <%s>."
+msgstr "Eine E-Mail-Benachrichtigung ist an <%s> gesendet worden."
 
 msgid "A username with only upper-cased characters is not allowed."
 msgstr ""
 "Ein Nutzername ausschliesslich aus Grossbuchstaben bestehend ist nicht "
 "zugelassen."
 
 msgid "Access History"
 msgstr "Zugriffsverlauf"
 
 msgid "Account"
 msgstr "Nutzerkonto"
 
-msgid "Account %(username)s created."
-msgstr "Konto %(username)s erstellt."
+msgid "Account Details"
+msgstr "Nutzerkontendetails"
 
 msgid "Account Notification"
 msgstr "Nutzerkontenbenachrichtigung"
 
 msgid "Account Status"
 msgstr "Nutzerkontenstatus"
 
-msgid ""
-"Account is pending approval. You may need to contact your administrator."
-msgstr ""
-"Das Konto muss noch genehmigt werden. Möglicherweise müssen Sie sich an "
-"Ihren Administrator wenden."
-
-msgid "Account lock (%(condition)s) for user %(user)s cleared"
-msgstr "Kontosperre (%(condition)s) für Benutzer %(user)s aufgehoben"
+msgid "Account guard"
+msgstr "Nutzerkontenwächter"
 
 msgid "Account locked"
 msgstr "Nutzerkonto gesperrt"
 
-msgid "Account locked, please try again after %(release_time)s"
+msgid ""
+"Account locked, please try again after\n"
+"                            %(release_time)s\n"
+"                            "
 msgstr "Nutzerkonto gesperrt, bitte nach %(release_time)s nochmals versuchen"
 
 msgid "Accounts"
 msgstr "Nutzerkonten"
 
+msgid "Accounts (%(slice)s)"
+msgstr "Nutzerkonten (%(slice)s)"
+
 msgid "Accounts: Cleanup"
 msgstr "Nutzerkonten: Bereinigung"
 
 msgid "Accounts: Configuration"
 msgstr "Nutzerkonten: Einstellungen"
 
 msgid "Accounts: Notification Configuration"
 msgstr "Nutzerkonten: Benachrichtigungseinstellungen"
 
-msgid "Apply changes"
-msgstr "Änderungen übernehmen"
+msgid "Add a new user account or edit an existing one."
+msgstr "Füge ein neues Benutzerkonto hinzu oder bearbeite ein bestehendes."
 
-msgid "Apply changes and go back"
-msgstr "Übernehmen Sie die Änderungen und gehe zurück"
+msgid "Add/Edit Account:"
+msgstr "Benutzerkonto hinzufügen/bearbeiten:"
 
-msgid "Apply changes and go on"
-msgstr "Übernehmen Sie die Änderungen und fahren Sie fort"
+msgid ""
+"Allow the user to be remembered across sessions without needing to\n"
+"          re-authenticate."
+msgstr "Erlaube das Wiedererkennen des Nutzers ohne Neuanmeldung."
+
+msgid "Already logged in"
+msgstr "Bereits angemeldet"
+
+msgid ""
+"An email has been sent to <%(email)s> with a token to\n"
+"                %(link)s."
+msgstr ""
+"Eine E-Mail-Nachricht mit einem Bestätigungscode wurde an <%(email)s> "
+"gesendet, um %(link)s."
+
+msgid ""
+"An email was sent to\n"
+"        %(email)s with a token to verify your new address.\n"
+"        Please check your email and enter the token in the form below."
+msgstr ""
+"Zur Bestätigung Ihrer neuen Adresse wurde eine E-Mail-Nachricht mit einem "
+"Bestätigungscode an %(email)s gesendet. Bitte sehen Sie Ihre Nachrichten "
+"durch, und tragen Sie den Code in das nachfolgende Feld ein."
+
+msgid ""
+"Another account or group already exists, who's name differs from %s only by "
+"case or is identical."
+msgstr ""
+"Es existiert bereits ein Benutzerkonto oder eine Gruppe namens %s oder mit "
+"einem nur bezüglich Gross-/Kleinschreibung abweichenden Namen."
 
 msgid "Are you human? If so, try harder!"
 msgstr "Sind Sie eine Person? Dann strengen Sie sich mehr an!"
 
 msgid "Are you sure you want to delete your account?"
 msgstr "Sind Sie sicher, dass Sie Ihr Nutzerkonto löschen möchten?"
 
-msgid "At least %(required_check)s must be configured and enabled."
-msgstr "Mindestens %(required_check)s muss konfiguriert und aktiviert sein."
-
 msgid "Attribute"
 msgstr "Eigenschaft"
 
 msgid "Authenticated Accounts"
 msgstr "Authentifizierte Nutzerkonten"
 
+msgid "Back to accounts"
+msgstr "Zurück zu Nutzerkonten"
+
 msgid "Better do not fill this field."
 msgstr "In dieses Feld tragen Sie lieber nichts ein."
 
-msgid "Cannot reset password: %(error)s"
-msgstr "Passwort kann nicht zurückgesetzt werden: %(error)s"
-
-msgid ""
-"Cannot send the new password to the user, because no email address is "
-"associated with %(username)s."
-msgstr ""
-"Das neue Passwort kann nicht an den Benutzer gesendet werden, da keine Email-"
-"Adresse lautet verknüpft mit %(username)s."
-
 msgid "Change Password"
 msgstr "Kennwortänderung"
 
-msgid "Change user ID ('username')"
-msgstr "Benutzer-ID ändern ('Benutzername')"
-
-msgid "Check IP address for authentication."
-msgstr "Überprüfen Sie die IP-Adresse für die Authentifizierung."
-
-msgid ""
-"Check for usernames referenced in the permission system.\n"
-"\n"
-"''This check is bypassed for requests by an authenticated user.''"
-msgstr ""
-"Nach Benutzernamen suchen, auf die im Berechtigungssystem verwiesen wird.\n"
-"\n"
-"''Diese Prüfung wird bei Anfragen eines authentifizierten Benutzers "
-"umgangen.''"
-
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgid "Confirm Password:"
 msgstr "Kennwortbestätigung:"
 
-msgid "Convert login names to lower case on registration and login."
-msgstr ""
-"Konvertieren Sie Anmeldenamen bei Registrierung und Anmeldung in "
-"Kleinbuchstaben."
-
 msgid "Create account"
 msgstr "Nutzerkonto erstellen"
 
+msgid ""
+"Credentials for this user are stored in AuthStore number\n"
+"              [1:%(order_num)s] (%(store)s)."
+msgstr ""
+"Identitätsmerkmale für diesen Nutzer sind im Beglaubigungsregister Nummer [1:"
+"%(order_num)s] (%(store)s) gespeichert."
+
 msgid "Current email address: <%(email)s>"
-msgstr "Aktuelle Email-Adresse: <%(email)s>"
+msgstr "Aktuelle E-Mail-Adresse: <%(email)s>"
+
+msgid "Default hash type of new/updated passwords"
+msgstr "Standard-Hash-Typ für neue/aktualisierte Kennwörter"
 
 msgid "Delete Account"
 msgstr "Nutzerkontolöschung"
 
 msgid "Delete Log"
 msgstr "Lösche Protokoll"
 
 msgid "Delete account"
 msgstr "Nutzerkonto löschen"
 
 msgid "Delete login failure log"
 msgstr "Lösche Anmeldefehlerprotokoll"
 
-msgid "Deleted %(attribute)s for %(username)s."
-msgstr "%(attribute)s für %(username)s gelöscht."
-
-msgid "Do not overwrite existing attributes"
-msgstr "Überschreiben Sie keine vorhandenen Attribute"
+msgid ""
+"Drop lock after\n"
+"            [1:]\n"
+"            seconds (0 = unlimited lock time)"
+msgstr "Aufhebung einer Sperre nach [1:] Sekunden (0 = unbegrenzte Sperrzeit)"
 
 msgid "Email"
-msgstr "Email"
+msgstr "E-Mail"
 
 msgid "Email Address"
-msgstr "Email-Adresse"
+msgstr "E-Mail-Adresse"
 
 msgid "Email Address:"
-msgstr "Email-Adresse:"
+msgstr "E-Mail-Adresse:"
 
-msgid "Email is required."
-msgstr "Email-Adresse ist erforderlich."
+msgid "Email is required"
+msgstr "E-Mail-Adresse ist erforderlich"
 
 msgid "Email:"
 msgstr "E-Mail:"
 
 msgid ""
-"Entering your email address will also enable you to reset your password if "
-"you ever forget it."
+"Entering your email address will also enable you\n"
+"                           to reset your password if you ever forget it."
 msgstr ""
-"Das Eintragen Ihrer Email-Adresse ermöglicht es Ihnen ausserdem, Ihr "
+"Das Eintragen Ihrer E-Mail-Adresse ermöglicht es Ihnen ausserdem, Ihr "
 "Kennwort zurückzusetzen, falls Sie es jemals vergessen sollten."
 
+msgid ""
+"Entering your email address will enable you to\n"
+"                           reset your password if you ever forget it."
+msgstr ""
+"Das Eintragen Ihrer E-Mail-Adresse ermöglicht es Ihnen, Ihr Kennwort "
+"zurückzusetzen, falls Sie es jemals vergessen sollten."
+
 msgid "Error"
 msgstr "Fehler"
 
-msgid "Error raised while sending a change notification."
+msgid ""
+"Error while reading configuration -\n"
+"                              Hint: Enable/install the required component."
 msgstr ""
-"Beim Senden einer Änderungsbenachrichtigung ist ein Fehler aufgetreten."
+"Fehler beim Lesen der Einstellungen - Hinweis: Aktivieren/installieren Sie "
+"erforderliche Komponenten."
+
+msgid ""
+"Extend user account lock time incrementally. This is\n"
+"              based on logarithmic calculation and decimal numbers "
+"accepted:\n"
+"              Value '1' means constant lock time per failed login attempt.\n"
+"              Value '2' means double locktime after 2nd lock activation,\n"
+"              four times the initial locktime after 3rd, and so on."
+msgstr ""
+"Die Sperrzeit wird schrittweise verlängert. Dies basiert auf einer "
+"logarithmischen Berechnung, die auch Dezimalzahlen nutzen kann: Wert '1' "
+"bedeutet konstante Sperrzeit pro Fehlversuch. Wert '2' bedeutet eine "
+"Verdopplung der Sperrzeit nach der 2. Sperrenaktivierung, eine "
+"Vervierfachung der ursprünglichen Sperrzeit nach der 3. Aktivierung, und so "
+"weiter."
 
 msgid "Failed login attempt count max:"
 msgstr "Anzahl Anmelde-Fehlversuche max.:"
 
 msgid "Failed login attempts for user %(user)s deleted"
 msgstr "Fehlgeschlagene Anmeldeversuche für Nutzer %(user)s gelöscht"
 
-msgid "Failed to save new login data to a password store."
-msgstr ""
-"Neue Anmeldedaten konnten nicht in einem Passwortspeicher gespeichert werden."
-
 msgid "Force users to change passwords after a password reset."
 msgstr "Zwinge Nutzer nach Zurücksetzen des Kennworts zur Kennwortänderung."
 
 msgid "Force users to verify their email addresses."
-msgstr "Zwinge Nutzer, ihre Email-Adresse zu bestätigen."
+msgstr "Zwinge Nutzer, ihre E-Mail-Adresse zu bestätigen."
 
 msgid "Forgot your password?"
 msgstr "Kennwort vergessen?"
 
 msgid "Get notified of account deletion"
 msgstr "Benutzerkontenlöschung melden"
 
 msgid "Get notified of new account creation"
 msgstr "Erstellung eines neuen Benutzerkontos melden"
 
 msgid "Get notified of password reset"
 msgstr "Kennwortrücksetzen melden"
 
-msgid "Go back"
-msgstr "Geh zurück"
-
 msgid "IP address"
 msgstr "IP-Adresse"
 
-msgid "Initial Trac authentication setup launched."
-msgstr "Ersteinrichtung der Trac-Authentifizierung gestartet."
+msgid "IPasswordHashMethod used to create new/updated passwords"
+msgstr "IPasswordHashMethod für neue/aktualisierte Kennwörter"
+
+msgid ""
+"If you've forgotten your password, enter your username and\n"
+"        email address below and you'll be emailed a new password."
+msgstr ""
+"Falls Sie Ihr Kennwort vergessen haben, dann tragen Sie bitte Ihren "
+"Nutzernamen und Ihre E-Mail-Adresse nachfolgend ein, und Sie erhalten  per E-"
+"Mail ein neues Kennwort."
+
+msgid "Invalid key type (%s) for StoreOrder"
+msgstr "Ungültiger Schlüsseltyp (%s) für Kennwortspeicherreihenfolge"
 
 msgid "Invalid username or password"
-msgstr "Nutzername oder Passwort ungültig"
+msgstr "Nutzername oder Kennwort ungültig"
 
 msgid "Invalid verification token"
 msgstr "Ungültiger Bestätigungscode"
 
 msgid "Last Login"
 msgstr "Letzte Anmeldung"
 
 msgid "Last login: %(time)s"
 msgstr "Letzte Anmeldung: %(time)s"
 
-msgid "Leave old login data"
-msgstr "Heutige Anmeldedaten belassen"
+msgid ""
+"Lock condition has been met\n"
+"                    %(count)s time by now."
+msgid_plural ""
+"Lock condition has been met\n"
+"                    %(count)s times by now."
+msgstr[0] "Sperrbedingung wurde bisher einmal erreicht."
+msgstr[1] "Sperrbedingung wurde bisher %(count)s mal erreicht."
 
 msgid "Lock condition has not been met yet."
 msgstr "Bisher wurde die Sperrbedingung nicht erreicht."
 
 msgid "Lock time progression factor:"
 msgstr "Sperrzeitverlängerungsfaktor:"
 
+msgid ""
+"Lock user account after specified number of failed attempts.\n"
+"              Value zero means 'no limit'."
+msgstr ""
+"Nutzerkontensperrung erfolgt nach angegebener Anzahl von Fehlversuchen. Wert "
+"Null bedeutet 'unbegrenzt'."
+
 msgid "Locked until %(t_release)s"
 msgstr "gesperrt bis %(t_release)s"
 
 msgid "Log time"
 msgstr "Protokollzeit"
 
 msgid "Login"
 msgstr "Anmelden"
 
 msgid "Login after %(attempts)s failed attempt"
 msgid_plural "Login after %(attempts)s failed attempts"
 msgstr[0] "Anmeldung nach %(attempts)s Fehlversuch"
 msgstr[1] "Anmeldung nach %(attempts)s Fehlversuchen"
 
+msgid "Manage User Accounts"
+msgstr "Benutzerkontenverwaltung"
+
+msgid ""
+"Max accounts per page\n"
+"          [1:]"
+msgstr "Nutzerkonten pro Seite maximal: [1:]"
+
 msgid "Name"
 msgstr "Name"
 
 msgid "Name:"
 msgstr "Name:"
 
+msgid ""
+"Neither are \"sha2\" hash algorithms supported by the\n"
+"                    \"crypt\" module on this platform nor is \"passlib\"\n"
+"                    available."
+msgstr ""
+"Weder unterstützt das \"crypt\"-Modul ist auf diesem System \"sha2\" "
+"Hashtypen noch ist \"passlib\" verfügbar."
+
 msgid "New Password:"
 msgstr "Neues Kennwort:"
 
-msgid "Next"
-msgstr "Folgende"
-
 msgid "Next Page"
 msgstr "Nächste Seite"
 
+msgid "No check method 'validate_registration' defined in %(module)s"
+msgstr "Keine Prüfmethode 'validate_registration' in %(module)s definiert"
+
 msgid "No constraints are set for this account."
 msgstr "Für dieses Nutzerkonto sind keine Beschränkungen festgelegt."
 
 msgid "No email address is registered for this account."
-msgstr "Für dieses Nutzerkonto ist keine Email-Adresse eingetragen."
+msgstr "Für dieses Nutzerkonto ist keine E-Mail-Adresse eingetragen."
 
 msgid ""
-"None of the IPasswordStore components listed in the trac.ini supports "
-"setting the password or creating users."
+"No store provides credentials for this user,\n"
+"              so the user currently can't be authenticated and\n"
+"              access to this [1:account is effectively blocked],\n"
+"              while account details may still be available."
+msgstr ""
+"Kein Register bietet Identitätsmerkmale für diesen Nutzer an, daher kann der "
+"Nutzer momentan nicht beglaubigt werden, und der Zugang zu diesem [1:"
+"Benutzerkonto ist praktisch gesperrt], während Nutzerkontendetails weiterhin "
+"verfügbar sein können."
+
+msgid ""
+"None of the IPasswordStore components listed in the\n"
+"                trac.ini supports setting the password or creating users.\n"
+"                "
 msgstr ""
 "Keine der in trac.ini aufgeführten IPasswordStore-Komponenten erlaubt das "
 "Festlegen des Kennworts oder das Erstellen neuer Nutzer."
 
-msgid "None of the configured password stores is writable."
-msgstr "Keiner der konfigurierten Kennwortspeicher ist beschreibbar."
+msgid "Not Authenticated Accounts"
+msgstr "Nicht authentifizierte Nutzerkonten"
 
 msgid "Notification"
 msgstr "Benachrichtigung"
 
 msgid "Notification Actions"
 msgstr "Benachrichtigungsaktionen"
 
 msgid "Notification Recipient Addresses"
 msgstr "Empfängeradressen für Benachrichtigungen"
 
-msgid "Objective for setting Authentication Options"
-msgstr "Ziel für die Einstellung von Authentifizierungsoptionen"
+msgid "Old Password cannot be empty."
+msgstr "Das alte Kennwort darf nicht leer sein."
+
+msgid "Old Password is incorrect."
+msgstr "Das alte Kennwort ist ungültig."
 
 msgid "Old Password:"
 msgstr "Altes Kennwort:"
 
 msgid "Only lowercase usernames allowed"
 msgstr "Nur Kleinschreibung für Nutzernamen zulässig"
 
 msgid "Optional"
 msgstr "Optional"
 
+msgid "Ordered list of password stores, queried in turn."
+msgstr ""
+"Geordnete Liste von Kennwortspeichern, die nacheinander abgefragt werden."
+
 msgid "Parole:"
 msgstr "Code:"
 
 msgid "Password"
 msgstr "Kennwort"
 
+msgid "Password Refresh"
+msgstr "Kennwortaktualisierung"
+
 msgid "Password Reset"
 msgstr "Kennwort zurücksetzen"
 
 msgid "Password cannot be empty."
 msgstr "Kennwort darf nicht leer sein."
 
 msgid "Password hash refresh procedure restarted."
 msgstr "Das Rücksetzen von Kennwörtern ist neu gestartet."
 
 msgid "Password is incorrect."
-msgstr "Das Passwort is ungültig."
+msgstr "Das Kennwort is ungültig."
 
-msgid "Password must not match old password."
-msgstr "Passwort darf nicht mit altem Passwort übereinstimmen."
+msgid "Password successfully updated."
+msgstr "Das Kennwort wurde erfolgreich aktualisiert."
 
-msgid "Password reset for %(accounts)s."
-msgstr "Zurücksetzen des Passworts für %(accounts)s."
+msgid "Password:"
+msgstr "Kennwort:"
 
-msgid "Password reset is a required action, but disabled yet."
+msgid ""
+"Path relative to Trac environment or full host machine\n"
+"                path to password file"
 msgstr ""
-"Das Zurücksetzen des Passworts ist eine erforderliche Aktion, aber noch "
-"deaktiviert."
+"Pfad relativ zur Trac-Umgebung oder vollständiger Verzeichnispfad zur "
+"Kennwortdatei"
 
-msgid "Password:"
-msgstr "Kennwort:"
+msgid ""
+"Path to the users file; leave blank to locate\n"
+"                the users file by reading svnserve.conf"
+msgstr ""
+"Pfad zur Nutzerdatei; zum Lesen der Nutzerdatei aus svnserve.conf freilassen"
 
 msgid "Permanently locked"
 msgstr "dauerhaft gesperrt"
 
-msgid "Please answer above: %(question)s"
-msgstr "Bitte antworten Sie oben: %(Frage)s"
+msgid "Persistent Sessions"
+msgstr "Dauerhafte Anmeldungen"
+
+msgid "Please change your password now."
+msgstr "Bitte ändern Sie jetzt Ihr Kennwort."
+
+msgid "Please choose account by username from list to proceed."
+msgstr ""
+"Zum Fortfahren bitte Nutzerkonto nach Benutzernamen aus der Liste auswählen."
 
 msgid "Please log in to finish email verification procedure."
 msgstr ""
 "Bitte melden Sie sich an, um den Bestätigungsvorgang für Ihre E-Mail-Adresse "
 "abzuschliessen."
 
 msgid ""
-"Please type [%(token)s] as verification token, exactly replicating "
-"everything within the braces."
+"Please type [%(token)s] as verification token,\n"
+"                exactly replicating everything within the braces."
 msgstr ""
 "Bitte tragen Sie [%(token)s] als Bestätigungscode ein, exakt wie zwischen "
 "den Klammern angegeben."
 
-msgid ""
-"Policy prohibits choosing %(username)s for an anonymous session because it's "
-"a registered username. Please login or choose another author name."
-msgstr ""
-"Die Richtlinie verbietet die Auswahl von %(username)s für eine anonyme "
-"Sitzung, weil Es ist ein registrierter Benutzername. Bitte melden Sie sich "
-"an oder wählen Sie einen anderen Autorennamen."
-
 msgid "Pre-/Surname (Nickname)"
 msgstr "Vor-/Nachname (Pseudonym)"
 
 msgid "Pre-/Surname (Nickname):"
 msgstr "Vor-/Nachname (Pseudonym):"
 
 msgid "Previous Page"
 msgstr "Vorige Seite"
 
-msgid "Provider-agnostic Authentication Options"
-msgstr "Anbieterunabhängige Authentifizierungsoptionen"
+msgid "Realm to select relevant htdigest db entries"
+msgstr "Namensraum (realm) zur Auswahl zutreffender HtDigest-Datenbankeinträge"
+
+msgid "Realm to select relevant htdigest file entries"
+msgstr ""
+"Namensraum (realm) zur Auswahl zutreffender Einträge aus HtDigest-Datei"
 
 msgid "Register"
 msgstr "Registrieren"
 
 msgid "Register an account"
 msgstr "Nutzerkonto registrieren"
 
 msgid "Registration Error"
 msgstr "Registrierungsfehler"
 
 msgid ""
-"Registration has been finished successfully. You may log in as user %(user)s "
-"now."
+"Registration has been finished successfully.\n"
+"                     You may log in as user %(user)s now."
 msgstr ""
 "Die Registrierung ist erfolgreich abgeschlossen worden. Sie können sich nun "
 "als Nutzer %(user)s anmelden."
 
 msgid "Release account lock"
 msgstr "Hebe Nutzerkontensperre auf"
 
 msgid "Remember me"
 msgstr "Angemeldet bleiben"
 
+msgid "Remove selected accounts"
+msgstr "Ausgewählte Nutzerkonten löschen"
+
 msgid "Remove selected entries"
 msgstr "Ausgewählte Einträge löschen"
 
-msgid "Removing the old user is not supported by %(store)s."
-msgstr ""
-"Das Entfernen des alten Benutzers wird von %(store)s nicht unterstützt."
-
 msgid "Required"
 msgstr "Erforderlich"
 
-msgid "Required, if the Trac instance is only accessible through HTTPS."
-msgstr "Erforderlich, wenn die Trac-Instanz nur über HTTPS erreichbar ist."
-
 msgid "Resend Email"
-msgstr "Email-Nachricht erneut versenden"
+msgstr "E-Mail-Nachricht erneut versenden"
 
 msgid "Reset Password"
 msgstr "Kennwort zurücksetzen"
 
 msgid "Reset password"
 msgstr "Kennwort zurücksetzen"
 
 msgid "Reset passwords"
 msgstr "Kennwörter zurücksetzen"
 
 msgid "Restart"
 msgstr "Neustart"
 
-msgid "Restrict sending cookies to HTTPS connections."
-msgstr "Beschränken Sie das Senden von Cookies auf HTTPS-Verbindungen."
+msgid "Review User Account Details"
+msgstr "Benutzerkontendetailprüfung"
 
 msgid "Review account attributes"
 msgstr "Nutzerkonteneigenschaftenprüfung"
 
+msgid "Save"
+msgstr "Speichern"
+
 msgid "Send another random password"
 msgstr "Versende anderes Zufallskennwort"
 
+msgid ""
+"Set the following options in order to be notified of\n"
+"          account creation, password reset and account deletion."
+msgstr ""
+"Wählen Sie die folgenden Optionen, um über Kontenerstellung, "
+"Kennwortrücksetzen und Kontenlöschung benachrichtigt zu werden."
+
 msgid "Silently update password hashes on next successful login."
 msgstr ""
 "Aktualisiere die Kennwort-Hash-Werte bei der nächsten erfolgreichen "
 "Anmeldung."
 
-msgid "Skip creating account and password reset"
-msgstr ""
-"Überspringen Sie das Erstellen eines Kontos und das Zurücksetzen des "
-"Passworts"
-
 msgid "Skip new email verification"
-msgstr "Bestätigung neuer Email-Adresse auslassen"
+msgstr "Bestätigung neuer E-Mail-Adresse auslassen"
 
 msgid ""
-"Sorry, but policy prohibits choosing '%(username)s' for an anonymous "
-"session. Login or choose another session ID, please."
+"Space-separated list of email addresses and/or\n"
+"          usernames that get notified of the above actions:"
 msgstr ""
-"Entschuldigung, aber die Richtlinie verbietet die Auswahl von '%(username)s' "
-"für einen anonymen Sitzung. Melden Sie sich an oder wählen Sie bitte eine "
-"andere Session-ID."
+"Liste von durch Leerzeichen getrennten E-Mail-Adressen und/oder Nutzernamen, "
+"die über die vorgenannten Aktionen benachrichtigt werden:"
 
-msgid "Step %(step)s: %(label)s"
-msgstr "Schritt %(step)s: %(label)s"
+msgid "Successfully deleted:"
+msgstr "Erfolgreich gelöscht:"
 
-msgid "Table %(table)s column %(column)s%(constraint)s: %(result)s change"
-msgid_plural ""
-"Table %(table)s column %(column)s%(constraint)s: %(result)s changes"
-msgstr[0] "Table %(table)s column %(column)s%(constraint)s: %(result)s change"
-msgstr[1] "Table %(table)s column %(column)s%(constraint)s: %(result)s changes"
+msgid "Successfully updated: %(success)s"
+msgstr "Erfolgreich aktualisiert: %(success)s"
 
 msgid "Table: Last failed login attempts log view"
 msgstr "Tabelle: Protokoll der letzten fehlgeschlagenen Anmeldeversuche"
 
 msgid "Thank you for taking the time to update your password."
 msgstr ""
-"Danke, dass Sie sich die Zeit genommen haben, Ihr Passwort zu aktualisieren."
+"Danke, dass Sie sich die Zeit genommen haben, Ihr Kennwort zu aktualisieren."
 
 msgid "Thank you for verifying your email address."
-msgstr "Vielen Dank, dass Sie Ihre Email-Adresse bestätigt haben."
+msgstr "Vielen Dank, dass Sie Ihre E-Mail-Adresse bestätigt haben."
 
 msgid ""
-"The authentication backend for user %(user)s does not support setting the "
-"password."
+"The \"crypt\" module is unavailable\n"
+"                                    on this platform."
+msgstr "Das \"crypt\"-Modul ist auf diesem System nicht verfügbar."
+
+msgid ""
+"The authentication backend for user %s does not support\n"
+"                setting the password.\n"
+"                "
 msgstr ""
-"Der Authentifikationsdienst für den Nutzer %(user)s erlaubt das Festlegen "
-"des Kennworts nicht."
+"Der Authentifikationsdienst für den Nutzer %s erlaubt das Festlegen des "
+"Kennworts nicht."
 
 msgid ""
-"The email address is required for Trac to send you a verification token."
+"The email address is required for Trac to send\n"
+"                           you a verification token."
 msgstr ""
-"Ihre Email-Adresse wird benötigt, damit Trac Ihnen einen Bestätigungscode "
+"Ihre E-Mail-Adresse wird benötigt, damit Trac Ihnen einen Bestätigungscode "
 "zusenden kann."
 
 msgid ""
 "The email address specified appears to be invalid. Please specify a valid "
 "email address."
 msgstr ""
-"Die angegebene Email-Adresse scheint ungültig zu sein. Bitte geben Sie eine "
-"gültige Email-Adresse an."
+"Die angegebene E-Mail-Adresse scheint ungültig zu sein. Bitte geben Sie eine "
+"gültige E-Mail-Adresse an."
 
 msgid ""
 "The email address specified is already in use. Please specify a different "
 "one."
 msgstr ""
-"Die angegebene Email-Adresse wird bereits verwendet. Bitte geben Sie eine "
+"Die angegebene E-Mail-Adresse wird bereits verwendet. Bitte geben Sie eine "
 "andere an."
 
+msgid "The email and username do not match a known account."
+msgstr ""
+"E-Mail-Adresse und Nutzername gehören zu keinem bekannten Benutzerkonto."
+
+msgid "The email and username must match a known account."
+msgstr ""
+"E-Mail-Adresse und Nutzername müssen zu einem bekannten Benutzerkonto "
+"gehören."
+
 msgid ""
-"The password file could not be read. Trac requires read and write access to "
-"both the password file and its parent directory."
+"The password file could not be read. Trac requires\n"
+"                    read and write access to both the password file\n"
+"                    and its parent directory."
 msgstr ""
 "Die Kennwortdatei konnte nicht gelesen werden. Trac benötigt Lese- und "
 "Schreibzugriff sowohl auf die Kennworddatei als auch auf deren "
 "übergeordnetes Verzeichnis."
 
 msgid ""
-"The password file could not be updated. Trac requires read and write access "
-"to both the password file and its parent directory."
+"The password file could not be updated. Trac requires\n"
+"                    read and write access to both the password file\n"
+"                    and its parent directory."
 msgstr ""
 "Die Kennwortdatei konnte nicht aktualisiert werden. Trac benötigt Lese- und "
 "Schreibzugriff sowohl auf die Kennworddatei als auch auf deren "
 "übergeordnetes Verzeichnis."
 
 msgid "The password reset procedure is not enabled."
 msgstr "Das Rücksetzen von Kennwörtern ist nicht aktiviert."
 
+msgid ""
+"The password store does not support\n"
+"                                changing passwords.\n"
+"                                "
+msgstr "Der Kennwortspeicher erlaubt das Löschen von Nutzern nicht."
+
+msgid "The password store does not support creating users."
+msgstr "Der Kennwortspeicher erlaubt das Auflisten von Nutzern nicht."
+
 msgid "The password store does not support deleting users."
 msgstr "Der Kennwortspeicher erlaubt das Auflisten von Nutzern nicht."
 
 msgid "The passwords must match."
 msgstr "Die Kennwörter müssen übereinstimmen."
 
 msgid "The user has not logged in before."
 msgstr "Der Nutzer hat sich bisher nicht angemeldet."
 
-msgid "The username must not contain any of these characters: %(chars)s"
-msgstr "Der Nutzername darf keines der folgenden Zeichen enthalten: %(chars)s"
+msgid "The username must not contain any of these characters: %s"
+msgstr "Der Nutzername darf keines der folgenden Zeichen enthalten: %s"
 
 msgid "There is currently no failed login attempt logged."
 msgstr "Aktuell ist kein fehlgeschlagener Anmeldeversuch protokolliert."
 
+msgid ""
+"Therefore after another failed login attempt authentication\n"
+"                  for this account would be retarded by %(time)s."
+msgstr ""
+"Deshalb würde die Anmeldung für dieses Benutzerkonto nach einem weiteren "
+"Fehlversuch um %(time)s verzögert."
+
 msgid "This account has been locked permanently."
 msgstr "Dieses Nutzerkonto ist dauerhaft gesperrt worden."
 
 msgid "This address has been verified successfully."
 msgstr "Diese Adresse ist erfolgreich bestätigt worden."
 
 msgid "This address has not been verified yet."
 msgstr "Diese Adresse ist bisher noch nicht bestätigt worden."
 
+msgid ""
+"This is a list of actions which you can\n"
+"          enable or disable by [1:checking] the [2:checkboxes]."
+msgstr ""
+"Dies ist eine Aktionsliste, die Sie durch [1:Wählen] der [2:Ankreuzfelder] "
+"aktivieren oder deaktivieren können."
+
+msgid ""
+"This is, user checks a \"Remember Me\"\n"
+"          [1:checkbox] and, next time he visits the site within\n"
+"          30 days, he'll be remembered and automatically authenticated."
+msgstr ""
+"D. h., der Nutzer aktiviert ein [1:Ankreuzfeld] \"Angemeldet bleiben\" und "
+"wird beim nächsten Besuch innerhalb von 30 Tagen wiedererkannt und "
+"automatisch angemeldet."
+
 msgid "This password store does not support listing users."
 msgstr "Der Kennwortspeicher erlaubt das Auflisten von Nutzern nicht."
 
-msgid "Time lock condition has been met %(count)s time by now."
-msgid_plural "Time lock condition has been met %(count)s times by now."
-msgstr[0] "Sperrbedingung wurde bisher einmal erreicht."
-msgstr[1] "Sperrbedingung wurde bisher %(count)s mal erreicht."
-
 msgid "Total failed attempts: %(count)s"
 msgstr "Fehlversuche gesamt: %(count)s"
 
+msgid "URL of the HTTP authentication service"
+msgstr "URL des HTTP-Authentifizierungsdienstes"
+
 msgid "Undo selection"
 msgstr "Auswahl aufheben"
 
+msgid "Unknown user %(user)s."
+msgstr "Nutzer %(user)s ist unbekannt."
+
 msgid "Unlock"
 msgstr "Nutzerkonto entsperren"
 
-msgid ""
-"Unsupported db schema version, please update %(plugin)s to a recent version."
-msgstr ""
-"Nicht unterstützte Database-Schema-Version, bitte aktualisieren Sie "
-"%(plugin)s auf eine neuere Ausführung."
-
 msgid "Update"
 msgstr "Aktualisieren"
 
-msgid "Update error in table %(table)s: %(message)s"
-msgstr "Aktualisierungsfehler in Tabelle %(table)s: %(message)s"
-
-msgid "Updated %(attributes)s for %(username)s."
-msgstr "%(attributes)s für %(username)s aktualisiert."
-
-msgid "User ID change requires additional components enabled"
+msgid ""
+"Upper lock time limit:\n"
+"              [1:]\n"
+"              seconds\n"
+"              [2:\n"
+"                This is relevant only with a lock time progression factor > "
+"1.\n"
+"              ]"
 msgstr ""
-"Für die Änderung der Benutzer-ID müssen zusätzliche Komponenten aktiviert "
-"werden"
+"Sperrzeitobergrenze: [1:] Sekunden [2:Dies ist nur bei einem "
+"Sperrzeitverlängerungsfaktor > 1 von Bedeutung.]"
 
-msgid "Username %(username)s doesn't match local naming policy."
-msgstr ""
-"Der Nutzername %(username)s entspricht nicht den hier geltenden Regeln."
+msgid "Username %s doesn't match local naming policy."
+msgstr "Der Nutzername %s entspricht nicht den hier geltenden Regeln."
 
-msgid "Username %(username)s is not allowed."
-msgstr "Der Nutzername %(username)s ist nicht zugelassen."
+msgid "Username %s is not allowed."
+msgstr "Der Nutzername %s ist nicht zugelassen."
 
 msgid "Username cannot be empty."
 msgstr "Nutzername darf nicht leer sein."
 
-msgid "Username is required."
-msgstr "Nutzername ist erforderlich."
+msgid "Username is required"
+msgstr "Nutzername ist erforderlich"
 
 msgid "Username matching is set to [1:case-sensitive]."
 msgstr "Nutzernamesvergleich beachtet [1:Groß-/Kleinschreibung]."
 
 msgid "Username matching is set to [1:not case-sensitive]."
 msgstr "Nutzernamesvergleich beachtet [1:Groß-/Kleinschreibung nicht]."
 
@@ -683,79 +782,91 @@
 
 msgid "Users"
 msgstr "Nutzer"
 
 msgid "Value"
 msgstr "Wert"
 
+msgid "Verification"
+msgstr "Bestätigung"
+
 msgid "Verification Token:"
 msgstr "Bestätigungscode:"
 
+msgid ""
+"Verification is pending\n"
+"                  ([1:token: '%(token)s' ])."
+msgstr "Die Bestätigung ist offen ([1:Code: '%(token)s' ])."
+
 msgid "Verify"
 msgstr "Bestätigen"
 
 msgid "Verify Email"
-msgstr "Email-Adresse bestätigen"
-
-msgid "You must specify a valid email address."
-msgstr "Sie müssen eine gültige Email-Adresse angeben."
+msgstr "E-Mail-Adresse bestätigen"
 
-msgid "You should report that issue to a Trac admin."
-msgstr "Sie sollten dieses Problem einem Trac-Administrator melden."
-
-msgid "You'll get details with TracLogging enabled."
-msgstr "Sie erhalten Details mit aktiviertem TracLogging."
+msgid "Verify email"
+msgstr "E-Mail-Adresse bestätigen"
 
 msgid ""
-"Your changes are cached until you either drop or save them all (see last "
-"step)."
+"You are required to change password because of a recent password change "
+"request. "
 msgstr ""
-"Ihre Änderungen werden zwischengespeichert, bis Sie sie entweder löschen "
-"oder alle speichern (siehe letztes Schritt)."
+"Sie müssen Ihr Kennwort wegen einer kürzlich angeforderten Kennwortänderung "
+"ändern. "
 
-msgid "Your changes have been saved."
-msgstr "Ihre Änderungen wurden gespeichert."
+msgid ""
+"You can [1:change your\n"
+"        email address], if it is incorrect."
+msgstr "Sie können [1: Ihre E-Mail-Adresse ändern], falls sie fehlerhaft ist."
 
-msgid "Your email is already verified."
-msgstr "Ihre Email-Adresse ist bereits bestätigt."
+msgid "You must specify a valid email address."
+msgstr "Sie müssen eine gültige E-Mail-Adresse angeben."
 
 msgid ""
-"Your username has been registered successfully, but your account requires "
-"administrative approval. Please proceed according to local policy."
+"You're already logged in. If you need to change\n"
+"          your password please use the\n"
+"          [1:Account Preferences] page."
 msgstr ""
-"Ihr Benutzername wurde erfolgreich registriert, aber Ihr Konto "
-"erfordertBehördliche Genehmigung. Bitte fahren Sie gemäß den örtlichen "
-"Richtlinien fort."
+"Sie sind bereits angemeldet. Falls Sie Ihr Kennwort ändern möchten, benutzen "
+"Sie bitte die Seite für [1:Nutzerkonto-Einstellungen]."
+
+msgid "Your email is already verified."
+msgstr "Ihre E-Mail-Adresse ist bereits bestätigt."
+
+msgid "Your permissions have been limited until you %(link)s."
+msgstr "Ihre Berechtigungen sind eingeschränkt worden, bis Sie %(link)s."
 
 msgid ""
-"Your username has been successfully registered but your account still "
-"requires activation. Please login as user %(user)s, and follow the "
-"instructions."
+"Your username has been successfully registered but\n"
+"                        your account still requires activation. Please "
+"login\n"
+"                        as user %(user)s, and follow the instructions."
 msgstr ""
 "Ihr Nutzername wurde erfolgreich registriert, aber Ihr Konto muss noch "
 "aktiviert werden. Bitte melden Sie sich als Nutzer %(user)s an und folgen "
 "Sie den Anweisungen."
 
-msgid "[%(section)s] %(name)s option for the password file is not configured"
+msgid ""
+"[1:]\n"
+"                This account has been locked until %(time)s[2:]\n"
+"                and even valid login attempts are rejected meanwhile."
 msgstr ""
-"[%(section)s] %(name)s-Option für die Passwortdatei ist nicht konfiguriert"
-
-msgid "email unverified"
-msgstr "Email unbestätigt"
+"[1:] Dieses Nutzerkonto ist bis %(time)s gesperrt worden,[2:] und auch "
+"gültige Anmeldeversuche werden bis dahin abgewiesen."
 
 msgid "for [1:%(name)s] ([2:%(user)s])"
 msgstr "für [1:%(name)s] ([2:%(user)s])"
 
 msgid "for [1:%(user)s]"
 msgstr "für [1:%(user)s]"
 
 msgid "less than %s"
 msgstr "weniger als %s"
 
 msgid "page %(num)s"
 msgstr "Seite %(num)s"
 
-msgid "pending approval"
-msgstr "Genehmigung ausstehend"
+msgid "verify your email address"
+msgstr "Ihre E-Mail-Adresse bestätigen"
 
-msgid "revoked"
-msgstr "widerrufen"
+msgid "verify your new email address"
+msgstr "Ihre neue E-Mail-Adresse zu bestätigen"
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/locale/fr/LC_MESSAGES/acct_mgr.po` & `TracAccountManager-0.6.dev0/acct_mgr/locale/messages.pot`

 * *Files 26% similar despite different names*

```diff
@@ -1,2253 +1,2050 @@
-# French (France) translations for TracAccountManager.
-# Copyright (C) 2012
+# Translations template for TracAccountManager.
+# Copyright (C) 2018 ORGANIZATION
 # This file is distributed under the same license as the
 # TracAccountManager project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2018.
 #
-# Translators:
-# Sukender (Benoit NEIL) <sukender at free dot fr>
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: TracAccountManager 0.6\n"
+"Project-Id-Version: TracAccountManager 0.5.1\n"
 "Report-Msgid-Bugs-To: hoff.st@shaas.net\n"
-"POT-Creation-Date: 2023-04-09 21:49+0000\n"
-"PO-Revision-Date: 2012-09-16 19:02+0000\n"
-"Last-Translator: Sukender (Benoit NEIL) <sukender at free dot fr>\n"
-"Language: fr\n"
-"Language-Team: French <trac-dev@googlegroups.com>\n"
-"Plural-Forms: nplurals=2; plural=(n > 1)\n"
+"POT-Creation-Date: 2018-06-21 22:46-0700\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.6.0\n"
 
-#: acct_mgr/admin.py:58
+#: acct_mgr/admin.py:59
 #, python-format
 msgid "Locked until %(t_release)s"
 msgstr ""
 
-#: acct_mgr/admin.py:213 acct_mgr/admin.py:892 acct_mgr/notification.py:197
-#: acct_mgr/templates/genshi/account_users.html:11
-#: acct_mgr/templates/jinja2/account_users.html:7
+#: acct_mgr/admin.py:171
+#, python-format
+msgid "Invalid key type (%s) for ExtensionOrder"
+msgstr ""
+
+#: acct_mgr/admin.py:214 acct_mgr/admin.py:901 acct_mgr/notification.py:192
+#: acct_mgr/templates/account_users.html:14
+#: acct_mgr/templates/account_users.html:158
 msgid "Accounts"
-msgstr "Comptes"
+msgstr ""
 
-#: acct_mgr/admin.py:213
+#: acct_mgr/admin.py:214
 msgid "Users"
-msgstr "Utilisateurs"
+msgstr ""
 
-#: acct_mgr/admin.py:288
+#: acct_mgr/admin.py:290
 #, python-format
 msgid "%(count)s account"
 msgid_plural "%(count)s accounts"
 msgstr[0] ""
 msgstr[1] ""
 
-#: acct_mgr/admin.py:293
+#: acct_mgr/admin.py:297
 #, python-format
 msgid "%(count)s account attribute"
 msgid_plural "%(count)s account attributes"
 msgstr[0] ""
 msgstr[1] ""
 
-#: acct_mgr/admin.py:298
+#: acct_mgr/admin.py:303
 #, python-format
 msgid "Successfully deleted: %(account)s"
 msgstr ""
 
-#: acct_mgr/admin.py:310
-#, fuzzy
+#: acct_mgr/admin.py:316
 msgid "Back to Account"
-msgstr "Créer compte"
+msgstr ""
 
-#: acct_mgr/admin.py:313 acct_mgr/admin.py:537
-#, fuzzy
+#: acct_mgr/admin.py:319 acct_mgr/admin.py:546
 msgid "Back to Accounts"
-msgstr "Créer compte"
+msgstr ""
 
-#: acct_mgr/admin.py:326
+#: acct_mgr/admin.py:333
 msgid "Please choose account by username from the list to proceed."
 msgstr ""
 
-#: acct_mgr/admin.py:356
+#: acct_mgr/admin.py:363
 msgid "Email Address"
-msgstr "Adresse email"
+msgstr ""
 
-#: acct_mgr/admin.py:357
+#: acct_mgr/admin.py:364
 msgid "Pre-/Surname (Nickname)"
 msgstr ""
 
-#: acct_mgr/admin.py:358
+#: acct_mgr/admin.py:365
 msgid "Password"
-msgstr "Mot de passe"
+msgstr ""
 
-#: acct_mgr/admin.py:374 acct_mgr/admin.py:380
+#: acct_mgr/admin.py:382 acct_mgr/admin.py:389
 #, python-format
 msgid "Deleted %(attribute)s for %(username)s."
 msgstr ""
 
-#: acct_mgr/admin.py:385 acct_mgr/register.py:121 acct_mgr/web_ui.py:278
+#: acct_mgr/admin.py:394 acct_mgr/register.py:122 acct_mgr/web_ui.py:278
 msgid "The passwords must match."
-msgstr "Les mots de passe doivent correspondre."
+msgstr ""
 
-#: acct_mgr/admin.py:419
+#: acct_mgr/admin.py:428
 #, python-format
 msgid "Updated %(attributes)s for %(username)s."
 msgstr ""
 
-#: acct_mgr/admin.py:431
+#: acct_mgr/admin.py:441
 #, python-format
 msgid "Update error in table %(table)s: %(message)s"
 msgstr ""
 
-#: acct_mgr/admin.py:446
+#: acct_mgr/admin.py:455
 #, python-format
 msgid "Table %(table)s column %(column)s%(constraint)s: %(result)s change"
 msgid_plural "Table %(table)s column %(column)s%(constraint)s: %(result)s changes"
 msgstr[0] ""
 msgstr[1] ""
 
-#: acct_mgr/admin.py:494
+#: acct_mgr/admin.py:504
 #, python-format
 msgid "Account lock (%(condition)s) for user %(user)s cleared"
 msgstr ""
 
-#: acct_mgr/admin.py:500
+#: acct_mgr/admin.py:510
 #, python-format
 msgid "Failed login attempts for user %(user)s deleted"
 msgstr ""
 
 #. TRANSLATOR: Optionally tabbed account editor's label
-#: acct_mgr/admin.py:528
+#: acct_mgr/admin.py:537
 msgid "Modify Account"
 msgstr ""
 
-#: acct_mgr/admin.py:530
-#, fuzzy
+#: acct_mgr/admin.py:539
 msgid "Change User ID"
-msgstr "Changer de mot de passe"
+msgstr ""
 
-#: acct_mgr/admin.py:534
+#: acct_mgr/admin.py:543
 msgid "Account Attributes"
 msgstr ""
 
-#: acct_mgr/admin.py:621
+#: acct_mgr/admin.py:630
 #, python-format
 msgid "Password reset for %(accounts)s."
 msgstr ""
 
-#: acct_mgr/admin.py:623
+#: acct_mgr/admin.py:632
 msgid "The password reset procedure is not enabled."
 msgstr ""
 
-#: acct_mgr/admin.py:633
-#, fuzzy, python-format
+#: acct_mgr/admin.py:642
+#, python-format
 msgid "Deleted account: %(accounts)s"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/admin.py:635
+#: acct_mgr/admin.py:644
 msgid "The password store does not support deleting users."
 msgstr ""
 
-#: acct_mgr/admin.py:644
+#: acct_mgr/admin.py:653
 msgid "active"
 msgstr ""
 
-#: acct_mgr/admin.py:645
+#: acct_mgr/admin.py:654
 msgid "revoked"
 msgstr ""
 
-#: acct_mgr/admin.py:646
+#: acct_mgr/admin.py:655
 msgid "pending approval"
 msgstr ""
 
-#: acct_mgr/admin.py:649
+#: acct_mgr/admin.py:658
 msgid "email unverified"
 msgstr ""
 
-#: acct_mgr/admin.py:670
-#, fuzzy
+#: acct_mgr/admin.py:679
 msgid "Are you sure you want to delete these accounts?"
-msgstr "Êtes-vous sûr(e) de vouloir supprimer votre compte ?"
+msgstr ""
 
-#: acct_mgr/admin.py:710
+#: acct_mgr/admin.py:719
 #, python-format
 msgid "Removing the old user is not supported by %(store)s."
 msgstr ""
 
-#: acct_mgr/admin.py:727 acct_mgr/admin.py:1573
+#: acct_mgr/admin.py:736 acct_mgr/admin.py:1584
 msgid "None of the configured password stores is writable."
 msgstr ""
 
-#: acct_mgr/admin.py:731
+#: acct_mgr/admin.py:740
 msgid "Password reset is a required action, but disabled yet."
 msgstr ""
 
-#: acct_mgr/admin.py:741
+#: acct_mgr/admin.py:750
 #, python-format
 msgid "At least %(required_check)s must be configured and enabled."
 msgstr ""
 
-#: acct_mgr/admin.py:772
+#: acct_mgr/admin.py:781
 msgid "Failed to save new login data to a password store."
 msgstr ""
 
-#: acct_mgr/admin.py:802
+#: acct_mgr/admin.py:811
 #, python-format
 msgid ""
-"Cannot send the new password to the user, because no email address is "
-"associated with %(username)s."
+"Cannot send the new password to the user, because no email address is"
+" associated with %(username)s."
 msgstr ""
 
-#: acct_mgr/admin.py:810 acct_mgr/admin.py:824 acct_mgr/admin.py:837
-#: acct_mgr/admin.py:1558 acct_mgr/register.py:428 acct_mgr/register.py:444
-#: acct_mgr/register.py:580 acct_mgr/register.py:614 acct_mgr/web_ui.py:355
-#: acct_mgr/web_ui.py:801
+#: acct_mgr/admin.py:819 acct_mgr/admin.py:833 acct_mgr/admin.py:846
+#: acct_mgr/admin.py:1569 acct_mgr/register.py:430 acct_mgr/register.py:447
+#: acct_mgr/register.py:588 acct_mgr/register.py:624 acct_mgr/web_ui.py:347
+#: acct_mgr/web_ui.py:810
 msgid "Error raised while sending a change notification."
 msgstr ""
 
-#: acct_mgr/admin.py:812 acct_mgr/admin.py:826 acct_mgr/admin.py:839
-#: acct_mgr/admin.py:1560 acct_mgr/web_ui.py:357
+#: acct_mgr/admin.py:821 acct_mgr/admin.py:835 acct_mgr/admin.py:848
+#: acct_mgr/admin.py:1571 acct_mgr/web_ui.py:349
 msgid "You'll get details with TracLogging enabled."
 msgstr ""
 
-#: acct_mgr/admin.py:855
+#: acct_mgr/admin.py:864
 #, python-format
 msgid "page %(num)s"
 msgstr ""
 
-#: acct_mgr/admin.py:866
+#: acct_mgr/admin.py:875
 msgid "Next Page"
 msgstr ""
 
-#: acct_mgr/admin.py:869
+#: acct_mgr/admin.py:878
 msgid "Previous Page"
 msgstr ""
 
-#: acct_mgr/admin.py:892 acct_mgr/templates/genshi/account_config.html:450
-#: acct_mgr/templates/jinja2/account_config.html:484
+#: acct_mgr/admin.py:901 acct_mgr/templates/account_config.html:438
 msgid "Configuration"
-msgstr "Configuration"
+msgstr ""
 
-#: acct_mgr/admin.py:946
+#: acct_mgr/admin.py:955
 msgid "Password hash refresh procedure restarted."
 msgstr ""
 
-#: acct_mgr/admin.py:1147
+#: acct_mgr/admin.py:1157
 msgid "Your changes have been saved."
 msgstr ""
 
-#: acct_mgr/admin.py:1150
+#: acct_mgr/admin.py:1160
 msgid ""
-"Your changes are cached until you either drop or save them all (see last "
-"step)."
+"Your changes are cached until you either drop or save them all (see "
+"last step)."
 msgstr ""
 
-#: acct_mgr/admin.py:1169
+#: acct_mgr/admin.py:1179
 msgid "Authentication Options"
 msgstr ""
 
-#: acct_mgr/admin.py:1170 acct_mgr/admin.py:1426
-#, fuzzy
+#: acct_mgr/admin.py:1180 acct_mgr/admin.py:1436
 msgid "Password Store"
-msgstr "Mot de passe incorrect."
+msgstr ""
 
-#: acct_mgr/admin.py:1171
-#, fuzzy
+#: acct_mgr/admin.py:1181
 msgid "Password Policy"
-msgstr "Mot de passe"
+msgstr ""
 
-#: acct_mgr/admin.py:1172
-#, fuzzy
+#: acct_mgr/admin.py:1182
 msgid "Account Policy"
-msgstr "Compte bloqué"
+msgstr ""
 
-#: acct_mgr/admin.py:1173 acct_mgr/admin.py:1445
-#, fuzzy
+#: acct_mgr/admin.py:1183 acct_mgr/admin.py:1455
 msgid "Account Guard"
-msgstr "Compte"
+msgstr ""
 
-#: acct_mgr/admin.py:1174
-#, fuzzy
+#: acct_mgr/admin.py:1184
 msgid "Initialization"
-msgstr "Notification"
+msgstr ""
 
-#: acct_mgr/admin.py:1218 acct_mgr/admin.py:1346
+#: acct_mgr/admin.py:1228 acct_mgr/admin.py:1356
 #, python-format
 msgid ""
 "Error while reading configuration - Hint: Enable/install required "
 "component '%s'."
 msgstr ""
 
-#: acct_mgr/admin.py:1431
+#: acct_mgr/admin.py:1441
 msgid "Password Reset"
-msgstr "Réinitialisation du mot de passe"
+msgstr ""
 
-#: acct_mgr/admin.py:1439
+#: acct_mgr/admin.py:1449
 msgid "Account Registration"
 msgstr ""
 
-#: acct_mgr/admin.py:1452
-#, fuzzy
+#: acct_mgr/admin.py:1462
 msgid "Admin user account"
-msgstr "Gestion des comptes utilisateurs"
+msgstr ""
 
-#: acct_mgr/admin.py:1456
-#, fuzzy
+#: acct_mgr/admin.py:1466
 msgid "Configuration Review"
-msgstr "Configuration"
+msgstr ""
 
-#: acct_mgr/admin.py:1531
+#: acct_mgr/admin.py:1542
 msgid "Initial Trac authentication setup launched."
 msgstr ""
 
-#: acct_mgr/admin.py:1569
+#: acct_mgr/admin.py:1580
 #, python-format
 msgid "Account %(username)s created."
 msgstr ""
 
-#: acct_mgr/api.py:264
+#: acct_mgr/api.py:256
 #, python-format
 msgid ""
-"The authentication backend for user %(user)s does not support setting the"
-" password."
+"The authentication backend for user %(user)s does not support setting"
+" the password."
 msgstr ""
 
-#: acct_mgr/api.py:281
+#: acct_mgr/api.py:273
 #, python-format
-msgid "Password for user %(user)s existed, couldn't create."
+msgid "Password for user %s existed, couldn't create."
 msgstr ""
 
-#: acct_mgr/api.py:286
+#: acct_mgr/api.py:278
 msgid ""
-"None of the IPasswordStore components listed in the trac.ini supports "
-"setting the password or creating users."
+"None of the IPasswordStore components listed in the\n"
+"                trac.ini supports setting the password or creating "
+"users.\n"
+"                "
 msgstr ""
 
-#: acct_mgr/api.py:475
-msgid "Account is pending approval. You may need to contact your administrator."
-msgstr ""
-
-#: acct_mgr/db.py:25
-msgid "IPasswordHashMethod used to create new/updated passwords"
+#: acct_mgr/api.py:468
+msgid ""
+"Account is pending approval. You may need to contact your "
+"administrator."
 msgstr ""
 
-#: acct_mgr/htfile.py:100
+#: acct_mgr/htfile.py:89
 #, python-format
 msgid "[%(section)s] %(name)s option for the password file is not configured"
 msgstr ""
 
-#: acct_mgr/htfile.py:115
+#: acct_mgr/htfile.py:140
 msgid ""
-"The password file could not be read. Trac requires read and write access "
-"to both the password file and its parent directory."
+"The password file could not be read. Trac requires\n"
+"                    read and write access to both the password file\n"
+"                    and its parent directory."
 msgstr ""
-"Le fichier de mots de pase n'est pas lisible. Trac nécessite les droits "
-"en lecture et écriture pour ce fichier et le répertoire parent."
 
-#: acct_mgr/htfile.py:165
+#: acct_mgr/htfile.py:158
 msgid ""
-"The password file could not be updated. Trac requires read and write "
-"access to both the password file and its parent directory."
-msgstr ""
-"Le fichier de mots de pase n'a pu être mis à jour. Trac nécessite les "
-"droits en lecture et écriture pour ce fichier et le répertoire parent."
-
-#: acct_mgr/htfile.py:193 acct_mgr/htfile.py:233
-msgid ""
-"Path relative to Trac environment or full host machine path to password "
-"file"
-msgstr ""
-
-#: acct_mgr/htfile.py:196
-msgid "Default hash type of new/updated passwords"
-msgstr ""
-
-#: acct_mgr/htfile.py:236
-msgid "Realm to select relevant htdigest file entries"
-msgstr ""
-
-#: acct_mgr/http.py:36
-msgid "URL of the HTTP authentication service"
+"The password file could not be updated. Trac requires\n"
+"                    read and write access to both the password file\n"
+"                    and its parent directory."
 msgstr ""
 
 #: acct_mgr/macros.py:92
 #, python-format
 msgid "(required %(perm)s missing)"
 msgstr ""
 
-#: acct_mgr/notification.py:198
+#: acct_mgr/notification.py:55
+msgid "The email and username do not match a known account."
+msgstr ""
+
+#: acct_mgr/notification.py:193
 msgid "Notification"
-msgstr "Notification"
+msgstr ""
 
-#: acct_mgr/pwhash.py:59
-msgid "Realm to select relevant htdigest db entries"
+#: acct_mgr/pwhash.py:130
+msgid "The \"crypt\" module is unavailable on this platform."
 msgstr ""
 
-#: acct_mgr/pwhash.py:197
-msgid "Neither passlib nor crypt module available"
+#: acct_mgr/pwhash.py:137
+msgid ""
+"Neither are \"sha2\" hash algorithms supported by the\n"
+"                    \"crypt\" module on this platform nor is "
+"\"passlib\"\n"
+"                    available."
 msgstr ""
 
-#: acct_mgr/register.py:35
+#: acct_mgr/register.py:36
 msgid "Registration Error"
 msgstr ""
 
-#: acct_mgr/register.py:55
+#: acct_mgr/register.py:56
 msgid ""
 "A collection of basic checks.\n"
 "\n"
 "This includes checking for\n"
 " * emptiness (no user input for username and/or password)\n"
 " * some blacklisted username characters\n"
 " * upper-cased usernames (reserved for Trac permission actions)\n"
 " * some reserved usernames\n"
 " * a username duplicate in configured password stores\n"
 "\n"
-"''This check is bypassed for requests regarding user's own preferences.''"
+"''This check is bypassed for requests regarding user's own "
+"preferences.''"
 msgstr ""
 
-#: acct_mgr/register.py:80
+#: acct_mgr/register.py:81
 msgid "Username cannot be empty."
-msgstr "Le nom d'utilisateur doit être renseigné."
+msgstr ""
 
-#: acct_mgr/register.py:89
+#: acct_mgr/register.py:90
 #, python-format
 msgid "The username must not contain any of these characters: %(chars)s"
-msgstr "Le nom d'utilisateur ne peut contenir les caractères suivants : %(chars)s"
+msgstr ""
 
-#: acct_mgr/register.py:93
+#: acct_mgr/register.py:94
 msgid "A username with only upper-cased characters is not allowed."
 msgstr ""
 
-#: acct_mgr/register.py:100
+#: acct_mgr/register.py:101
 #, python-format
 msgid "Username %(username)s is not allowed."
-msgstr "'%(username)s' n'est pas un nom d'utilisateur valide."
+msgstr ""
 
-#: acct_mgr/register.py:114 acct_mgr/register.py:343
+#: acct_mgr/register.py:115 acct_mgr/register.py:347
 #, python-format
 msgid ""
 "Another account or group already exists, who's name differs from "
 "%(username)s only by case or is identical."
 msgstr ""
 
-#: acct_mgr/register.py:119 acct_mgr/web_ui.py:276 acct_mgr/web_ui.py:295
+#: acct_mgr/register.py:120 acct_mgr/web_ui.py:276 acct_mgr/web_ui.py:295
 msgid "Password cannot be empty."
-msgstr "Le mot de passe doit être renseigné."
+msgstr ""
 
-#: acct_mgr/register.py:129
+#: acct_mgr/register.py:130
 msgid ""
 "A collection of simple bot checks.\n"
 "\n"
 "''This check is bypassed for requests by an authenticated user.''"
 msgstr ""
 
-#: acct_mgr/register.py:137
-msgid ""
-"A question to ask instead of the standard prompt, to which the value of "
-"register_basic_token is the answer. Setting to empty string (default "
-"value) keeps the standard prompt."
-msgstr ""
-
-#: acct_mgr/register.py:142
-msgid "A string required as input to pass verification."
-msgstr ""
-
 #. TRANSLATOR: Question-style hint for visible bot trap
 #. registration input field.
-#: acct_mgr/register.py:156
+#: acct_mgr/register.py:157
 #, python-format
 msgid "Please answer above: %(question)s"
 msgstr ""
 
-#: acct_mgr/register.py:165
+#: acct_mgr/register.py:166
 #, python-format
 msgid ""
 "Please type [%(token)s] as verification token, exactly replicating "
 "everything within the braces."
 msgstr ""
 
-#: acct_mgr/register.py:167
+#: acct_mgr/register.py:168
 msgid "Parole:"
 msgstr ""
 
-#: acct_mgr/register.py:176
+#: acct_mgr/register.py:177
 msgid "Better do not fill this field."
 msgstr ""
 
-#: acct_mgr/register.py:188
+#: acct_mgr/register.py:189
 msgid "Are you human? If so, try harder!"
 msgstr ""
 
-#: acct_mgr/register.py:196
+#: acct_mgr/register.py:197
 msgid ""
 "A collection of checks for email addresses.\n"
 "\n"
 "''This check is bypassed, if account verification is disabled.''"
 msgstr ""
 
-#: acct_mgr/register.py:207
+#: acct_mgr/register.py:208
 msgid "Email:"
-msgstr "Adresse email :"
+msgstr ""
 
 #. TRANSLATOR: Registration form hints for a mandatory input field.
-#: acct_mgr/register.py:217
-msgid "The email address is required for Trac to send you a verification token."
+#: acct_mgr/register.py:218
+msgid ""
+"\n"
+"                The email address is required for Trac to send you a\n"
+"                verification token.\n"
+"                "
 msgstr ""
 
-#: acct_mgr/register.py:220
+#: acct_mgr/register.py:223
 msgid ""
-"Entering your email address will also enable you to reset your password "
-"if you ever forget it."
+"\n"
+"                    Entering your email address will also enable you "
+"to reset\n"
+"                    your password if you ever forget it.\n"
+"                    "
 msgstr ""
 
 #. TRANSLATOR: Registration form hint, if email input is optional.
-#: acct_mgr/register.py:227
+#: acct_mgr/register.py:230
 msgid ""
-"Entering your email address will enable you to reset your password if you"
-" ever forget it."
+"Entering your email address will enable you to\n"
+"                           reset your password if you ever forget it."
 msgstr ""
 
-#: acct_mgr/register.py:241
+#: acct_mgr/register.py:244
 msgid "You must specify a valid email address."
-msgstr "Vous devez spécifier une adresse email valide."
+msgstr ""
 
-#: acct_mgr/register.py:248
+#: acct_mgr/register.py:251
 msgid ""
-"The email address specified is already in use. Please specify a different"
-" one."
+"The email address specified is already in use. Please specify a "
+"different one."
 msgstr ""
 
-#: acct_mgr/register.py:258
+#: acct_mgr/register.py:261
 msgid ""
 "A collection of checks based on regular expressions.\n"
 "\n"
-"''It depends on !EmailCheck being enabled too for using it's input field."
-"\n"
+"''It depends on !EmailCheck being enabled too for using it's input "
+"field.\n"
 "Likewise email checking is bypassed, if account verification is\n"
 "disabled.''"
 msgstr ""
 
-#: acct_mgr/register.py:268
-msgid ""
-"A validation regular expression describing new usernames. Define "
-"constraints for allowed user names corresponding to local naming policy."
-msgstr ""
-
-#: acct_mgr/register.py:274
-msgid ""
-"A validation regular expression describing new account emails. Define "
-"constraints for a valid email address. A custom pattern can narrow or "
-"widen scope i.e. to accept UTF-8 characters."
-msgstr ""
-
-#: acct_mgr/register.py:291
+#: acct_mgr/register.py:295
 #, python-format
 msgid "Username %(username)s doesn't match local naming policy."
 msgstr ""
 
-#: acct_mgr/register.py:301
+#: acct_mgr/register.py:305
 msgid ""
-"The email address specified appears to be invalid. Please specify a valid"
-" email address."
+"The email address specified appears to be invalid. Please specify a "
+"valid email address."
 msgstr ""
 
-#: acct_mgr/register.py:311
+#: acct_mgr/register.py:315
 msgid ""
 "Check for usernames referenced in the permission system.\n"
 "\n"
 "''This check is bypassed for requests by an authenticated user.''"
 msgstr ""
 
-#: acct_mgr/register.py:390 acct_mgr/templates/genshi/account_login.html:56
-#: acct_mgr/templates/genshi/account_register.html:11
-#: acct_mgr/templates/jinja2/account_login.html:65
-#: acct_mgr/templates/jinja2/account_register.html:7
+#: acct_mgr/register.py:394 acct_mgr/templates/account_login.html:58
+#: acct_mgr/templates/account_login.html:61
+#: acct_mgr/templates/account_register.html:14
 msgid "Register"
-msgstr "S'inscrire"
+msgstr ""
 
-#: acct_mgr/register.py:429 acct_mgr/register.py:446 acct_mgr/register.py:582
-#: acct_mgr/register.py:615 acct_mgr/web_ui.py:359 acct_mgr/web_ui.py:803
+#: acct_mgr/register.py:409 acct_mgr/register.py:413
+msgid "Invalid request arguments."
+msgstr ""
+
+#: acct_mgr/register.py:432 acct_mgr/register.py:449
+#: acct_mgr/register.py:590 acct_mgr/register.py:625 acct_mgr/web_ui.py:351
+#: acct_mgr/web_ui.py:812
 msgid "You should report that issue to a Trac admin."
 msgstr ""
 
-#: acct_mgr/register.py:452
+#: acct_mgr/register.py:455
 msgid ""
-"Your username has been registered successfully, but your account requires"
-" administrative approval. Please proceed according to local policy."
+"Your username has been registered successfully, but your account "
+"requires administrative approval. Please proceed according to local "
+"policy."
 msgstr ""
 
-#: acct_mgr/register.py:462
+#: acct_mgr/register.py:465
 #, python-format
 msgid ""
-"Your username has been successfully registered but your account still "
-"requires activation. Please login as user %(user)s, and follow the "
+"Your username has been successfully registered but your account still"
+" requires activation. Please login as user %(user)s, and follow the "
 "instructions."
 msgstr ""
 
-#: acct_mgr/register.py:467
+#: acct_mgr/register.py:470
 #, python-format
 msgid ""
 "Registration has been finished successfully. You may log in as user "
 "%(user)s now."
 msgstr ""
 
-#: acct_mgr/register.py:553
-msgid ""
-"Your permissions have been limited until you [1:verify your email "
-"address]."
+#. TRANSLATOR: Your permissions have been limited until you ...
+#: acct_mgr/register.py:560
+msgid "verify your email address"
 msgstr ""
 
-#: acct_mgr/register.py:586
+#. TRANSLATOR: ... verify your email address
+#: acct_mgr/register.py:564
 #, python-format
-msgid ""
-"An email has been sent to <%(email)s> with a token to [1:verify your new "
-"email address]."
+msgid "Your permissions have been limited until you %(link)s."
 msgstr ""
 
+#. TRANSLATOR: An email has been sent to <%(email)s>
+#. with a token to ... (the link label for following message)
+#: acct_mgr/register.py:596
+msgid "verify your new email address"
+msgstr ""
+
+#. TRANSLATOR: ... verify your new email address
 #: acct_mgr/register.py:601
+#, python-format
+msgid "An email has been sent to <%(email)s> with a token to %(link)s."
+msgstr ""
+
+#: acct_mgr/register.py:611
 msgid "Please log in to finish email verification procedure."
 msgstr ""
 
-#: acct_mgr/register.py:605
+#: acct_mgr/register.py:615
 msgid "Your email is already verified."
 msgstr ""
 
-#: acct_mgr/register.py:623
+#: acct_mgr/register.py:631
 #, python-format
-msgid "A notification email has been resent to <%(email)s>."
+msgid "A notification email has been resent to <%s>."
 msgstr ""
 
-#: acct_mgr/register.py:629
+#: acct_mgr/register.py:639
 msgid "Thank you for verifying your email address."
 msgstr ""
 
-#: acct_mgr/register.py:632
+#: acct_mgr/register.py:642
 msgid "Invalid verification token"
 msgstr ""
 
-#: acct_mgr/svnserve.py:29
-msgid ""
-"Path to the users file; leave blank to locate the users file by reading "
-"svnserve.conf from the default repository."
+#: acct_mgr/util.py:110
+#, python-format
+msgid "less than %s"
 msgstr ""
 
-#: acct_mgr/util.py:77
+#: acct_mgr/util.py:117
 #, python-format
-msgid "%(datepart)s %(timepart)s"
-msgstr ""
+msgid "%(num)i second"
+msgid_plural "%(num)i seconds"
+msgstr[0] ""
+msgstr[1] ""
+
+#. TRANSLATOR: Pretty datetime representation, time part provided by
+#. string substitution.
+#: acct_mgr/util.py:126
+#, python-format
+msgid "%(num)i day %%s"
+msgid_plural "%(num)i days %%s"
+msgstr[0] ""
+msgstr[1] ""
 
-#: acct_mgr/templates/genshi/account_login.html:42
-#: acct_mgr/templates/genshi/account_login.html:60
-#: acct_mgr/templates/jinja2/account_login.html:47
-#: acct_mgr/templates/jinja2/account_login.html:70 acct_mgr/web_ui.py:107
+#: acct_mgr/templates/account_login.html:45
+#: acct_mgr/templates/account_login.html:66
+#: acct_mgr/templates/account_login.html:69 acct_mgr/web_ui.py:108
 msgid "Forgot your password?"
-msgstr "Mot de passe oublié ?"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:11
-#: acct_mgr/templates/genshi/account_db_cleanup.html:22
-#: acct_mgr/templates/genshi/account_prefs.html:39
-#: acct_mgr/templates/genshi/account_user_table.html:20
-#: acct_mgr/templates/jinja2/account_admin.html:7
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:22
-#: acct_mgr/templates/jinja2/account_prefs.html:7
-#: acct_mgr/templates/jinja2/account_user_table.html:17 acct_mgr/web_ui.py:132
+#: acct_mgr/templates/account_admin.html:14
+#: acct_mgr/templates/account_db_cleanup.html:25
+#: acct_mgr/templates/account_prefs.html:43
+#: acct_mgr/templates/account_user_table.html:20 acct_mgr/web_ui.py:133
 msgid "Account"
-msgstr "Compte"
+msgstr ""
 
-#: acct_mgr/web_ui.py:156
+#: acct_mgr/web_ui.py:157
 #, python-format
 msgid ""
 "Sorry, but policy prohibits choosing '%(username)s' for an anonymous "
 "session. Login or choose another session ID, please."
 msgstr ""
 
-#: acct_mgr/web_ui.py:187
-#, fuzzy
+#: acct_mgr/web_ui.py:191
+#, python-format
 msgid ""
-"You're already logged in. If you need to change your password please use "
-"the [1:Account Preferences] page."
+"You're already logged in. If you need to change your password please "
+"use the %(prefs_href)s page."
+msgstr ""
+
+#: acct_mgr/web_ui.py:228
+msgid "author"
 msgstr ""
-"Vous êtes déjà connecté. Si vous souhaitez modifier votre mot de passe, "
-"merci d'utiliser la page des [1:préférences de compte]."
 
 #: acct_mgr/web_ui.py:232
 #, python-format
 msgid ""
-"Policy prohibits choosing %(username)s for an anonymous session because "
-"it's a registered username. Please login or choose another author name."
+"Policy prohibits choosing %(username)s for an anonymous session "
+"because it's a registered username. Please login or choose another "
+"author name."
 msgstr ""
 
 #: acct_mgr/web_ui.py:244
 msgid "Are you sure you want to delete your account?"
-msgstr "Êtes-vous sûr(e) de vouloir supprimer votre compte ?"
+msgstr ""
 
 #: acct_mgr/web_ui.py:252
 msgid "Thank you for taking the time to update your password."
-msgstr "Merci de prendre le temps de changer votre mot de passe."
+msgstr ""
 
-#: acct_mgr/web_ui.py:258
-#, fuzzy
+#: acct_mgr/web_ui.py:261
+#, python-format
 msgid ""
-"You are required to change password because of a recent password change "
-"request. [1:Please change your password now.]"
-msgstr "Suite à une réinitialisation, vous devez changer de mot de passe. "
+"You are required to change password because of a recent password "
+"change request. %(invitation)s"
+msgstr ""
 
 #: acct_mgr/web_ui.py:270
-#, fuzzy
 msgid "Old password is incorrect."
-msgstr "L'ancien mot de passe est incorrect."
+msgstr ""
 
 #: acct_mgr/web_ui.py:272
-#, fuzzy
 msgid "Old password cannot be empty."
-msgstr "L'ancien mot de passe doit être renseigné."
+msgstr ""
 
 #: acct_mgr/web_ui.py:280
 msgid "Password must not match old password."
 msgstr ""
 
 #: acct_mgr/web_ui.py:287
-#, fuzzy
 msgid "Password updated successfully."
-msgstr "Mot de passe mis à jour."
+msgstr ""
 
 #: acct_mgr/web_ui.py:297
 msgid "Password is incorrect."
-msgstr "Mot de passe incorrect."
+msgstr ""
 
 #: acct_mgr/web_ui.py:316
-#, fuzzy
 msgid "Username is required."
-msgstr "Le nom d'utilisateur doit être renseigné."
+msgstr ""
 
 #: acct_mgr/web_ui.py:318
-#, fuzzy
 msgid "Email is required."
-msgstr "L'adresse email doit être renseignée."
+msgstr ""
 
-#: acct_mgr/web_ui.py:325
-#, fuzzy
+#: acct_mgr/web_ui.py:324
 msgid "Email and username must match a known account."
-msgstr "L'email et/ou le nom d'utilisateur sont inconnus."
+msgstr ""
 
-#: acct_mgr/web_ui.py:348
+#: acct_mgr/web_ui.py:357
 #, python-format
 msgid "Cannot reset password: %(error)s"
 msgstr ""
 
-#: acct_mgr/web_ui.py:370
+#: acct_mgr/web_ui.py:364
 #, python-format
 msgid "A new password has been sent to you at <%(email)s>."
 msgstr ""
 
 #. TRANSLATOR: Intentionally obfuscated login error
 #: acct_mgr/web_ui.py:521
 msgid "Invalid username or password"
-msgstr "Utilisateur ou mot de passe incorrect."
+msgstr ""
 
 #: acct_mgr/web_ui.py:529
-#, python-format
-msgid "Account locked, please try again after %(release_time)s"
-msgstr "Compte bloqué. Merci de recommencer dans %(release_time) sec."
+msgid "Account locked, please try again after % (release_time)s"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:48
-#: acct_mgr/templates/jinja2/account_user_table.html:54 acct_mgr/web_ui.py:532
+#: acct_mgr/templates/account_user_table.html:45 acct_mgr/web_ui.py:532
 msgid "Account locked"
-msgstr "Compte bloqué"
+msgstr ""
 
 #: acct_mgr/web_ui.py:537
 #, python-format
 msgid "Login after %(attempts)s failed attempt"
 msgid_plural "Login after %(attempts)s failed attempts"
 msgstr[0] ""
 msgstr[1] ""
 
-#: acct_mgr/opt/announcer/uid_chg.py:39 acct_mgr/opt/tracforms/uid_chg.py:37
+#: acct_mgr/opt/announcer/uid_chg.py:39
+#: acct_mgr/opt/tracforms/uid_chg.py:37
 #, python-format
 msgid ""
 "Unsupported db schema version, please update %(plugin)s to a recent "
 "version."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:22
-#: acct_mgr/templates/jinja2/account_admin.html:24
-#, fuzzy
+#: acct_mgr/templates/account_admin.html:25
 msgid "Manage User Account"
-msgstr "Gestion des comptes utilisateurs"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:25
-#: acct_mgr/templates/jinja2/account_admin.html:27
-#, python-format
-msgid "for [1:%(name)s] ([2:%(user)s])"
+#: acct_mgr/templates/account_admin.html:27
+#: acct_mgr/templates/account_admin.html:30
+msgid "for"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:28
-#: acct_mgr/templates/jinja2/account_admin.html:30
-#, python-format
-msgid "for [1:%(user)s]"
+#: acct_mgr/templates/account_admin.html:33
+msgid "info"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:30
-#: acct_mgr/templates/jinja2/account_admin.html:35
+#: acct_mgr/templates/account_admin.html:33
 msgid "User ID change requires additional components enabled"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:53
-#: acct_mgr/templates/jinja2/account_admin.html:67
-#, fuzzy
+#: acct_mgr/templates/account_admin.html:55
 msgid "New Username:"
-msgstr "Utilisateur :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:54
-#: acct_mgr/templates/jinja2/account_admin.html:69
+#: acct_mgr/templates/account_admin.html:56
 msgid "Change user ID ('username')"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:62
-#: acct_mgr/templates/jinja2/account_admin.html:77
+#: acct_mgr/templates/account_admin.html:64
 msgid "Skip creating account and password reset"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:64
-#: acct_mgr/templates/jinja2/account_admin.html:79
-#, fuzzy
+#: acct_mgr/templates/account_admin.html:66
 msgid "Assume existing account"
-msgstr "S'inscrire"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:70
-#: acct_mgr/templates/jinja2/account_admin.html:85
+#: acct_mgr/templates/account_admin.html:72
 msgid "Do not overwrite existing attributes"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:72
-#: acct_mgr/templates/jinja2/account_admin.html:87
+#: acct_mgr/templates/account_admin.html:74
 msgid "Copy only new account attributes"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:78
-#: acct_mgr/templates/jinja2/account_admin.html:93
-#, fuzzy
+#: acct_mgr/templates/account_admin.html:80
 msgid "Skip final account deletion"
-msgstr "Être notifié de la suppression de compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:80
-#: acct_mgr/templates/jinja2/account_admin.html:95
+#: acct_mgr/templates/account_admin.html:82
 msgid "Leave old login data"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:90
-#: acct_mgr/templates/genshi/account_config.html:915
-#: acct_mgr/templates/genshi/account_login.html:35
-#: acct_mgr/templates/genshi/account_prefs.html:23
-#: acct_mgr/templates/genshi/account_register.html:43
-#: acct_mgr/templates/genshi/account_users.html:93
-#: acct_mgr/templates/jinja2/account_admin.html:106
-#: acct_mgr/templates/jinja2/account_config.html:1029
-#: acct_mgr/templates/jinja2/account_login.html:39
-#: acct_mgr/templates/jinja2/account_prefs.html:51
-#: acct_mgr/templates/jinja2/account_register.html:52
-#: acct_mgr/templates/jinja2/account_users.html:34
+#: acct_mgr/templates/account_admin.html:92
+#: acct_mgr/templates/account_config.html:894
+#: acct_mgr/templates/account_login.html:38
+#: acct_mgr/templates/account_prefs.html:27
+#: acct_mgr/templates/account_register.html:46
+#: acct_mgr/templates/account_users.html:96
 msgid "Password:"
-msgstr "Mot de passe :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:98
-#: acct_mgr/templates/genshi/account_config.html:921
-#: acct_mgr/templates/genshi/account_prefs.html:63
-#: acct_mgr/templates/genshi/account_register.html:49
-#: acct_mgr/templates/genshi/account_users.html:101
-#: acct_mgr/templates/jinja2/account_admin.html:113
-#: acct_mgr/templates/jinja2/account_config.html:1036
-#: acct_mgr/templates/jinja2/account_prefs.html:33
-#: acct_mgr/templates/jinja2/account_register.html:58
-#: acct_mgr/templates/jinja2/account_users.html:41
+#: acct_mgr/templates/account_admin.html:100
+#: acct_mgr/templates/account_config.html:901
+#: acct_mgr/templates/account_prefs.html:67
+#: acct_mgr/templates/account_register.html:52
+#: acct_mgr/templates/account_users.html:104
 msgid "Confirm Password:"
-msgstr "Confirmation du mot de passe :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:107
-#: acct_mgr/templates/genshi/account_users.html:112
-#: acct_mgr/templates/jinja2/account_admin.html:121
-#: acct_mgr/templates/jinja2/account_users.html:49
+#: acct_mgr/templates/account_admin.html:109
+#: acct_mgr/templates/account_users.html:115
 msgid "Pre-/Surname (Nickname):"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:111
-#: acct_mgr/templates/genshi/account_admin.html:121
-#: acct_mgr/templates/jinja2/account_admin.html:127
-#: acct_mgr/templates/jinja2/account_admin.html:138
-#, fuzzy
+#: acct_mgr/templates/account_admin.html:113
+#: acct_mgr/templates/account_admin.html:123
 msgid "Delete value"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:117
-#: acct_mgr/templates/genshi/account_reset_password.html:35
-#: acct_mgr/templates/genshi/account_users.html:118
-#: acct_mgr/templates/jinja2/account_admin.html:132
-#: acct_mgr/templates/jinja2/account_reset_password.html:41
-#: acct_mgr/templates/jinja2/account_users.html:55
+#: acct_mgr/templates/account_admin.html:119
+#: acct_mgr/templates/account_reset_password.html:38
+#: acct_mgr/templates/account_users.html:121
 msgid "Email Address:"
-msgstr "Adresse email :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:128
-#: acct_mgr/templates/genshi/account_users.html:124
-#: acct_mgr/templates/jinja2/account_admin.html:145
-#: acct_mgr/templates/jinja2/account_users.html:62
+#: acct_mgr/templates/account_admin.html:130
+#: acct_mgr/templates/account_users.html:127
 msgid "Skip new email verification"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:134
-#: acct_mgr/templates/genshi/account_config.html:993
-#: acct_mgr/templates/genshi/account_config.html:997
-#: acct_mgr/templates/genshi/account_notification.html:59
-#: acct_mgr/templates/jinja2/account_admin.html:152
-#: acct_mgr/templates/jinja2/account_config.html:1129
-#: acct_mgr/templates/jinja2/account_config.html:1139
-#: acct_mgr/templates/jinja2/account_notification.html:64
+#: acct_mgr/templates/account_admin.html:136
+#: acct_mgr/templates/account_config.html:978
+#: acct_mgr/templates/account_config.html:981
+#: acct_mgr/templates/account_notification.html:50
 msgid "Apply changes"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:145
-#: acct_mgr/templates/jinja2/account_admin.html:165
+#: acct_mgr/templates/account_admin.html:147
 msgid "Account Status"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:150
-#: acct_mgr/templates/jinja2/account_admin.html:175
+#: acct_mgr/templates/account_admin.html:150
 #, python-format
 msgid ""
-"This account has been locked until %(time)s[1:]and even valid login "
-"attempts are rejected meanwhile."
+"[1:]\n"
+"                This account has been locked until %(time)s[2:]\n"
+"                and even valid login attempts are rejected meanwhile."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:156
-#: acct_mgr/templates/jinja2/account_admin.html:185
+#: acct_mgr/templates/account_admin.html:155
 msgid "This account has been locked permanently."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:160
-#: acct_mgr/templates/jinja2/account_admin.html:190
-#: acct_mgr/templates/jinja2/account_admin.html:191
+#: acct_mgr/templates/account_admin.html:159
 msgid "Release account lock"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:160
-#: acct_mgr/templates/jinja2/account_admin.html:192
+#: acct_mgr/templates/account_admin.html:159
 msgid "Unlock"
-msgstr "Débloquer"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:170
+#: acct_mgr/templates/account_admin.html:169
 #, python-format
 msgid "Time lock condition has been met %(count)s time by now."
 msgid_plural "Time lock condition has been met %(count)s times by now."
 msgstr[0] ""
 msgstr[1] ""
 
-#: acct_mgr/templates/genshi/account_admin.html:174
-#: acct_mgr/templates/jinja2/account_admin.html:210
+#: acct_mgr/templates/account_admin.html:184
 #, python-format
 msgid ""
-"Therefore after another failed login attempt authentication for this "
-"account would be retarded by %(time)s."
+"Therefore after another failed login attempt authentication\n"
+"                for this account would be retarded by %(time)s."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:182
-#: acct_mgr/templates/jinja2/account_admin.html:219
+#: acct_mgr/templates/account_admin.html:191
 msgid "Lock condition has not been met yet."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:186
-#: acct_mgr/templates/jinja2/account_admin.html:225
+#: acct_mgr/templates/account_admin.html:195
 msgid "No constraints are set for this account."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:192
-#: acct_mgr/templates/jinja2/account_admin.html:237
+#: acct_mgr/templates/account_admin.html:201
 #, python-format
 msgid ""
-"Credentials for this user are stored in AuthStore number "
-"[1:%(order_num)s] (%(store)s)."
+"Credentials for this user are stored in AuthStore number\n"
+"              [1:%(order_num)s] (%(store)s)."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:196
-#: acct_mgr/templates/jinja2/account_admin.html:245
+#: acct_mgr/templates/account_admin.html:204
 msgid "Username matching is set to [1:not case-sensitive]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:199
-#: acct_mgr/templates/jinja2/account_admin.html:251
+#: acct_mgr/templates/account_admin.html:206
 msgid "Username matching is set to [1:case-sensitive]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:204
-#: acct_mgr/templates/jinja2/account_admin.html:262
+#: acct_mgr/templates/account_admin.html:210
 msgid ""
-"No readable store provides credentials for this user, so the user may not"
-" get authenticated and access to this [1:account might be effectively "
-"blocked]."
+"No readable store provides credentials for this user,\n"
+"              so the user may not get authenticated and access to "
+"this\n"
+"              [1:account might be effectively blocked]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:211
-#: acct_mgr/templates/jinja2/account_admin.html:274
+#: acct_mgr/templates/account_admin.html:216
 #, python-format
 msgid "Current email address: <%(email)s>"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:215
-#: acct_mgr/templates/jinja2/account_admin.html:280
+#: acct_mgr/templates/account_admin.html:219
 msgid "This address has been verified successfully."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:216
-#: acct_mgr/templates/jinja2/account_admin.html:284
+#: acct_mgr/templates/account_admin.html:221
 #, python-format
-msgid "Verification is pending [1:(token: %(token)s)]"
+msgid ""
+"Verification is pending\n"
+"                [1:(token: %(token)s)]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:219
-#: acct_mgr/templates/jinja2/account_admin.html:290
+#: acct_mgr/templates/account_admin.html:224
 msgid "This address has not been verified yet."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:225
-#: acct_mgr/templates/jinja2/account_admin.html:298
+#: acct_mgr/templates/account_admin.html:229
 msgid "No email address is registered for this account."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:230
-#: acct_mgr/templates/jinja2/account_admin.html:306
+#: acct_mgr/templates/account_admin.html:234
 msgid "Access History"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:231
-#: acct_mgr/templates/jinja2/account_admin.html:309
+#: acct_mgr/templates/account_admin.html:235
 #, python-format
 msgid "Last login: %(time)s"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:231
-#: acct_mgr/templates/jinja2/account_admin.html:311
+#: acct_mgr/templates/account_admin.html:237
 msgid "The user has not logged in before."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:237
-#: acct_mgr/templates/jinja2/account_admin.html:317
+#: acct_mgr/templates/account_admin.html:239
 #, python-format
 msgid "Total failed attempts: %(count)s"
-msgstr "Nombre de tentatives ayant échoué : %(count)s"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:238
-#: acct_mgr/templates/jinja2/account_admin.html:321
+#: acct_mgr/templates/account_admin.html:240
 msgid "Table: Last failed login attempts log view"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:243
-#: acct_mgr/templates/jinja2/account_admin.html:326
+#: acct_mgr/templates/account_admin.html:245
 msgid "IP address"
-msgstr "Adresse IP"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:244
-#: acct_mgr/templates/jinja2/account_admin.html:327
+#: acct_mgr/templates/account_admin.html:246
 msgid "Log time"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:255
-#: acct_mgr/templates/jinja2/account_admin.html:342
+#: acct_mgr/templates/account_admin.html:257
 msgid "Delete login failure log"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:255
-#: acct_mgr/templates/jinja2/account_admin.html:343
+#: acct_mgr/templates/account_admin.html:257
 msgid "Delete Log"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:261
-#: acct_mgr/templates/jinja2/account_admin.html:350
+#: acct_mgr/templates/account_admin.html:264
 msgid "There is currently no failed login attempt logged."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_admin.html:266
-#: acct_mgr/templates/genshi/account_config.html:1002
-#: acct_mgr/templates/jinja2/account_admin.html:357
-#: acct_mgr/templates/jinja2/account_config.html:1132
+#: acct_mgr/templates/account_admin.html:269
+#: acct_mgr/templates/account_config.html:985
 msgid "Refresh"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:11
-#: acct_mgr/templates/genshi/account_config.html:24
-#: acct_mgr/templates/jinja2/account_config.html:7
-#: acct_mgr/templates/jinja2/account_config.html:14
+#: acct_mgr/templates/account_config.html:14
+#: acct_mgr/templates/account_config.html:27
 msgid "Accounts: Configuration"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:50
-#: acct_mgr/templates/genshi/account_config.html:985
-#: acct_mgr/templates/jinja2/account_config.html:47
-#: acct_mgr/templates/jinja2/account_config.html:1118
+#: acct_mgr/templates/account_config.html:53
+#: acct_mgr/templates/account_config.html:971
 msgid "Apply changes and go back"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:50
-#: acct_mgr/templates/genshi/account_config.html:54
-#: acct_mgr/templates/genshi/account_config.html:985
-#: acct_mgr/templates/genshi/account_config.html:989
-#: acct_mgr/templates/jinja2/account_config.html:48
-#: acct_mgr/templates/jinja2/account_config.html:52
-#: acct_mgr/templates/jinja2/account_config.html:1119
-#: acct_mgr/templates/jinja2/account_config.html:1123
+#: acct_mgr/templates/account_config.html:53
+#: acct_mgr/templates/account_config.html:57
+#: acct_mgr/templates/account_config.html:971
+#: acct_mgr/templates/account_config.html:975
 msgid "Previous"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:54
-#: acct_mgr/templates/genshi/account_config.html:989
-#: acct_mgr/templates/jinja2/account_config.html:51
-#: acct_mgr/templates/jinja2/account_config.html:1122
+#: acct_mgr/templates/account_config.html:57
+#: acct_mgr/templates/account_config.html:975
 msgid "Go back"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:57
-#: acct_mgr/templates/genshi/account_config.html:1006
-#: acct_mgr/templates/jinja2/account_config.html:57
-#: acct_mgr/templates/jinja2/account_config.html:1134
+#: acct_mgr/templates/account_config.html:60
+#: acct_mgr/templates/account_config.html:988
 msgid "Apply changes and go on"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:57
-#: acct_mgr/templates/genshi/account_config.html:1006
-#: acct_mgr/templates/jinja2/account_config.html:58
-#: acct_mgr/templates/jinja2/account_config.html:1135
+#: acct_mgr/templates/account_config.html:60
+#: acct_mgr/templates/account_config.html:988
 msgid "Next"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:67
-#: acct_mgr/templates/genshi/account_config.html:260
-#: acct_mgr/templates/genshi/account_config.html:553
-#: acct_mgr/templates/genshi/account_config.html:601
-#: acct_mgr/templates/genshi/account_config.html:750
-#: acct_mgr/templates/genshi/account_config.html:878
-#: acct_mgr/templates/jinja2/account_config.html:68
-#: acct_mgr/templates/jinja2/account_config.html:285
-#: acct_mgr/templates/jinja2/account_config.html:610
-#: acct_mgr/templates/jinja2/account_config.html:667
-#: acct_mgr/templates/jinja2/account_config.html:838
-#: acct_mgr/templates/jinja2/account_config.html:981
+#: acct_mgr/templates/account_config.html:70
+#: acct_mgr/templates/account_config.html:256
+#: acct_mgr/templates/account_config.html:540
+#: acct_mgr/templates/account_config.html:589
+#: acct_mgr/templates/account_config.html:731
+#: acct_mgr/templates/account_config.html:856
 #, python-format
 msgid "Step %(step)s: %(label)s"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:70
-#: acct_mgr/templates/jinja2/account_config.html:71
+#: acct_mgr/templates/account_config.html:73
 msgid "Objective for setting Authentication Options"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:71
-#: acct_mgr/templates/jinja2/account_config.html:73
+#: acct_mgr/templates/account_config.html:74
 msgid ""
-"Decide, whether to use HTTP authentication (Trac default) or a HTML login"
-" form provided by AccountManagerPlugin."
+"Decide, whether to use HTTP authentication (Trac default) or\n"
+"            a HTML login form provided by AccountManagerPlugin."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:76
-#: acct_mgr/templates/jinja2/account_config.html:78
+#: acct_mgr/templates/account_config.html:78
 msgid ""
-"After initial login Trac sessions are authenticated per request based on "
-"browser cookies. Therefore a number of options provide control over some "
-"critical browser cookie properties."
+"After initial login Trac sessions are authenticated per request\n"
+"            based on browser cookies.  Therefor a number of options "
+"provide\n"
+"            control over some critical browser cookie properties."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:83
-#: acct_mgr/templates/jinja2/account_config.html:83
+#: acct_mgr/templates/account_config.html:84
 msgid "Provider-agnostic Authentication Options"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:88
-#: acct_mgr/templates/jinja2/account_config.html:89
+#: acct_mgr/templates/account_config.html:89
 msgid "Convert login names to lower case on registration and login."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:91
-#: acct_mgr/templates/jinja2/account_config.html:93
+#: acct_mgr/templates/account_config.html:92
 msgid ""
-"Adapt to careless username typing, where casing does not matter, like on "
-"Windows. Potentially troublesome, because [1:case matters for Trac "
-"permission assignment lookup] anyway."
+"Adapt to careless username typing, where casing does not matter,\n"
+"              like on Windows.  Potentially troublesome, because "
+"[1:case\n"
+"              matters for Trac permission assignment lookup] anyway."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:101
-#: acct_mgr/templates/jinja2/account_config.html:105
+#: acct_mgr/templates/account_config.html:102
 msgid "Check IP address for authentication."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:104
-#: acct_mgr/templates/jinja2/account_config.html:108
+#: acct_mgr/templates/account_config.html:105
 msgid ""
-"Potentially troublesome for users with dynamic IP address, but "
-"disregarded for persistent sessions."
+"Potentially troublesome for users with dynamic IP adress, but\n"
+"              disregarded for persistent sessions."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:114
-#: acct_mgr/templates/jinja2/account_config.html:118
+#: acct_mgr/templates/account_config.html:114
 msgid "Restrict sending cookies to HTTPS connections."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:117
-#: acct_mgr/templates/jinja2/account_config.html:121
+#: acct_mgr/templates/account_config.html:117
 msgid "Required, if the Trac instance is only accessible through HTTPS."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:128
-#: acct_mgr/templates/jinja2/account_config.html:131
+#: acct_mgr/templates/account_config.html:129
 #, python-format
-msgid "Lifetime of the authentication cookie: [1:] seconds [2:(%(timedelta)s)]"
+msgid ""
+"Lifetime of the authentication cookie:\n"
+"              [1:]\n"
+"              seconds\n"
+"              [2:\n"
+"                (%(timedelta)s)\n"
+"              ]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:141
-#: acct_mgr/templates/jinja2/account_config.html:142
+#: acct_mgr/templates/account_config.html:140
 msgid ""
-"Determines how long the browser will cache authentication information, "
-"and therefore, after how much inactivity a user will have to log in "
-"again. Default (0 s) makes cookie expire at browsing sessions end."
+"Determines how long the browser will cache authentication\n"
+"              information, and therefore, after how much inactivity a"
+" user\n"
+"              will have to log in again.  Default (0 s) makes cookie\n"
+"              expire at browsing sessions end."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:150
-#: acct_mgr/templates/jinja2/account_config.html:150
+#: acct_mgr/templates/account_config.html:148
 msgid "Authentication Front-end"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:156
-#: acct_mgr/templates/jinja2/account_config.html:157
+#: acct_mgr/templates/account_config.html:153
 msgid ""
-"Use HTTP authentication and credentials as configured in and provided by "
-"your web-server."
+"Use HTTP authentication and credentials as configured in and\n"
+"              provided by your web-server."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:160
-#: acct_mgr/templates/jinja2/account_config.html:163
+#: acct_mgr/templates/account_config.html:157
 msgid ""
-"You can still manage some password stores with AccountManagerPlugin, if "
-"you configure them in the next step."
+"You can still manage some password stores with\n"
+"              AccountManagerPlugin, if you configure them in the next"
+" step."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:169
-#: acct_mgr/templates/jinja2/account_config.html:172
+#: acct_mgr/templates/account_config.html:164
 msgid ""
-"Use a HTML login form backed by one or more password stores managed by "
-"AccountManagerPlugin."
+"Use a HTML login form backed by one or more password stores\n"
+"              managed by AccountManagerPlugin."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:173
-#: acct_mgr/templates/jinja2/account_config.html:179
+#: acct_mgr/templates/account_config.html:168
 msgid ""
-"AccountManagerPlugin provides a custom version of the [1:LoginModule] "
-"accompanied by a form-based HTML login page."
+"AccountManagerPlugin provides a custom version of the\n"
+"              [1:LoginModule] accompanied by a form-based HTML\n"
+"              login page."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:178
-#: acct_mgr/templates/jinja2/account_config.html:187
+#: acct_mgr/templates/account_config.html:173
 msgid ""
-"If you enable this feature, you'll want to review and adjust some more "
-"options related to session authentication. Note, that "
-"AccountManagerPlugin's LoginModule [1:changes the default lifetime of "
-"authentication cookies to 30 days]."
+"If you enable this feature, you'll want to review and adjust\n"
+"              some more options related to session authentication.\n"
+"              Note, that AccountManagerPlugin's LoginModule "
+"[1:changes the\n"
+"              default lifetime of authentication cookies to 30 days]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:187
-#: acct_mgr/templates/jinja2/account_config.html:198
+#: acct_mgr/templates/account_config.html:182
 msgid "AccountManagerPlugin Authentication Options"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:192
-#: acct_mgr/templates/jinja2/account_config.html:204
+#: acct_mgr/templates/account_config.html:187
 msgid "Integrate links to related actions into the login form."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:195
-#: acct_mgr/templates/jinja2/account_config.html:209
+#: acct_mgr/templates/account_config.html:190
 msgid ""
-"[1:If enabled, links to][2:[3:[4:Lost password/Password "
-"reset]][5:[6:Registration for new users]]][7:that normally reside in "
-"Trac's meta-navigation bar, will appear inside the login form. CSS "
-"styling allows further customization of the login prompt.]"
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:216
-#: acct_mgr/templates/jinja2/account_config.html:228
-msgid ""
-"Allow the user to be remembered across sessions without needing to re-"
-"authenticate."
+"[1:\n"
+"                  If enabled, links to\n"
+"                ]\n"
+"                [2:\n"
+"                  [3:\n"
+"                    [4:Lost password/Password reset]\n"
+"                  ]\n"
+"                  [5:\n"
+"                    [6:Registration for new users]\n"
+"                  ]\n"
+"                ]\n"
+"                [7:\n"
+"                  that normally reside in Trac's meta-navigation bar,"
+" will\n"
+"                  appear inside the login form.  CSS styling allows "
+"further\n"
+"                  customization of the login prompt.\n"
+"                ]"
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:213
+msgid ""
+"Allow the user to be remembered across sessions without\n"
+"                needing to re-authenticate."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:217
+msgid ""
+"This is, user checks a \"Remember Me\"\n"
+"                [1:checkbox] in the AccountManagerPlugin login form "
+"and,\n"
+"                next time he visits the site within 30 days, he'll be"
+"\n"
+"                remembered and authenticated automatically."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:220
-#: acct_mgr/templates/jinja2/account_config.html:235
+#: acct_mgr/templates/account_config.html:224
 msgid ""
-"This is, user checks a \"Remember Me\" [1:checkbox] in the "
-"AccountManagerPlugin login form and, next time he visits the site within "
-"30 days, he'll be remembered and authenticated automatically."
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:228
-#: acct_mgr/templates/jinja2/account_config.html:246
-msgid "Likelihood of session cookie ID change: [1:] % per work hour"
+"Likelihood of session cookie ID change:\n"
+"                [1:]\n"
+"                % per work hour"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:235
-#: acct_mgr/templates/jinja2/account_config.html:253
+#: acct_mgr/templates/account_config.html:231
 msgid ""
-"Driving a refresh process to decrease vulnerability of long-lasting "
-"sessions. Zero means [1:never]."
+"Driving a refresh process to decrease vulnerability of\n"
+"                long-lasting sessions.  Zero means [1:never]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:241
-#: acct_mgr/templates/jinja2/account_config.html:262
+#: acct_mgr/templates/account_config.html:237
 msgid "Path for authentication cookie:"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:247
-#: acct_mgr/templates/jinja2/account_config.html:269
+#: acct_mgr/templates/account_config.html:243
 msgid ""
-"This enables AccountManagerPlugin's authentication data distribution to "
-"Trac instances with matching cookie path. Set this to a common base path "
-"of several Trac instances to share the cookie, providing a cheap [1"
-":Single-Sign-On] experience."
+"This enables AccountManagerPlugin's authentication data\n"
+"                distribution to Trac instances with matching cookie "
+"path.\n"
+"                Set this to a common base path of several Trac "
+"instances to\n"
+"                share the cookie, providing a cheap [1:Single-Sign-"
+"On]\n"
+"                experience."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:263
-#: acct_mgr/templates/jinja2/account_config.html:288
-#, fuzzy
-msgid "Password store"
-msgstr "Mot de passe incorrect."
+#: acct_mgr/templates/account_config.html:259
+msgid "Password store icon"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:265
-#: acct_mgr/templates/jinja2/account_config.html:291
+#: acct_mgr/templates/account_config.html:262
 msgid "Objective for configuring a Password Store"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:266
-#: acct_mgr/templates/jinja2/account_config.html:293
+#: acct_mgr/templates/account_config.html:263
 msgid ""
-"AccountManagerPlugin manages user credentials in a modular back-end "
-"providing access to at least one password store."
+"AccountManagerPlugin manages user credentials in a modular\n"
+"              back-end providing access to at least one password "
+"store."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:273
-#: acct_mgr/templates/jinja2/account_config.html:300
+#: acct_mgr/templates/account_config.html:269
 msgid "Initial Authentication Back-end selection"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:279
-#: acct_mgr/templates/jinja2/account_config.html:307
+#: acct_mgr/templates/account_config.html:276
 msgid "Use a password store embedded into Trac db."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:282
-#: acct_mgr/templates/jinja2/account_config.html:311
+#: acct_mgr/templates/account_config.html:279
 msgid ""
-"The [1:SessionStore] implements password storage in Trac db table "
-"'session_attribute'. Its the default choice mainly for avoiding "
-"additional dependencies like directory and file permissions."
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:288
-#: acct_mgr/templates/jinja2/account_config.html:319
-msgid ""
-"While great to resolve some concurrent access issues too, this password "
-"store has shortcomings as well. Notably it does not support seamless hash"
-" type migration, and its no candidate for shared use by multiple Trac "
-"instances or even by applications beyond Trac."
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:298
-#: acct_mgr/templates/genshi/account_config.html:340
-#: acct_mgr/templates/genshi/account_config.html:362
-#: acct_mgr/templates/genshi/account_config.html:385
-#: acct_mgr/templates/genshi/account_config.html:416
-#: acct_mgr/templates/genshi/account_config.html:965
-#: acct_mgr/templates/jinja2/account_config.html:328
-#: acct_mgr/templates/jinja2/account_config.html:373
-#: acct_mgr/templates/jinja2/account_config.html:396
-#: acct_mgr/templates/jinja2/account_config.html:419
-#: acct_mgr/templates/jinja2/account_config.html:453
-#: acct_mgr/templates/jinja2/account_config.html:1096
+"The [1:SessionStore] implements password\n"
+"                  storage in Trac db table 'session_attributes'.\n"
+"                  Its the default choice mainly for avoiding "
+"additional\n"
+"                  dependencies like directory and file permissions."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:285
+msgid ""
+"While great to resolve some concurrent access issues too,\n"
+"                  this password store has shortcomings as well.  "
+"Notably it\n"
+"                  does not support seamless hash type migration, and "
+"its no\n"
+"                  candidate for shared use by multiple Trac instances"
+" or even\n"
+"                  by applications beyond Trac."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:293
+#: acct_mgr/templates/account_config.html:334
+#: acct_mgr/templates/account_config.html:355
+#: acct_mgr/templates/account_config.html:378
+#: acct_mgr/templates/account_config.html:407
+#: acct_mgr/templates/account_config.html:944
 msgid "Details (Preview)"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:301
-#: acct_mgr/templates/genshi/account_config.html:343
-#: acct_mgr/templates/genshi/account_config.html:365
-#: acct_mgr/templates/genshi/account_config.html:388
-#: acct_mgr/templates/genshi/account_config.html:419
-#: acct_mgr/templates/jinja2/account_config.html:333
-#: acct_mgr/templates/jinja2/account_config.html:377
-#: acct_mgr/templates/jinja2/account_config.html:400
-#: acct_mgr/templates/jinja2/account_config.html:423
-#: acct_mgr/templates/jinja2/account_config.html:457
+#: acct_mgr/templates/account_config.html:296
+#: acct_mgr/templates/account_config.html:410
 msgid ""
-"Please apply these default options first. You'll be able to change values"
-" afterwards."
+"Please apply these default options first. You'll be\n"
+"                      able to change values afterwards."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:312
-#: acct_mgr/templates/jinja2/account_config.html:344
+#: acct_mgr/templates/account_config.html:307
 msgid "Use a file-based password store."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:315
-#: acct_mgr/templates/jinja2/account_config.html:347
+#: acct_mgr/templates/account_config.html:310
 msgid ""
-"AccountManagerPlugin includes native support for common Apache file "
-"formats 'htpasswd' and 'htdigest' as well as support for reading "
-"svnserve's password file format."
+"AccountManagerPlugin includes native support for common\n"
+"                  Apache file formats 'htpasswd' and 'htdigest' as "
+"well as\n"
+"                  support for reading svnserve's password file format."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:321
+#: acct_mgr/templates/account_config.html:315
 msgid ""
-"You may use the same file for several Trac environments. Note that "
-"setting appropriate directory and file permissions is crucial for these "
-"stores, but not covered by this configuration wizard."
+"You may use the same file for several Trac environments.\n"
+"                  Note that setting appropriate directory and file "
+"permissions\n"
+"                  is crucial for these stores, but not covered by "
+"this\n"
+"                  configuration wizard."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:335
-#: acct_mgr/templates/jinja2/account_config.html:368
-msgid "'htdigest' format [1:([2:HtDigestStore])]"
+#: acct_mgr/templates/account_config.html:324
+msgid ""
+"[1:]\n"
+"                    'htdigest' format\n"
+"                    [2:([3:HtDigestStore])]"
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:337
+#: acct_mgr/templates/account_config.html:358
+#: acct_mgr/templates/account_config.html:381
+msgid ""
+"Please apply these default options first. You'll be\n"
+"                        able to change values afterwards."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:357
-#: acct_mgr/templates/jinja2/account_config.html:391
-msgid "'htpasswd' format [1:([2:HtPasswdStore])]"
+#: acct_mgr/templates/account_config.html:345
+msgid ""
+"[1:]\n"
+"                    'htpasswd' format\n"
+"                    [2:([3:HtPasswdStore])]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:379
-#: acct_mgr/templates/jinja2/account_config.html:414
-msgid "svnserve's password file format [1:([2:SvnServePasswordStore])]"
+#: acct_mgr/templates/account_config.html:366
+msgid ""
+"[1:]\n"
+"                    svnserve's password file format\n"
+"                    [2:\n"
+"                        ([3:SvnServePasswordStore])\n"
+"                    ]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:402
-#: acct_mgr/templates/jinja2/account_config.html:436
+#: acct_mgr/templates/account_config.html:394
 msgid "Delegate authentication using HTTP authentication."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:405
-#: acct_mgr/templates/jinja2/account_config.html:440
+#: acct_mgr/templates/account_config.html:397
 msgid ""
-"AccountManagerPlugin enables use of standard HTTP-Auth by its "
-"[1:HttpAuthStore] component. Both Basic and Digest authentication "
-"challenges are supported."
+"AccountManagerPlugin enables use of standard HTTP-Auth\n"
+"                  by its [1:HttpAuthStore] component.  Both\n"
+"                  Basic and Digest authentication challenges are "
+"supported."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:410
-#: acct_mgr/templates/jinja2/account_config.html:448
+#: acct_mgr/templates/account_config.html:402
 msgid ""
-"In addition to being read-only this password store does not even support "
-"listing users for obvious reasons."
+"In addition to being read-only this password store does not\n"
+"                  even support listing users for obvious reasons."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:435
-#: acct_mgr/templates/jinja2/account_config.html:471
+#: acct_mgr/templates/account_config.html:425
 msgid "Use a different password store."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:438
-#: acct_mgr/templates/jinja2/account_config.html:474
+#: acct_mgr/templates/account_config.html:428
 msgid ""
-"AccountManagerPlugin's modular password store concept encourages creation"
-" of more ways to provide user credential beyond the natively supported "
-"stores. While a specific setup assistance for these 3rd-party "
-"authentication providers is not implemented, you may fill-in appropriate "
-"configuration details for an already installed component below."
+"AccountManagerPlugin's modular password store concept\n"
+"                  encourages creation of more ways to provide user "
+"credential\n"
+"                  beyond the natively supported stores.  While "
+"specific setup\n"
+"                  assistance for these 3rd-party authentication "
+"providers is not\n"
+"                  implemented, you may fill-in approprate "
+"configuration details\n"
+"                  for an already installed component below."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:453
-#: acct_mgr/templates/jinja2/account_config.html:488
+#: acct_mgr/templates/account_config.html:441
 msgid ""
-"Type the custom configuration options as provided by that components "
-"documentation and apply it."
+"Type the custom configuration options as provided by that\n"
+"                    components documentation and apply it."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:464
-#: acct_mgr/templates/jinja2/account_config.html:498
+#: acct_mgr/templates/account_config.html:451
 msgid "Password Store Configuration"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:465
-#: acct_mgr/templates/jinja2/account_config.html:501
+#: acct_mgr/templates/account_config.html:452
 #, python-format
 msgid ""
-"All enabled stores are listed below, but most won't work at all without "
-"additional configuration.[1:]Currently configured: [2:%(store_list)s]"
+"All enabled stores are listed below, but most won't work at\n"
+"                all without additional configuration.[1:]\n"
+"                Currently configured:\n"
+"                [2:\n"
+"                  %(store_list)s\n"
+"                ]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:470
-#: acct_mgr/templates/jinja2/account_config.html:511
+#: acct_mgr/templates/account_config.html:460
 msgid "This is an experts-only type of store configuration."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:475
-#: acct_mgr/templates/genshi/account_config.html:655
-#: acct_mgr/templates/jinja2/account_config.html:519
-#: acct_mgr/templates/jinja2/account_config.html:734
+#: acct_mgr/templates/account_config.html:464
 #, python-format
-msgid "Required disabled component(s): [1:%(components)s]"
+msgid ""
+"[1:Required disabled component(s):\n"
+"                  [2:%(components)s]]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:480
-#: acct_mgr/templates/jinja2/account_config.html:528
+#: acct_mgr/templates/account_config.html:469
 msgid ""
-"Select one or more stores and configure related options. Concurrent use "
-"of multiple password stores is supported too."
+"Select one or more stores and configure related options.\n"
+"                Concurrent use of multiple password stores is "
+"supported too."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:485
-#: acct_mgr/templates/jinja2/account_config.html:533
+#: acct_mgr/templates/account_config.html:473
 msgid "Password stores are queried in turn, so order matters."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:530
-#: acct_mgr/templates/jinja2/account_config.html:585
+#: acct_mgr/templates/account_config.html:519
 msgid "Silently update password hashes on next successful login."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:533
-#: acct_mgr/templates/jinja2/account_config.html:588
+#: acct_mgr/templates/account_config.html:522
 msgid ""
-"Use it after changing hash type or to migrate to a new primary password "
-"store."
+"Use it after changing hash type or to migrate to a new\n"
+"                  primary password store."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:538
-#: acct_mgr/templates/jinja2/account_config.html:593
+#: acct_mgr/templates/account_config.html:526
 msgid ""
-"The update will run only once. Restarting the procedure for all accounts "
-"allows to propagate subsequent changes."
+"The update will run only once.  Restarting the procedure\n"
+"                  for all accounts allows to propagate subsequent "
+"changes."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:544
-#: acct_mgr/templates/jinja2/account_config.html:599
+#: acct_mgr/templates/account_config.html:531
 msgid "Restart"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:556
-#: acct_mgr/templates/jinja2/account_config.html:613
-#, fuzzy
-msgid "Password refresh"
-msgstr "Mot de passe incorrect."
+#: acct_mgr/templates/account_config.html:543
+msgid "Password refresh icon"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:558
-#: acct_mgr/templates/jinja2/account_config.html:616
+#: acct_mgr/templates/account_config.html:546
 msgid "Objective for Password Policy rules"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:559
-#: acct_mgr/templates/jinja2/account_config.html:618
+#: acct_mgr/templates/account_config.html:547
 msgid ""
-"While AccountManagerPlugin does not enforce password rules in general, "
-"there are some other ways to alter password handling."
+"While AccountManagerPlugin does not enforce password rules in\n"
+"              general, there are some other ways to alter password "
+"handling."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:569
-#: acct_mgr/templates/jinja2/account_config.html:628
+#: acct_mgr/templates/account_config.html:556
 msgid "Enable the password reset procedure."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:572
-#: acct_mgr/templates/jinja2/account_config.html:631
+#: acct_mgr/templates/account_config.html:559
 msgid ""
-"It relies on a working email sender for Trac, supporting both "
-"TracAnnouncer and TracNotification."
+"It relies on a working email sender for Trac, supporting both\n"
+"                TracAnnouncer and TracNotification."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:579
-#: acct_mgr/templates/jinja2/account_config.html:639
-msgid "Length of the randomly-generated passwords: [1:] characters"
+#: acct_mgr/templates/account_config.html:565
+msgid ""
+"Length of the randomly-generated passwords:\n"
+"                [1:]\n"
+"                characters"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:585
-#: acct_mgr/templates/jinja2/account_config.html:648
+#: acct_mgr/templates/account_config.html:573
 msgid "These passwords are used as alternative passwords on request."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:593
-#: acct_mgr/templates/jinja2/account_config.html:657
+#: acct_mgr/templates/account_config.html:581
 msgid "Force users to change passwords after a password reset."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:604
-#: acct_mgr/templates/jinja2/account_config.html:670
-#, fuzzy
-msgid "Account approval"
-msgstr "Compte"
+#: acct_mgr/templates/account_config.html:592
+msgid "Account approval icon"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:606
-#: acct_mgr/templates/jinja2/account_config.html:673
+#: acct_mgr/templates/account_config.html:595
 msgid "Objective for Account Registration and Verification rules"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:607
-#: acct_mgr/templates/jinja2/account_config.html:676
+#: acct_mgr/templates/account_config.html:596
 msgid ""
-"You may require administrative approval of new accounts for the user "
-"registration process. The ability to immediately ban existing accounts is"
-" another, related but independent feature."
+"You may require administrative approval of new accounts for the\n"
+"              user registration process.  The ability to immediately "
+"ban\n"
+"              existing accounts is another, related but independed "
+"feature."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:619
-#: acct_mgr/templates/jinja2/account_config.html:686
+#: acct_mgr/templates/account_config.html:606
 msgid "Allow administrative user ID changes."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:628
-#: acct_mgr/templates/jinja2/account_config.html:694
+#: acct_mgr/templates/account_config.html:615
 msgid "Allow users to register for a new account."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:637
-#: acct_mgr/templates/jinja2/account_config.html:702
+#: acct_mgr/templates/account_config.html:624
 msgid "Allow users to delete their own account."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:642
-#: acct_mgr/templates/jinja2/account_config.html:707
+#: acct_mgr/templates/account_config.html:629
 msgid "Checks to use for validating Registration requests"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:643
-#: acct_mgr/templates/jinja2/account_config.html:711
+#: acct_mgr/templates/account_config.html:630
 #, python-format
 msgid ""
-"All checks provided by AccountManagerPlugin are enabled per default, but "
-"some are configurable on their own.[1:]Currently configured: "
-"[2:%(check_list)s]"
+"All checks provided by AccountManagerPlugin are enabled per\n"
+"              default, but some are configurable on their own.[1:]\n"
+"              Currently configured:\n"
+"              [2:\n"
+"                %(check_list)s\n"
+"              ]"
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:638
+msgid ""
+"Checks like [1:BotTrapCheck] won't work at all\n"
+"              without additional configuration."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:649
-#: acct_mgr/templates/jinja2/account_config.html:723
+#: acct_mgr/templates/account_config.html:643
+#, python-format
 msgid ""
-"Checks like [1:BotTrapCheck] won't work at all without additional "
-"configuration."
+"[1:Required disabled component(s):\n"
+"                [2:%(components)s]]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:660
-#: acct_mgr/templates/jinja2/account_config.html:743
+#: acct_mgr/templates/account_config.html:648
 msgid ""
-"Select one or more checks and configure related options. Concurrent use "
-"of multiple registration checks is encouraged."
+"Select one or more checks and configure related options.\n"
+"              Concurrent use of multiple registration checks is "
+"encouraged."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:666
-#: acct_mgr/templates/jinja2/account_config.html:748
+#: acct_mgr/templates/account_config.html:652
 msgid ""
-"Checks are applied in turn, so order matters. Note that some checks are "
-"used to validate admin user actions too."
+"Checks are applied in turn, so order matters.  Note that some\n"
+"              checks are used to validate admin user actions too."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:714
-#: acct_mgr/templates/jinja2/account_config.html:801
+#: acct_mgr/templates/account_config.html:698
 msgid "Other Account Policy options"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:720
-#: acct_mgr/templates/jinja2/account_config.html:808
+#: acct_mgr/templates/account_config.html:704
 msgid "Require administrative account approval after registration."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:723
-#: acct_mgr/templates/jinja2/account_config.html:811
+#: acct_mgr/templates/account_config.html:707
 msgid ""
-"For admin notification on registration time it relies on a working email "
-"sender for Trac, supporting both TracAnnouncer and TracNotification."
+"For admin notification on registration time it relies on a\n"
+"                  working email sender for Trac, supporting both "
+"TracAnnouncer\n"
+"                  and TracNotification."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:736
-#: acct_mgr/templates/jinja2/account_config.html:823
+#: acct_mgr/templates/account_config.html:718
 msgid "Force users to verify their email addresses."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:739
-#: acct_mgr/templates/jinja2/account_config.html:826
+#: acct_mgr/templates/account_config.html:721
 msgid ""
-"For sending a verification token to the user it relies on a working email"
-" sender for Trac, supporting both TracAnnouncer and TracNotification."
+"For sending a verificaton token to the user it relies on a\n"
+"                working email sender for Trac, supporting both "
+"TracAnnouncer\n"
+"                and TracNotification."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:753
-#: acct_mgr/templates/jinja2/account_config.html:841
-#, fuzzy
-msgid "Account guard"
-msgstr "Compte"
+#: acct_mgr/templates/account_config.html:734
+msgid "Account guard icon"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:755
-#: acct_mgr/templates/jinja2/account_config.html:844
+#: acct_mgr/templates/account_config.html:737
 msgid "Objective for Account Protection rules"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:756
-#: acct_mgr/templates/jinja2/account_config.html:846
+#: acct_mgr/templates/account_config.html:738
 msgid ""
-"Passwords are often not constructed as carefully as they should be. And "
-"even a strong passphrase could be sift out, if an attacker is able to "
-"test millions of variants in hours, if not seconds. Firewalls and full-"
-"featured web-servers already offer sophisticated protection, if one can "
-"afford them, handle their installation, configuration and maintenance."
+"Passwords are often not constructed as carefully as they should\n"
+"              be.  And even a strong passphrase could be sift out, if"
+" an\n"
+"              attacker is able to test millions of variants in hours,"
+" if not\n"
+"              seconds.  Firewalls and full-featured web-servers "
+"already offer\n"
+"              sophisticated protection, if one can afford them, "
+"handle their\n"
+"              installation, configuration and maintenance."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:766
-#: acct_mgr/templates/jinja2/account_config.html:857
+#: acct_mgr/templates/account_config.html:746
 msgid ""
-"The [1:AccountGuard] component is another option. It is an add-on to "
-"AccountManagerPlugin's own [2:LoginModule] and provides account "
-"protection by discouraging brute-force login attempts."
+"The [1:AccountGuard] component is another option.\n"
+"              It is an add-on to AccountManagerPlugin's own\n"
+"              [2:LoginModule] and provides account protection\n"
+"              by discouraging brute-force login attempts."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:779
-#: acct_mgr/templates/jinja2/account_config.html:872
+#: acct_mgr/templates/account_config.html:759
 msgid "Enable the guard add-on component."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:782
-#: acct_mgr/templates/jinja2/account_config.html:876
+#: acct_mgr/templates/account_config.html:762
 msgid "AccountManagerPlugin's LoginModule is disabled."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:788
-#: acct_mgr/templates/jinja2/account_config.html:883
-#, fuzzy
+#: acct_mgr/templates/account_config.html:768
 msgid "Failed login attempt count max:"
-msgstr "Nombre de tentatives ayant échoué : %(count)s"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:795
-#: acct_mgr/templates/jinja2/account_config.html:891
+#: acct_mgr/templates/account_config.html:775
 msgid ""
-"Lock user account after the specified number of failed attempts. Value "
-"zero means [1:no limit]."
+"Lock user account after the specified number of failed\n"
+"                  attempts.  Value zero means [1:no limit]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:802
-#: acct_mgr/templates/jinja2/account_config.html:902
-msgid "Drop lock after [1:] seconds"
+#: acct_mgr/templates/account_config.html:782
+msgid ""
+"Drop lock after\n"
+"                    [1:]\n"
+"                    seconds"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:808
-#: acct_mgr/templates/jinja2/account_config.html:909
+#: acct_mgr/templates/account_config.html:789
 msgid "Zero means [1:unlimited] lock time here."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:814
-#: acct_mgr/templates/jinja2/account_config.html:916
+#: acct_mgr/templates/account_config.html:795
 msgid "Lock time progression factor:"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:821
-#: acct_mgr/templates/jinja2/account_config.html:922
+#: acct_mgr/templates/account_config.html:802
 msgid ""
-"Extend user account lock duration incrementally. It uses logarithmic "
-"calculation with the factor as exponent, accepting decimal numbers >= 1."
+"Extend user account lock duration incrementally.\n"
+"                      It uses logarithmic calculation with the factor"
+" as\n"
+"                      exponent, accepting decimal numbers >= 1."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:827
-#: acct_mgr/templates/jinja2/account_config.html:929
+#: acct_mgr/templates/account_config.html:807
 msgid ""
-"[1:Lock time will grow for any value > 1, if the failure happens before "
-"lock expiration. I.e. value '2' means][2:[3:[4:double lock time after 2nd"
-" failure,]][5:[6:four times the initial lock time after 3rd,]][7:[8:eight"
-" times as long after 4th failure, etc.]]]"
+"Lock time will grow for any value > 1, if the failure\n"
+"                      happens before lock expiration.  I.e. value '2'"
+" means"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:842
-#: acct_mgr/templates/jinja2/account_config.html:946
+#: acct_mgr/templates/account_config.html:811
 msgid ""
-"At any time after lock expiration a login failure will just trigger a "
-"lock and set a new lock timeout, but not extend the total lock duration."
+"[1:[2:\n"
+"                        double lock time after 2nd failure,]\n"
+"                      ]\n"
+"                      [3:[4:\n"
+"                        four times the initial lock time after 3rd,]\n"
+"                      ]\n"
+"                      [5:[6:\n"
+"                        eight times as long after 4th failure, etc.]\n"
+"                      ]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:854
-#: acct_mgr/templates/jinja2/account_config.html:958
-#, python-format
-msgid "Upper lock time limit: [1:] seconds [2:(%(time)s)]"
+#: acct_mgr/templates/account_config.html:822
+msgid ""
+"At any time after lock expiration a login failure will\n"
+"                      just trigger a lock and set a new lock timeout,"
+" but not\n"
+"                      extend the total lock duration."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:832
+msgid "Upper lock time limit:"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:867
-#: acct_mgr/templates/jinja2/account_config.html:969
+#: acct_mgr/templates/account_config.html:837
+msgid "seconds"
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:845
 msgid "This is relevant only with a progression factor > 1."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:882
-#: acct_mgr/templates/jinja2/account_config.html:986
+#: acct_mgr/templates/account_config.html:860
 msgid "Objective for additional preparation"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:883
-#: acct_mgr/templates/jinja2/account_config.html:988
+#: acct_mgr/templates/account_config.html:861
 msgid "Enable yourself to proceed beyond this initial setup."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:884
-#: acct_mgr/templates/jinja2/account_config.html:990
-#, fuzzy
+#: acct_mgr/templates/account_config.html:864
 msgid "Initial Admin Account"
-msgstr "S'inscrire"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:886
-#: acct_mgr/templates/jinja2/account_config.html:992
+#: acct_mgr/templates/account_config.html:866
 msgid "Add Admin Account:"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:887
-#: acct_mgr/templates/jinja2/account_config.html:995
+#: acct_mgr/templates/account_config.html:867
 msgid ""
-"The user will get [1:TRAC_ADMIN] assigned, that inherits all available "
-"permissions. One such account is required to configure Trac via the admin"
-" web-UI. Create and manage more limited admin accounts as well as actual "
-"user accounts on your own later via the Accounts admin panel."
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:895
-#: acct_mgr/templates/jinja2/account_config.html:1006
-msgid ""
-"In detail: AccountManagerPlugin requires [1:ACCTMGR_USER_ADMIN] for "
-"regular user administration, [2:ACCTMGR_CONFIG_ADMIN] for viewing these "
-"pages and changing the configuration later. Both are inherited by "
-"[3:ACCTMGR_ADMIN] permission. To assign permissions you'll need "
-"[4:PERMISSION_GRANT] inherited by [5:PERMISSION_ADMIN] too."
-msgstr ""
-
-#: acct_mgr/templates/genshi/account_config.html:906
-#: acct_mgr/templates/genshi/account_login.html:30
-#: acct_mgr/templates/genshi/account_register.html:33
-#: acct_mgr/templates/genshi/account_reset_password.html:29
-#: acct_mgr/templates/genshi/account_users.html:83
-#: acct_mgr/templates/jinja2/account_config.html:1017
-#: acct_mgr/templates/jinja2/account_login.html:33
-#: acct_mgr/templates/jinja2/account_register.html:40
-#: acct_mgr/templates/jinja2/account_reset_password.html:35
-#: acct_mgr/templates/jinja2/account_users.html:21
+"The user will get [1:TRAC_ADMIN] assigned, that\n"
+"                  inherits all available permissions.  One such "
+"account is\n"
+"                  required to configure Trac via the admin web-UI.  "
+"Create and\n"
+"                  manage more limitted admin accounts as well as "
+"actual user\n"
+"                  accounts on your own later via the Accounts admin "
+"panel."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:874
+msgid ""
+"In detail: AccountManagerPlugin requires\n"
+"                  [1:ACCTMGR_USER_ADMIN] for regular user\n"
+"                  administration, [2:ACCTMGR_CONFIG_ADMIN] for\n"
+"                  viewing these pages and changing the configuration "
+"later.\n"
+"                  Both are inherited by [3:ACCTMGR_ADMIN]\n"
+"                  permission.  To assign permissions you'll need\n"
+"                  [4:PERMISSION_GRANT] inherited by\n"
+"                  [5:PERMISSION_ADMIN] too."
+msgstr ""
+
+#: acct_mgr/templates/account_config.html:885
+#: acct_mgr/templates/account_login.html:33
+#: acct_mgr/templates/account_register.html:36
+#: acct_mgr/templates/account_reset_password.html:32
+#: acct_mgr/templates/account_users.html:86
 msgid "Username:"
-msgstr "Utilisateur :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:910
-#: acct_mgr/templates/genshi/account_register.html:38
-#: acct_mgr/templates/genshi/account_users.html:87
-#: acct_mgr/templates/jinja2/account_config.html:1023
-#: acct_mgr/templates/jinja2/account_register.html:46
-#: acct_mgr/templates/jinja2/account_users.html:27
+#: acct_mgr/templates/account_config.html:889
+#: acct_mgr/templates/account_register.html:41
+#: acct_mgr/templates/account_users.html:90
 msgid "Only lowercase usernames allowed"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:927
-#: acct_mgr/templates/jinja2/account_config.html:1043
+#: acct_mgr/templates/account_config.html:908
 msgid ""
-"Please take care, that the username is known by the HTTP authentication "
-"provider."
+"Please take care, that the username is known by the HTTP\n"
+"                  authentication provider."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:932
-#: acct_mgr/templates/jinja2/account_config.html:1049
+#: acct_mgr/templates/account_config.html:912
 msgid ""
-"Please take care for a valid username, because no configured password "
-"store supports creating a new account."
+"Please take care for a valid username, because no\n"
+"                  configured password store supports creating a new "
+"account."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:938
-#: acct_mgr/templates/genshi/account_users.html:130
-#: acct_mgr/templates/jinja2/account_config.html:1055
-#: acct_mgr/templates/jinja2/account_users.html:69
+#: acct_mgr/templates/account_config.html:917
+#: acct_mgr/templates/account_users.html:133
 msgid " Add "
-msgstr "Ajouter"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:942
-#: acct_mgr/templates/jinja2/account_config.html:1061
+#: acct_mgr/templates/account_config.html:922
 msgid "Check-up"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:951
-#: acct_mgr/templates/jinja2/account_config.html:1077
+#: acct_mgr/templates/account_config.html:931
 msgid "Please resolve all issues marked as critical."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:955
-#: acct_mgr/templates/jinja2/account_config.html:1085
+#: acct_mgr/templates/account_config.html:935
 msgid ""
-"By now you did almost finish AccountManagerPlugin configuration, but any "
-"changes are temporary yet. Please test and adjust the configuration as "
-"required, or cancel to revert all changes. Apply settings to [1:trac.ini]"
-" only if you really want to preserve them permanently."
+"By now you did almost finish AccountManagerPlugin\n"
+"                configuration, but any changes are temporary yet. "
+"Please test\n"
+"                and adjust the configuration as required, or cancel "
+"to revert\n"
+"                all changes.  Apply settings to [1:trac.ini] only if "
+"you\n"
+"                really want to preserve them permanently."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:993
-#: acct_mgr/templates/jinja2/account_config.html:1128
+#: acct_mgr/templates/account_config.html:978
 msgid "Stay on page"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:997
-#: acct_mgr/templates/jinja2/account_config.html:1138
+#: acct_mgr/templates/account_config.html:981
 msgid "Save changes and exit wizard"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:1002
-#: acct_mgr/templates/jinja2/account_config.html:1131
+#: acct_mgr/templates/account_config.html:985
 msgid "Drop unsaved changes"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:1010
-#: acct_mgr/templates/jinja2/account_config.html:1142
+#: acct_mgr/templates/account_config.html:991
 msgid "Drop changes and exit wizard"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_config.html:1010
-#: acct_mgr/templates/jinja2/account_config.html:1143
+#: acct_mgr/templates/account_config.html:991
 msgid "Cancel"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:11
-#: acct_mgr/templates/genshi/account_db_cleanup.html:15
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:7
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:14
+#: acct_mgr/templates/account_db_cleanup.html:14
+#: acct_mgr/templates/account_db_cleanup.html:18
 msgid "Accounts: Cleanup"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:27
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:27
+#: acct_mgr/templates/account_db_cleanup.html:30
 msgid "Attribute"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:28
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:28
+#: acct_mgr/templates/account_db_cleanup.html:31
 msgid "Value"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:62
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:33
+#: acct_mgr/templates/account_db_cleanup.html:65
 msgid "Authenticated Accounts"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:94
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:60
+#: acct_mgr/templates/account_db_cleanup.html:97
 msgid "Remove selected entries"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_db_cleanup.html:96
-#: acct_mgr/templates/jinja2/account_db_cleanup.html:62
+#: acct_mgr/templates/account_db_cleanup.html:99
 msgid "Undo selection"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_login.html:11
-#: acct_mgr/templates/genshi/account_login.html:23
-#: acct_mgr/templates/genshi/account_login.html:50
-#: acct_mgr/templates/jinja2/account_login.html:7
-#: acct_mgr/templates/jinja2/account_login.html:24
-#: acct_mgr/templates/jinja2/account_login.html:58
+#: acct_mgr/templates/account_login.html:14
+#: acct_mgr/templates/account_login.html:26
+#: acct_mgr/templates/account_login.html:54
 msgid "Login"
-msgstr "Connexion"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_login.html:47
-#: acct_mgr/templates/jinja2/account_login.html:54
+#: acct_mgr/templates/account_login.html:51
 msgid "Remember me"
-msgstr "Se souvenir de moi"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_login.html:70
-#: acct_mgr/templates/genshi/account_register.html:24
-#: acct_mgr/templates/jinja2/account_login.html:82
-#: acct_mgr/templates/jinja2/account_register.html:28
+#: acct_mgr/templates/account_login.html:79
+#: acct_mgr/templates/account_register.html:27
 msgid "Error"
-msgstr "Erreur"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:11
-#: acct_mgr/templates/genshi/account_notification.html:15
-#: acct_mgr/templates/jinja2/account_notification.html:7
-#: acct_mgr/templates/jinja2/account_notification.html:14
+#: acct_mgr/templates/account_notification.html:14
+#: acct_mgr/templates/account_notification.html:18
 msgid "Accounts: Notification Configuration"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:19
-#: acct_mgr/templates/jinja2/account_notification.html:20
+#: acct_mgr/templates/account_notification.html:22
 msgid "Account Notification"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:20
-#: acct_mgr/templates/jinja2/account_notification.html:22
+#: acct_mgr/templates/account_notification.html:23
 msgid ""
-"Set the following options in order to be notified of account creation, "
-"password reset and account deletion."
+"Set the following options in order to be notified of\n"
+"          account creation, password reset and account deletion."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:26
-#: acct_mgr/templates/jinja2/account_notification.html:27
+#: acct_mgr/templates/account_notification.html:26
 msgid "Notification Actions"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:27
-#: acct_mgr/templates/jinja2/account_notification.html:30
+#: acct_mgr/templates/account_notification.html:27
 msgid ""
-"This is a list of actions which you can enable or disable by [1:checking]"
-" the [2:checkboxes]."
+"This is a list of actions which you can\n"
+"          enable or disable by [1:checking] the [2:checkboxes]."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:33
-#: acct_mgr/templates/jinja2/account_notification.html:39
+#: acct_mgr/templates/account_notification.html:31
 msgid "Get notified of new account creation"
-msgstr "Être notifié de la création de compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:39
-#: acct_mgr/templates/jinja2/account_notification.html:45
+#: acct_mgr/templates/account_notification.html:35
 msgid "Get notified of password reset"
-msgstr "Être notifié de la réinitialisation de mot de passe"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:45
-#: acct_mgr/templates/jinja2/account_notification.html:51
+#: acct_mgr/templates/account_notification.html:39
 msgid "Get notified of account deletion"
-msgstr "Être notifié de la suppression de compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:49
-#: acct_mgr/templates/jinja2/account_notification.html:54
+#: acct_mgr/templates/account_notification.html:42
 msgid "Notification Recipient Addresses"
-msgstr "Adresse pour les notifications"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_notification.html:50
-#: acct_mgr/templates/jinja2/account_notification.html:56
-#, fuzzy
+#: acct_mgr/templates/account_notification.html:43
 msgid ""
-"Space-separated list of email addresses and/or usernames that get "
-"notified of the above actions:"
+"Space-separated list of email addresses and/or\n"
+"          usernames that get notified of the above actions:"
 msgstr ""
-"Liste d'emails séparés par des espaces et/ou noms d'utilisateurs qui "
-"seront notifié des actions suivantes :"
 
-#: acct_mgr/templates/genshi/account_prefs.html:19
-#: acct_mgr/templates/jinja2/account_prefs.html:45
+#: acct_mgr/templates/account_prefs.html:23
 msgid "Delete Account"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_prefs.html:30
-#: acct_mgr/templates/jinja2/account_prefs.html:57
+#: acct_mgr/templates/account_prefs.html:34
 msgid "Delete account"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_prefs.html:49
-#: acct_mgr/templates/jinja2/account_prefs.html:22
+#: acct_mgr/templates/account_prefs.html:53
 msgid "Change Password"
-msgstr "Changer de mot de passe"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_prefs.html:51
-#: acct_mgr/templates/jinja2/account_prefs.html:25
+#: acct_mgr/templates/account_prefs.html:55
 msgid "Old Password:"
-msgstr "Ancien mot de passe :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_prefs.html:57
-#: acct_mgr/templates/jinja2/account_prefs.html:29
+#: acct_mgr/templates/account_prefs.html:61
 msgid "New Password:"
-msgstr "Nouveau mot de passe :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_register.html:21
-#: acct_mgr/templates/jinja2/account_register.html:24
+#: acct_mgr/templates/account_register.html:24
 msgid "Register an account"
-msgstr "S'inscrire"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_register.html:30
-#: acct_mgr/templates/jinja2/account_register.html:36
+#: acct_mgr/templates/account_register.html:33
 msgid "Required"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_register.html:61
-#: acct_mgr/templates/jinja2/account_register.html:71
+#: acct_mgr/templates/account_register.html:64
 msgid "Optional"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_register.html:63
-#: acct_mgr/templates/jinja2/account_register.html:74
+#: acct_mgr/templates/account_register.html:66
 msgid "Name:"
-msgstr "Nom :"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_register.html:74
-#: acct_mgr/templates/jinja2/account_register.html:86
+#: acct_mgr/templates/account_register.html:77
 msgid "Create account"
-msgstr "Créer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_reset_password.html:11
-#: acct_mgr/templates/genshi/account_reset_password.html:21
-#: acct_mgr/templates/jinja2/account_reset_password.html:7
-#: acct_mgr/templates/jinja2/account_reset_password.html:24
+#: acct_mgr/templates/account_reset_password.html:14
+#: acct_mgr/templates/account_reset_password.html:24
 msgid "Reset Password"
-msgstr "Réinitialiser le mot de passe"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_reset_password.html:22
-#: acct_mgr/templates/jinja2/account_reset_password.html:26
+#: acct_mgr/templates/account_reset_password.html:25
 msgid ""
-"If you've forgotten your password, enter your username and email address "
-"below, and a new password will be sent to you."
+"If you've forgotten your password, enter your username and\n"
+"        email address below, and a new password will be sent to you."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_reset_password.html:40
-#: acct_mgr/templates/jinja2/account_reset_password.html:46
+#: acct_mgr/templates/account_reset_password.html:43
 msgid "Reset password"
-msgstr "Réinitialiser le mot de passe"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:21
-#: acct_mgr/templates/jinja2/account_user_table.html:19
+#: acct_mgr/templates/account_user_table.html:21
 msgid "Name"
-msgstr "Nom"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:22
-#: acct_mgr/templates/jinja2/account_user_table.html:22
+#: acct_mgr/templates/account_user_table.html:22
 msgid "Email"
-msgstr "Adresse email"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:23
-#: acct_mgr/templates/jinja2/account_user_table.html:24
+#: acct_mgr/templates/account_user_table.html:23
 msgid "Last Login"
-msgstr "Dernière connexion"
+msgstr ""
+
+#: acct_mgr/templates/account_user_table.html:28
+msgid "Email not verified"
+msgstr ""
+
+#: acct_mgr/templates/account_user_table.html:28
+msgid "Approval pending"
+msgstr ""
+
+#: acct_mgr/templates/account_user_table.html:28
+msgid "Approval revoked"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:51
-#: acct_mgr/templates/jinja2/account_user_table.html:57
-#: acct_mgr/templates/jinja2/account_user_table.html:58
+#: acct_mgr/templates/account_user_table.html:48
 msgid "Permanently locked"
-msgstr "Bloqué définitivement"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_user_table.html:58
-#: acct_mgr/templates/jinja2/account_user_table.html:70
-#, fuzzy
+#: acct_mgr/templates/account_user_table.html:55
 msgid "Send email"
-msgstr "Renvoyer email"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:81
-#: acct_mgr/templates/jinja2/account_users.html:18
-#, fuzzy
+#: acct_mgr/templates/account_users.html:84
 msgid "Add New Account:"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:138
-#: acct_mgr/templates/jinja2/account_users.html:78
+#: acct_mgr/templates/account_users.html:141
 msgid "This password store does not support listing users."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:143
-#: acct_mgr/templates/jinja2/account_users.html:86
+#: acct_mgr/templates/account_users.html:146
 msgid "Max accounts per page [1:]"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:149
-#: acct_mgr/templates/genshi/account_users.html:172
-#: acct_mgr/templates/jinja2/account_users.html:90
-#: acct_mgr/templates/jinja2/account_users.html:123
+#: acct_mgr/templates/account_users.html:152
+#: acct_mgr/templates/account_users.html:175
 msgid "Update"
 msgstr ""
 
-#. Position (# to # of #) or total, if not paginating
-#: acct_mgr/templates/genshi/account_users.html:155
-#: acct_mgr/templates/jinja2/account_users.html:100
-#, python-format
-msgid "Accounts [1:(%(count)s)]"
+#: acct_mgr/templates/account_users.html:164
+msgid "Filters"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:161
-#: acct_mgr/templates/genshi/account_users.html:162
-#: acct_mgr/templates/jinja2/account_users.html:107
-#: acct_mgr/templates/jinja2/account_users.html:108
-msgid "Filters"
+#: acct_mgr/templates/account_users.html:165
+msgid "Account filters"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:163
-#: acct_mgr/templates/jinja2/account_users.html:109
+#: acct_mgr/templates/account_users.html:166
 msgid "Status"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:186
-#: acct_mgr/templates/jinja2/account_users.html:148
+#: acct_mgr/templates/account_users.html:190
 msgid "Send another random password"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:186
-#: acct_mgr/templates/jinja2/account_users.html:149
+#: acct_mgr/templates/account_users.html:190
 msgid "Reset passwords"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:190
-#: acct_mgr/templates/jinja2/account_users.html:152
+#: acct_mgr/templates/account_users.html:194
 msgid "Approve pending registrations, ban/unban accounts"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:190
-#: acct_mgr/templates/jinja2/account_users.html:153
+#: acct_mgr/templates/account_users.html:194
 msgid "Toggle account approval"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:193
-#: acct_mgr/templates/jinja2/account_users.html:156
-#, fuzzy
+#: acct_mgr/templates/account_users.html:197
 msgid "Delete accounts"
-msgstr "Supprimer compte"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:193
-#: acct_mgr/templates/jinja2/account_users.html:157
-#, fuzzy
+#: acct_mgr/templates/account_users.html:197
 msgid "Remove selected items"
-msgstr "Supprimer les comptes sélectionnés"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_users.html:197
-#: acct_mgr/templates/jinja2/account_users.html:161
+#: acct_mgr/templates/account_users.html:202
 msgid "Review account attributes"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_verify_email.html:11
-#: acct_mgr/templates/genshi/account_verify_email.html:21
-#: acct_mgr/templates/jinja2/account_verify_email.html:7
-#: acct_mgr/templates/jinja2/account_verify_email.html:23
+#: acct_mgr/templates/account_verify_email.html:14
+#: acct_mgr/templates/account_verify_email.html:25
 msgid "Verify Email"
-msgstr "Vérifier email"
+msgstr ""
 
-#: acct_mgr/templates/genshi/account_verify_email.html:23
-#: acct_mgr/templates/jinja2/account_verify_email.html:26
+#: acct_mgr/templates/account_verify_email.html:27
 #, python-format
 msgid ""
-"An email was sent to %(email)s with a token to verify your new address. "
-"Please check your email and enter the token in the form below."
+"An email was sent to\n"
+"        %(email)s with a token to verify your new address.\n"
+"        Please check your email and enter the token in the form below."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_verify_email.html:29
-#: acct_mgr/templates/jinja2/account_verify_email.html:33
-msgid "You can [1:change your email address], if it is incorrect."
+#: acct_mgr/templates/account_verify_email.html:30
+msgid ""
+"You can [1:change your\n"
+"        email address], if it is incorrect."
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_verify_email.html:34
-#: acct_mgr/templates/jinja2/account_verify_email.html:41
+#: acct_mgr/templates/account_verify_email.html:35
 msgid "Verification Token:"
 msgstr ""
 
-#: acct_mgr/templates/genshi/account_verify_email.html:39
-#: acct_mgr/templates/jinja2/account_verify_email.html:47
+#: acct_mgr/templates/account_verify_email.html:40
 msgid "Verify"
-msgstr "Vérifier"
-
-#: acct_mgr/templates/genshi/account_verify_email.html:41
-#: acct_mgr/templates/jinja2/account_verify_email.html:49
-msgid "Resend Email"
-msgstr "Renvoyer email"
-
-#: acct_mgr/templates/jinja2/account_user_table.html:32
-msgid "Email not verified"
-msgstr ""
-
-#: acct_mgr/templates/jinja2/account_user_table.html:34
-msgid "Approval pending"
 msgstr ""
 
-#: acct_mgr/templates/jinja2/account_user_table.html:36
-msgid "Approval revoked"
+#: acct_mgr/templates/account_verify_email.html:42
+msgid "Resend Email"
 msgstr ""
 
-#~ msgid "Please change your password now."
-#~ msgstr "Merci changer votre mot de passe maintenant."
-
-#~ msgid "Already logged in"
-#~ msgstr "Déjà connecté"
-
-#~ msgid "The \"crypt\" module is unavailable on this platform."
-#~ msgstr "Le module \"crypt\" n'est pas disponible sur cette plateforme."
-
-#~ msgid ""
-#~ "Drop lock after\n"
-#~ "                    [1:]\n"
-#~ "                    seconds"
-#~ msgstr ""
-#~ "Compte bloqué. Merci de recommencer dans\n"
-#~ "%(release_time) sec.\n"
-#~ " "
-
-#~ msgid "Account filters"
-#~ msgstr "Compte bloqué"
-
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/macros.py` & `TracAccountManager-0.6.dev0/acct_mgr/macros.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
-from trac.core import Component, implements
+from trac.core import implements
 from trac.perm import PermissionSystem
 from trac.util.html import html as tag
 from trac.web.chrome import Chrome
 from trac.wiki.api import IWikiMacroProvider, WikiSystem, parse_args
 from trac.wiki.formatter import format_to_oneliner
 
-from .admin import fetch_user_data
-from .api import AccountManager, tag_
-from .guard import AccountGuard
+from acct_mgr.admin import fetch_user_data
+from acct_mgr.api import AccountManager, CommonTemplateProvider, tag_
+from acct_mgr.guard import AccountGuard
 
 
-class AccountManagerWikiMacros(Component):
+class AccountManagerWikiMacros(CommonTemplateProvider):
     """Provides wiki macros related to Trac accounts/authenticated users."""
 
     implements(IWikiMacroProvider)
 
     # IWikiMacroProvider
 
     def get_macros(self):
@@ -60,15 +60,15 @@
  no match and output style isn't 'count' either
 
 'count' is also recognized without prepended key name. Other non-keyed
 parameters are:
  * '''locked''' -- alias for 'locked=True'
  * '''visit''' -- show a list of accounts with last-login information, only
  available in table format
- * '''name''' -- forces replacement of matching username with their
+ * '''name''' -- forces replacement of maching username with their
  corresponding full names, if available; adds a full names column if combined
  with 'visit'
  * '''email''' -- append email address to usernames, if available
 
 Requires `USER_VIEW` permission for output in any format other then 'count'.
 A misc placeholder with this statement is presented to unprivileged users.
 """
@@ -78,40 +78,40 @@
         req = formatter.req
         if not content:
             args = []
             kw = {}
         else:
             args, kw = parse_args(content)
         if name == 'ProjectStats':
-            if 'wiki' in kw:
-                prefix = 'prefix' in kw and kw['prefix'] or None
+            if 'wiki' in kw.keys():
+                prefix = 'prefix' in kw.keys() and kw['prefix'] or None
                 wiki = WikiSystem(env)
                 if kw['wiki'] == 'count' or 'count' in args:
                     return tag(len(list(wiki.get_pages(prefix))))
         elif name == 'UserQuery':
             msg_no_perm = tag.p(tag_("(required %(perm)s missing)",
                                      perm=tag.strong('USER_VIEW')),
                                 class_='hint')
-            if 'perm' in kw:
+            if 'perm' in kw.keys():
                 perm_sys = PermissionSystem(self.env)
                 users = perm_sys.get_users_with_permission(kw['perm'].upper())
             else:
                 acct_mgr = AccountManager(env)
                 users = list(set(acct_mgr.get_users()))
-            if 'locked' in kw or 'locked' in args:
+            if 'locked' in kw.keys() or 'locked' in args:
                 guard = AccountGuard(env)
                 locked = []
                 for user in users:
                     if guard.user_locked(user):
                         locked.append(user)
                 if kw.get('locked', 'True').lower() in ('true', 'yes', '1'):
                     users = locked
                 else:
                     users = list(set(users) - set(locked))
-            elif 'visit' in kw or 'visit' in args:
+            elif 'visit' in kw.keys() or 'visit' in args:
                 if 'USER_VIEW' not in req.perm:
                     return msg_no_perm
                 cols = []
                 data = {'accounts': fetch_user_data(env, req), 'cls': 'wiki'}
                 for col in ('email', 'name'):
                     if col in args:
                         cols.append(col)
@@ -130,15 +130,15 @@
                             name = username
                         if 'email' in args and email is not None:
                             email = ''.join(['<', email, '>'])
                             name = ' '.join([name, email])
                         if not username == name:
                             users.pop(users.index(username))
                             users.append(name)
-            if not users and 'nomatch' in kw:
+            if not users and 'nomatch' in kw.keys():
                 return format_to_oneliner(env, formatter.context,
                                           kw['nomatch'])
             users = sorted(users)
             if kw.get('format') == 'list':
                 return tag.ul([tag.li(Chrome(env).format_author(req, user))
                                for user in users])
             else:
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/model.py` & `TracAccountManager-0.6.dev0/acct_mgr/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 
 import hashlib
 import re
 
+from acct_mgr.api import GenericUserIdChanger
 from trac.util import as_int
 from trac.util.text import exception_to_unicode, to_unicode
 
-from .api import GenericUserIdChanger
-from .compat import iteritems
-
-
 _USER_KEYS = {
     'auth_cookie': 'name',
     'permission': 'username',
 }
 
 
 def _get_cc_list(cc_value):
@@ -61,15 +58,15 @@
                         db("UPDATE %s SET %s=%%s WHERE %s=%%s"
                            % (self.table, self.column, self.column),
                            (new_uid, old_uid))
                     result = int(count)
                 self.log.debug(self.msg(old_uid, new_uid, self.table,
                                         self.column,
                                         result='%s time(s)' % result))
-        except _get_db_exc(self.env) as e:
+        except _get_db_exc(self.env), e:
             result = exception_to_unicode(e)
             msg = 'failed: %s' % exception_to_unicode(e, traceback=True)
             self.log.debug(self.msg(old_uid, new_uid, self.table,
                                     self.column, result=msg))
             return dict(error={(self.table, self.column, None): result})
         return {(self.table, self.column, None): result}
 
@@ -83,15 +80,15 @@
 
     # IUserIdChanger method
     def replace(self, old_uid, new_uid):
         try:
             self.env.db_transaction("""
                 DELETE FROM %s WHERE %s=%%s
                 """ % (self.table, self.column), (new_uid,))
-        except _get_db_exc(self.env) as e:
+        except _get_db_exc(self.env), e:
             result = exception_to_unicode(e)
             msg = 'failed: %s' % exception_to_unicode(e, traceback=True)
             self.log.debug(self.msg(old_uid, new_uid, self.table,
                                     self.column, result=msg))
             return dict(error={(self.table, self.column, None): result})
         return super(UniqueUserIdChanger, self).replace(old_uid, new_uid)
 
@@ -167,15 +164,15 @@
                 cc = _get_cc_list(row[1])
                 for i in [i for i, r in enumerate(cc) if r == old_uid]:
                     cc[i] = new_uid
                     try:
                         db("UPDATE ticket SET cc=%s WHERE id=%s",
                            (', '.join(cc), int(row[0])))
                         result += 1
-                    except _get_db_exc(self.env) as e:
+                    except _get_db_exc(self.env), e:
                         result = exception_to_unicode(e)
                         msg = 'failed: %s' \
                               % exception_to_unicode(e, traceback=True)
                         self.log.debug(
                             self.msg(old_uid, new_uid, self.table, 'cc',
                                      result=msg))
                         return dict(error={(self.table, 'cc', None): result})
@@ -202,15 +199,15 @@
                 if result:
                     try:
                         db("""
                             UPDATE %s SET %s=%%s
                             WHERE %s=%%s AND
                              (field='owner' OR field='reporter')
                             """ % (table, column, column), (new_uid, old_uid))
-                    except _get_db_exc(self.env) as e:
+                    except _get_db_exc(self.env), e:
                         result = exception_to_unicode(e)
                         msg = 'failed: %s' % \
                               exception_to_unicode(e, traceback=True)
                         self.log.debug(
                             self.msg(old_uid, new_uid, table, column,
                                      constraint, result=msg))
                         return dict(error={(self.table, column,
@@ -231,19 +228,19 @@
                               ('%' + db.like_escape(old_uid) + '%',)):
                     cc = _get_cc_list(row[2])
                     for i in [i for i, r in enumerate(cc) if r == old_uid]:
                         cc[i] = new_uid
                         try:
                             db("""
                                 UPDATE %s SET %s=%%s
-                                WHERE ticket=%%s AND time=%%s AND field='cc'
+                                WHERE ticket=%%s AND time=%%s
                                 """ % (table, column),
                                (', '.join(cc), int(row[0]), int(row[1])))
                             result += 1
-                        except _get_db_exc(self.env) as e:
+                        except _get_db_exc(self.env), e:
                             result = exception_to_unicode(e)
                             msg = 'failed: %s' % \
                                   exception_to_unicode(e, traceback=True)
                             self.log.debug(
                                 self.msg(old_uid, new_uid, table, column,
                                          constraint, result=msg))
                             return dict(error={(self.table, column,
@@ -381,15 +378,15 @@
             attrs_new = get_user_attribute(env, new_uid)
             if not (attrs_new and new_uid in attrs_new and
                         attrs_new[new_uid].get(1)):
                 # No attributes found.
                 attrs_new = None
             # Remove value id hashes.
             attrs[username][1].pop('id')
-            for attribute, value in iteritems(attrs[username][1]):
+            for attribute, value in attrs[username][1].iteritems():
                 if not (attrs_new and attribute in attrs_new[new_uid][1]):
                     db("""
                         INSERT INTO session_attribute
                           (sid,authenticated,name,value)
                         VALUES (%s,1,%s,%s)
                         """, (new_uid, attribute, value))
                     count += 1
@@ -443,22 +440,22 @@
         %s
         """ % (sel_stmt, where_stmt)
     sql_args = tuple(constraints)
 
     def unique_id(*values):
         # Generate sha1 digest from NUL value1 NUL value2 NUL value3 NUL
         m = hashlib.sha1()
-        m.update(b'\0')
+        m.update('\0')
         for value in values:
-            if isinstance(value, str):
+            if isinstance(value, unicode):
                 value = value.encode('utf-8')
             elif not isinstance(value, str):
-                value = bytes([value])
+                value = str(value)
             m.update(value)
-            m.update(b'\0')
+            m.update('\0')
         return m.hexdigest()
 
     res = {}
     for row in env.db_query(sql, sql_args):
         if sel_stmt == 'COUNT(*)':
             return [row[0]]
         res_row = {}
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/notification.py` & `TracAccountManager-0.6.dev0/acct_mgr/notification.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from trac.config import ListOption
 from trac.core import Component, TracError, implements
 from trac.notification.api import (
     IEmailDecorator, INotificationFormatter, NotificationEvent,
     NotificationSystem)
 from trac.notification.mail import RecipientMatcher, set_header
 from trac.util.text import exception_to_unicode
-from trac.util.translation import deactivate, dgettext, reactivate
+from trac.util.translation import deactivate, reactivate
 from trac.web.chrome import Chrome
 
-from .api import IAccountChangeListener, _
-from .compat import iteritems, use_jinja2
-from .util import i18n_tag
+from acct_mgr.api import (
+    IAccountChangeListener, CommonTemplateProvider, _, dgettext)
+from acct_mgr.compat import genshi_template_args
 
 
 class NotificationError(TracError):
     pass
 
 
 class AccountChangeEvent(NotificationEvent):
@@ -58,18 +58,18 @@
     action_category_map = {
         'new': 'created',
         'change': 'password changed',
         'delete': 'deleted'
     }
 
     def __init__(self):
-        self._notify_categories = [category
-                                   for action, category
-                                   in iteritems(self.action_category_map)
-                                   if action in self._notify_actions]
+        self._notify_categories = []
+        for action, category in self.action_category_map.iteritems():
+            if action in self._notify_actions:
+                self._notify_categories.append(category)
 
     # IAccountChangeListener methods
 
     def user_created(self, username, password):
         data = {'password': password}
         self._send_notification('created', username, data)
 
@@ -164,36 +164,38 @@
         elif event.category == 'verify email':
             token = event.data['token']
             data['account']['token'] = token
             data['verify'] = {
                 'link': self.env.abs_href.verify_email(token=token, verify=1)
             }
             template_name = 'account_verify_email.txt'
-        t = deactivate()  # don't translate the e-mail stream
-        try:
-            return self._format_body(data, template_name)
-        finally:
-            reactivate(t)
+        return self._format_body(data, template_name)
 
     # Internal methods
 
     def _format_body(self, data, template_name):
+        # 3 commented lines are replacements for when Trac < 1.4 is dropped
         chrome = Chrome(self.env)
         data = chrome.populate_data(None, data)
-        if use_jinja2:
-            template = chrome.load_template(template_name, text=True)
-            body = chrome.render_template_string(template, data, text=True)
-            return body.encode('utf-8')
-        else:
-            template = chrome.load_template(template_name, method='text')
+        template = chrome.load_template(template_name, method='text')
+        #template = chrome.load_template(template_name, text=True)
+        t = deactivate()  # don't translate the e-mail stream
+        try:
             stream = template.generate(**data)
             return stream.render('text', encoding='utf-8')
+            #body = chrome.render_template_string(template, data, text=True)
+            #return body.encode('utf-8')
+        except Exception as e:
+            self.log.error("Failed to format body of notification mail: %s",
+                           exception_to_unicode(e, traceback=True))
+        finally:
+            reactivate(t)
 
 
-class AccountChangeNotificationAdminPanel(Component):
+class AccountChangeNotificationAdminPanel(CommonTemplateProvider):
     implements(IAdminPanelProvider)
 
     # IAdminPageProvider methods
 
     def get_admin_panels(self, req):
         if 'ACCTMGR_CONFIG_ADMIN' in req.perm:
             yield ('accounts', _("Accounts"), 'notification',
@@ -213,12 +215,13 @@
             self.config.save()
             req.redirect(req.href.admin('accounts', 'notification'))
 
         notify_addresses = cfg.getlist('account_changes_notify_addresses',
                                        sep=' ')
         notify_actions = cfg.getlist('notify_actions')
         data = {
-            'i18n_tag': i18n_tag,
+            '_dgettext': dgettext,
             'notify_actions': notify_actions,
             'notify_addresses': notify_addresses
         }
-        return 'account_notification.html', data
+        return genshi_template_args(self.env, 'account_notification.html',
+                                    data)
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/opt/announcer/uid_chg.py` & `TracAccountManager-0.6.dev0/acct_mgr/opt/announcer/uid_chg.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
 from announcer.api import AnnouncementSystem
 
-from ...api import _
-from ...model import PrimitiveUserIdChanger
+from acct_mgr.api import _
+from acct_mgr.model import PrimitiveUserIdChanger
 
 
 class TracAnnouncerUserIdChanger(PrimitiveUserIdChanger):
     """Change user IDs for TracAnnouncer tables, schema version > 2."""
 
     enabled = False
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/opt/radius.py` & `TracAccountManager-0.6.dev0/acct_mgr/opt/radius.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Chris Shenton <chris@koansys.com>
 
-from io import StringIO
+from StringIO import StringIO
 
+from acct_mgr.api import IPasswordStore
 from trac.config import IntOption, Option
 from trac.core import Component, implements
 from trac.util.text import unicode_passwd
 
-from ..api import IPasswordStore
-
-
 DICTIONARY = u"""
 ATTRIBUTE User-Name     1 string
 ATTRIBUTE User-Password 2 string encrypt=1
 """
 
 
 class RadiusAuthStore(Component):
@@ -59,15 +57,15 @@
     def check_password(self, username, password):
         """Checks if the password is valid for the user."""
         # Handle pyrad lib absence and upstream incompatibilities gracefully.
         try:
             import pyrad.packet
             from pyrad.client import Client, Timeout
             from pyrad.dictionary import Dictionary
-        except ImportError as e:
+        except ImportError, e:
             self.log.error("RADIUS auth store could not import pyrad, "
                            "need to install the egg: %s", e)
             return
 
         self.log.debug("RADIUS server=%s:%s (authport), secret='%s'",
                        self.radius_server, self.radius_authport,
                        self.radius_secret)
@@ -83,29 +81,29 @@
         req = client.CreateAuthPacket(code=pyrad.packet.AccessRequest,
                                       User_Name=username.encode('utf-8'))
         req['User-Password'] = req.PwCrypt(password)
 
         self.log.debug("RADIUS auth sending packet req=%s", req)
         try:
             reply = client.SendPacket(req)
-        except Timeout as e:
+        except Timeout, e:
             self.log.error("RADIUS timeout contacting server=%s:%s (%s)",
                            self.radius_server, self.radius_authport, e)
             return
         # DEVEL: Too broad, narrow down that exception handler scope.
-        except Exception as e:
+        except Exception, e:
             self.log.error("RADIUS error while using server=%s:%s: (%s)",
                            self.radius_server, self.radius_authport, e)
             return
         self.log.debug("RADIUS authentication reply code=%s", reply.code)
 
         if pyrad.packet.AccessAccept == reply.code:
             self.log.debug("RADIUS Accept for username=%s", username)
             return True
-        # Rejection of login attempt, stopping further auth store interaction.
+        # Rejection of login attempt, stopping further auth store interation.
         elif pyrad.packet.AccessReject == reply.code:
             self.log.debug("RADIUS Reject for username=%s", username)
             return False
         # DEVEL: Any way to alert users that RSA token is in 'Next Token' mode
         #        so they know to fix it?
         elif pyrad.packet.AccessChallenge == reply.code:
             self.log.info("RADIUS returned Challenge for username=%s; "
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/opt/tests/__init__.py` & `TracAccountManager-0.6.dev0/acct_mgr/opt/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 def test_suite():
     msg_fail = 'Issue with %s (%s): skipping acct_mgr.opt.tests.%s'
 
     suite = unittest.TestSuite()
 
     try:
         import acct_mgr.opt.tests.announcer
-    except ImportError as e:
+    except ImportError, e:
         print(msg_fail % ('UID changer for TracAnnouncer', e, 'announcer'))
     else:
         suite.addTest(acct_mgr.opt.tests.announcer.test_suite())
 
     try:
         import acct_mgr.opt.tests.tracforms
-    except ImportError as e:
+    except ImportError, e:
         print(msg_fail % ('UID changer for TracForms', e, 'tracforms'))
     else:
         suite.addTest(acct_mgr.opt.tests.tracforms.test_suite())
 
     try:
         import acct_mgr.opt.tests.tracscreenshots
-    except ImportError as e:
+    except ImportError, e:
         print(msg_fail % ('UID changer for TracScreenshots', e,
                           'tracscreenshots'))
     else:
         suite.addTest(acct_mgr.opt.tests.tracscreenshots.test_suite())
 
     try:
         import acct_mgr.opt.tests.tracvote
-    except ImportError as e:
+    except ImportError, e:
         print(msg_fail % ('UID changer for TracVote', e, 'tracvote'))
     else:
         suite.addTest(acct_mgr.opt.tests.tracvote.test_suite())
 
     try:
         import acct_mgr.opt.tests.radius
-    except ImportError as e:
+    except ImportError, e:
         print(msg_fail % ('RADIUS auth', e, 'radius'))
     else:
         suite.addTest(acct_mgr.opt.tests.radius.test_suite())
     return suite
 
 
 # Start test suite directly from command line like so:
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/opt/tests/radius.py` & `TracAccountManager-0.6.dev0/acct_mgr/opt/tests/radius.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
 import os.path
 import shutil
 import tempfile
 import unittest
 
+from acct_mgr.opt.radius import RadiusAuthStore
 from trac.test import EnvironmentStub
 
-from ..radius import RadiusAuthStore
-
 
 class _BaseTestCase(unittest.TestCase):
     def setUp(self):
         self.basedir = os.path.realpath(tempfile.mkdtemp())
         self.env = EnvironmentStub(default_data=True, enable=
             ['trac.*', 'acct_mgr.api.*',
              'acct_mgr.opt.radius.RadiusAuthStore'])
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/opt/tracforms/uid_chg.py` & `TracAccountManager-0.6.dev0/acct_mgr/opt/tracforms/uid_chg.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
 from tracforms.tracdb import DBComponent
 
-from ...api import _
-from ...model import PrimitiveUserIdChanger
+from acct_mgr.api import _
+from acct_mgr.model import PrimitiveUserIdChanger
 
 
 class TracFormsUserIdChanger(PrimitiveUserIdChanger):
     """Change user IDs for TracForms tables, schema version > 12."""
 
     enabled = False
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/register.py` & `TracAccountManager-0.6.dev0/acct_mgr/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 #
 # Author: Matthew Good <trac@matt-good.net>
 
 import base64
 import os
 import re
 
+from acct_mgr.api import AccountManager, CommonTemplateProvider
+from acct_mgr.api import IAccountRegistrationInspector
+from acct_mgr.api import _, N_, cleandoc_, dgettext, tag_
+from acct_mgr.model import email_associated, get_user_attribute
+from acct_mgr.model import set_user_attribute
+from acct_mgr.notification import NotificationError
+from acct_mgr.util import contains_any
 from trac import perm
 from trac.config import BoolOption, Option
 from trac.core import Component, TracError, implements
 from trac.util.html import html as tag
 from trac.util.text import exception_to_unicode
-from trac.web import HTTPBadRequest, auth, chrome
+from trac.web import auth, chrome
+from trac.web.api import HTTPBadRequest
 from trac.web.main import IRequestFilter, IRequestHandler
 
-from .api import (AccountManager, IAccountRegistrationInspector, _, N_,
-                  cleandoc_, tag_)
-from .compat import process_request_compat
-from .model import email_associated, get_user_attribute, set_user_attribute
-from .notification import NotificationError
-from .util import contains_any, i18n_tag
-
 
 class RegistrationError(TracError):
     """Exception raised when a registration check fails."""
 
     title = N_("Registration Error")
 
     def __init__(self, message, *args, **kwargs):
@@ -89,15 +90,15 @@
                 "%(chars)s", chars=tag.tt(' '.join(blacklist))))
 
         # All upper-cased names are reserved for permission action names.
         if username.isupper():
             raise RegistrationError(_("A username with only upper-cased "
                                       "characters is not allowed."))
 
-        # Prohibit some user names, that are important for Trac and therefore
+        # Prohibit some user names, that are important for Trac and therefor
         # reserved, even if not in the permission store for some reason.
         if username.lower() in ['anonymous', 'authenticated']:
             raise RegistrationError(tag_("Username %(username)s is not "
                                          "allowed.", username=tag.b(username)))
 
         # NOTE: A user may exist in a password store but not in the permission
         #   store.  I.e. this happens, when the user (from the password store)
@@ -130,20 +131,20 @@
     A collection of simple bot checks.
 
     ''This check is bypassed for requests by an authenticated user.''
     """)
 
     reg_basic_question = Option(
         'account-manager', 'register_basic_question', '',
-        doc=N_("A question to ask instead of the standard prompt, to which "
-               "the value of register_basic_token is the answer. Setting to "
-               "empty string (default value) keeps the standard prompt."))
+        doc="A question to ask instead of the standard prompt, to which "
+            "the value of register_basic_token is the answer. Setting to "
+            "empty string (default value) keeps the standard prompt.")
     reg_basic_token = Option(
         'account-manager', 'register_basic_token', '',
-        doc=N_("A string required as input to pass verification."))
+        doc="A string required as input to pass verification.")
 
     def render_registration_fields(self, req, data):
         """Add a hidden text input field to the registration form, and
         a visible one with mandatory input as well, if token is configured.
         """
         if self.reg_basic_token:
             # Preserve last input for editing on failure instead of typing
@@ -203,33 +204,35 @@
         """Add an email address text input field to the registration form."""
         # Preserve last input for editing on failure instead of typing
         # everything again.
         old_value = req.args.get('email', '').strip()
         insert = tag.label(_("Email:"),
                            tag.input(type='text', name='email', size=20,
                                      class_='textwidget', value=old_value))
-        # Deferred import required to avoid circular import dependencies.
-        from .web_ui import AccountModule
+        # Deferred import required to aviod circular import dependencies.
+        from acct_mgr.web_ui import AccountModule
         reset_password = AccountModule(self.env).reset_password_enabled
         verify_account = self.env.is_enabled(EmailVerificationModule) and \
                          EmailVerificationModule(self.env).verify_email
         if verify_account:
             # TRANSLATOR: Registration form hints for a mandatory input field.
-            hint = tag.p(_("The email address is required for Trac to send "
-                           "you a verification token."), class_='hint')
+            hint = tag.p(_("""
+                The email address is required for Trac to send you a
+                verification token.
+                """), class_='hint')
             if reset_password:
-                hint = tag(hint, tag.p(_("Entering your email address will "
-                                         "also enable you to reset your "
-                                         "password if you ever forget it."),
-                                       class_='hint'))
+                hint = tag(hint, tag.p(_("""
+                    Entering your email address will also enable you to reset
+                    your password if you ever forget it.
+                    """), class_='hint'))
             return tag(insert, hint), data
         elif reset_password:
             # TRANSLATOR: Registration form hint, if email input is optional.
-            hint = tag.p(_("Entering your email address will enable you to "
-                           "reset your password if you ever forget it."),
+            hint = tag.p(_("""Entering your email address will enable you to
+                           reset your password if you ever forget it."""),
                          class_='hint')
             return dict(optional=tag(insert, hint)), data
         else:
             # Always return the email text input itself as optional field.
             return dict(optional=insert), data
 
     def validate_registration(self, req):
@@ -260,25 +263,26 @@
 
     ''It depends on !EmailCheck being enabled too for using it's input field.
     Likewise email checking is bypassed, if account verification is
     disabled.''
     """)
 
     username_regexp = Option('account-manager', 'username_regexp',
-                             r'(?i)^[A-Z0-9.\-_]{5,}$',
-        doc=N_("A validation regular expression describing new usernames. "
-               "Define constraints for allowed user names corresponding to "
-               "local naming policy."))
+                             r'(?i)^[A-Z0-9.\-_]{5,}$', doc="""
+        A validation regular expression describing new usernames. Define
+        constraints for allowed user names corresponding to local naming
+        policy.
+        """)
 
     email_regexp = Option('account-manager', 'email_regexp',
         r'(?i)^[A-Z0-9._%+-]+@(?:[A-Z0-9-]+\.)+[A-Z0-9-]{2,63}$',
-        doc=N_("A validation regular expression describing new account "
-               "emails. Define constraints for a valid email address. A "
-               "custom pattern can narrow or widen scope i.e. to accept UTF-8 "
-               "characters."))
+        doc="""A validation regular expression describing new account emails.
+        Define constraints for a valid email address. A custom pattern can
+        narrow or widen scope i.e. to accept UTF-8 characters.
+        """)
 
     def render_registration_fields(self, req, data):
         return None, None
 
     def validate_registration(self, req):
         acctmgr = AccountManager(self.env)
 
@@ -339,15 +343,15 @@
             if perm_user.lower() == username.lower():
                 raise RegistrationError(tag_(
                     "Another account or group already exists, who's name "
                     "differs from %(username)s only by case or is identical.",
                     username=tag.b(username)))
 
 
-class RegistrationModule(Component):
+class RegistrationModule(CommonTemplateProvider):
     """Provides users the ability to register a new account.
 
     Requires configuration of the AccountManager module in trac.ini.
     """
 
     implements(chrome.INavigationContributor, IRequestHandler)
 
@@ -391,60 +395,59 @@
                                                href=req.href.register())
 
     # IRequestHandler methods
 
     def match_request(self, req):
         return req.path_info == '/register' and self._enable_check(log=True)
 
-    @process_request_compat
     def process_request(self, req):
         acctmgr = self.acctmgr
         if req.authname != 'anonymous':
             req.redirect(req.href.prefs('account'))
         action = req.args.get('action')
         name = req.args.get('name', '')
         if isinstance(name, list):
-            raise HTTPBadRequest("Invalid request arguments")
+            raise HTTPBadRequest(_("Invalid request arguments."))
         name = name.strip()
         username = req.args.get('username', '')
         if isinstance(username, list):
-            raise HTTPBadRequest("Invalid request arguments")
+            raise HTTPBadRequest(_("Invalid request arguments."))
         username = acctmgr.handle_username_casing(username.strip())
         data = {
-            'i18n_tag': i18n_tag,
+            '_dgettext': dgettext,
             'acctmgr': {'name': name, 'username': username},
             'ignore_auth_case': self.config.getbool('trac',
                                                     'ignore_auth_case')
         }
         verify_enabled = self.env.is_enabled(EmailVerificationModule) and \
                          EmailVerificationModule(self.env).verify_email
         data['verify_account_enabled'] = verify_enabled
         if req.method == 'POST' and action == 'create':
             try:
                 try:
                     # Check request and prime account on success.
                     acctmgr.validate_account(req, True)
-                except NotificationError as e:
-                    chrome.add_warning(req, '%s %s' % (
-                        _("Error raised while sending a change notification."),
-                        _("You should report that issue to a Trac admin.")))
+                except NotificationError, e:
+                    chrome.add_warning(req, _(
+                        "Error raised while sending a change notification."
+                    ) + _("You should report that issue to a Trac admin."))
                     self.log.error(
                         'Unable to send registration notification: %s',
                         exception_to_unicode(e, traceback=True))
-            except RegistrationError as e:
+            except RegistrationError, e:
                 chrome.add_warning(req, e)
             else:
                 if self.require_approval:
                     set_user_attribute(self.env, username, 'approval',
                                        'pending')
                     # Notify admin user about registration pending for review.
                     try:
                         acctmgr._notify('registration_approval_required',
                                         username)
-                    except NotificationError as e:
+                    except NotificationError, e:
                         chrome.add_warning(req, _(
                             "Error raised while sending a change "
                             "notification.") + _(
                             "You should report that issue to a Trac admin."))
                         self.log.error(
                             'Unable to send admin notification: %s',
                             exception_to_unicode(e, traceback=True))
@@ -455,49 +458,53 @@
                             "approval. Please proceed according to local "
                             "policy."))
                 if verify_enabled:
                     chrome.add_notice(req, tag_(
                         "Your username has been successfully registered but "
                         "your account still requires activation. Please "
                         "login as user %(user)s, and follow the "
-                        "instructions.", user=tag.strong(username)))
+                        "instructions.", user=tag.b(username)))
                     req.redirect(req.href.login())
                 chrome.add_notice(req, tag_(
                     "Registration has been finished successfully. "
                     "You may log in as user %(user)s now.",
                     user=tag.b(username)))
                 req.redirect(req.href.login())
         # Collect additional fields from IAccountRegistrationInspector's.
         fragments = dict(required=[], optional=[])
         for inspector in acctmgr.register_checks:
             try:
                 fragment, f_data = inspector.render_registration_fields(req,
                                                                         data)
-            except TypeError as e:
+            except TypeError, e:
                 # Add some robustness by logging the most likely errors.
                 self.log.warning("%s.render_registration_fields failed: %s",
                                  inspector.__class__.__name__, e)
                 fragment = None
             if fragment:
                 try:
-                    if 'optional' in fragment.keys():
-                        fragments['optional'].append(fragment['optional'])
-                except AttributeError:
-                    # No dict, just append Genshi Fragment or str/unicode.
-                    fragments['required'].append(fragment)
-                else:
-                    fragments['required'].append(fragment.get('required', ''))
+                    # Python<2.5: Can't have 'except' and 'finally' in same
+                    #   'try' statement together.
+                    try:
+                        if 'optional' in fragment.keys():
+                            fragments['optional'].append(fragment['optional'])
+                    except AttributeError:
+                        # No dict, just append Genshi Fragment or str/unicode.
+                        fragments['required'].append(fragment)
+                    else:
+                        fragments['required'].append(fragment.get('required',
+                                                                  ''))
                 finally:
                     data.update(f_data)
         data['required_fields'] = fragments['required']
         data['optional_fields'] = fragments['optional']
-        return 'account_register.html', data
+        return 'account_register.html', data, None
 
 
-class EmailVerificationModule(Component):
+class EmailVerificationModule(CommonTemplateProvider):
     """Performs email verification on every new or changed address.
 
     A working email sender for Trac (!TracNotification or !TracAnnouncer)
     is strictly required to enable this module's functionality.
 
     Anonymous users should register and perms should be tweaked, so that
     anonymous users can't edit wiki pages and change or create tickets.
@@ -529,15 +536,15 @@
                         req.method == 'POST' and \
                         'restore' not in req.args and \
                         req.get_header(
                             'X-Requested-With') != 'XMLHttpRequest':
             try:
                 AccountManager(self.env).validate_account(req)
                 # Check passed without error: New email address seems good.
-            except RegistrationError as e:
+            except RegistrationError, e:
                 # Always warn about issues.
                 chrome.add_warning(req, e)
                 # Look, if the issue existed before.
                 attributes = get_user_attribute(self.env, req.authname,
                                                 attribute='email')
                 email = req.authname in attributes and \
                         attributes[req.authname][1].get('email') or None
@@ -545,20 +552,21 @@
                 if (email or new_email) and email != new_email:
                     # Attempt to change email to an empty or invalid
                     # address detected, resetting to previously stored value.
                     req.redirect(req.href.prefs(None))
         if self.verify_email and handler is not self and \
                 'email_verification_token' in req.session and \
                 'ACCTMGR_ADMIN' not in req.perm:
-            message = i18n_tag(
-                _("Your permissions have been limited until you [1:verify "
-                "your email address]."),
-                tag.a(href=req.href('verify_email')),
-            )
-            chrome.add_warning(req, message)
+            # TRANSLATOR: Your permissions have been limited until you ...
+            link = tag.a(_("verify your email address"),
+                         href=req.href.verify_email())
+            # TRANSLATOR: ... verify your email address
+            chrome.add_warning(req,
+                               tag_("Your permissions have been limited "
+                                    "until you %(link)s.", link=link))
             req.perm = perm.PermissionCache(self.env, 'anonymous')
         return handler
 
     def post_process_request(self, req, template, data, content_type):
         if template is None or not req.session.authenticated:
             # Don't start the email verification procedure on anonymous users.
             return template, data, content_type
@@ -572,69 +580,72 @@
             req.session['email_verification_sent_to'] = email
             try:
                 AccountManager(self.env)._notify(
                     'email_verification_requested',
                     req.authname,
                     req.session['email_verification_token']
                 )
-            except NotificationError as e:
+            except NotificationError, e:
                 chrome.add_warning(req, _(
                     "Error raised while sending a change notification."
                 ) + _("You should report that issue to a Trac admin."))
                 self.log.error('Unable to send registration notification: %s',
                                exception_to_unicode(e, traceback=True))
             else:
-                message = i18n_tag(_("An email has been sent to <%(email)s> "
-                                     "with a token to [1:verify your new "
-                                     "email address].", email=email),
-                                   tag.a(href=req.href('verify_email')))
-                chrome.add_notice(req, message)
+                # TRANSLATOR: An email has been sent to <%(email)s>
+                # with a token to ... (the link label for following message)
+                link = tag.a(_("verify your new email address"),
+                             href=req.href.verify_email())
+                # TRANSLATOR: ... verify your new email address
+                chrome.add_notice(req, tag_(
+                    "An email has been sent to <%(email)s> with a token to "
+                    "%(link)s.", email=tag(email), link=link))
         return template, data, content_type
 
     # IRequestHandler methods
 
     def match_request(self, req):
         return req.path_info == '/verify_email'
 
-    @process_request_compat
     def process_request(self, req):
         if not req.session.authenticated:
             chrome.add_warning(req, tag_(
                 "Please log in to finish email verification procedure."))
             req.redirect(req.href.login())
         if 'email_verification_token' not in req.session:
             chrome.add_notice(req, _("Your email is already verified."))
         elif req.method == 'POST' and 'resend' in req.args:
             try:
                 AccountManager(self.env)._notify(
                     'email_verification_requested',
                     req.authname,
                     req.session['email_verification_token']
                 )
-            except NotificationError as e:
+            except NotificationError, e:
                 chrome.add_warning(req, _("Error raised while sending a "
                                           "change notification.") + _(
                     "You should "
                     "report that issue to a Trac admin."))
                 self.log.error('Unable to send verification notification: %s',
                                exception_to_unicode(e, traceback=True))
             else:
                 chrome.add_notice(req, _("A notification email has been "
-                                         "resent to <%(email)s>.",
-                                         email=req.session.get('email')))
+                                         "resent to <%s>."),
+                                  req.session.get('email'))
         elif 'verify' in req.args:
             # allow via POST or GET (the latter for email links)
             if req.args['token'] == req.session['email_verification_token']:
                 del req.session['email_verification_token']
                 chrome.add_notice(
                     req, _("Thank you for verifying your email address."))
                 req.redirect(req.href.prefs())
             else:
                 chrome.add_warning(req, _("Invalid verification token"))
-        data = {'i18n_tag': i18n_tag}
+        data = {'_dgettext': dgettext}
         if 'token' in req.args:
             data['token'] = req.args['token']
-        data['button_disabled'] = 'email_verification_token' not in req.session
-        return 'account_verify_email.html', data
+        if 'email_verification_token' not in req.session:
+            data['button_state'] = {'disabled': 'disabled'}
+        return 'account_verify_email.html', data, None
 
     def _gen_token(self):
         return base64.urlsafe_b64encode(os.urandom(6))
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/svnserve.py` & `TracAccountManager-0.6.dev0/acct_mgr/svnserve.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
 import os
 
+from acct_mgr.api import IPasswordStore
+from acct_mgr.util import EnvRelativePathOption
 from trac.config import Configuration
 from trac.core import Component, implements
 from trac.versioncontrol.api import RepositoryManager
 from trac.versioncontrol.cache import CachedRepository
 
-from .api import IPasswordStore, N_
-from .util import EnvRelativePathOption
-
 
 class SvnServePasswordStore(Component):
     """PasswordStore implementation for reading svnserve's password file format
     """
 
     implements(IPasswordStore)
 
     filename = EnvRelativePathOption('account-manager', 'password_file',
-        doc=N_("Path to the users file; leave blank to locate the users file "
-               "by reading svnserve.conf from the default repository."))
+        doc="""Path to the users file; leave blank to locate the users file
+        by reading svnserve.conf from the default repository.
+        """)
 
     _userconf = None
 
     @property
     def _config(self):
         filename = self.filename or self._get_password_file()
         if self._userconf is None or filename != self._userconf.filename:
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_admin.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_admin.html`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,40 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="admin.html" />
+  <?python
+    if _dgettext:
+        dgettext = _dgettext ?>
   <head>
     <title>Account</title>
     <script type="text/javascript">
       jQuery(document).ready(function($) {
           $('#password').focus();
       });
     </script>
   </head>
 
   <body>
     <div id="account_details">
       <div>
         <h2>Manage User Account</h2>
         <p py:choose="">
-          <py:when test="acctmgr.name">
-            <i18n:msg params="name, user">for <b>${acctmgr.name}</b> (<em>$user</em>)</i18n:msg>
+          <py:when test="acctmgr.name" i18n:msg="name, user">
+            for <b>${acctmgr.name}</b> (<em>$user</em>)
           </py:when>
-          <py:otherwise>
-            <i18n:msg params="user">for <b>$user</b></i18n:msg>
+          <py:otherwise i18n:msg="user">
+            for <b>$user</b>
           </py:otherwise>
-          <img py:if="not change_uid_enabled"
-               src="${href.chrome('/acct_mgr/info.png')}" alt="${''}"
+          <img src="${href.chrome('/acct_mgr/info.png')}" alt="info"
                title="User ID change requires additional components enabled"
-               height="16" width="16" />
+               heigth="16" width="16" py:if="not change_uid_enabled" />
         </p>
       </div>
 
       <!--! Account property editor -->
       <form id="account-editor" class="addnew" method="post" py:choose="">
         <ul id="forms" py:if="len(forms) > 1">
           <li py:for="name, label in sorted(forms)"
@@ -141,21 +143,18 @@
       <hr style="clear: right" py:strip="action_aside" />
 
       <form method="get" action="${url}">
         <fieldset>
           <legend><label>Account Status</label></legend>
           <div id="user_locked" py:if="approval or user_locked">
             <p>
-              <span py:if="release_time and not approval">
+              <span py:if="release_time and not approval" i18n:msg="time">
                 <img src="${href.chrome('/acct_mgr/time-locked.png')}" />
-                <i18n:msg params="time">
-                  This account has been locked until ${release_time}<br /><!--!
-               -->and even valid login attempts are rejected meanwhile.
-                </i18n:msg>
-              </span>
+                This account has been locked until ${release_time}<br />
+                and even valid login attempts are rejected meanwhile.</span>
               <span py:if="approval or not release_time">
                 <img src="${href.chrome('/acct_mgr/locked.png')}" />
                 This account has been locked permanently.
               </span>
               <span class="buttons">
                 <input type="submit" name="release"
                        alt="Release account lock"
@@ -163,100 +162,104 @@
                        value="${dgettext('acct_mgr', 'Unlock')}" />
               </span>
             </p>
           </div>
 
           <div id="restricted" py:if="lock_count" py:choose="">
             <div py:when="not lock_count == 0">
-              <i18n:choose numeral="lock_count" params="count">
-                <p i18n:singular="">Time lock condition has been met ${lock_count} time by now.</p>
-                <p i18n:plural="">Time lock condition has been met ${lock_count} times by now.</p>
+              <i18n:choose numeral="lock_count" params="count"
+                           py:if="not _dgettext">
+                <p i18n:singular="">
+                  Time lock condition has been met ${lock_count} time by now.
+                </p>
+                <p i18n:plural="">
+                  Time lock condition has been met ${lock_count} times by now.
+                </p>
               </i18n:choose>
-              <p py:if="not (approval or (user_locked and not release_time))">${
-                dgettext("acct_mgr",
-                         "Therefore after another failed login attempt "
-                         "authentication for this account would be retarded "
-                         "by %(time)s.", time=pretty_lock_time)
-              }</p>
+              <!--! i18n:choose doesn't play nicely with Trac releases
+                before Trac 0.12, so we provide an alternative message
+                that is excluded from extraction and translation. -->
+              <p py:if="_dgettext" xml:lang="en">
+                Time lock condition has been met ${lock_count} time(s) by now.
+              </p>
+              <p py:if="not (approval or (user_locked and not release_time))"
+                 i18n:msg="time">
+                Therefore after another failed login attempt authentication
+                for this account would be retarded by ${pretty_lock_time}.
+              </p>
             </div>
             <div py:otherwise="">
               <p>Lock condition has not been met yet.</p>
             </div>
           </div>
           <div id="unrestricted" py:if="not (approval or lock_count)">
             <p>No constraints are set for this account.</p>
           </div>
 
           <hr py:if="user_locked or approval" />
 
           <div id="user_store" py:if="user_store">
             <p i18n:msg="order_num,store">
-              Credentials for this user are stored in AuthStore number <!--!
-           --><em>${store_order_num}</em> (${user_store}).
-            </p>
+              Credentials for this user are stored in AuthStore number
+              <em>${store_order_num}</em> (${user_store}).</p>
             <p class="hint" py:if="ignore_auth_case" i18n:msg="">
-              Username matching is set to <b>not case-sensitive</b>.
-            </p>
+              Username matching is set to <b>not case-sensitive</b>.</p>
             <p class="hint" py:if="not ignore_auth_case" i18n:msg="">
-              Username matching is set to <em>case-sensitive</em>.
-            </p>
+              Username matching is set to <em>case-sensitive</em>.</p>
           </div>
           <div id="no_user_store" py:if="not (approval or user_store)">
             <p i18n:msg="">
-              No readable store provides credentials for this user, <!--!
-           -->so the user may not get authenticated and access to this <!--!
-           --><em>account might be effectively blocked</em>.
-            </p>
+              No readable store provides credentials for this user,
+              so the user may not get authenticated and access to this
+              <em>account might be effectively blocked</em>.</p>
           </div>
           <div py:if="acctmgr.email">
             <p i18n:msg="email">
-              Current email address: &lt;${acctmgr.email}&gt;
-            </p>
+              Current email address: &lt;${acctmgr.email}&gt;</p>
             <py:choose py:if="verification">
-              <p py:when="email_verified">This address has been verified successfully.</p>
+              <p py:when="email_verified">
+                This address has been verified successfully.</p>
               <p py:when="not email_verified and email_verification_token" i18n:msg="token">
-                Verification is pending <span class="hint">(token: ${email_verification_token})</span>
-              </p>
-              <p py:otherwise=""><!--! not email_verified -->
-                This address has not been verified yet.
-              </p>
+                Verification is pending
+                <span class="hint">(token: ${email_verification_token})</span></p>
+              <p py:otherwise=""> <!--! not email_verified -->
+                This address has not been verified yet.</p>
             </py:choose>
           </div>
           <div py:if="not acctmgr.email">
             <p>No email address is registered for this account.</p>
           </div>
         </fieldset>
 
         <fieldset>
           <legend><label>Access History</label></legend>
-          <p>${
-            dgettext('acct_mgr', 'Last login: %(time)s', time=format_datetime(last_visit)) \
-            if last_visit else \
-            dgettext('acct_mgr', 'The user has not logged in before.')
-          }</p>
+          <p py:if="last_visit" i18n:msg="time">
+            Last login: ${last_visit}</p>
+          <p py:if="not last_visit">The user has not logged in before.</p>
           <div id="failed_attempts" py:if="attempts_count">
             <p i18n:msg="count">Total failed attempts: ${attempts_count}</p>
             <p class="tableheader">
               Table: Last failed login attempts log view</p>
             <table class="listing" id="login_attempts">
               <thead>
                 <tr>
                   <th>IP address</th>
                   <th>Log time</th>
                 </tr>
               </thead>
               <tbody>
                 <tr py:for="attempt in attempts">
                   <td>${attempt.ipnr}</td>
-                  <td>${format_datetime(attempt.time)}</td>
+                  <td>${attempt.time}</td>
                 </tr>
               </tbody>
             </table>
             <div class="buttons" py:if="not user_locked">
               <input type="submit" name="delete"
+                     alt="Delete login failure log"
                      title="Delete login failure log"
                      value="${dgettext('acct_mgr', 'Delete Log')}" />
             </div>
           </div>
           <div id="no_failed_attempts" py:if="not attempts_count">
             <p>There is currently no failed login attempt logged.</p>
           </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
+>
 ********** MMaannaaggee UUsseerr AAccccoouunntt **********
-for $${{aaccccttmmggrr..nnaammee}} ($$uusseerr) for $$uusseerr[${''}]
+for $${{aaccccttmmggrr..nnaammee}} ($$uusseerr) for $$uusseerr[info]
     * _$_{_l_a_b_e_l_}
 New Username:
 [${acctmgr.new_uid}  ]
 Assume existing account
 Copy only new account attributes
 Leave old login data
 Password:
@@ -21,17 +22,17 @@
 [${href.chrome('/acct_mgr/time-locked.png')}]This account has been locked until
 ${release_time}
 and even valid login attempts are rejected meanwhile. [${href.chrome('/
 acct_mgr/locked.png')}]This account has been locked permanently.[${dgettext
 ('acct_mgr', 'Unlock')}]
 Time lock condition has been met ${lock_count} time by now.
 Time lock condition has been met ${lock_count} times by now.
-${ dgettext("acct_mgr", "Therefore after another failed login attempt "
-"authentication for this account would be retarded " "by %(time)s.",
-time=pretty_lock_time) }
+Time lock condition has been met ${lock_count} time(s) by now.
+Therefore after another failed login attempt authentication for this account
+would be retarded by ${pretty_lock_time}.
 Lock condition has not been met yet.
 No constraints are set for this account.
 ===============================================================================
 Credentials for this user are stored in AuthStore number $${{ssttoorree__oorrddeerr__nnuumm}} ($
 {user_store}).
 Username matching is set to nnoott ccaassee--sseennssiittiivvee.
 Username matching is set to ccaassee--sseennssiittiivvee.
@@ -39,17 +40,16 @@
 authenticated and access to this aaccccoouunntt mmiigghhtt bbee eeffffeeccttiivveellyy bblloocckkeedd.
 Current email address: <${acctmgr.email}>
 This address has been verified successfully.
 Verification is pending (token: ${email_verification_token})
 This address has not been verified yet.
 No email address is registered for this account.
 Access History
-${ dgettext('acct_mgr', 'Last login: %(time)s', time=format_datetime
-(last_visit)) \ if last_visit else \ dgettext('acct_mgr', 'The user has not
-logged in before.') }
+Last login: ${last_visit}
+The user has not logged in before.
 Total failed attempts: ${attempts_count}
 Table: Last failed login attempts log view
 IIPP aaddddrreessss      LLoogg ttiimmee
-${attempt.ipnr} ${format_datetime(attempt.time)}
+${attempt.ipnr} ${attempt.time}
 [${dgettext('acct_mgr', 'Delete Log')}]
 There is currently no failed login attempt logged.
 [${dgettext('acct_mgr', 'Refresh')}]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_config.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_config.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 <!DOCTYPE html
     PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:xi="http://www.w3.org/2001/XInclude"
-      xmlns:py="http://genshi.edgewall.org/"
+      xmlns:py="http://genshi.edgewall.org/" 
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="admin.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Accounts: Configuration</title>
     <script type="text/javascript"
             src="${chrome.htdocs_location}js/folding.js"></script>
     <script type="text/javascript">/*<![CDATA[*/
       jQuery(document).ready(function($) {
         // Hide configuration preview sections by default
@@ -32,15 +35,15 @@
             id="${idx == len(steps) - 1 and 'last' or None}"
             style="${'width:' + str(100 / len(steps)) + '%'}">
           <span>
             <a href="$url">${idx + 1}</a>
           </span>
           <a href="$url" title="${step.image and step.label or None}">
           <img class="icon" alt="${step.label}" py:if="step.image"
-               height="32" width="32"
+               heigth="32" width="32"
                src="${href.chrome('/acct_mgr/' + step.image + '.png')}" />
           <py:if test="not step.image">$step.label</py:if>
           </a>
         </li>
       </ul>
 
       <form id="cfg_wiz" method="post"
@@ -64,428 +67,413 @@
 
           <!--! Page 1 -->
           <fieldset py:when="0">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
           <h3>Objective for setting Authentication Options</h3>
-          <p>${
-            dgettext("acct_mgr",
-                     "Decide, whether to use HTTP authentication (Trac default) or a HTML login"
-                     " form provided by AccountManagerPlugin.")
-          }</p>
-          <p>${
-            dgettext("acct_mgr",
-                     "After initial login Trac sessions are authenticated per request based on "
-                     "browser cookies. Therefore a number of options provide control over some "
-                     "critical browser cookie properties.")
-          }</p>
+          <p>
+            Decide, whether to use HTTP authentication (Trac default) or
+            a HTML login form provided by AccountManagerPlugin.
+          </p>
+          <p>
+            After initial login Trac sessions are authenticated per request
+            based on browser cookies.  Therefor a number of options provide
+            control over some critical browser cookie properties.
+          </p>
 
           <h3>Provider-agnostic Authentication Options</h3>
           <div class="field">
             <label>
               <input type="checkbox" name="ignore_auth_case" value="true"
                      title="${'[trac] ignore_auth_case'}"
                      checked="${ignore_auth_case and 'checked' or None}" />
               Convert login names to lower case on registration and login.
             </label>
             <p class="hint" i18n:msg="">
-              Adapt to careless username typing, where casing does not <!--!
-           -->matter, like on Windows. Potentially troublesome, because <!--!
-           --><tt>case matters for Trac permission assignment lookup</tt> anyway.
+              Adapt to careless username typing, where casing does not matter,
+              like on Windows.  Potentially troublesome, because <tt>case
+              matters for Trac permission assignment lookup</tt> anyway.
             </p>
           </div>
           <div class="field">
             <label>
               <input type="checkbox" name="check_auth_ip" value="true"
                      title="${'[trac] check_auth_ip'}"
                      checked="${check_auth_ip and 'checked' or None}" />
               Check IP address for authentication.
             </label>
-            <p class="hint">${
-              dgettext("acct_mgr",
-                       "Potentially troublesome for users with dynamic IP address, but "
-                       "disregarded for persistent sessions.")
-            }</p>
+            <p class="hint">
+              Potentially troublesome for users with dynamic IP adress, but
+              disregarded for persistent sessions.
+            </p>
           </div>
           <div class="field">
             <label>
               <input type="checkbox" name="secure_cookies" value="true"
                      title="${'[trac] secure_cookies'}"
                      checked="${secure_cookies and 'checked' or None}" />
               Restrict sending cookies to HTTPS connections.
             </label>
             <p class="hint">
               Required, if the Trac instance is only accessible through HTTPS.
             </p>
           </div>
-          <div class="field">
-            <!--! Last value cache for JS code -->
+          <div class="field"
+               py:with="value = acctmgr_login and auth_cookie_lifetime or 
+                                acctmgr_login and 2592000 or
+                                auth_cookie_lifetime">
+
+            <!-- Last value cache for JS code -->
             <input type="hidden" id="auth_cookie_lifetime_old"
                    value="$auth_cookie_lifetime" disabled="disabled" />
-            <label py:with="
-                lifetime_value = ((auth_cookie_lifetime or 2592000)
-                                  if acctmgr_login else auth_cookie_lifetime)
-              ">${
-              i18n_tag(
-                dgettext("acct_mgr",
-                         "Lifetime of the authentication cookie: [1:] seconds [2:(%(timedelta)s)]"),
-                ('input', {'type': 'text', 'class': 'numwidget',
-                           'name': 'auth_cookie_lifetime',
-                           'title': '[trac] auth_cookie_lifetime',
-                           'value': auth_cookie_lifetime}),
-                ('span', {'class': 'hint',
-                          'style': None if lifetime_value else 'display:none'}),
-                timedelta=format_timespan(lifetime_value),
-              )
-            }</label>
-            <p class="hint">${
-              dgettext("acct_mgr",
-                       "Determines how long the browser will cache authentication "
-                       "information, and therefore, after how much inactivity a user will "
-                       "have to log in again. Default (0 s) makes cookie expire at "
-                       "browsing sessions end.")
-            }</p>
+            <label i18n:msg="timedelta">
+              Lifetime of the authentication cookie:
+              <input type="text" class="numwidget" name="auth_cookie_lifetime"
+                     title="${'[trac] auth_cookie_lifetime'}"
+                     value="$auth_cookie_lifetime" />
+              seconds
+              <span class="hint" py:if="value"
+                    id="pretty_auth_cookie_lifetime">
+                (${pretty_precise_timedelta(None, diff=value)})
+              </span>
+            </label>
+            <p class="hint">
+              Determines how long the browser will cache authentication
+              information, and therefore, after how much inactivity a user
+              will have to log in again.  Default (0&nbsp;s) makes cookie
+              expire at browsing sessions end.
+            </p>
           </div>
 
           <h3>Authentication Front-end</h3>
           <div class="field">
             <label>
               <input type="radio" name="acctmgr_login" value="0"
                      checked="${acctmgr_login and None or 'checked'}"
                      title="${'[components] trac.web.auth.loginmodule'}" />
-              ${dgettext("acct_mgr",
-                         "Use HTTP authentication and credentials as configured "
-                         "in and provided by your web-server.")}
+              Use HTTP authentication and credentials as configured in and
+              provided by your web-server.
             </label>
-            <p class="hint">${
-              dgettext("acct_mgr",
-                       "You can still manage some password stores with "
-                       "AccountManagerPlugin, if you configure them in the next step.")
-            }</p>
+            <p class="hint">
+              You can still manage some password stores with
+              AccountManagerPlugin, if you configure them in the next step.
+            </p>
             <label>
               <input type="radio" name="acctmgr_login" value="1"
                      checked="${acctmgr_login and 'checked' or None}"
                      title="${'[components] acct_mgr.web_ui.loginmodule'}" />
-              ${dgettext("acct_mgr",
-                         "Use a HTML login form backed by one or more "
-                         "password stores managed by AccountManagerPlugin.")}
+              Use a HTML login form backed by one or more password stores
+              managed by AccountManagerPlugin.
             </label>
             <p class="hint" i18n:msg="">
-              AccountManagerPlugin provides a custom version of the <!--!
-           --><strong>LoginModule</strong> accompanied by a form-based <!--!
-           -->HTML login page.
+              AccountManagerPlugin provides a custom version of the
+              <strong>LoginModule</strong> accompanied by a form-based HTML
+              login page.
             </p>
             <p class="hint" i18n:msg="">
-              If you enable this feature, you'll want to review and adjust <!--!
-           -->some more options related to session authentication. <!--!
-           -->Note, that AccountManagerPlugin's LoginModule <tt>changes <!--!
-           -->the default lifetime of authentication cookies to 30 days</tt>.
+              If you enable this feature, you'll want to review and adjust
+              some more options related to session authentication.
+              Note, that AccountManagerPlugin's LoginModule <tt>changes the
+              default lifetime of authentication cookies to 30 days</tt>.
             </p>
           </div>
 
           <div id="acctmgr_login_opts">
             <h3>AccountManagerPlugin Authentication Options</h3>
             <div class="field">
               <label>
                 <input type="checkbox" name="login_opt_list" value="true"
                        checked="${login_opt_list and 'checked' or None}"
                        title="${'[account-manager] login_opt_list'}" />
                 Integrate links to related actions into the login form.
               </label>
-              ${
-                i18n_tag(
-                  dgettext(
-                    "acct_mgr",
-                    "[1:If enabled, links to][2:[3:[4:Lost password/Password "
-                    "reset]][5:[6:Registration for new users]]][7:that normally reside in "
-                    "Trac's meta-navigation bar, will appear inside the login form. CSS "
-                    "styling allows further customization of the login prompt.]"
-                  ),
-                  ('p', {'class': 'hint'}), 'ul',
-                  'li', ('span', {'class': 'hint'}),
-                  'li', ('span', {'class': 'hint'}),
-                  ('p', {'class': 'hint'}),
-                )
-              }
+              <i18n:msg>
+                <p class="hint">
+                  If enabled, links to
+                </p>
+                <ul>
+                  <li>
+                    <span class="hint">Lost password/Password reset</span>
+                  </li>
+                  <li>
+                    <span class="hint">Registration for new users</span>
+                  </li>
+                </ul>
+                <p class="hint">
+                  that normally reside in Trac's meta-navigation bar, will
+                  appear inside the login form.  CSS styling allows further
+                  customization of the login prompt.
+                </p>
+              </i18n:msg>
             </div>
             <div class="field">
               <label>
                 <input type="checkbox" name="persistent_sessions" value="true"
                        checked="${persistent_sessions and 'checked' or None}"
                        title="${'[account-manager] persistent_sessions'}" />
-                ${dgettext("acct_mgr",
-                           "Allow the user to be remembered across sessions "
-                           "without needing to re-authenticate.")}
+                Allow the user to be remembered across sessions without
+                needing to re-authenticate.
               </label>
-              <p class="hint" i18n:msg="">
-                This is, user checks a "Remember Me" <tt>checkbox</tt> in <!--!
-             -->the AccountManagerPlugin login form and, next time he <!--!
-             -->visits the site within 30 days, he'll be remembered and <!--!
-             -->authenticated automatically.
+              <p class="hint" i18n:msg="">This is, user checks a "Remember Me"
+                <tt>checkbox</tt> in the AccountManagerPlugin login form and,
+                next time he visits the site within 30 days, he'll be
+                remembered and authenticated automatically.
               </p>
             </div>
             <div class="field">
               <label i18n:msg="">
-                Likelihood of session cookie ID change: <!--!
-             --><input type="text" class="numwidget" name="cookie_refresh_pct"
+                Likelihood of session cookie ID change:
+                <input type="text" class="numwidget" name="cookie_refresh_pct"
                        title="${'[account-manager] cookie_refresh_pct'}"
-                       value="$cookie_refresh_pct" /> <!--!
-             -->% per work hour
+                       value="$cookie_refresh_pct" />
+                % per work hour
               </label>
               <p class="hint" i18n:msg="">
-                Driving a refresh process to decrease vulnerability of <!--!
-             -->long-lasting sessions. Zero means <strong>never</strong>.
+                Driving a refresh process to decrease vulnerability of
+                long-lasting sessions.  Zero means <strong>never</strong>.
               </p>
             </div>
             <div class="field">
               <label>
                 Path for authentication cookie:
                 <input type="text" class="textwidget" name="auth_cookie_path"
                        title="${'[trac] auth_cookie_path'}"
                        value="$auth_cookie_path" />
               </label>
               <p class="hint" i18n:msg="">
-                This enables AccountManagerPlugin's authentication data <!--!
-             -->distribution to Trac instances with matching cookie path. <!--!
-             -->Set this to a common base path of several Trac instances <!--!
-             -->to share the cookie, providing a cheap <!--!
-             --><tt>Single-Sign-On</tt> experience.
+                This enables AccountManagerPlugin's authentication data
+                distribution to Trac instances with matching cookie path.
+                Set this to a common base path of several Trac instances to
+                share the cookie, providing a cheap <tt>Single-Sign-On</tt>
+                experience.
               </p>
             </div>
           </div>
           </fieldset>
 
           <!--! Page 2 -->
           <fieldset py:when="1">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
-            <img class="icon" alt="Password store" src="${href.chrome('/acct_mgr/users.png')}" />
+            <img class="icon" alt="Password store icon"
+                 src="${href.chrome('/acct_mgr/users.png')}" />
 
             <h3>Objective for configuring a Password Store</h3>
-            <p>${
-              dgettext("acct_mgr",
-                       "AccountManagerPlugin manages user credentials in a modular "
-                       "back-end providing access to at least one password store.")
-            }</p>
+            <p>
+              AccountManagerPlugin manages user credentials in a modular
+              back-end providing access to at least one password store.
+            </p>
 
             <div py:if="len(password_store) == 0">
               <h3>Initial Authentication Back-end selection</h3>
               <!-- Initial setup content -->
               <div class="field">
                 <label>
                   <input type="radio" name="init_store" value="db"
-                         checked="${'checked' if init_store == 'db' else None}"
+                         checked="${init_store == 'db' and
+                                    'checked' or None}"
                          title="${'[account-manager] password_store'}" />
                   Use a password store embedded into Trac db.
                 </label>
                 <p class="hint" i18n:msg="">
-                  The <strong>SessionStore</strong> implements password <!--!
-               -->storage in Trac db table 'session_attribute'. Its the <!--!
-               -->default choice mainly for avoiding additional dependencies <!--!
-               -->like directory and file permissions.
-                </p>
-                <p class="hint">${
-                  dgettext(
-                    "acct_mgr",
-                    "While great to resolve some concurrent access issues too, "
-                    "this password store has shortcomings as well. Notably it "
-                    "does not support seamless hash type migration, and its no "
-                    "candidate for shared use by multiple Trac instances or even "
-                    "by applications beyond Trac.")
-                }</p>
+                  The <strong>SessionStore</strong> implements password
+                  storage in Trac db table 'session_attributes'.
+                  Its the default choice mainly for avoiding additional
+                  dependencies like directory and file permissions.
+                </p>
+                <p class="hint">
+                  While great to resolve some concurrent access issues too,
+                  this password store has shortcomings as well.  Notably it
+                  does not support seamless hash type migration, and its no
+                  candidate for shared use by multiple Trac instances or even
+                  by applications beyond Trac.
+                </p>
                 <fieldset class="ini" id="db">
                   <legend class="foldable">Details (Preview)</legend>
                   <div class="compact">
                     <pre>$init_store_hint.db</pre>
-                    <p class="hint">${
-                      dgettext("acct_mgr",
-                               "Please apply these default options first. "
-                               "You'll be able to change values afterwards.")
-                    }</p>
+                    <p class="hint">
+                      Please apply these default options first. You'll be
+                      able to change values afterwards.
+                    </p>
                   </div>
                 </fieldset>
               </div>
               <div class="field">
                 <label>
                   <input type="radio" name="init_store" value="file"
-                         checked="${'checked' if init_store in ('htdigest', 'htpasswd') else None}" />
+                         checked="${init_store in ('htdigest', 'htpasswd') and
+                                    'checked' or None}" />
                   Use a file-based password store.
                 </label>
-                <p class="hint">${
-                  dgettext("acct_mgr",
-                           "AccountManagerPlugin includes native support for common "
-                           "Apache file formats 'htpasswd' and 'htdigest' as well as "
-                           "support for reading svnserve's password file format.")
-                }</p>
-                <p class="hint">${
-                  dgettext("acct_mgr",
-                           "You may use the same file for several Trac environments. "
-                           "Note that setting appropriate directory and file permissions "
-                           "is crucial for these stores, but not covered by this "
-                           "configuration wizard.")
-                }</p>
+                <p class="hint">
+                  AccountManagerPlugin includes native support for common
+                  Apache file formats 'htpasswd' and 'htdigest' as well as
+                  support for reading svnserve's password file format.
+                </p>
+                <p class="hint">
+                  You may use the same file for several Trac environments.
+                  Note that setting appropriate directory and file permissions
+                  is crucial for these stores, but not covered by this
+                  configuration wizard.
+                </p>
               </div>
               <fieldset id="init_store_file">
                 <div class="field">
-                  <label>
-                    <input type="radio" name="init_store_file" value="htdigest"
-                           checked="${'checked' if init_store == 'htdigest' or not htpasswd else None}"
+                  <label i18n:msg="">
+                    <input type="radio" name="init_store_file"
+                           value="htdigest"
+                           checked="${init_store == 'htdigest' or
+                                      not htpasswd and 'checked' or None}"
                            title="${'[account-manager] password_store'}" />
-                    <i18n:msg>
-                      'htdigest' format <span class="hint">(<strong>HtDigestStore</strong>)</span>
-                    </i18n:msg>
+                    'htdigest' format
+                    <span class="hint">(<strong>HtDigestStore</strong>)</span>
                   </label>
                   <fieldset class="ini" id="htdigest">
                     <legend class="foldable">Details (Preview)</legend>
                     <div class="compact">
                       <pre>$init_store_hint.htdigest</pre>
-                      <p class="hint">${
-                        dgettext("acct_mgr",
-                                 "Please apply these default options first. "
-                                 "You'll be able to change values afterwards.")
-                      }</p>
+                      <p class="hint">
+                        Please apply these default options first. You'll be
+                        able to change values afterwards.
+                      </p>
                     </div>
                   </fieldset>
                 </div>
                 <div class="field">
-                  <label>
+                  <label i18n:msg="">
                     <input type="radio" name="init_store_file"
                            value="htpasswd"
-                           checked="${'checked' if init_store == 'htpasswd' else None}"
+                           checked="${init_store == 'htpasswd' and
+                                      'checked' or None}"
                            title="${'[account-manager] password_store'}" />
-                    <i18n:msg>
-                      'htpasswd' format <span class="hint">(<strong>HtPasswdStore</strong>)</span>
-                    </i18n:msg>
+                    'htpasswd' format
+                    <span class="hint">(<strong>HtPasswdStore</strong>)</span>
                   </label>
                   <fieldset class="ini" id="htpasswd">
                     <legend class="foldable">Details (Preview)</legend>
                     <div class="compact">
                       <pre>$init_store_hint.htpasswd</pre>
-                      <p class="hint">${
-                        dgettext("acct_mgr",
-                                 "Please apply these default options first. "
-                                 "You'll be able to change values afterwards.")
-                      }</p>
+                      <p class="hint">
+                        Please apply these default options first. You'll be
+                        able to change values afterwards.
+                      </p>
                     </div>
                   </fieldset>
                 </div>
                 <div class="field">
-                  <label>
+                  <label i18n:msg="">
                     <input type="radio" name="init_store_file"
                            value="svn_file"
-                           checked="${'checked' if init_store == 'svn_file' else None}"
+                           checked="${init_store == 'svn_file' and 
+                                      'checked' or None}"
                            title="${'[account-manager] password_store'}" />
-                    <i18n:msg>
-                      svnserve's password file format <span
-                        class="hint">(<strong>SvnServePasswordStore</strong>)</span>
-                    </i18n:msg>
+                    svnserve's password file format
+                    <span class="hint">
+                        (<strong>SvnServePasswordStore</strong>)
+                    </span>
                   </label>
                   <fieldset class="ini" id="svn_file">
                     <legend class="foldable">Details (Preview)</legend>
                     <div class="compact">
                       <pre>$init_store_hint.svn_file</pre>
-                      <p class="hint">${
-                        dgettext("acct_mgr",
-                                 "Please apply these default options first. "
-                                 "You'll be able to change values afterwards.")
-                      }</p>
+                      <p class="hint">
+                        Please apply these default options first. You'll be
+                        able to change values afterwards.
+                      </p>
                     </div>
                   </fieldset>
                 </div>
               </fieldset>
               <div class="field">
                 <label>
                   <input type="radio" name="init_store" value="http"
                          checked="${init_store == 'http' and
                                     'checked' or None}"
                          title="${'[account-manager] password_store'}" />
                   Delegate authentication using HTTP authentication.
                 </label>
                 <p class="hint" i18n:msg="">
-                  AccountManagerPlugin enables use of standard HTTP-Auth <!--!
-               -->by its <strong>HttpAuthStore</strong> component. Both <!--!
-               -->Basic and Digest authentication challenges are supported.
-                </p>
-                <p class="hint">${
-                  dgettext("acct_mgr",
-                           "In addition to being read-only this password store does "
-                           "not even support listing users for obvious reasons.")
-                }</p>
+                  AccountManagerPlugin enables use of standard HTTP-Auth
+                  by its <strong>HttpAuthStore</strong> component.  Both
+                  Basic and Digest authentication challenges are supported.
+                </p>
+                <p class="hint">
+                  In addition to being read-only this password store does not
+                  even support listing users for obvious reasons.
+                </p>
                 <fieldset class="ini" id="http">
                   <legend class="foldable">Details (Preview)</legend>
                   <div class="compact">
                     <pre>$init_store_hint.http</pre>
-                    <p class="hint">${
-                      dgettext("acct_mgr",
-                               "Please apply these default options first. "
-                               "You'll be able to change values afterwards.")
-                    }</p>
+                    <p class="hint">
+                      Please apply these default options first. You'll be
+                      able to change values afterwards.
+                    </p>
                   </div>
                 </fieldset>
               </div>
 
               <div class="field">
                 <label>
                   <!-- Disabled to speed-up initial publication -->
                   <input type="radio" name="init_store" value="etc"
                          checked="${init_store == 'etc' and
                                     'checked' or None}"
                          disabled="disabled"
                          title="${'[account-manager] password_store'}" />
                   Use a different password store.
                 </label>
-                <p class="hint">${
-                  dgettext(
-                    "acct_mgr",
-                    "AccountManagerPlugin's modular password store concept "
-                    "encourages creation of more ways to provide user credential "
-                    "beyond the natively supported stores. While a specific setup "
-                    "assistance for these 3rd-party authentication providers is not "
-                    "implemented, you may fill-in appropriate configuration details "
-                    "for an already installed component below.")
-                }</p>
+                <p class="hint">
+                  AccountManagerPlugin's modular password store concept
+                  encourages creation of more ways to provide user credential
+                  beyond the natively supported stores.  While specific setup
+                  assistance for these 3rd-party authentication providers is not
+                  implemented, you may fill-in approprate configuration details
+                  for an already installed component below.
+                </p>
               </div>
               <fieldset id="etc_store_cfg">
                 <legend>Configuration</legend>
                 <div class="compact field">
                   <textarea name="etc_cfg">$init_store_hint.http</textarea>
-                  <p class="hint">${
-                    dgettext("acct_mgr",
-                             "Type the custom configuration options as provided by "
-                             "that components documentation and apply it.")
-                  }</p>
+                  <p class="hint">
+                    Type the custom configuration options as provided by that
+                    components documentation and apply it.
+                  </p>
                 </div>
               </fieldset>
             </div>
 
             <div py:if="len(password_store) > 0">
               <!-- Standard page content -->
               <h3>Password Store Configuration</h3>
               <p i18n:msg="store_list">
-                All enabled stores are listed below, but most won't work at <!--!
-                -->all without additional configuration.<br />Currently configured: <!--!
-                --><em title="${'[account-manager] password_store'}">${', '.join(password_store)}</em>
+                All enabled stores are listed below, but most won't work at
+                all without additional configuration.<br />
+                Currently configured:
+                <em title="${'[account-manager] password_store'}">
+                  ${', '.join(password_store)}
+                </em>
               </p>
               <p class="hint" py:if="len(password_store) > 1">
                 This is an experts-only type of store configuration.
               </p>
               <div class="system-message" py:if="disabled_store">
-                <p>
-                  <strong i18n:msg="components">
-                    Required disabled component(s): <em>${', '.join(disabled_store)}</em>
-                  </strong>
+                <p i18n:msg="components">
+                  <strong>Required disabled component(s):
+                  <em>${', '.join(disabled_store)}</em></strong>
                 </p>
               </div>
-              <p>${
-                dgettext("acct_mgr",
-                         "Select one or more stores and configure related options. "
-                         "Concurrent use of multiple password stores is supported too.")
-              }</p>
+              <p>
+                Select one or more stores and configure related options.
+                Concurrent use of multiple password stores is supported too.
+              </p>
               <p class="hint">
                 Password stores are queried in turn, so order matters.
               </p>
 
               <fieldset py:for="section in store_list">
                 <legend>
                   <label>
@@ -505,16 +493,17 @@
                            py:when="isinstance(option.value, dict) and
                                     'error' in option.value.keys()" >
                         <p>${option.value['error']}</p>
                       </div>
                       <select name="$option.name"
                               py:when="isinstance(option.value, dict)" >
                         <option py:for="opt in option.value['options']"
-                                class="textwidget"
-                                selected="${opt == option.value['selected'] or None}"
+                                class="textwidget" 
+                                selected="${opt == option.value['selected'] or
+                                          None}"
                                 value="${opt}">
                           ${opt}
                         </option>
                       </select>
                       <input type="text" class="textwidget" py:otherwise=""
                              name="$option.name" value="$option.value" />
                     </py:choose>
@@ -526,65 +515,64 @@
               <div class="field">
                 <label>
                   <input type="checkbox" name="refresh_passwd" value="true"
                          checked="${refresh_passwd and 'checked' or None}"
                          title="${'[account-manager] refresh_passwd'}" />
                   Silently update password hashes on next successful login.
                 </label>
-                <p class="hint">${
-                  dgettext("acct_mgr",
-                           "Use it after changing hash type or to migrate to a new "
-                           "primary password store.")
-                }</p>
-                <p class="hint">${
-                  dgettext("acct_mgr",
-                           "The update will run only once. Restarting the procedure "
-                           "for all accounts allows to propagate subsequent changes.")
-                }</p>
+                <p class="hint">
+                  Use it after changing hash type or to migrate to a new
+                  primary password store.
+                </p>
+                <p class="hint">
+                  The update will run only once.  Restarting the procedure
+                  for all accounts allows to propagate subsequent changes.
+                </p>
                 <div class="buttons">
                   <input type="submit" name="restart" id="restart"
                          value="${dgettext('acct_mgr', 'Restart')}" />
                 </div>
               </div>
             </div>
           </fieldset>
 
           <!--! Page 3 -->
           <fieldset py:when="2">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
-            <img class="icon" alt="Password refresh" src="${href.chrome('/acct_mgr/refresh.png')}" />
+            <img class="icon" alt="Password refresh icon"
+                 src="${href.chrome('/acct_mgr/refresh.png')}" />
 
             <h3>Objective for Password Policy rules</h3>
-            <p>${
-              dgettext("acct_mgr",
-                       "While AccountManagerPlugin does not enforce password rules in "
-                       "general, there are some other ways to alter password handling.")
-            }</p>
+            <p>
+              While AccountManagerPlugin does not enforce password rules in
+              general, there are some other ways to alter password handling.
+            </p>
 
             <div class="field">
               <label>
                 <input type="checkbox" name="reset_password" value="true"
                        checked="${reset_password and 'checked' or None}"
                        title="${'[account-manager] reset_password'}" />
                 Enable the password reset procedure.
               </label>
-              <p class="hint">${
-                dgettext("acct_mgr",
-                         "It relies on a working email sender for Trac, supporting "
-                         "both TracAnnouncer and TracNotification.")
-              }</p>
+              <p class="hint">
+                It relies on a working email sender for Trac, supporting both
+                TracAnnouncer and TracNotification.
+              </p>
             </div>
             <div class="field">
               <label i18n:msg="">
-                Length of the randomly-generated passwords: <input
-                  type="text" class="numwidget" name="generated_password_length"
-                  title="${'[account-manager] generated_password_length'}"
-                  value="$generated_password_length" /> characters
+                Length of the randomly-generated passwords:
+                <input type="text" class="numwidget"
+                       name="generated_password_length"
+                       title="${'[account-manager] generated_password_length'}"
+                       value="$generated_password_length" />
+                characters
               </label>
               <p class="hint">
                 These passwords are used as alternative passwords on request.
               </p>
             </div>
             <div class="field">
               <label>
@@ -597,24 +585,23 @@
           </fieldset>
 
           <!--! Page 4 -->
           <fieldset py:when="3">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
-            <img class="icon" alt="Account approval" src="${href.chrome('/acct_mgr/approval.png')}" />
+            <img class="icon" alt="Account approval icon"
+                 src="${href.chrome('/acct_mgr/approval.png')}" />
 
             <h3>Objective for Account Registration and Verification rules</h3>
-            <p>${
-              dgettext(
-                "acct_mgr",
-                "You may require administrative approval of new accounts for the user "
-                "registration process. The ability to immediately ban existing accounts is"
-                " another, related but independent feature.")
-            }</p>
+            <p>
+              You may require administrative approval of new accounts for the
+              user registration process.  The ability to immediately ban
+              existing accounts is another, related but independed feature.
+            </p>
             <div class="field">
               <label>
                 <input type="checkbox" name="change_uid_enabled"
                        checked="${change_uid_enabled and 'checked' or None}"
                        title="${'[components] acct_mgr.model.*'}"
                        value="true" />
                 Allow administrative user ID changes.
@@ -637,42 +624,39 @@
                        value="true" />
                 Allow users to delete their own account.
               </label>
             </div>
 
             <h3>Checks to use for validating Registration requests</h3>
             <p i18n:msg="check_list">
-              All checks provided by AccountManagerPlugin are enabled per <!--!
-              -->default, but some are configurable on their own.<br /><!--
-              -->Currently configured: <!--!
-              --><em title="${'[account-manager] register_check'}">${', '.join(register_check)}</em>
+              All checks provided by AccountManagerPlugin are enabled per
+              default, but some are configurable on their own.<br />
+              Currently configured:
+              <em title="${'[account-manager] register_check'}">
+                ${', '.join(register_check)}
+              </em>
             </p>
             <p class="hint" i18n:msg="">
-              Checks like <strong>BotTrapCheck</strong> won't work at all <!--!
-           -->without additional configuration.
+              Checks like <strong>BotTrapCheck</strong> won't work at all
+              without additional configuration.
             </p>
             <div class="system-message" py:if="disabled_check">
-              <p>
-                <strong i18n:msg="components">
-                  Required disabled component(s): <em>${', '.join(disabled_check)}</em>
-                </strong>
-              </p>
-            </div>
-            <p>${
-              dgettext(
-                "acct_mgr",
-                "Select one or more checks and configure related options. "
-                "Concurrent use of multiple registration checks is encouraged.")
-            }</p>
-            <p class="hint">${
-              dgettext(
-                "acct_mgr",
-                "Checks are applied in turn, so order matters. Note that some "
-                "checks are used to validate admin user actions too.")
-            }</p>
+              <p i18n:msg="components">
+                <strong>Required disabled component(s):
+                <em>${', '.join(disabled_check)}</em></strong>
+              </p>
+            </div>
+            <p>
+              Select one or more checks and configure related options.
+              Concurrent use of multiple registration checks is encouraged.
+            </p>
+            <p class="hint">
+              Checks are applied in turn, so order matters.  Note that some
+              checks are used to validate admin user actions too.
+            </p>
 
             <fieldset py:for="section in check_list">
               <legend>
                 <label>
                   <select name="${section.classname}" >
                     <option py:for="order in check_count" value="${order}"
                             selected="${order == section.order or None}">
@@ -692,15 +676,15 @@
                          py:when="isinstance(option.value, dict) and
                                   'error' in option.value.keys()" >
                       <p>${option.value['error']}</p>
                     </div>
                     <select name="$option.name"
                             py:when="isinstance(option.value, dict)" >
                       <option py:for="opt in option.value['options']"
-                              class="textwidget"
+                              class="textwidget" 
                               selected="${opt == option.value['selected'] or
                                           None}"
                               value="${opt}">
                         ${opt}
                       </option>
                     </select>
                     <input type="text" class="textwidget" py:otherwise=""
@@ -716,62 +700,58 @@
               <div class="field">
                 <label>
                   <input type="checkbox" name="require_approval" value="true"
                          checked="${require_approval and 'checked' or None}"
                          title="${'[account-manager] require_approval'}" />
                   Require administrative account approval after registration.
                 </label>
-                <p class="hint">${
-                  dgettext(
-                    "acct_mgr",
-                    "For admin notification on registration time it relies on a "
-                    "working email sender for Trac, supporting both TracAnnouncer "
-                    "and TracNotification.")
-                }</p>
+                <p class="hint">
+                  For admin notification on registration time it relies on a
+                  working email sender for Trac, supporting both TracAnnouncer
+                  and TracNotification.
+                </p>
               </div>
             </div>
             <div class="field">
               <label>
                 <input type="checkbox" name="verify_email" value="true"
                        checked="${verify_email and 'checked' or None}"
                        title="${'[account-manager] verify_email'}" />
                 Force users to verify their email addresses.
               </label>
-              <p class="hint">${
-                dgettext(
-                  "acct_mgr",
-                  "For sending a verification token to the user it relies on a working email "
-                  "sender for Trac, supporting both TracAnnouncer and TracNotification.")
-              }</p>
+              <p class="hint">
+                For sending a verificaton token to the user it relies on a
+                working email sender for Trac, supporting both TracAnnouncer
+                and TracNotification.
+              </p>
             </div>
           </fieldset>
 
           <!--! Page 5 -->
           <fieldset py:when="4">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
-            <img class="icon" alt="Account guard" src="${href.chrome('/acct_mgr/guard.png')}" />
+            <img class="icon" alt="Account guard icon"
+                 src="${href.chrome('/acct_mgr/guard.png')}" />
 
             <h3>Objective for Account Protection rules</h3>
-            <p>${
-              dgettext(
-                "acct_mgr",
-                "Passwords are often not constructed as carefully as they should "
-                "be. And even a strong passphrase could be sift out, if an "
-                "attacker is able to test millions of variants in hours, if not "
-                "seconds. Firewalls and full-featured web-servers already offer "
-                "sophisticated protection, if one can afford them, handle their "
-                "installation, configuration and maintenance.")
-            }</p>
+            <p>
+              Passwords are often not constructed as carefully as they should
+              be.  And even a strong passphrase could be sift out, if an
+              attacker is able to test millions of variants in hours, if not
+              seconds.  Firewalls and full-featured web-servers already offer
+              sophisticated protection, if one can afford them, handle their
+              installation, configuration and maintenance.
+            </p>
             <p i18n:msg="">
-              The <strong>AccountGuard</strong> component is another option. <!--!
-           -->It is an add-on to AccountManagerPlugin's own <!--!
-           --><strong>LoginModule</strong> and provides account protection <!--!
-           -->by discouraging brute-force login attempts.
+              The <strong>AccountGuard</strong> component is another option.
+              It is an add-on to AccountManagerPlugin's own
+              <strong>LoginModule</strong> and provides account protection
+              by discouraging brute-force login attempts.
             </p>
 
             <div class="field">
               <label>
                 <input type="checkbox" name="acctmgr_guard"
                        checked="${acctmgr_guard and 'checked' or None}"
                        disabled="${not acctmgr_login and 'disabled' or None}"
@@ -789,85 +769,83 @@
                   Failed login attempt count max:
                   <input type="text" class="numwidget"
                          name="login_attempt_max_count"
                          title="${'[account-manager] login_attempt_max_count'}"
                          value="$login_attempt_max_count" />
                 </label>
                 <p class="hint" i18n:msg="">
-                  Lock user account after the specified number of failed <!--!
-                  -->attempts. Value zero means <strong>no limit</strong>.
+                  Lock user account after the specified number of failed
+                  attempts.  Value zero means <strong>no limit</strong>.
                 </p>
               </div>
               <div id="user_lock_time">
                 <div class="field">
                   <label i18n:msg="">
-                    Drop lock after <input
-                      type="text" class="numwidget" name="user_lock_time"
-                      title="${'[account-manager] user_lock_time'}"
-                      value="$user_lock_time" /> seconds
+                    Drop lock after
+                    <input type="text" class="numwidget" name="user_lock_time"
+                           title="${'[account-manager] user_lock_time'}"
+                           value="$user_lock_time" />
+                    seconds
                   </label>
                   <p class="hint" i18n:msg="">
                     Zero means <strong>unlimited</strong> lock time here.
                   </p>
                 </div>
                 <div id="user_lock_time_progression">
                   <div class="field">
                     <label>
                       Lock time progression factor:
                       <input type="text" class="numwidget"
                              name="user_lock_time_progression"
                              title="${'[account-manager] user_lock_time_progression'}"
                              value="$user_lock_time_progression" />
                     </label>
-                    <p class="hint">${
-                      dgettext("acct_mgr",
-                              "Extend user account lock duration incrementally. "
-                              "It uses logarithmic calculation with the factor as "
-                              "exponent, accepting decimal numbers >= 1.")
-                    }</p>
-                    ${
-                      i18n_tag(
-                        dgettext(
-                          "acct_mgr",
-                          "[1:Lock time will grow for any value > 1, if the failure happens before "
-                          "lock expiration. I.e. value '2' means][2:[3:[4:double lock time after 2nd"
-                          " failure,]][5:[6:four times the initial lock time after 3rd,]][7:[8:eight"
-                          " times as long after 4th failure, etc.]]]"),
-                        ('p', {'class': 'hint'}),
-                        'ul',
-                        'li', ('span', {'class': 'hint'}),
-                        'li', ('span', {'class': 'hint'}),
-                        'li', ('span', {'class': 'hint'}),
-                      )
-                    }
-                    <p class="hint">${
-                      dgettext("acct_mgr",
-                               "At any time after lock expiration a login failure will "
-                               "just trigger a lock and set a new lock timeout, but not "
-                               "extend the total lock duration.")
-                    }</p>
+                    <p class="hint">
+                      Extend user account lock duration incrementally.
+                      It uses logarithmic calculation with the factor as
+                      exponent, accepting decimal numbers >= 1.
+                    </p>
+                    <p class="hint">
+                      Lock time will grow for any value > 1, if the failure
+                      happens before lock expiration.  I.e. value '2' means
+                    </p>
+                    <ul i18n:msg="">
+                      <li><span class="hint">
+                        double lock time after 2nd failure,</span>
+                      </li>
+                      <li><span class="hint">
+                        four times the initial lock time after 3rd,</span>
+                      </li>
+                      <li><span class="hint">
+                        eight times as long after 4th failure, etc.</span>
+                      </li>
+                    </ul>
+                    <p class="hint">
+                      At any time after lock expiration a login failure will
+                      just trigger a lock and set a new lock timeout, but not
+                      extend the total lock duration.
+                      </p>
                   </div>
-                  <!--! Last value cache for JS code -->
+                  <!-- Last value cache for JS code -->
                   <input type="hidden" id="user_lock_max_time_old"
                          value="$user_lock_max_time" disabled="disabled" />
                   <div id="user_lock_max_time" class="field">
-                    <label py:with="
-                      ">${
-                      i18n_tag(
-                        dgettext("acct_mgr",
-                                 "Upper lock time limit: [1:] seconds [2:(%(time)s)]"),
-                        ('input', {'type': 'text', 'class': 'numwidget',
-                                   'name': 'user_lock_max_time',
-                                   'title': '[account-manager] user_lock_max_time',
-                                   'value': user_lock_max_time}),
-                        ('span', {'class': 'hint',
-                                  'style': None if user_lock_max_time else 'display:none'}),
-                        time=format_timespan(user_lock_max_time) if user_lock_max_time else '', \
-                      )
-                    }</label>
+                    <label>
+                      Upper lock time limit:
+                      <input type="text" class="numwidget"
+                             name="user_lock_max_time"
+                             title="${'[account-manager] user_lock_max_time'}"
+                             value="$user_lock_max_time" />
+                      seconds
+                      <span class="hint" py:if="user_lock_max_time"
+                            id="pretty_user_lock_max_time">
+                        (${pretty_precise_timedelta(None,
+                                                    diff=user_lock_max_time)})
+                      </span>
+                    </label>
                     <p class="hint">
                       This is relevant only with a progression factor > 1.
                     </p>
                   </div>
                 </div>
               </div>
             </div>
@@ -876,143 +854,145 @@
           <!--! Page 6 -->
           <fieldset py:otherwise="">
             <legend class="step" i18n:msg="step,label">
               Step ${str(active + 1)}: ${steps[active].label}
             </legend>
             <div py:if="not admin_available">
               <h3>Objective for additional preparation</h3>
-              <p>Enable yourself to proceed beyond this initial setup.</p>
+                <p>
+                  Enable yourself to proceed beyond this initial setup.
+                </p>
               <h3>Initial Admin Account</h3>
               <fieldset>
                 <legend>Add Admin Account:</legend>
                 <p i18n:msg="">
-                  The user will get <strong>TRAC_ADMIN</strong> assigned, <!--!
-               -->that inherits all available permissions. One such <!--!
-               -->account is required to configure Trac via the admin <!--!
-               -->web-UI. Create and manage more limited admin accounts <!--!
-               -->as well as actual user accounts on your own later via <!--!
-               -->the Accounts admin panel.
+                  The user will get <strong>TRAC_ADMIN</strong> assigned, that
+                  inherits all available permissions.  One such account is
+                  required to configure Trac via the admin web-UI.  Create and
+                  manage more limitted admin accounts as well as actual user
+                  accounts on your own later via the Accounts admin panel.
                 </p>
                 <p class="hint" i18n:msg="">
-                  In detail: AccountManagerPlugin requires <!--!
-               --><strong>ACCTMGR_USER_ADMIN</strong> for regular user <!--!
-               -->administration, <strong>ACCTMGR_CONFIG_ADMIN</strong> <!--!
-               -->for viewing these pages and changing the configuration <!--!
-               -->later. Both are inherited by <!--!
-               --><strong>ACCTMGR_ADMIN</strong> permission. To assign <!--!
-               -->permissions you'll need <strong>PERMISSION_GRANT</strong> <!--!
-               -->inherited by <strong>PERMISSION_ADMIN</strong> too.
+                  In detail: AccountManagerPlugin requires
+                  <strong>ACCTMGR_USER_ADMIN</strong> for regular user
+                  administration, <strong>ACCTMGR_CONFIG_ADMIN</strong> for
+                  viewing these pages and changing the configuration later.
+                  Both are inherited by <strong>ACCTMGR_ADMIN</strong>
+                  permission.  To assign permissions you'll need
+                  <strong>PERMISSION_GRANT</strong> inherited by
+                  <strong>PERMISSION_ADMIN</strong> too.
                 </p>
                 <div class="field">
                   <label>Username:<br />
                     <input type="text" class="textwidget" id="username"
                            name="username" value="$acctmgr.username" />
                   </label>
                   <p class="hint" py:if="ignore_auth_case">
                     Only lowercase usernames allowed
                   </p>
                 </div>
                 <div class="field">
-                  <label>Password:<br />
+                  <label py:choose="">Password:<br />
                     <input type="password" class="textwidget" name="password"
-                           disabled="${None if set_password else 'disabled'}" />
+                           disabled="${not set_password and 'disabled' or
+                                       None}" />
                   </label>
                 </div>
                 <div class="field">
                   <label >Confirm Password:<br />
                     <input type="password" class="textwidget"
                            name="password_confirm"
-                           disabled="${None if set_password else 'disabled'}" />
+                           disabled="${not set_password and 'disabled' or
+                                       None}" />
                   </label>
                 </div>
-                <p py:if="not password_store">${
-                  dgettext("acct_mgr",
-                           "Please take care, that the username is known by "
-                           "the HTTP authentication provider.")
-                }</p>
-                <p py:if="password_store and not set_password">${
-                  dgettext("acct_mgr",
-                           "Please take care for a valid username, because no configured "
-                           "password store supports creating a new account.")
-                }</p>
+                <p py:if="not password_store">
+                  Please take care, that the username is known by the HTTP
+                  authentication provider.
+                </p>
+                <p py:if="password_store and not set_password">
+                  Please take care for a valid username, because no
+                  configured password store supports creating a new account.
+                </p>
                 <div class="buttons">
-                  <input type="submit" name="add" value="${dgettext('acct_mgr', ' Add ')}" />
+                  <input type="submit" name="add"
+                         value="${dgettext('acct_mgr', ' Add ')}" />
                 </div>
               </fieldset>
             </div>
             <h3>Check-up</h3>
             <ul>
               <li py:for="goal in completion.details" class="$goal.status">
                 <a href="${href.admin('accounts', 'config', step=goal.step)}"
                    py:strip="not goal.step">
                   $goal.desc
                 </a>
               </li>
             </ul>
             <p class="hint" py:if="admin_available and not completion.ready">
-              Please resolve all issues marked as critical.
+              Please resolve all issues marked as critical. 
             </p>
             <div py:if="completion.ready">
               <p i18n:msg="">
-                By now you did almost finish AccountManagerPlugin <!--!
-             -->configuration, but any changes are temporary yet. Please <!--!
-             -->test and adjust the configuration as required, or cancel <!--!
-             -->to revert all changes. Apply settings to <!--!
-             --><em>trac.ini</em> only if you really want to preserve <!--!
-             -->them permanently.
+                By now you did almost finish AccountManagerPlugin
+                configuration, but any changes are temporary yet. Please test
+                and adjust the configuration as required, or cancel to revert
+                all changes.  Apply settings to <em>trac.ini</em> only if you
+                really want to preserve them permanently.
               </p>
               <!--! Final configuration preview listing -->
               <fieldset>
                 <legend class="foldable">Details (Preview)</legend>
-                <div class="ini">
-                  <py:for each="section in sorted(roundup)">
+                <div class="ini" py:with="sections = sorted(roundup.keys())"
+                     xml:lang="en">
+                  <py:for each="section in sections">
                     [$section]<br />
-                    <py:for each="option, value in sorted(roundup[section])">
-                      <span class="${'defaults'
-                                     if option in roundup_defaults.get(section, {}) else
-                                     None}"
-                            >${option} = ${value}</span><br />
+                    <py:for each="option in sorted(roundup[section])"
+                            py:choose="">
+                      <py:when test="option[0] in roundup_defaults[section]">
+                        <span class="defaults">
+                          ${option[0]} = ${option[1]}
+                        </span><br />
+                      </py:when>
+                      <py:otherwise>
+                        ${option[0]} = ${option[1]}<br />
+                      </py:otherwise>
                     </py:for>
                     <br />
                   </py:for>
                 </div>
               </fieldset>
             </div>
+            
           </fieldset>
         </py:choose>
 
         <!-- Bottom navigation -->
         <div class="buttons">
-          <input py:if="active != 0 and active != (len(steps) - 1)"
-                 type="submit" name="back"
+          <input type="submit" name="back"
+                 py:if="active != 0 and active != (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Apply changes and go back')}"
                  value="${dgettext('acct_mgr', 'Previous')}" />
-          <input py:if="active == (len(steps) - 1)"
-                 type="submit" name="prev"
+          <input type="submit" name="prev" py:if="active == (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Go back')}"
                  value="${dgettext('acct_mgr', 'Previous')}" />
-          <input py:if="active != (len(steps) - 1)"
-                 type="submit" name="save"
+          <input type="submit" name="save" py:if="active != (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Stay on page')}"
                  value="${dgettext('acct_mgr', 'Apply changes')}" />
-          <input py:if="active == (len(steps) - 1)"
-                 type="submit" name="save"
+          <input type="submit" name="save" py:if="active == (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Save changes and exit wizard')}"
                  value="${dgettext('acct_mgr', 'Apply changes')}"
                  disabled="${not completion.ready and 'disabled' or None}" />
-          <input py:if="active != (len(steps) - 1)"
-                 type="submit" name="reset"
+          <input type="submit" name="reset" py:if="active != (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Drop unsaved changes')}"
                  value="${dgettext('acct_mgr', 'Refresh')}" />
-          <input py:if="active != (len(steps) - 1)"
-                 type="submit" name="next"
+          <input type="submit" name="next" py:if="active != (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Apply changes and go on')}"
                  value="${dgettext('acct_mgr', 'Next')}" />
-          <input py:if="active == (len(steps) - 1)"
-                 type="submit" name="exit"
+          <input type="submit" name="exit" py:if="active == (len(steps) - 1)"
                  title="${dgettext('acct_mgr', 'Drop changes and exit wizard')}"
                  value="${dgettext('acct_mgr', 'Cancel')}" />
         </div>
       </form>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,263 +1,246 @@
+_dgettext ?>
 ********** AAccccoouunnttss:: CCoonnffiigguurraattiioonn **********
     * _$_{_i_d_x_ _+_ _1_} _[_$_{_s_t_e_p_._l_a_b_e_l_}_]_$_s_t_e_p_._l_a_b_e_l
 [${dgettext('acct_mgr', 'Previous')}][${dgettext('acct_mgr', 'Previous')}][$
 {dgettext('acct_mgr', 'Next')}]
 Step ${str(active + 1)}: ${steps[active].label}
 ******** OObbjjeeccttiivvee ffoorr sseettttiinngg AAuutthheennttiiccaattiioonn OOppttiioonnss ********
-${ dgettext("acct_mgr", "Decide, whether to use HTTP authentication (Trac
-default) or a HTML login" " form provided by AccountManagerPlugin.") }
-${ dgettext("acct_mgr", "After initial login Trac sessions are authenticated
-per request based on " "browser cookies. Therefore a number of options provide
-control over some " "critical browser cookie properties.") }
+Decide, whether to use HTTP authentication (Trac default) or a HTML login form
+provided by AccountManagerPlugin.
+After initial login Trac sessions are authenticated per request based on
+browser cookies. Therefor a number of options provide control over some
+critical browser cookie properties.
 ******** PPrroovviiddeerr--aaggnnoossttiicc AAuutthheennttiiccaattiioonn OOppttiioonnss ********
 Convert login names to lower case on registration and login.
 Adapt to careless username typing, where casing does not matter, like on
 Windows. Potentially troublesome, because case matters for Trac permission
 assignment lookup anyway.
 Check IP address for authentication.
-${ dgettext("acct_mgr", "Potentially troublesome for users with dynamic IP
-address, but " "disregarded for persistent sessions.") }
+Potentially troublesome for users with dynamic IP adress, but disregarded for
+persistent sessions.
 Restrict sending cookies to HTTPS connections.
 Required, if the Trac instance is only accessible through HTTPS.
-${ i18n_tag( dgettext("acct_mgr", "Lifetime of the authentication cookie: [1:
-] seconds [2:(%(timedelta)s)]"), ('input', {'type': 'text', 'class':
-'numwidget', 'name': 'auth_cookie_lifetime', 'title': '[trac]
-auth_cookie_lifetime', 'value': auth_cookie_lifetime}), ('span', {'class':
-'hint', 'style': None if lifetime_value else 'display:none'}),
-timedelta=format_timespan(lifetime_value), ) }
-${ dgettext("acct_mgr", "Determines how long the browser will cache
-authentication " "information, and therefore, after how much inactivity a user
-will " "have to log in again. Default (0 s) makes cookie expire at " "browsing
-sessions end.") }
+Lifetime of the authentication cookie: [$auth_cookie_lifetime]seconds ($
+{pretty_precise_timedelta(None, diff=value)})
+Determines how long the browser will cache authentication information, and
+therefore, after how much inactivity a user will have to log in again. Default
+(0 s) makes cookie expire at browsing sessions end.
 ******** AAuutthheennttiiccaattiioonn FFrroonntt--eenndd ********
-#${dgettext("acct_mgr", "Use HTTP authentication and credentials as configured
-" "in and provided by your web-server.")}
-${ dgettext("acct_mgr", "You can still manage some password stores with "
-"AccountManagerPlugin, if you configure them in the next step.") }
-#${dgettext("acct_mgr", "Use a HTML login form backed by one or more "
-"password stores managed by AccountManagerPlugin.")}
+#Use HTTP authentication and credentials as configured in and provided by your
+web-server.
+You can still manage some password stores with AccountManagerPlugin, if you
+configure them in the next step.
+#Use a HTML login form backed by one or more password stores managed by
+AccountManagerPlugin.
 AccountManagerPlugin provides a custom version of the LLooggiinnMMoodduullee accompanied
 by a form-based HTML login page.
 If you enable this feature, you'll want to review and adjust some more options
 related to session authentication. Note, that AccountManagerPlugin's
 LoginModule changes the default lifetime of authentication cookies to 30 days.
 ******** AAccccoouunnttMMaannaaggeerrPPlluuggiinn AAuutthheennttiiccaattiioonn OOppttiioonnss ********
-Integrate links to related actions into the login form. ${ i18n_tag( dgettext
-( "acct_mgr", "[1:If enabled, links to][2:[3:[4:Lost password/Password "
-"reset]][5:[6:Registration for new users]]][7:that normally reside in " "Trac's
-meta-navigation bar, will appear inside the login form. CSS " "styling allows
-further customization of the login prompt.]" ), ('p', {'class': 'hint'}), 'ul',
-'li', ('span', {'class': 'hint'}), 'li', ('span', {'class': 'hint'}), ('p',
-{'class': 'hint'}), ) }
-${dgettext("acct_mgr", "Allow the user to be remembered across sessions "
-"without needing to re-authenticate.")}
+Integrate links to related actions into the login form.
+If enabled, links to
+    * Lost password/Password reset
+    * Registration for new users
+that normally reside in Trac's meta-navigation bar, will appear inside the
+login form. CSS styling allows further customization of the login prompt.
+Allow the user to be remembered across sessions without needing to re-
+authenticate.
 This is, user checks a "Remember Me" checkbox in the AccountManagerPlugin login
 form and, next time he visits the site within 30 days, he'll be remembered and
 authenticated automatically.
 Likelihood of session cookie ID change: [$cookie_refresh_pct ]% per work hour
 Driving a refresh process to decrease vulnerability of long-lasting sessions.
 Zero means nneevveerr.
 Path for authentication cookie:[$auth_cookie_path   ]
 This enables AccountManagerPlugin's authentication data distribution to Trac
 instances with matching cookie path. Set this to a common base path of several
 Trac instances to share the cookie, providing a cheap Single-Sign-On
 experience.
-Step ${str(active + 1)}: ${steps[active].label}[Password store]
+Step ${str(active + 1)}: ${steps[active].label}[Password store icon]
 ******** OObbjjeeccttiivvee ffoorr ccoonnffiigguurriinngg aa PPaasssswwoorrdd SSttoorree ********
-${ dgettext("acct_mgr", "AccountManagerPlugin manages user credentials in a
-modular " "back-end providing access to at least one password store.") }
+AccountManagerPlugin manages user credentials in a modular back-end providing
+access to at least one password store.
 ******** IInniittiiaall AAuutthheennttiiccaattiioonn BBaacckk--eenndd sseelleeccttiioonn ********
 #Use a password store embedded into Trac db.
 The SSeessssiioonnSSttoorree implements password storage in Trac db table
-'session_attribute'. Its the default choice mainly for avoiding additional
+'session_attributes'. Its the default choice mainly for avoiding additional
 dependencies like directory and file permissions.
-${ dgettext( "acct_mgr", "While great to resolve some concurrent access issues
-too, " "this password store has shortcomings as well. Notably it " "does not
-support seamless hash type migration, and its no " "candidate for shared use by
-multiple Trac instances or even " "by applications beyond Trac.") }
+While great to resolve some concurrent access issues too, this password store
+has shortcomings as well. Notably it does not support seamless hash type
+migration, and its no candidate for shared use by multiple Trac instances or
+even by applications beyond Trac.
 Details (Preview)
 $init_store_hint.db
-${ dgettext("acct_mgr", "Please apply these default options first. " "You'll be
-able to change values afterwards.") }
+Please apply these default options first. You'll be able to change values
+afterwards.
 #Use a file-based password store.
-${ dgettext("acct_mgr", "AccountManagerPlugin includes native support for
-common " "Apache file formats 'htpasswd' and 'htdigest' as well as " "support
-for reading svnserve's password file format.") }
-${ dgettext("acct_mgr", "You may use the same file for several Trac
-environments. " "Note that setting appropriate directory and file permissions "
-"is crucial for these stores, but not covered by this " "configuration
-wizard.") }
+AccountManagerPlugin includes native support for common Apache file formats
+'htpasswd' and 'htdigest' as well as support for reading svnserve's password
+file format.
+You may use the same file for several Trac environments. Note that setting
+appropriate directory and file permissions is crucial for these stores, but not
+covered by this configuration wizard.
 #'htdigest' format (HHttDDiiggeessttSSttoorree) Details (Preview)
 $init_store_hint.htdigest
-${ dgettext("acct_mgr", "Please apply these default options first. " "You'll be
-able to change values afterwards.") }
+Please apply these default options first. You'll be able to change values
+afterwards.
 #'htpasswd' format (HHttPPaasssswwddSSttoorree) Details (Preview)
 $init_store_hint.htpasswd
-${ dgettext("acct_mgr", "Please apply these default options first. " "You'll be
-able to change values afterwards.") }
+Please apply these default options first. You'll be able to change values
+afterwards.
 #svnserve's password file format (SSvvnnSSeerrvveePPaasssswwoorrddSSttoorree) Details (Preview)
 $init_store_hint.svn_file
-${ dgettext("acct_mgr", "Please apply these default options first. " "You'll be
-able to change values afterwards.") }
+Please apply these default options first. You'll be able to change values
+afterwards.
 #Delegate authentication using HTTP authentication.
 AccountManagerPlugin enables use of standard HTTP-Auth by its HHttttppAAuutthhSSttoorree
 component. Both Basic and Digest authentication challenges are supported.
-${ dgettext("acct_mgr", "In addition to being read-only this password store
-does " "not even support listing users for obvious reasons.") }
+In addition to being read-only this password store does not even support
+listing users for obvious reasons.
 Details (Preview)
 $init_store_hint.http
-${ dgettext("acct_mgr", "Please apply these default options first. " "You'll be
-able to change values afterwards.") }
+Please apply these default options first. You'll be able to change values
+afterwards.
 #Use a different password store.
-${ dgettext( "acct_mgr", "AccountManagerPlugin's modular password store concept
-" "encourages creation of more ways to provide user credential " "beyond the
-natively supported stores. While a specific setup " "assistance for these 3rd-
-party authentication providers is not " "implemented, you may fill-in
-appropriate configuration details " "for an already installed component
-below.") }
+AccountManagerPlugin's modular password store concept encourages creation of
+more ways to provide user credential beyond the natively supported stores.
+While specific setup assistance for these 3rd-party authentication providers is
+not implemented, you may fill-in approprate configuration details for an
+already installed component below.
 Configuration
 $init_store_hint.http
-${ dgettext("acct_mgr", "Type the custom configuration options as provided by "
-"that components documentation and apply it.") }
+Type the custom configuration options as provided by that components
+documentation and apply it.
 ******** PPaasssswwoorrdd SSttoorree CCoonnffiigguurraattiioonn ********
 All enabled stores are listed below, but most won't work at all without
 additional configuration.
 Currently configured: $${{'',, ''..jjooiinn((ppaasssswwoorrdd__ssttoorree))}}
 This is an experts-only type of store configuration.
 RReeqquuiirreedd ddiissaabblleedd ccoommppoonneenntt((ss)):: $${{'',, ''..jjooiinn((ddiissaabblleedd__ssttoorree))}}
-${ dgettext("acct_mgr", "Select one or more stores and configure related
-options. " "Concurrent use of multiple password stores is supported too.") }
+Select one or more stores and configure related options. Concurrent use of
+multiple password stores is supported too.
 Password stores are queried in turn, so order matters.
 [One of: ${order == 0 and '--' or order}]$section.name
 $option.label:
 ${option.value['error']}
 [One of: ${opt}][$option.value       ]
 $option.doc
 Silently update password hashes on next successful login.
-${ dgettext("acct_mgr", "Use it after changing hash type or to migrate to a new
-" "primary password store.") }
-${ dgettext("acct_mgr", "The update will run only once. Restarting the
-procedure " "for all accounts allows to propagate subsequent changes.") }
+Use it after changing hash type or to migrate to a new primary password store.
+The update will run only once. Restarting the procedure for all accounts allows
+to propagate subsequent changes.
 [${dgettext('acct_mgr', 'Restart')}]
-Step ${str(active + 1)}: ${steps[active].label}[Password refresh]
+Step ${str(active + 1)}: ${steps[active].label}[Password refresh icon]
 ******** OObbjjeeccttiivvee ffoorr PPaasssswwoorrdd PPoolliiccyy rruulleess ********
-${ dgettext("acct_mgr", "While AccountManagerPlugin does not enforce password
-rules in " "general, there are some other ways to alter password handling.") }
+While AccountManagerPlugin does not enforce password rules in general, there
+are some other ways to alter password handling.
 Enable the password reset procedure.
-${ dgettext("acct_mgr", "It relies on a working email sender for Trac,
-supporting " "both TracAnnouncer and TracNotification.") }
+It relies on a working email sender for Trac, supporting both TracAnnouncer and
+TracNotification.
 Length of the randomly-generated passwords:
 [$generated_password_length]characters
 These passwords are used as alternative passwords on request.
 Force users to change passwords after a password reset.
-Step ${str(active + 1)}: ${steps[active].label}[Account approval]
+Step ${str(active + 1)}: ${steps[active].label}[Account approval icon]
 ******** OObbjjeeccttiivvee ffoorr AAccccoouunntt RReeggiissttrraattiioonn aanndd VVeerriiffiiccaattiioonn rruulleess ********
-${ dgettext( "acct_mgr", "You may require administrative approval of new
-accounts for the user " "registration process. The ability to immediately ban
-existing accounts is" " another, related but independent feature.") }
+You may require administrative approval of new accounts for the user
+registration process. The ability to immediately ban existing accounts is
+another, related but independed feature.
 Allow administrative user ID changes.
 Allow users to register for a new account.
 Allow users to delete their own account.
 ******** CChheecckkss ttoo uussee ffoorr vvaalliiddaattiinngg RReeggiissttrraattiioonn rreeqquueessttss ********
 All checks provided by AccountManagerPlugin are enabled per default, but some
 are configurable on their own.
 Currently configured: $${{'',, ''..jjooiinn((rreeggiisstteerr__cchheecckk))}}
 Checks like BBoottTTrraappCChheecckk won't work at all without additional configuration.
 RReeqquuiirreedd ddiissaabblleedd ccoommppoonneenntt((ss)):: $${{'',, ''..jjooiinn((ddiissaabblleedd__cchheecckk))}}
-${ dgettext( "acct_mgr", "Select one or more checks and configure related
-options. " "Concurrent use of multiple registration checks is encouraged.") }
-${ dgettext( "acct_mgr", "Checks are applied in turn, so order matters. Note
-that some " "checks are used to validate admin user actions too.") }
+Select one or more checks and configure related options. Concurrent use of
+multiple registration checks is encouraged.
+Checks are applied in turn, so order matters. Note that some checks are used to
+validate admin user actions too.
 [One of: ${order == 0 and '--' or order}]$section.name
 ${safe_wiki_to_html(context, section.doc)}
 $option.label:
 ${option.value['error']}
 [One of: ${opt}][$option.value       ]
 $option.doc
 ******** OOtthheerr AAccccoouunntt PPoolliiccyy ooppttiioonnss ********
 Require administrative account approval after registration.
-${ dgettext( "acct_mgr", "For admin notification on registration time it relies
-on a " "working email sender for Trac, supporting both TracAnnouncer " "and
-TracNotification.") }
+For admin notification on registration time it relies on a working email sender
+for Trac, supporting both TracAnnouncer and TracNotification.
 Force users to verify their email addresses.
-${ dgettext( "acct_mgr", "For sending a verification token to the user it
-relies on a working email " "sender for Trac, supporting both TracAnnouncer and
-TracNotification.") }
-Step ${str(active + 1)}: ${steps[active].label}[Account guard]
+For sending a verificaton token to the user it relies on a working email sender
+for Trac, supporting both TracAnnouncer and TracNotification.
+Step ${str(active + 1)}: ${steps[active].label}[Account guard icon]
 ******** OObbjjeeccttiivvee ffoorr AAccccoouunntt PPrrootteeccttiioonn rruulleess ********
-${ dgettext( "acct_mgr", "Passwords are often not constructed as carefully as
-they should " "be. And even a strong passphrase could be sift out, if an "
-"attacker is able to test millions of variants in hours, if not " "seconds.
-Firewalls and full-featured web-servers already offer " "sophisticated
-protection, if one can afford them, handle their " "installation, configuration
-and maintenance.") }
+Passwords are often not constructed as carefully as they should be. And even a
+strong passphrase could be sift out, if an attacker is able to test millions of
+variants in hours, if not seconds. Firewalls and full-featured web-servers
+already offer sophisticated protection, if one can afford them, handle their
+installation, configuration and maintenance.
 The AAccccoouunnttGGuuaarrdd component is another option. It is an add-on to
 AccountManagerPlugin's own LLooggiinnMMoodduullee and provides account protection by
 discouraging brute-force login attempts.
 Enable the guard add-on component.
 AccountManagerPlugin's LoginModule is disabled.
 Failed login attempt count max:[$login_attempt_max_count]
 Lock user account after the specified number of failed attempts. Value zero
 means nnoo lliimmiitt.
 Drop lock after [$user_lock_time     ]seconds
 Zero means uunnlliimmiitteedd lock time here.
 Lock time progression factor:[$user_lock_time_progression]
-${ dgettext("acct_mgr", "Extend user account lock duration incrementally. " "It
-uses logarithmic calculation with the factor as " "exponent, accepting decimal
-numbers >= 1.") }
-${ i18n_tag( dgettext( "acct_mgr", "[1:Lock time will grow for any value > 1,
-if the failure happens before " "lock expiration. I.e. value '2' means][2:[3:
-[4:double lock time after 2nd" " failure,]][5:[6:four times the initial lock
-time after 3rd,]][7:[8:eight" " times as long after 4th failure, etc.]]]"),
-('p', {'class': 'hint'}), 'ul', 'li', ('span', {'class': 'hint'}), 'li',
-('span', {'class': 'hint'}), 'li', ('span', {'class': 'hint'}), ) }
-${ dgettext("acct_mgr", "At any time after lock expiration a login failure will
-" "just trigger a lock and set a new lock timeout, but not " "extend the total
-lock duration.") }
-${ i18n_tag( dgettext("acct_mgr", "Upper lock time limit: [1:] seconds [2:(%
-(time)s)]"), ('input', {'type': 'text', 'class': 'numwidget', 'name':
-'user_lock_max_time', 'title': '[account-manager] user_lock_max_time', 'value':
-user_lock_max_time}), ('span', {'class': 'hint', 'style': None if
-user_lock_max_time else 'display:none'}), time=format_timespan
-(user_lock_max_time) if user_lock_max_time else '', \ ) }
+Extend user account lock duration incrementally. It uses logarithmic
+calculation with the factor as exponent, accepting decimal numbers >= 1.
+Lock time will grow for any value > 1, if the failure happens before lock
+expiration. I.e. value '2' means
+    * double lock time after 2nd failure,
+    * four times the initial lock time after 3rd,
+    * eight times as long after 4th failure, etc.
+At any time after lock expiration a login failure will just trigger a lock and
+set a new lock timeout, but not extend the total lock duration.
+Upper lock time limit: [$user_lock_max_time ]seconds ($
+{pretty_precise_timedelta(None, diff=user_lock_max_time)})
 This is relevant only with a progression factor > 1.
 Step ${str(active + 1)}: ${steps[active].label}
 ******** OObbjjeeccttiivvee ffoorr aaddddiittiioonnaall pprreeppaarraattiioonn ********
 Enable yourself to proceed beyond this initial setup.
 ******** IInniittiiaall AAddmmiinn AAccccoouunntt ********
 Add Admin Account:
 The user will get TTRRAACC__AADDMMIINN assigned, that inherits all available permissions.
 One such account is required to configure Trac via the admin web-UI. Create and
-manage more limited admin accounts as well as actual user accounts on your own
+manage more limitted admin accounts as well as actual user accounts on your own
 later via the Accounts admin panel.
 In detail: AccountManagerPlugin requires AACCCCTTMMGGRR__UUSSEERR__AADDMMIINN for regular user
 administration, AACCCCTTMMGGRR__CCOONNFFIIGG__AADDMMIINN for viewing these pages and changing the
 configuration later. Both are inherited by AACCCCTTMMGGRR__AADDMMIINN permission. To assign
 permissions you'll need PPEERRMMIISSSSIIOONN__GGRRAANNTT inherited by PPEERRMMIISSSSIIOONN__AADDMMIINN too.
 Username:
 [$acctmgr.username   ]
 Only lowercase usernames allowed
 Password:
 [********************]
 Confirm Password:
 [********************]
-${ dgettext("acct_mgr", "Please take care, that the username is known by " "the
-HTTP authentication provider.") }
-${ dgettext("acct_mgr", "Please take care for a valid username, because no
-configured " "password store supports creating a new account.") }
+Please take care, that the username is known by the HTTP authentication
+provider.
+Please take care for a valid username, because no configured password store
+supports creating a new account.
 [${dgettext('acct_mgr', ' Add ')}]
 ******** CChheecckk--uupp ********
     * _$_g_o_a_l_._d_e_s_c
 Please resolve all issues marked as critical.
 By now you did almost finish AccountManagerPlugin configuration, but any
 changes are temporary yet. Please test and adjust the configuration as
 required, or cancel to revert all changes. Apply settings to ttrraacc..iinnii only if
 you really want to preserve them permanently.
 Details (Preview)
 [$section]
-${option} = ${value}
+${option[0]} = ${option[1]}
+${option[0]} = ${option[1]}
 
 [${dgettext('acct_mgr', 'Previous')}][${dgettext('acct_mgr', 'Previous')}][$
 {dgettext('acct_mgr', 'Apply changes')}][${dgettext('acct_mgr', 'Apply
 changes')}][${dgettext('acct_mgr', 'Refresh')}][${dgettext('acct_mgr',
 'Next')}][${dgettext('acct_mgr', 'Cancel')}]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_db_cleanup.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_db_cleanup.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:py="http://genshi.edgewall.org/" 
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="admin.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Accounts: Cleanup</title>
   </head>
 
   <body>
     <h2>Accounts: Cleanup</h2>
     <form id="cleanup" class="mod" method="post">
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+_dgettext ?>
 ********** AAccccoouunnttss:: CClleeaannuupp **********
 ?  AAccccoouunntt
 ?  ?  AAttttrriibbuuttee VVaalluuee
 Authenticated Accounts
 ??? ''$${{aaccccoouunntt}}''
   ?? '${name}' '${value}'
 [${dgettext('acct_mgr', 'Remove selected entries')}][${dgettext('acct_mgr',
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_login.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_login.html`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="layout.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Login</title>
     <script type="text/javascript">
     jQuery(document).ready(function($) {
         $("body").addClass("login");
         $('#username').focus();
     });
@@ -32,39 +35,45 @@
                  size="20" />
         </div>
         <div class="textbox">
           <label for="password">Password:</label><br />
           <input type="password" id="password" name="password"
                  class="textwidget" size="20" />
         </div>
-        <div id="login_options" class="central">
-          <div py:if="reset_password_enabled and not login_opt_list">
-            <p class="hint">
-              <a href="${href.reset_password()}">Forgot your password?</a>
-            </p>
-          </div>
-          <div class="textbox" py:if="persistent_sessions">
-            <input type="checkbox" id="rememberme" name="rememberme" value="1" />
-            <label for="rememberme">Remember me</label>
-          </div>
-          <div class="buttons">
-            <input type="submit" value="${dgettext('acct_mgr', 'Login')}" />
-          </div>
-          <div class="nav" py:if="login_opt_list">
-            <ul>
-              <li py:if="registration_enabled"
-                  class="${classes(first=True, last=not reset_password_enabled)}">
+        <div id="login_options" class="central"
+             py:if="reset_password_enabled and login_opt_list != True">
+          <p class="hint">
+            <a href="${href.reset_password()}">Forgot your password?</a>
+          </p>
+        </div>
+        <div class="textbox" py:if="persistent_sessions">
+          <input type="checkbox" id="rememberme" name="rememberme"
+                 value="1" />
+          <label for="rememberme">Remember me</label>
+        </div>
+        <div id="login_options" class="buttons central nav">
+          <input type="submit" value="${dgettext('acct_mgr', 'Login')}" />
+          <ul py:if="login_opt_list is True">
+            <py:choose py:if="registration_enabled">
+              <li class="first" py:when="reset_password_enabled">
+                <a href="${href.register()}">Register</a>
+              </li>
+              <li class="first last" py:otherwise="">
                 <a href="${href.register()}">Register</a>
               </li>
-              <li py:if="reset_password_enabled"
-                  class="${classes(first=not registration_enabled, last=True)}">
+            </py:choose>
+            <py:choose py:if="reset_password_enabled">
+              <li class="last" py:when="registration_enabled">
+                <a href="${href.reset_password()}">Forgot your password?</a>
+              </li>
+              <li class="first last" py:otherwise="">
                 <a href="${href.reset_password()}">Forgot your password?</a>
               </li>
-            </ul>
-          </div>
+            </py:choose>
+          </ul>
         </div>
       </form>
 
     </div>
 
     <div class="central system-message" py:if="login_error">
       <h2>Error</h2>
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
+_dgettext ?>
 ************ LLooggiinn ************
 Username:
 [username            ]
 Password:
 [********************]
 _F_o_r_g_o_t_ _y_o_u_r_ _p_a_s_s_w_o_r_d_?
 ??Remember me
 [${dgettext('acct_mgr', 'Login')}]
     * _R_e_g_i_s_t_e_r
+    * _R_e_g_i_s_t_e_r
+    * _F_o_r_g_o_t_ _y_o_u_r_ _p_a_s_s_w_o_r_d_?
     * _F_o_r_g_o_t_ _y_o_u_r_ _p_a_s_s_w_o_r_d_?
 ********** EErrrroorr **********
 ${login_error}
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_notification.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_notification.html`

 * *Files 10% similar despite different names*

```diff
@@ -3,61 +3,52 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="admin.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Accounts: Notification Configuration</title>
   </head>
 
   <body>
     <h2>Accounts: Notification Configuration</h2>
 
     <form id="accountsconfig" class="mod" method="post">
       <fieldset>
         <legend>Account Notification</legend>
-        <p>${
-          dgettext("acct_mgr",
-                   "Set the following options in order to be notified of "
-                   "account creation, password reset and account deletion.")
-        }</p>
+        <p>Set the following options in order to be notified of
+          account creation, password reset and account deletion.</p>
 
         <h3>Notification Actions</h3>
-        <p class="help" i18n:msg="">
-          This is a list of actions which you can enable or disable by <!--!
-       --><em>checking</em> the <em>checkboxes</em>.
-        </p>
+        <p class="help" i18n:msg="">This is a list of actions which you can
+          enable or disable by <em>checking</em> the <em>checkboxes</em>.</p>
         <label>
           <input type="checkbox" name="notify_actions" value="new"
                  checked="${'new' in notify_actions or None}" />
-          Get notified of new account creation
-        </label>
-        <br/>
+          Get notified of new account creation</label><br/>
         <label>
           <input type="checkbox" name="notify_actions" value="change"
                  checked="${'change' in notify_actions or None}" />
-          Get notified of password reset
-        </label>
-        <br/>
+          Get notified of password reset</label><br/>
         <label>
           <input type="checkbox" name="notify_actions" value="delete"
                  checked="${'delete' in notify_actions or None}" />
-          Get notified of account deletion
-        </label>
+          Get notified of account deletion</label><br/>
 
         <h3>Notification Recipient Addresses</h3>
-        <p class="help">${
-          dgettext("acct_mgr",
-                   "Space-separated list of email addresses and/or usernames "
-                   "that get notified of the above actions:")
-        }</p>
-        <textarea class="trac-fullwidth" name="notify_addresses"
-                  cols="60" rows="2">${' '.join(notify_addresses)}</textarea>
+        <p class="help">Space-separated list of email addresses and/or
+          usernames that get notified of the above actions:
+        </p>
+        <textarea cols="60" name="notify_addresses"
+                  rows="2">${' '.join(notify_addresses)}</textarea>
       </fieldset>
       <div class="buttons">
         <input type="submit" name="save"
                value="${dgettext('acct_mgr', 'Apply changes')}" />
       </div>
     </form>
   </body>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
+_dgettext ?>
 ********** AAccccoouunnttss:: NNoottiiffiiccaattiioonn CCoonnffiigguurraattiioonn **********
 Account Notification
-${ dgettext("acct_mgr", "Set the following options in order to be notified of "
-"account creation, password reset and account deletion.") }
+Set the following options in order to be notified of account creation, password
+reset and account deletion.
 ******** NNoottiiffiiccaattiioonn AAccttiioonnss ********
 This is a list of actions which you can enable or disable by cchheecckkiinngg the
 cchheecckkbbooxxeess.
 Get notified of new account creation
 Get notified of password reset
 Get notified of account deletion
 ******** NNoottiiffiiccaattiioonn RReecciippiieenntt AAddddrreesssseess ********
-${ dgettext("acct_mgr", "Space-separated list of email addresses and/or
-usernames " "that get notified of the above actions:") }
+Space-separated list of email addresses and/or usernames that get notified of
+the above actions:
 ${' '.join(notify_addresses)}
 [${dgettext('acct_mgr', 'Apply changes')}]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_prefs.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_prefs.html`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,18 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:xi="http://www.w3.org/2001/XInclude" 
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="prefs.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
+
   <!--! Begin insert, to be appended below common content, see body -->
   <!--! FIXME: [1] prevents this from matching its own output.
         Should that really be necessary? -->
   <div py:match="div[@id='tabcontent'][1]" py:attrs="select('@*')">
     ${select('*')}
 
     <py:if test="delete_enabled">
@@ -40,15 +44,15 @@
      <script type="text/javascript">
        jQuery(document).ready(function($) {
           $('#old_password').focus();
        });
      </script>
   </head>
 
-  <!--! Common content, will get wrapped in a form with 'save' button -->
+  <!--! Commont content, will get wrapped in a form with 'save' button -->
   <body>
     <h2>Change Password</h2>
     <div class="field">
       <label>Old Password:
         <input type="password" id="old_password" name="old_password"
                class="textwidget" size="20" />
       </label>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+_dgettext ?>
 ${select('*')}
 ===============================================================================
 ********** DDeelleettee AAccccoouunntt **********
 Password:[********************]
 [${dgettext('acct_mgr', 'Delete account')}]
 ********** CChhaannggee PPaasssswwoorrdd **********
 Old Password:[********************]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_register.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_register.html`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:xi="http://www.w3.org/2001/XInclude" 
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="layout.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Register</title>
     <script type="text/javascript">
       jQuery(document).ready(function($) {
           $('#username').focus();
       });
     </script>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+_dgettext ?>
 ************ RReeggiisstteerr aann aaccccoouunntt ************
 ********** EErrrroorr **********
 $registration_error
 Required
 Username:[${acctmgr.username} ]
 Only lowercase usernames allowed
 Password:[********************]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_reset_password.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_reset_password.html`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="layout.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Reset Password</title>
     <script type="text/javascript">
       jQuery(document).ready(function($) {
           $('#username').focus();
       });
     </script>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
+_dgettext ?>
 ************ RReesseett PPaasssswwoorrdd ************
 If you've forgotten your password, enter your username and email address below,
 and a new password will be sent to you.
 Username:[username            ]
 Email Address:[email               ]
 [${dgettext('acct_mgr', 'Reset password')}]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_user_table.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_user_table.html`

 * *Files 16% similar despite different names*

```diff
@@ -20,47 +20,45 @@
         <th>Account</th>
         <th py:if="'name' in cols">Name</th>
         <th py:if="'email' in cols">Email</th>
         <th>Last Login</th>
       </tr>
     </thead>
     <tbody>
-      <tr py:for="idx, acct in enumerate(accounts)"
-          py:with="
-            title = None
-                    if not acct.approval else
-                    dgettext('acct_mgr', 'Email not verified')
-                    if 'email' in acct.approval else
-                    dgettext('acct_mgr', 'Approval pending')
-                    if acct.approval[0] == 'pending' else
-                    dgettext('acct_mgr', 'Approval revoked')
-                    if acct.approval[0] == 'revoked' else
-                    None;
-          "
-          class="${classes('odd' if idx % 2 else 'even', missing=acct.approval)}"
-          title="${title}">
-        <td class="sel" py:if="delete_enabled">
-          <input type="checkbox" name="sel" value="${acct.username}" />
-        </td>
-        <td>
-          <a href="${acct.url}">${acct.username}</a>
-          <!--! Additional account status icons -->
-          <py:choose py:if="acct.locked">
-            <img src="${href.chrome('/acct_mgr/time-locked.png')}"
-                 py:when="acct.release_hint" alt="Account locked"
-                 title="${acct.release_hint}" />
-            <img src="${href.chrome('/acct_mgr/locked.png')}"
-                 py:otherwise="" alt="Permanently locked"
-                 title="${dgettext('acct_mgr', 'Permanently locked')}" />
-          </py:choose>
-        </td>
-        <td py:if="'name' in cols">${acct.name}</td>
-        <td py:if="'email' in cols">
-          <a href="mailto:$acct.email" title="Send email"
-             py:strip="not acct.email or acct.email.endswith('…')"
-             >${acct.email}</a>
-        </td>
-        <td>${pretty_dateinfo(acct.last_visit) if acct.last_visit else ''}</td>
-      </tr>
+      <py:for each="idx, acct in enumerate(accounts)">
+        <tr class="${('even', 'odd')[idx % 2] + (acct.approval and ' missing' or '')}"
+            title="${acct.approval and
+                     ('email' in acct.approval and
+                      dgettext('acct_mgr', 'Email not verified') or
+                      acct.approval[0] == 'pending' and
+                      dgettext('acct_mgr', 'Approval pending') or
+                      acct.approval[0] == 'revoked' and
+                      dgettext('acct_mgr', 'Approval revoked')
+                      ) or None}">
+          <td class="sel" py:if="delete_enabled">
+            <input type="checkbox" name="sel"
+                   value="${acct.username}" />
+          </td>
+          <td>
+            <a href="${acct.url}">${acct.username}</a>
+            <!--! Additional account status icons -->
+            <py:choose py:if="acct.locked">
+              <img src="${href.chrome('/acct_mgr/time-locked.png')}"
+                   py:when="acct.release_hint" alt="Account locked"
+                   title="${acct.release_hint}" />
+              <img src="${href.chrome('/acct_mgr/locked.png')}"
+                   py:otherwise="" alt="Permanently locked"
+                   title="${dgettext('acct_mgr', 'Permanently locked')}" />
+            </py:choose>
+          </td>
+          <td py:if="'name' in cols">${acct.name}</td>
+          <td py:if="'email' in cols">
+            <a href="mailto:$acct.email" title="Send email"
+               py:strip="not acct.email or acct.email.endswith('…')">
+              ${acct.email}</a>
+          </td>
+          <td>${acct.last_visit and pretty_dateinfo(acct.last_visit) or ''}</td>
+        </tr>
+      </py:for>
     </tbody>
   </table>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 ?  AAccccoouunntt                  NNaammee         EEmmaaiill         LLaasstt LLooggiinn
-  _$_{_a_c_c_t_._u_s_e_r_n_a_m_e_}[Account                            ${pretty_dateinfo
-?? locked][Permanently      ${acct.name} _$_{_a_c_c_t_._e_m_a_i_l_} (acct.last_visit) if
-  locked]                                             acct.last_visit else ''}
+  _$_{_a_c_c_t_._u_s_e_r_n_a_m_e_}[Account                            ${acct.last_visit and
+?? locked][Permanently      ${acct.name} _$_{_a_c_c_t_._e_m_a_i_l_} pretty_dateinfo
+  locked]                                             (acct.last_visit) or ''}
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/templates/genshi/account_users.html` & `TracAccountManager-0.6.dev0/acct_mgr/templates/account_users.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:xi="http://www.w3.org/2001/XInclude"
       xmlns:py="http://genshi.edgewall.org/"
       xmlns:i18n="http://genshi.edgewall.org/i18n"
       i18n:domain="acct_mgr">
   <xi:include href="admin.html" />
+  <?python
+    if _dgettext is not None:
+        dgettext = _dgettext ?>
   <head>
     <title>Accounts</title>
     <script type="text/javascript"
             src="${chrome.htdocs_location}js/folding.js"></script>
     <script type="text/javascript">/*<![CDATA[*/
       jQuery(document).ready(function($) {
         // Compatibility: The prop function doesn't exist before jQuery 1.6
@@ -148,57 +151,61 @@
           <div class="buttons">
             <input type="submit" value="${dgettext('acct_mgr', 'Update')}" />
           </div>
         </form>
       </div>
 
       <!--! TRANSLATOR: Position (# to # of #) or total, if not paginating -->
-      <h2 class="report-result" i18n:msg="count">
+      <h2 class="report-result">
         Accounts <span class="trac-count">($displayed_items)</span>
       </h2>
 
       <form id="filter" method="get" action="">
         <fieldset id="filters">
           <legend class="foldable">Filters</legend>
-          <table summary="Filters">
+          <table summary="Account filters">
             <th scope="row">Status</th>
             <td class="filter">
               <label class="control" py:for="filter in filters">
                 <input type="checkbox" name="${'filter_%s' % filter.name}"
                        checked="${filter.enabled or None}"/> ${filter.label}
               </label>
             </td>
             <td>
               <div class="inlinebuttons">
-                <input type="submit" name="update" value="${dgettext('acct_mgr', 'Update')}" />
+                <input type="submit" name="update"
+                       value="${dgettext('acct_mgr', 'Update')}" />
               </div>
             </td>
           </table>
         </fieldset>
       </form>
 
       <form id="manage-accounts" method="post">
         <xi:include py:with="paginator = accounts" href="page_index.html" />
         <!--! Main account list -->
         <xi:include href="account_user_table.html"/>
         <xi:include py:with="paginator = accounts" href="page_index.html" />
 
         <div class="buttons">
-          <input py:if="password_reset_enabled"
-                 type="submit" id="reset" name="reset"
+          <input type="submit" id="reset" name="reset"
+                 py:if="password_reset_enabled"
                  title="Send another random password"
                  value="${dgettext('acct_mgr', 'Reset passwords')}" />
           <input type="submit" id="approve" name="approve"
                  title="Approve pending registrations, ban/unban accounts"
                  value="${dgettext('acct_mgr', 'Toggle account approval')}" />
-          <input py:if="delete_enabled"
-                 type="submit" id="remove" name="remove"
+          <input type="submit" id="remove" name="remove"
+                 py:if="delete_enabled"
                  title="Delete accounts"
-                 value="${dgettext('acct_mgr', 'Remove selected items')}" />
-          <input py:if="'ACCTMGR_ADMIN' in req.perm"
-                 type="submit" id="cleanup" name="cleanup"
-                 value="${dgettext('acct_mgr', 'Review account attributes')}" />
+                 value="${dgettext('acct_mgr',
+                                   'Remove selected items')}" />
+          <input type="submit" id="cleanup" name="cleanup"
+                 py:if="'ACCTMGR_ADMIN' in req.perm"
+                 value="${dgettext('acct_mgr',
+                                   'Review account attributes')}" />
         </div>
       </form>
     </div>
+
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+_dgettext ?>
 Add New Account:
 Username:
 [${acctmgr.username} ]
 Only lowercase usernames allowed
 Password:
 [********************][********************]
 Confirm Password:
@@ -14,9 +15,11 @@
 [${dgettext('acct_mgr', ' Add ')}]
 This password store does not support listing users.
 Max accounts per page[${accounts.max_per_page}]
 [${dgettext('acct_mgr', 'Update')}]
 ********** AAccccoouunnttss (($$ddiissppllaayyeedd__iitteemmss)) **********
 Filters
 [${dgettext('acct_mgr', 'Reset passwords')}][${dgettext('acct_mgr', 'Toggle
-account approval')}][${dgettext('acct_mgr', 'Remove selected items')}][$
-{dgettext('acct_mgr', 'Review account attributes')}]
+account approval')}][${dgettext('acct_mgr',
+                                   'Remove selected items')}][${dgettext
+('acct_mgr',
+                                   'Review account attributes')}]
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/admin.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 import tempfile
 import unittest
 
 from trac.core import Component, implements
 from trac.perm import PermissionCache, PermissionSystem
 from trac.test import EnvironmentStub, Mock
 
-from ..admin import ExtensionOrder, ConfigurationAdminPanel, UserAdminPanel
-from ..api import AccountManager, IAccountRegistrationInspector
-from ..db import SessionStore
-from ..register import BasicCheck, RegistrationError
+from acct_mgr.admin import ExtensionOrder, ConfigurationAdminPanel, \
+                           UserAdminPanel
+from acct_mgr.api import AccountManager, IAccountRegistrationInspector
+from acct_mgr.db import SessionStore
+from acct_mgr.register import BasicCheck, RegistrationError
 
 
 class BadCheck(Component):
     """Attributes/methods left out intentionally for testing."""
     implements(IAccountRegistrationInspector)
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/api.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import unittest
 
 from trac.core import TracError
 from trac.perm import PermissionCache, PermissionSystem
 from trac.test import EnvironmentStub, MockRequest
 from trac.web.session import Session
 
-from ..api import AccountManager
-from ..db import SessionStore
+from acct_mgr.api import AccountManager
+from acct_mgr.db import SessionStore
 
 
 class _BaseTestCase(unittest.TestCase):
     def setUp(self):
         self.env = EnvironmentStub(default_data=True,
                                    enable=['trac.*', 'acct_mgr.api.*',
                                            'acct_mgr.db.SessionStore',
@@ -159,15 +159,15 @@
         self.actions = ['ACCTMGR_ADMIN', 'ACCTMGR_CONFIG_ADMIN',
                         'ACCTMGR_USER_ADMIN', 'EMAIL_VIEW', 'USER_VIEW']
 
         # Tests
 
     def test_available_actions(self):
         for action in self.actions:
-            self.assertFalse(action not in self.perm.get_actions())
+            self.failIf(action not in self.perm.get_actions())
 
     def test_available_actions_no_perms(self):
         for action in self.actions:
             self.assertFalse(self.perm.check_permission(action, 'anonymous'))
 
     def test_available_actions_config_admin(self):
         user = 'config_admin'
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/db.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Author: Matthew Good <trac@matt-good.net>
 
 import unittest
 
 from trac.test import EnvironmentStub
 
-from ..db import SessionStore
+from acct_mgr.db import SessionStore
 
 
 class _BaseTestCase(unittest.TestCase):
     def setUp(self):
         self.env = EnvironmentStub(enable=['trac.*', 'acct_mgr.*'])
         self.env.config.set('account-manager', 'password_store',
                             'SessionStore')
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/functional/testcases.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/functional/testcases.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,138 +4,39 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Pedro Algarvio <ufs@ufsoft.org>
 
-import email
-import re
-import unittest
-
-from . import FunctionalTestSuite, FunctionalTestCaseSetup, tc
-
-
-def parse_smtp_message(data):
-    assert data is not None
-    if isinstance(data, bytes):
-        data = data.decode('utf-8')
-    message = email.message_from_string(data)
-    headers = dict(message.items())
-    if message.is_multipart():
-        for part in message.walk():
-            if part.get_content_type() == 'text/plain':
-                break
-        else:
-            return headers, u''
-    else:
-        part = message
-    payload = part.get_payload(decode=True)
-    encoding = part.get_content_charset()
-    body = payload.decode(encoding)
-    return headers, body
+import base64
 
+from trac.tests.notification import parse_smtp_message
 
-class TestInitialSetup(FunctionalTestCaseSetup):
-    def runTest(self):
-        """initial Trac authentication setup"""
-        tc.find('Login')
-        tc.follow('Login')
-        tc.find(r'logged in as <span[^>]+>setup</span>')
-        # step 1
-        tc.find(r'>\s*Step 1: Authentication Options\s*</legend>')
-        tc.formvalue('cfg_wiz', 'acctmgr_login', '1')
-        tc.formvalue('cfg_wiz', 'next', '1')
-        tc.submit()
-        # step 2
-        tc.find(r'>\s*Step 2: Password Store\s*</legend>')
-        tc.formvalue('cfg_wiz', 'init_store', 'file')
-        tc.formvalue('cfg_wiz', 'init_store_file', 'htpasswd')
-        tc.formvalue('cfg_wiz', 'next', '1')
-        tc.submit()
-        # step 3
-        tc.find(r'>\s*Step 3: Password Policy\s*</legend>')
-        tc.formvalue('cfg_wiz', 'next', '1')
-        tc.submit()
-        # step 4
-        tc.find(r'>\s*Step 4: Account Policy\s*</legend>')
-        tc.formvalue('cfg_wiz', 'acctmgr_register', 'true')
-        tc.formvalue('cfg_wiz', 'BasicCheck', '1')
-        tc.formvalue('cfg_wiz', 'EmailCheck', '2')
-        tc.formvalue('cfg_wiz', 'RegExpCheck', '3')
-        tc.formvalue('cfg_wiz', 'RegExpCheck.username_regexp',
-                     '^[-A-Za-z0-9._]{3,}$')
-        tc.formvalue('cfg_wiz', 'UsernamePermCheck', '4')
-        tc.formvalue('cfg_wiz', 'next', '1')
-        tc.submit()
-        # step 5
-        tc.find(r'>\s*Step 5: Account Guard\s*</legend>')
-        tc.formvalue('cfg_wiz', 'next', '1')
-        tc.submit()
-        # step 6 - admin
-        tc.find(r'>\s*Step 6: Initialization\s*</legend>')
-        tc.find(r'>\s*Add Admin Account:\s*</legend>')
-        tc.formvalue('cfg_wiz', 'username', 'admin')
-        tc.formvalue('cfg_wiz', 'password', 'admin')
-        tc.formvalue('cfg_wiz', 'password_confirm', 'admin')
-        tc.formvalue('cfg_wiz', 'add', '1')
-        tc.submit()
-        # step 6 - admin created
-        tc.find(r'\bAccount <[a-z]+>admin</[a-z]+> created\.')
-        tc.find(r'>\s*Step 6: Initialization\s*</legend>')
-        #tc.notfind(r'>\s*Add Admin Account:\s*</legend>')
-        tc.formvalue('cfg_wiz', 'save', '1')
-        tc.submit()
-        # wizard finished
-        tc.url(re.escape(self._tester.url))
-        tc.find(r'>WikiStart</a>')
-        tc.find(r'logged in as <span[^>]+>setup</span>')
-        self._tester.logout()
+from acct_mgr.tests.functional import *
 
 
-class TestFormLoginAdmin(FunctionalTestCaseSetup):
+class TestFormLoginAdmin(FunctionalTwillTestCaseSetup):
     def runTest(self):
         """Login with test user 'admin'"""
         self._tester.login('admin')
         self._tester.logout()
 
 
-class TestAdminFormAddUser(FunctionalTestCaseSetup):
-    def runTest(self):
-        self._tester.login('admin')
-        tc.find('Admin')
-        tc.follow('Admin')
-        tc.find('Users')
-        tc.follow('Users')
-        tc.find(r'<legend>\s*Add New Account:\s*</legend>')
-        form = 'account-editor'
-        tc.formvalue(form, 'username', 'user')
-        tc.formvalue(form, 'password', 'user')
-        tc.formvalue(form, 'password_confirm', 'user')
-        tc.formvalue(form, 'email', 'user@trac.example.org')
-        tc.formvalue(form, 'email_approved', [])
-        tc.submit()
-        tc.find(r'\bAccount <[a-z]+>user</[a-z]+> created\.')
-        tc.find('Users')
-        tc.follow('Users')
-        tc.find(r'<a\s*[^>]*>user</a>')
-        self._tester.logout()
-
-
-class TestFormLoginUser(FunctionalTestCaseSetup):
+class TestFormLoginUser(FunctionalTwillTestCaseSetup):
     def runTest(self):
         """Login with test user 'user'"""
         self._tester.login('user')
         self._tester.logout()
 
 
 class TestRegisterNewUser(FunctionalTestCaseSetup):
     def runTest(self):
         """Register 'testuser'"""
-        self._tester.register('testuser', 'testuser@trac.example.org')
+        self._tester.register('testuser')
 
 
 class TestLoginNewUser(FunctionalTestCaseSetup):
     def runTest(self):
         """Login just registered 'testuser'"""
         self._tester.login('testuser')
         self._tester.logout()
@@ -147,29 +48,29 @@
         reg_form_name = 'acctmgr_registerform'
         username = 'testuser1'
         tc.find("Register")
         tc.follow("Register")
         tc.formvalue(reg_form_name, 'user', username)
         tc.formvalue(reg_form_name, 'password', username)
         tc.submit()
-        tc.find(r'The passwords must match\.')
+        tc.find("The passwords must match.")
 
 
 class TestFailRegisterDuplicateUsername(FunctionalTestCaseSetup):
     def runTest(self):
         """Fail if username exists"""
         reg_form_name = 'acctmgr_registerform'
         username = 'testuser'
         tc.find("Register")
         tc.follow("Register")
         tc.formvalue(reg_form_name, 'user', username)
         tc.formvalue(reg_form_name, 'password', username)
         tc.formvalue(reg_form_name, 'password_confirm', username)
         tc.submit()
-        tc.find("Another account or group already exists")
+        tc.find("Another account with that name already exists.")
 
 
 class TestNewAccountNotification(FunctionalTestCaseSetup):
     def runTest(self):
         """Send out notification on new account registrations"""
         tc.notfind('Logout')
         address_to_notify = 'admin@testenv%s.tld' % self._testenv.port
@@ -184,54 +85,56 @@
         env.config.save()
         self._tester.register(new_username, new_username_email)
 
         headers, body = parse_smtp_message(self._smtpd.get_message())
 
         self.assertEqual(self._smtpd.get_recipients(), [address_to_notify])
         self.assertEqual(headers['Subject'],
-                         '[testenv%d] Account created: %s' %
-                         (self._testenv.port, new_username))
+                         '[%s] New user registration: %s' % (
+                                            'testenv%s' % self._testenv.port,
+                                            new_username))
         self.assertEqual(headers['X-URL'], self._testenv.url)
 
 
 class TestNewAccountEmailVerification(FunctionalTestCaseSetup):
     def runTest(self):
         """User is shown info that he needs to verify his address"""
         user_email = "foo@testenv%s.tld" % self._testenv.port
         self._tester.login("foo")
 
-        tc.find(r'An email has been sent to &lt;%s&gt; with a token to '
-                r'<a href="/trac/verify_email">verify your new email address'
-                r'</a>' % re.escape(user_email))
+        tc.find('<strong>Notice:</strong> <span>An email has been sent to '
+                '%s with a token to <a href="/verify_email">verify your new '
+                'email address</a></span>' % user_email)
         self._tester.go_to_front()
-        tc.find(r'<strong>Warning:</strong>\s*'
-                r'Your permissions have been limited until you '
-                r'<a href="/trac/verify_email">verify your email address</a>')
+        tc.find('<strong>Warning:</strong> <span>Your permissions have been '
+                'limited until you <a href="/verify_email">verify your email '
+                'address</a></span>')
 
 
 class VerifyNewAccountEmailAddress(FunctionalTestCaseSetup):
     def runTest(self):
         """User confirms his address with mailed token"""
         headers, body = parse_smtp_message(self._smtpd.get_message())
-        blines = body.splitlines()
+        blines = base64.decodestring(body).splitlines()
         token = [l.split() for l in blines if 'Verification Token' in l][0][-1]
-        warning = (r'<strong>Warning:</strong>\s*'
-                   r'Your permissions have been limited until you <a '
-                   r'href="/trac/verify_email">verify your email address</a>')
 
         tc.find('Logout') # User is logged in from previous test
         self._tester.go_to_front()
-        tc.find(warning)
+        tc.find('<strong>Warning:</strong> <span>Your permissions have been '
+                'limited until you <a href="/verify_email">verify your email '
+                'address</a></span>')
         tc.go(self._testenv.url + '/verify_email')
 
         reg_form_name = 'acctmgr_verify_email'
         tc.formvalue(reg_form_name, 'token', token)
         tc.submit('verify')
 
-        tc.notfind(warning)
+        tc.notfind('<strong>Warning:</strong> <span>Your permissions have been '
+                   'limited until you <a href="/verify_email">verify your email'
+                   ' address</a></span>')
         tc.find('Thank you for verifying your email address')
         self._tester.go_to_front()
 
 
 class PasswdResetsNotifiesAdmin(FunctionalTestCaseSetup):
     def runTest(self):
         """User password resets notifies admin by mail"""
@@ -252,81 +155,85 @@
         tc.formvalue(reset_form_name, 'username', username)
         tc.formvalue(reset_form_name, 'email', email_addr)
         tc.submit()
 
         headers, body = parse_smtp_message(
             self._smtpd.get_message('admin@testenv%s.tld' % self._testenv.port))
         self.assertEqual(headers['Subject'],
-                         '[testenv%s] Account password reset: %s' %
-                         (self._testenv.port, username))
+                         '[%s] Password reset for user: %s' % (
+                                            'testenv%s' % self._testenv.port,
+                                            username))
         self.assertEqual(headers['X-URL'], self._testenv.url)
 
 
 class PasswdResetsNotifiesUser(FunctionalTestCaseSetup):
     def runTest(self):
         """Password reset sends new password to user by mail"""
         username = "foo"
         email_addr = "foo@testenv%s.tld" % self._testenv.port
         headers, self.body = parse_smtp_message(self._smtpd.get_message(email_addr))
         self.assertEqual(headers['Subject'],
-                         '[testenv%d] Account password reset: %s' %
-                         (self._testenv.port, username))
+                         '[%s] Trac password reset for user: %s' % (
+                                            'testenv%s' % self._testenv.port,
+                                            username))
 
 
 class UserLoginWithMailedPassword(PasswdResetsNotifiesUser):
     def runTest(self):
         """User is able to login with the new password"""
         PasswdResetsNotifiesUser.runTest(self)
         # Does it include a new password
-        body = self.body
+        body = base64.decodestring(self.body)
         username = 'foo'
         self.assertTrue('Username: %s' % username in body)
         self.assertTrue('Password:' in body)
 
         passwd = [l.split(':')[1].strip() for l in
                   body.splitlines() if 'Password:' in l][0]
 
         self._tester.login(username, passwd)
 
 
 class UserIsForcedToChangePassword(FunctionalTestCaseSetup):
     def runTest(self):
         """User is forced to change password after resets"""
         tc.find('Logout')
-        tc.find(r'You are required to change password because of a recent '
-                r'password change request\.')
+        tc.find("You are required to change password because of a recent "
+                "password change request.")
 
 
 class UserCantBrowseUntilPasswdChange(PasswdResetsNotifiesUser):
     def runTest(self):
         """User can't navigate out of '/prefs/account' before password change"""
         PasswdResetsNotifiesUser.runTest(self)
         tc.find('Logout')
         forced_passwd_change_url = '^%s/prefs/account$' % self._tester.url
         tc.follow('Roadmap')
         tc.url(forced_passwd_change_url)
         tc.follow('View Tickets')
         tc.url(forced_passwd_change_url)
         tc.follow('New Ticket')
         tc.url(forced_passwd_change_url)
+        tc.follow('Browse Source')
+        tc.url(forced_passwd_change_url)
 
         # Now, let's change his password
-        body = self.body
+        body = base64.decodestring(self.body)
         passwd = [l.split(':')[1].strip() for l in
                   body.splitlines() if 'Password:' in l][0]
         username = 'foo'
         change_passwd_form = 'userprefs'
         tc.formvalue(change_passwd_form, 'old_password', passwd)
         tc.formvalue(change_passwd_form, 'password', username)
         tc.formvalue(change_passwd_form, 'password_confirm', username)
         tc.submit()
 
         tc.notfind("You are required to change password because of a recent "
-                   "password change request")
-        tc.find(r'Thank you for taking the time to update your password\.')
+                   "password change request.")
+        tc.find("Thank you for taking the time to update your password.")
 
         # We can now browse away from /prefs/accounts
         tc.follow('Roadmap')
         tc.url(self._tester.url + '/roadmap')
         # Clear the mailstore
         self._smtpd.full_reset()
 
@@ -341,16 +248,16 @@
 
         delete_account_form_name = 'acctmgr_delete_account'
         tc.formvalue(delete_account_form_name, 'password', 'foo')
         tc.submit()
         tc.find("Login") # We're logged out when we delete our account
         headers, _ = parse_smtp_message(self._smtpd.get_message())
         self.assertEqual(headers['Subject'],
-                         '[testenv%d] Account deleted: %s' %
-                         (self._testenv.port, 'foo'))
+                         '[%s] Deleted User: %s' % (
+                                'testenv%s' % self._testenv.port, 'foo'))
 
 
 class UserNoLongerLogins(FunctionalTestCaseSetup):
     def runTest(self):
         """Deleted user can't login"""
         tc.follow('Login')
         login_form_name = 'acctmgr_loginform'
@@ -360,44 +267,41 @@
         tc.find("Invalid username or password")
         tc.notfind('Logout')
 
 
 class UserIsAbleToRegisterWithSameUserName(FunctionalTestCaseSetup):
     def runTest(self):
         """Register with deleted username (session and session_attributes clean)"""
-        self._tester.register('foo', 'foo@trac.example.org')
+        self._tester.register('foo')
         self._tester.login('foo')
         self._tester.logout()
         self._smtpd.full_reset()
 
 
 class NoEmailVerificationForAnonymousUsers(FunctionalTestCaseSetup):
     def runTest(self):
         """Anonymous users don't get their email address verified"""
         tc.find("Login")
         tc.follow("Preferences")
         form_name = 'userprefs'
         email_address = 'anonyous.user@fakedomain.tld'
         tc.formvalue(form_name, 'email', email_address)
         tc.submit()
-        tc.notfind(r'<strong>Notice:</strong>\s*<span>An email has been sent '
-                   r'to {0} with a token to <a href="/verify_email">verify '
-                   r'your new email address</a></span>'
-                   .format(re.escape(email_address)))
+        tc.notfind('<strong>Notice:</strong> <span>An email has been sent to '
+                   '%s with a token to <a href="/verify_email">verify your new '
+                   'email address</a></span>' % email_address)
         self._tester.go_to_front()
-        tc.notfind(r'<strong>Warning:</strong>\s*<span>Your permissions have '
-                   r'been limited until you <a href="/verify_email">verify '
-                   r'your email address</a></span>')
+        tc.notfind('<strong>Warning:</strong> <span>Your permissions have been '
+                   'limited until you <a href="/verify_email">verify your email '
+                   'address</a></span>')
 
 
 def test_suite():
     suite = FunctionalTestSuite()
-    suite.addTest(TestInitialSetup())
     suite.addTest(TestFormLoginAdmin())
-    suite.addTest(TestAdminFormAddUser())
     suite.addTest(TestFormLoginUser())
     suite.addTest(TestRegisterNewUser())
     suite.addTest(TestLoginNewUser())
     suite.addTest(TestFailRegisterPasswdConfirmNotPassed())
     suite.addTest(TestFailRegisterDuplicateUsername())
     suite.addTest(TestNewAccountNotification())
     suite.addTest(TestNewAccountEmailVerification())
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/functional/tester.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/functional/tester.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,74 +4,47 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Pedro Algarvio <ufs@ufsoft.org>
 
-import re
+from acct_mgr.tests.functional import *
 
-from . import tc
+class AcctMgrFunctionalTester(FunctionalTester):
 
-
-internal_error = 'Trac detected an internal error:'
-
-
-class FunctionalTester(object):
-
-    url = None
-
-    def __init__(self, url):
-        self.url = url
-        self.go_to_front()
-
-    def go_to_url(self, url):
-        tc.go(url)
-        tc.url(re.escape(url))
-        tc.notfind(internal_error)
-
-    def go_to_front(self):
-        """Go to the Trac front page"""
-        self.go_to_url(self.url)
+    def __init__(self, url, repo_url):
+        super(AcctMgrFunctionalTester, self).__init__(url)
+        # Don't stay logged in as admin.
+        self.logout()
 
     def login(self, username, passwd=None):
         """Override FunctionalTester.login, we're not using Basic
         Authentication."""
         if not passwd:
             passwd = username
         login_form_name = 'acctmgr_loginform'
         self.go_to_front()
         tc.find('Login')
         tc.follow('Login')
         tc.formvalue(login_form_name, 'user', username)
         tc.formvalue(login_form_name, 'password', passwd)
         tc.submit()
-        tc.find("logged in as <span[^>]+>%s</span>" % username)
+        tc.find("logged in as %s" % username)
         tc.find("Logout")
         tc.url(self.url)
         tc.notfind(internal_error)
 
-    def logout(self):
-        tc.formvalue('logout', 'logout', 'Logout')
-        tc.submit()
-        tc.notfind(internal_error)
-        tc.notfind('logged in as')
-
     def register(self, username, email='', passwd=None):
         """Allow user registration."""
         if not passwd:
             passwd = username
         reg_form_name = 'acctmgr_registerform'
         tc.find("Register")
         tc.follow("Register")
         tc.formvalue(reg_form_name, 'user', username)
         tc.formvalue(reg_form_name, 'password', passwd)
         tc.formvalue(reg_form_name, 'password_confirm', passwd)
         tc.formvalue(reg_form_name, 'email', email)
         tc.submit()
         tc.notfind("The passwords must match.")
         tc.notfind(internal_error)
-        tc.find(r'Your username has been successfully registered but your '
-                r'account still requires activation\. Please login as user '
-                r'<strong>{0}</strong>, and follow the instructions\.'
-                .format(re.escape(username)))
-        tc.url('/login$')
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/guard.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/guard.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import unittest
 from time import sleep
 
 from trac.test import EnvironmentStub, MockRequest
 from trac.util.datefmt import to_datetime, to_timestamp
 from trac.web.session import Session
 
-from ..guard import AccountGuard
+from acct_mgr.guard import AccountGuard
 
 
 class AccountGuardTestCase(unittest.TestCase):
     def setUp(self):
         self.env = EnvironmentStub(default_data=True,
                                    enable=['trac.*', 'acct_mgr.guard.*'])
         self.env.path = tempfile.mkdtemp()
@@ -77,15 +77,15 @@
         # Regular account without failed attempts logged.
         user = self.user
         # Start without failed attempts logged, accumulating failed attempts.
         self.assertEqual(self.guard.failed_count(user, ipnr), 1)
         self.assertEqual(self.guard.failed_count(user, ipnr), 2)
         # Read failed attempts.
         self.assertEqual(self.guard.failed_count(user, ipnr, None), 2)
-        # Reset failed attempts, returning deleted attempts.
+        # Reset failed attempts, returning deleted attemps.
         self.assertEqual(self.guard.failed_count(user, reset=True), 2)
         self.assertEqual(self.guard.failed_count(user, reset=None), 0)
 
     def test_functional(self):
         ipnr = '127.0.0.1'
         user = self.user
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/htfile.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/htfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-import io
 import os.path
 import shutil
 import tempfile
 import unittest
 
 from trac.test import EnvironmentStub
 
-from ..htfile import HtDigestStore, HtPasswdStore
+from acct_mgr.htfile import HtDigestStore, HtPasswdStore
 
 
 class _BaseTestCase(unittest.TestCase):
     def setUp(self):
         self.basedir = os.path.realpath(tempfile.mkdtemp())
         self.env = EnvironmentStub()
         self.env.path = os.path.join(self.basedir, 'trac-tempenv')
@@ -33,20 +32,19 @@
     # Helpers
 
     def _create_file(self, *path, **kw):
         filename = os.path.join(self.basedir, *path)
         dirname = os.path.dirname(filename)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
+        fd = file(filename, 'w')
         content = kw.get('content')
-        with io.open(filename, 'w', encoding='utf-8') as fd:
-            if content is not None:
-                if isinstance(content, bytes):
-                    content = content.decode('utf-8')
-                fd.write(content)
+        if content is not None:
+            fd.write(content)
+        fd.close()
         return filename
 
     def _init_password_file(self, flavor, filename, content=''):
         filename = self._create_file(filename, content=content)
         self.env.config.set('account-manager', flavor + '_file', filename)
 
     def _do_password_test(self, flavor, filename, content):
@@ -131,54 +129,24 @@
             self._do_password_test(self.flavor, 'test_sha256',
                                    'user:$5$rounds=535000$saltsaltsaltsalt$'
                                    'wfx3LZ09XA7qrZB.ttuCbBidMXt51Kgu5YQ.YFq'
                                    'zxA7\n')
         except NotImplementedError:
             pass
 
-        try:
-            self._do_password_test(self.flavor, 'test_sha256',
-                                   'user:$5$.YGr6HhGl0TNN7dT$Jrq.j68U8/rrBo5Ks'
-                                   'YycA05JS3ZXzGn5C1u54Fh8l7.\n')
-        except NotImplementedError:
-            pass
-
-        try:
-            self._do_password_test(self.flavor, 'test_sha256',
-                                   'user:$5$/sSmB.1hM8M7YlWP$qQwILOVGJ7Z/JNIml'
-                                   'ZmweMBy7VKO9pwmmAwBf0YrOB6\n')
-        except NotImplementedError:
-            pass
-
     def test_sha512(self):
         try:
             self._do_password_test(self.flavor, 'test_sha512',
                                    'user:$6$rounds=535000$saltsaltsaltsalt$'
                                    '9ExQK2S3YXW7/FlfUcw2vy7WF.NH5ZF6SIT14Dj'
                                    'ngOGkcx.5mINko67cLRrqFFh1AltOT4uPnET7Bs'
                                    'JXuI56H/\n')
         except NotImplementedError:
             pass
 
-        try:
-            self._do_password_test(self.flavor, 'test_sha512',
-                                   'user:$6$.Gz0dqxtsVYNeES3$H9cLym9oGJqILw1fj'
-                                   'XHm2Ha54ZJhQ/h8XMaxWpKnPziXqI0nu45a1Rsbrde'
-                                   '42gNbh.78EiFB0A0Qlpdps7JTg1\n')
-        except NotImplementedError:
-            pass
-
-        try:
-            self._do_password_test(self.flavor, 'test_sha512',
-                                   'user:$6$/X87Imrz04AZGkLr$fxSvADugt7V3ufvvg'
-                                   'NGG0BStDjEAwLYRUGjWxlJX0zcD64RxBOAldIDdqNZ'
-                                   'bDHoDv.GjVOVfQxjMZwWVBFxgz0\n')
-        except NotImplementedError:
-            pass
-
     def test_no_trailing_newline(self):
         self._do_password_test(self.flavor, 'test_no_trailing_newline',
                                'user:$apr1$xW/09...$fb150dT95SoL1HwXtHS/I0')
 
     def test_add_with_no_trailing_newline(self):
         filename = self._create_file(
             'test_add_with_no_trailing_newline',
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/model.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Steffen Hoffmann <hoff.st@web.de>
 
+import new
+import pkg_resources
 import shutil
 import tempfile
 import time
 import unittest
 
+from trac import __version__ as VERSION
 from trac.test import EnvironmentStub, MockRequest
 from trac.web.session import Session
 
-from ..model import (
+from acct_mgr.model import (
     change_uid, del_user_attribute, delete_user, get_user_attribute,
     last_seen, prime_auth_session, set_user_attribute, user_known)
 
 
 class ModelTestCase(unittest.TestCase):
     def setUp(self):
         self.env = EnvironmentStub(default_data=True, enable=['trac.*'])
@@ -79,15 +82,16 @@
                       ('user', 0, 'attribute2', 'value2'),
                       ('user', 1, 'attribute1', 'value1'),
                       ('user', 1, 'attribute2', 'value2'),
                       ('another', 1, 'attribute2', 'value3')])
 
         no_constraints = get_user_attribute(self.env, authenticated=None)
         # Distinct session IDs form top-level keys.
-        self.assertEqual(set(no_constraints), set([u'user', u'another']))
+        self.assertEqual(set(no_constraints.keys()),
+                         set([u'user', u'another']))
         # There are probably anonymous sessions named equally to
         # authenticated ones, causing different nested dicts below each
         # session ID.  Btw, only authenticated ones are real usernames.
         self.assertTrue(0 in no_constraints['user'])
         self.assertTrue(1 in no_constraints['user'])
         self.assertFalse(0 in no_constraints['another'])
         self.assertTrue(1 in no_constraints['another'])
@@ -124,14 +128,19 @@
                 self.assertEqual(('attribute1', '0'), (name, value))
 
 
 class KnownUsersCacheUpdateTestCase(unittest.TestCase):
 
     def setUp(self):
         self.env = EnvironmentStub(default_data=True)
+        if pkg_resources.parse_version(VERSION) < \
+                pkg_resources.parse_version('1.2'):
+            from trac.env import Environment
+            self.env.get_known_users = \
+                new.instancemethod(Environment.get_known_users, self.env, None)
 
     def tearDown(self):
         self.env.shutdown()
         self.env.reset_db()
 
     def _insert_user(self):
         sid = 'user1'
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/register.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
 from trac.perm import PermissionCache, PermissionSystem
 from trac.util.html import Markup
 from trac.test import EnvironmentStub, MockRequest
 from trac.web.api import RequestDone
 from trac.web.session import Session
 
-from ..api import AccountManager
-from ..compat import unicode
-from ..db import SessionStore
-from ..model import set_user_attribute
-from ..register import (
-    BasicCheck, BotTrapCheck, EmailCheck, EmailVerificationModule, RegExpCheck,
-    RegistrationError, RegistrationModule, UsernamePermCheck)
+from acct_mgr.api import AccountManager
+from acct_mgr.db import SessionStore
+from acct_mgr.model import set_user_attribute
+from acct_mgr.register import BasicCheck, BotTrapCheck, EmailCheck
+from acct_mgr.register import EmailVerificationModule
+from acct_mgr.register import RegExpCheck
+from acct_mgr.register import RegistrationError, RegistrationModule
+from acct_mgr.register import UsernamePermCheck
 
 
 class _BaseTestCase(unittest.TestCase):
     def setUp(self, method='GET'):
         self.env = EnvironmentStub(
             enable=['trac.*', 'acct_mgr.api.*'])
         self.env.path = tempfile.mkdtemp()
@@ -109,15 +110,15 @@
         field_res = check.render_registration_fields(req, data)
         self.assertEqual(len(field_res), 2)
         self.assertTrue(Markup(field_res[0]).startswith('<label>Parole:'))
 
         # 1st attempt: Wrong input.
         self.assertRaises(RegistrationError, check.validate_registration, req)
         # Ensure, that old input is restored on failure.
-        self.assertIn(wrong_input, Markup(field_res[0]))
+        self.assertTrue(wrong_input in Markup(field_res[0]))
         # Ensure, that template data dict is passed unchanged.
         self.assertEqual(field_res[1], data)
 
         # 2nd attempt: No input.
         req.args['basic_token'] = ''
         self.assertRaises(RegistrationError, check.validate_registration, req)
         # 3rd attempt: As before, but request done by authenticated user.
@@ -167,15 +168,15 @@
         old_email_input = 'email@foo.bar'
         acct = dict(username='user', email=old_email_input, name='User')
         req.args.update(acct)
         field_res = check.render_registration_fields(req, acct)
         self.assertEqual(len(field_res), 2)
         self.assertTrue(Markup(field_res[0]).startswith('<label>Email:'))
         # Ensure, that old input is restored on failure.
-        self.assertIn(old_email_input, Markup(field_res[0]))
+        self.assertTrue(old_email_input in Markup(field_res[0]))
         # Ensure, that template data dict is passed unchanged.
         self.assertEqual(field_res[1], acct)
         req.args.update(dict(email=''))
 
         # 1st: Initially try with account verification disabled by setting.
         self.env.config.set('account-manager', 'verify_email', False)
         self.assertEqual(check.validate_registration(req), None)
@@ -299,15 +300,15 @@
             'username': user,
             'name': 'Tester',
             'password': passwd,
             'password_confirm': passwd
         })
         # Fail to register the user.
         self.rmod.process_request(req)
-        self.assertIn('email address', unicode(req.chrome['warnings']))
+        self.assertTrue('email address' in str(req.chrome['warnings']))
         self.assertEqual(list(self.store.get_users()), [])
 
     def test_optional_email_registration(self):
         user = 'user1'
         passwd = 'test'
 
         req = MockRequest(self.env, path_info='/register', method='POST',
@@ -349,28 +350,28 @@
     def test_check_email_used(self):
         set_user_attribute(self.env, 'admin', 'email', 'admin@foo.bar')
         # Try email, that is already associated to another user.
         self.req.args['email'] = 'admin@foo.bar'
         self.assertRaises(RequestDone, self.vmod.pre_process_request,
                           self.req, None)
         warnings = self.req.chrome.get('warnings')
-        self.assertIn('already in use',
-                      unicode(warnings and warnings[0] or ''))
+        self.assertTrue(string.find(str(warnings and warnings[0] or ''),
+                                    'already in use') > 0)
 
     def test_check_no_email(self):
         self.assertRaises(RequestDone, self.vmod.pre_process_request,
                           self.req, None)
         warnings = self.req.chrome.get('warnings')
-        self.assertNotEqual(unicode(warnings and warnings[0] or ''), '')
+        self.assertNotEqual(str(warnings and warnings[0] or ''), '')
 
     def test_check(self):
         self.req.args['email'] = 'user@foo.bar'
         self.vmod.pre_process_request(self.req, None)
         warnings = self.req.chrome.get('warnings')
-        self.assertEqual(unicode(warnings and warnings[0] or ''), '')
+        self.assertEqual(str(warnings and warnings[0] or ''), '')
 
 
 def test_suite():
     suite = unittest.TestSuite()
     suite.addTest(unittest.makeSuite(BasicCheckTestCase))
     suite.addTest(unittest.makeSuite(BotTrapCheckTestCase))
     suite.addTest(unittest.makeSuite(EmailCheckTestCase))
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/tests/svnserve.py` & `TracAccountManager-0.6.dev0/acct_mgr/tests/svnserve.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 
 import os.path
 import shutil
 import tempfile
 import unittest
 
-from trac.test import EnvironmentStub
+from acct_mgr.svnserve import SvnServePasswordStore
 
-from ..svnserve import SvnServePasswordStore
+from trac.test import EnvironmentStub
 
 
 class SvnServePasswordTestCase(unittest.TestCase):
     """Test cases for SvnServePasswordStore.
     """
 
     def setUp(self):
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/util.py` & `TracAccountManager-0.6.dev0/acct_mgr/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,42 +6,69 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Matthew Good <trac@matt-good.net>
 
-from datetime import datetime
 import os
 import re
+import sys
+import urllib2
 
-try:
-    from babel.support import LazyProxy
-except ImportError:
-    LazyProxy = None
-
+from acct_mgr.api import _, ngettext
 from trac.config import Option
-from trac.util.datefmt import utc
-from trac.util.html import tag
-from trac.util.translation import dngettext
-
-from .api import _
-from .compat import basestring
+from trac.util.datefmt import format_datetime, to_datetime, utc
 
 
 class EnvRelativePathOption(Option):
     def __get__(self, instance, owner):
         if instance is None:
             return self
         path = super(EnvRelativePathOption, self).__get__(instance, owner)
         if not path:
             return path
         return os.path.normpath(os.path.join(instance.env.path, path))
 
 
+# Fix for issue http://bugs.python.org/issue8797 in Python 2.6
+# following Bitten changeset 974.
+if sys.version_info[:2] == (2, 6):
+    import base64
+
+
+    class HTTPBasicAuthHandler(urllib2.HTTPBasicAuthHandler):
+        """Patched version of Python 2.6's HTTPBasicAuthHandler.
+
+        The fix for [1]_ introduced an infinite recursion bug [2]_ into
+        Python 2.6.x that is triggered by attempting to connect using
+        Basic authentication with a bad username and/or password. This
+        class fixes the problem using the simple solution outlined in [3]_.
+
+        .. [1] http://bugs.python.org/issue3819
+        .. [2] http://bugs.python.org/issue8797
+        .. [3] http://bugs.python.org/issue8797#msg126657
+        """
+
+        def retry_http_basic_auth(self, host, req, realm):
+            user, pw = self.passwd.find_user_password(realm, host)
+            if pw is not None:
+                raw = "%s:%s" % (user, pw)
+                auth = 'Basic %s' % base64.b64encode(raw).strip()
+                if req.get_header(self.auth_header, None) == auth:
+                    return None
+                req.add_unredirected_header(self.auth_header, auth)
+                return self.parent.open(req, timeout=req.timeout)
+            else:
+                return None
+
+else:
+    HTTPBasicAuthHandler = urllib2.HTTPBasicAuthHandler
+
+
 # taken from a comment of Horst Hansen
 # at http://code.activestate.com/recipes/65441
 def contains_any(str, set):
     for c in set:
         if c in str:
             return True
     return False
@@ -52,33 +79,56 @@
         if not self.enabled:
             return None
         return func(self, *args, **kwds)
 
     return wrap
 
 
-def format_timespan(seconds):
-    if not seconds or seconds <= 0:
-        return ''
-
-    _dngettext = dngettext
-    total = seconds
-    days, seconds = divmod(total, 86400)
-    if days != 0:
-        datepart = _dngettext('messages', '%(num)d day', '%(num)d days', days)
-    if seconds == 0:
-        return datepart
-    if seconds < 120:
-        timepart = _dngettext('messages', '%(num)i second', '%(num)i seconds',
-                              seconds)
+def pretty_precise_timedelta(time1, time2=None, resolution=None, diff=0):
+    """Calculate time delta between two `datetime` objects and format
+    for pretty-printing.
+
+    If either `time1` or `time2` is None, the current time will be used
+    instead.  Extending the signature of trac.util.datefmt.pretty_timedelta
+    pre-calculated timedeltas may be specified by the alternative `diff`
+    keyword argument that takes precedence if used.
+    """
+    if diff:
+        age_s = diff
     else:
-        timepart = datetime.fromtimestamp(seconds, utc).strftime('%H:%M:%S')
-    if days == 0:
-        return timepart
-    return _("%(datepart)s %(timepart)s", datepart=datepart, timepart=timepart)
+        time1 = to_datetime(time1)
+        time2 = to_datetime(time2)
+        if time1 > time2:
+            time2, time1 = time1, time2
+        diff = time2 - time1
+        age_s = int(diff.days * 86400 + diff.seconds)
+    age_d = age_s // 86400
+
+    # DEVEL: Always reduce resolution as required by `resolution` argument.
+    if resolution:
+        if age_s < resolution:
+            return _("less than %s"
+                     % pretty_precise_timedelta(None, diff=resolution))
+    # Get a compact string by stripping non-significant parts.
+    if age_s == 0:
+        return ''
+    # Show seconds for small time values, even in timedeltas > 1 day.
+    t = age_s - age_d * 86400
+    if 0 < t < 120:
+        t = ngettext('%(num)i second', '%(num)i seconds', t)
+        if age_d == 0:
+            return t
+    elif age_d != age_s / 86400.0:
+        t = format_datetime(age_s - age_d * 86400, format='%X', tzinfo=utc)
+        if age_d == 0:
+            return t
+    # TRANSLATOR: Pretty datetime representation, time part provided by
+    # string substitution.
+    return (ngettext("%(num)i day %%s", "%(num)i days %%s", age_d)
+            % (str(t) != '0' and t or '')).rstrip()
 
 
 def _create_zwsp_re():
     ucs2_range = u'\\s\u200b-\u200f\u061c\u202a-\u202e\u2066-\u2069\u00ad' \
                  u'\u2060\ufeff\u2061-\u2064\u115f\u1160\u180b-\u180d' \
                  u'\ufe00-\ufe0f'
     try:
@@ -94,74 +144,7 @@
 _zwsp_re = _create_zwsp_re()
 
 
 def remove_zwsp(text):
     """Strips unicode zero-width and whitespace characters.
     """
     return _zwsp_re.sub('', text)
-
-
-_i18n_tag_re = re.compile(r'(?:\[([1-9][0-9]*)\:)|(?<!\\)\]')
-
-
-def i18n_tag(string, *args, **kwargs):
-    START = 'start'
-    END = 'end'
-    TEXT = 'text'
-
-    def parse(string):
-        stack = [0]
-        while True:
-            mo = _i18n_tag_re.search(string)
-            if not mo:
-                break
-
-            if mo.start() or stack[-1]:
-                yield TEXT, stack[-1], string[:mo.start()]
-            string = string[mo.end():]
-
-            orderno = mo.group(1)
-            if orderno is not None:
-                orderno = int(orderno)
-                stack.append(orderno)
-                yield START, orderno, None
-            else:
-                yield END, stack.pop(), None
-            if not stack:
-                break
-
-        if string:
-            yield TEXT, stack[-1], string
-
-    def to_element(arg):
-        if isinstance(arg, (tuple, list)):
-            arg = tag.__getattr__(arg[0])(**arg[1])
-        elif isinstance(arg, basestring):
-            arg = tag.__getattr__(arg)
-        return arg
-
-    def generate(string, args, kwargs):
-        fragment = tag()
-        args = (fragment,) + tuple(to_element(arg) for arg in args)
-        stack = [fragment]
-        for kind, n, data in parse(string):
-            if kind is TEXT:
-                if data:
-                    stack[-1].append(data % kwargs if kwargs else data)
-                continue
-            if kind is START:
-                if 0 <= n < len(args):
-                    arg = args[n]
-                else:
-                    raise IndexError('index %d out of range (%d given for %r)'
-                                     % (n, len(args), string))
-                stack[-1].append(arg)
-                stack.append(arg)
-                continue
-            if kind is END:
-                stack.pop()
-                continue
-        return fragment
-
-    if LazyProxy and isinstance(string, LazyProxy):
-        string = string.value
-    return generate(string, args, kwargs)
```

### Comparing `tracaccountmanager-0.6.0/acct_mgr/web_ui.py` & `TracAccountManager-0.6.dev0/acct_mgr/web_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,47 +12,48 @@
 import random
 import string
 import time
 
 from trac.attachment import IAttachmentManipulator
 from trac.config import BoolOption, ConfigurationError
 from trac.config import IntOption, Option
-from trac.core import Component, implements
+from trac.core import implements
 from trac.env import open_environment
 from trac.prefs import IPreferencePanelProvider
 from trac.ticket.api import ITicketManipulator
 from trac.util import hex_entropy
 from trac.util.html import html as tag
 from trac.util.presentation import separated
 from trac.util.text import exception_to_unicode
 from trac.web import auth
 from trac.web.chrome import INavigationContributor, add_notice
 from trac.web.chrome import add_warning
 from trac.web.main import IRequestHandler, IRequestFilter, get_environments
 from trac.wiki.api import IWikiPageManipulator
 
-from .api import AccountManager, _, ngettext, tag_
-from .compat import iteritems, process_request_compat
-from .db import SessionStore
-from .guard import AccountGuard
-from .model import last_seen, set_user_attribute
-from .notification import NotificationError
-from .register import RegistrationModule
-from .util import i18n_tag, if_enabled, remove_zwsp
+from acct_mgr.api import AccountManager, CommonTemplateProvider
+from acct_mgr.api import _, dgettext, ngettext, tag_
+from acct_mgr.compat import genshi_template_args
+from acct_mgr.db import SessionStore
+from acct_mgr.guard import AccountGuard
+from acct_mgr.model import last_seen, set_user_attribute
+from acct_mgr.notification import NotificationError
+from acct_mgr.register import RegistrationModule
+from acct_mgr.util import if_enabled, remove_zwsp
 
 
 class ResetPwStore(SessionStore):
     """User password store for the 'lost password' procedure."""
 
     def __init__(self):
         super(ResetPwStore, self).__init__()
         self.key = 'password_reset'
 
 
-class AccountModule(Component):
+class AccountModule(CommonTemplateProvider):
     """Exposes methods for users to do account management on their own.
 
     Allows users to change their password, reset their password, if they've
     forgotten it, even delete their account.  The settings for the
     AccountManager module must be set in trac.ini in order to use this.
     Password reset procedure depends on both, ResetPwStore and an
     IPasswordHashMethod implementation being enabled as well.
@@ -128,25 +129,25 @@
             return
         if req.authname and req.authname != 'anonymous':
             user_store = self.acctmgr.find_user_store(req.authname)
             if user_store in writable_stores:
                 yield 'account', _("Account")
 
     def render_preference_panel(self, req, panel):
-        data = dict(i18n_tag=i18n_tag)
+        data = dict(_dgettext=dgettext)
         data.update(self._do_account(req))
-        return 'account_prefs.html', data
+        return genshi_template_args(self.env, 'account_prefs.html', data)
 
     # IRequestFilter methods
 
     def pre_process_request(self, req, handler):
         if not req.authname or req.authname == 'anonymous':
             if req.path_info == '/prefs/account':
                 # An anonymous session has no account associated with it, and
-                # no account properties either, but general session preferences
+                # no account properies too, but general session preferences
                 # should always be available.
                 req.redirect(req.href.prefs())
             elif req.path_info == '/prefs/advanced' and req.method == 'POST':
                 # Prevent setting session ID to one of an authenticated user.
                 username = req.args.get('loadsid')
                 if username and last_seen(self.env, username):
                     add_warning(req, tag_(
@@ -176,27 +177,26 @@
 
     # IRequestHandler methods
 
     def match_request(self, req):
         return req.path_info == '/reset_password' and \
                self._reset_password_enabled(log=True)
 
-    @process_request_compat
     def process_request(self, req):
-        data = dict(i18n_tag=i18n_tag)
+        data = dict(_dgettext=dgettext)
         if req.authname and req.authname != 'anonymous':
-            message = i18n_tag(_("You're already logged in. If you need to "
-                                 "change your password please use the "
-                                 "[1:Account Preferences] page."),
-                               tag.a(href=req.href('prefs/account')))
-            add_notice(req, message)
+            add_notice(req, tag_(
+                "You're already logged in. If you need to change your "
+                "password please use the %(prefs_href)s page.",
+                prefs_href=tag.a(_("Account Preferences"),
+                                 href=req.href.prefs('account'))))
             data['authenticated'] = True
         if req.method == 'POST':
             self._do_reset_password(req)
-        return 'account_reset_password.html', data
+        return 'account_reset_password.html', data, None
 
     # IAttachmentManipulator
 
     def prepare_attachment(self, req, attachment, fields):
         pass
 
     def validate_attachment(self, req, attachment):
@@ -221,15 +221,15 @@
     def _check_author(self, req):
         author = req.args.get('field_reporter') or req.args.get('author')
         if (not req.authname or req.authname == 'anonymous') and author:
             author = remove_zwsp(author)
             if author and last_seen(self.env, author):
                 # Prevent impersonating an authenticated user in author field.
                 # Use degraded formatting due to T:#6634.
-                return [("author", tag_(
+                return [(_("author"), tag_(
                          "Policy prohibits choosing %(username)s for an "
                          "anonymous session because it's a registered "
                          "username. Please login or choose another author "
                          "name.", username=tag.em(author)))]
             return []  # author is not authenticated, but still fine
         return []  # author is authenticated
 
@@ -251,18 +251,18 @@
                     req.session.save()
                     add_notice(req, _("Thank you for taking the time to "
                                       "update your password."))
                     force_change_password = False
             elif action == 'delete' and delete_enabled:
                 self._do_delete(req)
         if force_change_password:
-            add_warning(req, i18n_tag(_("You are required to change password "
-                                        "because of a recent password change "
-                                        "request. [1:Please change your "
-                                        "password now.]"), 'b'))
+            add_warning(req, tag_(
+                "You are required to change password because of a recent "
+                "password change request. %(invitation)s",
+                invitation=tag.b(_("Please change your password now."))))
         return data
 
     def _do_change_password(self, req):
         username = req.authname
 
         old_password = req.args.get('old_password')
         if not self.acctmgr.check_password(username, old_password):
@@ -277,16 +277,16 @@
         elif password != req.args.get('password_confirm'):
             add_warning(req, _("The passwords must match."))
         elif password == old_password:
             add_warning(req, _("Password must not match old password."))
         else:
             _set_password(self.env, req, username, password, old_password)
             if req.session.get('password') is not None:
-                # Fetch all 'session_attribute's in case new user password is
-                # in SessionStore, preventing overwrite by session.save().
+                # Fetch all session_attributes in case new user password is in
+                # SessionStore, preventing overwrite by session.save().
                 req.session.get_session(req.authname, authenticated=True)
             add_notice(req, _("Password updated successfully."))
             return True
 
     def _do_delete(self, req):
         username = req.authname
 
@@ -294,16 +294,16 @@
         if not password:
             add_warning(req, _("Password cannot be empty."))
         elif not self.acctmgr.check_password(username, password):
             add_warning(req, _("Password is incorrect."))
         else:
             try:
                 self.acctmgr.delete_user(username)
-            except NotificationError as e:
-                # User won't care for notification, but only for logging here.
+            except NotificationError, e:
+                # User wont care for notification, only care for logging here.
                 self.log.error(
                     "Unable to send account deletion notification: "
                     "%s", exception_to_unicode(e, traceback=True))
             # Delete the whole session, since records in session_attribute
             # would get restored on logout otherwise.
             req.session.clear()
             req.session.save()
@@ -328,34 +328,34 @@
     @property
     def _random_password(self):
         """Create a new random password on admin or user request.
 
         This method is used by acct_mgr.admin.AccountManagerAdminPanel too.
         """
         return ''.join([random.choice(self._password_chars)
-                        for _ in range(self.password_length)])
+                        for _ in xrange(self.password_length)])
 
     def _reset_password(self, req, username, email):
         """Store a new, temporary password on admin or user request.
 
         This method is used by acct_mgr.admin.AccountManagerAdminPanel too.
         """
         acctmgr = self.acctmgr
         new_password = self._random_password
         try:
             self.store.set_password(username, new_password)
-        except Exception as e:
+        except Exception, e:
             add_warning(req, _("Cannot reset password: %(error)s",
                                error=exception_to_unicode(e)))
             self.log.error("Unable to reset password: %s",
                            exception_to_unicode(e, traceback=True))
             return
         try:
             acctmgr._notify('password_reset', username, email, new_password)
-        except NotificationError as e:
+        except NotificationError, e:
             msg = _("Error raised while sending a change notification.")
             if req.path_info.startswith('/admin'):
                 msg += _("You'll get details with TracLogging enabled.")
             else:
                 msg += _("You should report that issue to a Trac admin.")
             add_warning(req, msg)
             self.log.error("Unable to send password reset notification: %s",
@@ -368,15 +368,15 @@
         # No message, if method has been called from user admin panel.
         if not req.path_info.startswith('/admin'):
             add_notice(req, _("A new password has been sent to you at "
                               "<%(email)s>.", email=email))
             req.redirect(req.href.login())
 
 
-class LoginModule(auth.LoginModule):
+class LoginModule(auth.LoginModule, CommonTemplateProvider):
     """Custom login form and processing.
 
     This is woven with the trac.auth.LoginModule it inherits and overwrites.
     But both can't co-exist, so Trac's built-in authentication module
     must be disabled to use this one.
     """
 
@@ -401,27 +401,32 @@
 
     auth_cookie_path = Option('trac', 'auth_cookie_path', '',
         """Path for the authentication cookie. Set this to the common
         base path of several Trac instances if you want them to share
         the cookie.  (''since 0.12'')""")
 
     # Options dedicated to acct_mgr.web_ui.LoginModule.
+    login_opt_list = BoolOption(
+        'account-manager', 'login_opt_list', False,
+        """Set to True, to switch login page style showing alternative actions
+        in a single listing together.""")
+
     cookie_refresh_pct = IntOption(
         'account-manager', 'cookie_refresh_pct', 10,
         """Persistent sessions randomly get a new session cookie ID with
         likelihood in percent per work hour given here (zero equals to never)
         to decrease vulnerability of long-lasting sessions.""")
 
     environ_auth_overwrite = BoolOption(
         'account-manager', 'environ_auth_overwrite', True,
         """Whether environment variable REMOTE_USER should get overwritten
         after processing login form input. Otherwise it will only be set,
         if unset at the time of authentication.""")
 
-    # Update cookies for persistent sessions only 1/day.
+    # Update cookies for persistant sessions only 1/day.
     #   hex_entropy returns 32 chars per call equal to 128 bit of entropy,
     #   so it should be technically impossible to explore the hash even within
     #   a year by just throwing forged HTTP requests at the server.
     #   I.e. it would require 1.000.000 machines, each at 5*10^24 requests/s,
     #   equal to a full-scale DDoS attack - an entirely different issue.
     UPDATE_INTERVAL = 86400
 
@@ -487,29 +492,29 @@
                 req.environ['REMOTE_USER'] = username
         return super(LoginModule, self).authenticate(req)
 
     authenticate = if_enabled(authenticate)
 
     match_request = if_enabled(auth.LoginModule.match_request)
 
-    @process_request_compat
     def process_request(self, req):
         if req.path_info.startswith('/login') and req.authname == 'anonymous':
             try:
                 referer = self._referer(req)
             except AttributeError:
                 # Fallback for Trac 0.11 compatibility.
                 referer = req.get_header('Referer')
             # Steer clear of requests going nowhere or loop to self.
             if referer is None or \
                     referer.startswith(req.abs_href('/login')) or \
                     referer.startswith(req.abs_href('/captcha')):
                 referer = req.abs_href()
             data = {
-                'i18n_tag': i18n_tag,
+                '_dgettext': dgettext,
+                'login_opt_list': self.login_opt_list,
                 'persistent_sessions':
                     AccountManager(self.env).persistent_sessions,
                 'referer': referer,
                 'registration_enabled': RegistrationModule(self.env).enabled,
                 'reset_password_enabled':
                     AccountModule(self.env).reset_password_enabled
             }
@@ -522,22 +527,22 @@
                 else:
                     f_user = req.args.get('username')
                     release_time = AccountGuard(self.env
                                                 ).pretty_release_time(req,
                                                                       f_user)
                     if release_time is not None:
                         data['login_error'] = \
-                            _("Account locked, please try again after "
-                              "%(release_time)s", release_time=release_time)
+                            _("Account locked, please try again after % "
+                              "(release_time)s", release_time=release_time)
                     else:
                         data['login_error'] = _("Account locked")
-            return 'account_login.html', data
+            return 'account_login.html', data, None
         else:
             n_plural = req.args.get('failed_logins')
-            if n_plural is not None and n_plural > 0:
+            if n_plural > 0:
                 add_warning(req, tag(ngettext(
                     "Login after %(attempts)s failed attempt",
                     "Login after %(attempts)s failed attempts",
                     n_plural, attempts=n_plural
                 )))
         return super(LoginModule, self).process_request(req)
 
@@ -550,15 +555,15 @@
         by the browser.
         """
 
         acctmgr = AccountManager(self.env)
         name = None
         # Replicate _get_name_for_cookie() or _cookie_to_name() since Trac 1.0
         # adding special handling of persistent sessions, as the user may have
-        # a dynamic IP address and this would lead to the user being logged out
+        # a dynamic IP adress and this would lead to the user being logged out
         # due to an IP address conflict.
         if 'trac_auth_session' in req.incookie or True:
             sql = "SELECT name FROM auth_cookie WHERE cookie=%s AND ipnr=%s"
             args = (cookie.value, req.remote_addr)
             if acctmgr.persistent_sessions or not self.check_ip:
                 sql = "SELECT name FROM auth_cookie WHERE cookie=%s"
                 args = (cookie.value,)
@@ -683,15 +688,15 @@
     # Internal methods
 
     def _distribute_auth(self, req, trac_auth, name=None):
         # Single Sign On authentication distribution between multiple
         #   Trac environments managed by AccountManager.
         local_env_name = req.base_path.lstrip('/')
 
-        for env_name, env_path in iteritems(get_environments(req.environ)):
+        for env_name, env_path in get_environments(req.environ).iteritems():
             if env_name != local_env_name:
                 try:
                     # Cache environment for subsequent invocations.
                     env = open_environment(env_path, use_cache=True)
                     auth_cookie_path = env.config.get('trac',
                                                       'auth_cookie_path')
                     # Consider only Trac environments with equal, non-default
@@ -715,24 +720,24 @@
                                 """, (trac_auth, name, req.remote_addr,
                                       int(time.time())))
 
                         env.log.debug("Auth data received from: %s",
                                       local_env_name)
                         self.log.debug("Auth distribution success: %s",
                                        env_name)
-                except Exception as e:
+                except Exception, e:
                     self.log.debug("Auth distribution skipped for env %s: %s",
                                    env_name,
                                    exception_to_unicode(e, traceback=True))
 
     def _get_cookie_path(self, req):
         """Determine "path" cookie property from setting or request object."""
         return self.auth_cookie_path or req.base_path or '/'
 
-    # Keep this code in a separate method to be able to expire the session
+    # Keep this code in a separate methode to be able to expire the session
     # cookie trac_auth_session independently of the trac_auth cookie.
     def _expire_session_cookie(self, req):
         """Instruct the user agent to drop the session cookie.
 
         This is achieved by setting "expires" property to a date in the past.
         """
         cookie_path = self._get_cookie_path(req)
@@ -793,13 +798,13 @@
                not self.env.is_enabled(auth.LoginModule)
 
 
 def _set_password(env, req, username, password, old_password=None):
     try:
         AccountManager(env).set_password(username, password,
                                          old_password=old_password)
-    except NotificationError as e:
+    except NotificationError, e:
         add_warning(req, _("Error raised while sending a change "
                            "notification.") +
                     _("You should report that issue to a Trac admin."))
         env.log.error('Unable to send password change notification: %s',
                       exception_to_unicode(e, traceback=True))
```

### Comparing `tracaccountmanager-0.6.0/changelog` & `TracAccountManager-0.6.dev0/changelog`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/contrib/approval.xcf.bz2` & `TracAccountManager-0.6.dev0/contrib/approval.xcf.bz2`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/contrib/fix-session_attribute-failed_logins.py` & `TracAccountManager-0.6.dev0/contrib/fix-session_attribute-failed_logins.py`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/contrib/refresh.xcf.bz2` & `TracAccountManager-0.6.dev0/contrib/refresh.xcf.bz2`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/contrib/sessionstore_convert.py` & `TracAccountManager-0.6.dev0/contrib/sessionstore_convert.py`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/contrib/style.css` & `TracAccountManager-0.6.dev0/contrib/style.css`

 * *Files identical despite different names*

### Comparing `tracaccountmanager-0.6.0/setup.cfg` & `TracAccountManager-0.6.dev0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+[egg_info]
+tag_build = dev
+tag_date = 0
+
 [aliases]
 release = sdist bdist_wheel
 
-[bdist_wheel]
-universal = 1
-
 [extract_messages]
 add_comments = TRANSLATOR:
 msgid_bugs_address = hoff.st@shaas.net
 output_file = acct_mgr/locale/messages.pot
 keywords = _ ngettext:1,2 N_ tag_  cleandoc_
 width = 72
-mapping_file = messages.cfg
 
 [init_catalog]
 input_file = acct_mgr/locale/messages.pot
 output_dir = acct_mgr/locale
 domain = acct_mgr
 
 [compile_catalog]
@@ -26,11 +26,7 @@
 output_dir = acct_mgr/locale
 domain = acct_mgr
 
 [check_catalog]
 input_dir = acct_mgr/locale
 domain = acct_mgr
 
-[egg_info]
-tag_build = 
-tag_date = 0
-
```

### Comparing `tracaccountmanager-0.6.0/setup.py` & `TracAccountManager-0.6.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,42 +6,47 @@
 # Author: Matthew Good <trac@matt-good.net>
 
 from setuptools import find_packages, setup
 
 extra = {}
 
 try:
-    import babel
     from trac.dist import get_l10n_cmdclass
+    from trac.dist import extract_python
 except ImportError:
     pass
 else:
-    extra['cmdclass'] = get_l10n_cmdclass()
+    cmdclass = get_l10n_cmdclass()
+    if cmdclass:
+        extra['cmdclass'] = cmdclass
+        extractors = [
+            ('**/templates/**.html', 'genshi', None),
+            ('**.py', 'trac.dist:extract_python', None),
+        ]
+        extra['message_extractors'] = {
+            'acct_mgr': extractors,
+        }
 
 setup(
     name='TracAccountManager',
-    version='0.6.0',
+    version='0.6',
     author='Matthew Good',
     author_email='trac@matt-good.net',
     maintainer='Steffen Hoffmann',
     maintainer_email='hoff.st@web.de',
     url='https://trac-hacks.org/wiki/AccountManagerPlugin',
     description='User account management plugin for Trac',
     license='3-Clause BSD',
-    classifiers=[
-        'Framework :: Trac',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-    ],
+    classifiers = ['Framework :: Trac'],
     packages=find_packages(exclude=['*.tests*']),
     package_data={
         'acct_mgr': [
             'htdocs/*.css', 'htdocs/js/*', 'htdocs/*.png',
             'locale/*/LC_MESSAGES/*.mo', 'locale/.placeholder',
-            'templates/*/*.html', 'templates/*/*.txt'
+            'templates/*.html', 'templates/*.txt'
         ]
     },
     test_suite='acct_mgr.tests.test_suite',
     zip_safe=True,
     install_requires=['Trac'],
     extras_require={
         'Babel': 'Babel>= 0.9.5',
```

