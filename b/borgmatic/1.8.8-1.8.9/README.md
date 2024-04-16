# Comparing `tmp/borgmatic-1.8.8.tar.gz` & `tmp/borgmatic-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borgmatic-1.8.8.tar", last modified: Wed Jan 31 18:55:04 2024, max compression
+gzip compressed data, was "borgmatic-1.8.9.tar", last modified: Mon Mar 11 20:28:10 2024, max compression
```

## Comparing `borgmatic-1.8.8.tar` & `borgmatic-1.8.9.tar`

### file list

```diff
@@ -1,340 +1,343 @@
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.083243 borgmatic-1.8.8/
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.8.8/.dockerignore
--rw-r--r--   0 witten    (1000) witten    (1000)     2239 2023-12-26 05:59:57.000000 borgmatic-1.8.8/.drone.yml
--rw-r--r--   0 witten    (1000) witten    (1000)     1624 2023-12-26 05:49:05.000000 borgmatic-1.8.8/.eleventy.js
--rw-r--r--   0 witten    (1000) witten    (1000)       12 2023-12-26 05:48:44.000000 borgmatic-1.8.8/.flake8
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.036575 borgmatic-1.8.8/.gitea/
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.043242 borgmatic-1.8.8/.gitea/issue_template/
--rw-r--r--   0 witten    (1000) witten    (1000)     2113 2023-12-26 05:59:57.000000 borgmatic-1.8.8/.gitea/issue_template/bug_template.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)       27 2023-12-26 05:59:57.000000 borgmatic-1.8.8/.gitea/issue_template/config.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)      334 2023-12-26 05:59:57.000000 borgmatic-1.8.8/.gitea/issue_template/feature_template.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)      105 2023-05-12 23:35:39.000000 borgmatic-1.8.8/.gitignore
--rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.8.8/AUTHORS
--rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.8.8/LICENSE
--rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.8.8/MANIFEST.in
--rw-r--r--   0 witten    (1000) witten    (1000)    70678 2024-01-31 18:52:26.000000 borgmatic-1.8.8/NEWS
--rw-r--r--   0 witten    (1000) witten    (1000)      920 2024-01-31 18:55:04.083243 borgmatic-1.8.8/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     6856 2023-12-26 05:59:57.000000 borgmatic-1.8.8/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      658 2023-12-26 05:59:57.000000 borgmatic-1.8.8/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.043242 borgmatic-1.8.8/borgmatic/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.046575 borgmatic-1.8.8/borgmatic/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:46:46.000000 borgmatic-1.8.8/borgmatic/actions/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      327 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1190 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      878 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1322 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1914 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/compact.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.046575 borgmatic-1.8.8/borgmatic/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3698 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/actions/config/bootstrap.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1622 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/config/generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      858 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/config/validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3869 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/actions/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)      863 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/export_key.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1521 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1962 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1571 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)      398 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/json.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1709 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1385 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1380 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1091 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13507 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1228 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1162 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      705 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/actions/transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.049909 borgmatic-1.8.8/borgmatic/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2465 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1434 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15943 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1855 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)    20188 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1995 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2412 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/export_key.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2628 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5954 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1368 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/borg/feature.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4088 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/borg/flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3731 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8719 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2996 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3368 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3123 2024-01-24 23:42:05.000000 borgmatic-1.8.8/borgmatic/borg/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2197 2024-01-24 23:37:17.000000 borgmatic-1.8.8/borgmatic/borg/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5539 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/borg/state.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2191 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)      673 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1046 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/borg/version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.049909 borgmatic-1.8.8/borgmatic/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/commands/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    53949 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/commands/arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    33465 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/commands/borgmatic.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.049909 borgmatic-1.8.8/borgmatic/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1382 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/completion/actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2390 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/completion/bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6785 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/completion/fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/commands/validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.053242 borgmatic-1.8.8/borgmatic/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      322 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/config/checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2210 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/config/collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2170 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/constants.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1573 2024-01-07 06:49:02.000000 borgmatic-1.8.8/borgmatic/config/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10993 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15578 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/load.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11373 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/config/normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4227 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/override.py
--rw-r--r--   0 witten    (1000) witten    (1000)    67646 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/schema.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     7318 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/config/validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16771 2024-01-24 23:37:17.000000 borgmatic-1.8.8/borgmatic/execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.056575 borgmatic-1.8.8/borgmatic/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/borgmatic/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2362 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/apprise.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3302 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/hooks/command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1929 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1810 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3315 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2460 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4896 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4405 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/loki.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9168 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/mariadb.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7251 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/hooks/mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)      199 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/monitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9153 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2852 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2606 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/hooks/pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12643 2024-01-31 18:41:59.000000 borgmatic-1.8.8/borgmatic/hooks/postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4921 2024-01-24 22:25:14.000000 borgmatic-1.8.8/borgmatic/hooks/sqlite.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7142 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1120 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)      586 2023-12-26 05:59:57.000000 borgmatic-1.8.8/borgmatic/verbosity.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.083243 borgmatic-1.8.8/borgmatic.egg-info/
--rw-r--r--   0 witten    (1000) witten    (1000)      920 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     9244 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/SOURCES.txt
--rw-r--r--   0 witten    (1000) witten    (1000)        1 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/dependency_links.txt
--rw-r--r--   0 witten    (1000) witten    (1000)      200 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/entry_points.txt
--rw-r--r--   0 witten    (1000) witten    (1000)      100 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/requires.txt
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2024-01-31 18:55:03.000000 borgmatic-1.8.8/borgmatic.egg-info/top_level.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.056575 borgmatic-1.8.8/docs/
--rw-r--r--   0 witten    (1000) witten    (1000)     1544 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/Dockerfile
--rw-r--r--   0 witten    (1000) witten    (1000)     6856 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      672 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.056575 borgmatic-1.8.8/docs/_data/
--rw-r--r--   0 witten    (1000) witten    (1000)      112 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_data/borgmatic.js
--rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/_data/layout.json
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.056575 borgmatic-1.8.8/docs/_includes/
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/_includes/asciinema.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.059909 borgmatic-1.8.8/docs/_includes/components/
--rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/_includes/components/external-links.css
--rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/_includes/components/info-blocks.css
--rw-r--r--   0 witten    (1000) witten    (1000)     5125 2023-12-26 05:48:44.000000 borgmatic-1.8.8/docs/_includes/components/lists.css
--rw-r--r--   0 witten    (1000) witten    (1000)     1788 2023-12-26 05:48:44.000000 borgmatic-1.8.8/docs/_includes/components/minilink.css
--rw-r--r--   0 witten    (1000) witten    (1000)      219 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_includes/components/suggestion-link.html
--rw-r--r--   0 witten    (1000) witten    (1000)     1849 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_includes/components/toc.css
--rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/_includes/header.njk
--rw-r--r--   0 witten    (1000) witten    (1000)    26314 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_includes/index.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.059909 borgmatic-1.8.8/docs/_includes/layouts/
--rw-r--r--   0 witten    (1000) witten    (1000)      909 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_includes/layouts/base.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     1184 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/_includes/layouts/main.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     3039 2023-05-12 23:35:39.000000 borgmatic-1.8.8/docs/_includes/prism-theme.css
--rw-r--r--   0 witten    (1000) witten    (1000)      422 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/docker-compose.yaml
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.059909 borgmatic-1.8.8/docs/how-to/
--rw-r--r--   0 witten    (1000) witten    (1000)     5252 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
--rw-r--r--   0 witten    (1000) witten    (1000)    17420 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/backup-your-databases.md
--rw-r--r--   0 witten    (1000) witten    (1000)     2820 2024-01-24 22:25:14.000000 borgmatic-1.8.8/docs/how-to/customize-warnings-and-errors.md
--rw-r--r--   0 witten    (1000) witten    (1000)     8724 2023-12-28 17:53:07.000000 borgmatic-1.8.8/docs/how-to/deal-with-very-large-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6341 2024-01-24 22:25:14.000000 borgmatic-1.8.8/docs/how-to/develop-on-borgmatic.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6826 2024-01-24 22:25:14.000000 borgmatic-1.8.8/docs/how-to/extract-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)       77 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/index.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6531 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/inspect-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     2165 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/make-backups-redundant.md
--rw-r--r--   0 witten    (1000) witten    (1000)    20919 2024-01-24 22:25:14.000000 borgmatic-1.8.8/docs/how-to/make-per-application-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    17299 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/monitor-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     4149 2023-12-30 23:48:52.000000 borgmatic-1.8.8/docs/how-to/provide-your-passwords.md
--rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.8.8/docs/how-to/restore-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)     5925 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/run-arbitrary-borg-commands.md
--rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.8.8/docs/how-to/run-preparation-steps-before-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    15688 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/how-to/set-up-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     7316 2024-01-24 22:25:14.000000 borgmatic-1.8.8/docs/how-to/upgrade.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/docs/reference/
--rw-r--r--   0 witten    (1000) witten    (1000)      853 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/reference/command-line.md
--rw-r--r--   0 witten    (1000) witten    (1000)      757 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/reference/configuration.md
--rw-r--r--   0 witten    (1000) witten    (1000)       80 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/reference/index.md
--rw-r--r--   0 witten    (1000) witten    (1000)     2358 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/reference/source-code.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/docs/static/
--rw-r--r--   0 witten    (1000) witten    (1000)   160907 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/static/apprise.png
--rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/borgbase.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/borgmatic.png
--rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/borgmatic.svg
--rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/cronhub.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/cronitor.png
--rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/healthchecks.png
--rw-r--r--   0 witten    (1000) witten    (1000)    15536 2023-12-26 05:59:57.000000 borgmatic-1.8.8/docs/static/loki.png
--rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/mariadb.png
--rw-r--r--   0 witten    (1000) witten    (1000)    12839 2023-05-12 23:35:39.000000 borgmatic-1.8.8/docs/static/mongodb.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/mysql.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10266 2023-05-12 23:35:39.000000 borgmatic-1.8.8/docs/static/ntfy.png
--rw-r--r--   0 witten    (1000) witten    (1000)    20107 2023-05-12 23:35:39.000000 borgmatic-1.8.8/docs/static/pagerduty.png
--rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.8.8/docs/static/postgresql.png
--rw-r--r--   0 witten    (1000) witten    (1000)     4668 2023-12-26 05:48:44.000000 borgmatic-1.8.8/docs/static/sqlite.png
--rw-r--r--   0 witten    (1000) witten    (1000)       64 2023-04-15 02:33:57.000000 borgmatic-1.8.8/pyproject.toml
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.036575 borgmatic-1.8.8/sample/
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/sample/cron/
--rw-r--r--   0 witten    (1000) witten    (1000)      183 2023-05-12 23:35:39.000000 borgmatic-1.8.8/sample/cron/borgmatic
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/sample/systemd/
--rw-r--r--   0 witten    (1000) witten    (1000)      499 2023-12-26 05:59:57.000000 borgmatic-1.8.8/sample/systemd/borgmatic-user.service
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.8/sample/systemd/borgmatic-user.timer
--rw-r--r--   0 witten    (1000) witten    (1000)     2574 2023-12-26 05:59:57.000000 borgmatic-1.8.8/sample/systemd/borgmatic.service
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.8/sample/systemd/borgmatic.timer
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/scripts/
--rwxr-xr-x   0 witten    (1000) witten    (1000)      259 2023-12-26 05:59:57.000000 borgmatic-1.8.8/scripts/dev-docs
--rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2023-05-12 23:35:39.000000 borgmatic-1.8.8/scripts/find-unsupported-borg-options
--rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.8.8/scripts/push
--rwxr-xr-x   0 witten    (1000) witten    (1000)     1685 2023-12-26 05:59:57.000000 borgmatic-1.8.8/scripts/release
--rwxr-xr-x   0 witten    (1000) witten    (1000)      658 2023-12-26 05:59:57.000000 borgmatic-1.8.8/scripts/run-end-to-end-dev-tests
--rwxr-xr-x   0 witten    (1000) witten    (1000)     1343 2023-12-26 05:59:57.000000 borgmatic-1.8.8/scripts/run-full-tests
--rw-r--r--   0 witten    (1000) witten    (1000)      505 2024-01-31 18:55:04.083243 borgmatic-1.8.8/setup.cfg
--rw-r--r--   0 witten    (1000) witten    (1000)     1349 2024-01-31 18:52:35.000000 borgmatic-1.8.8/setup.py
--rw-r--r--   0 witten    (1000) witten    (1000)      537 2024-01-24 22:25:14.000000 borgmatic-1.8.8/test_requirements.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.063242 borgmatic-1.8.8/tests/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/end-to-end/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/end-to-end/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1700 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/docker-compose.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     2981 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      268 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_completion.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19474 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_database.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1711 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_dev_parity_with_build_server.py
--rw-r--r--   0 witten    (1000) witten    (1000)      588 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      358 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_invalid_flag.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1980 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1630 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/end-to-end/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/integration/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/actions/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/actions/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1088 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/actions/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/borg/test_commands.py
--rw-r--r--   0 witten    (1000) witten    (1000)      546 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/integration/borg/test_feature.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/integration/commands/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.066576 borgmatic-1.8.8/tests/integration/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      811 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/completion/test_actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/completion/test_bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/completion/test_fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)    24013 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)      432 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/integration/commands/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/commands/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.069909 borgmatic-1.8.8/tests/integration/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/integration/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8839 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    44398 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/integration/config/test_load.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1594 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1142 2023-12-29 04:06:02.000000 borgmatic-1.8.8/tests/integration/config/test_schema.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7885 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/integration/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.069909 borgmatic-1.8.8/tests/integration/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)      753 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3144 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/integration/hooks/test_loki.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13671 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/integration/test_execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.069909 borgmatic-1.8.8/tests/unit/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/unit/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.073243 borgmatic-1.8.8/tests/unit/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:46:46.000000 borgmatic-1.8.8/tests/unit/actions/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.073243 borgmatic-1.8.8/tests/unit/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)     6690 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/config/test_bootstrap.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1305 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      599 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/config/test_validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      390 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)      821 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2847 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3049 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9107 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/actions/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)      670 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_export_key.py
--rw-r--r--   0 witten    (1000) witten    (1000)      967 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1074 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2085 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)      889 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_json.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2084 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)      824 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2609 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1748 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    20005 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1575 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1526 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      630 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/actions/test_transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.076576 borgmatic-1.8.8/tests/unit/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/unit/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12673 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4204 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    46706 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7282 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)   133420 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2075 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9727 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_export_key.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12008 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)    22446 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7120 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/borg/test_flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19581 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/borg/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)    27870 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12356 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16640 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13365 2024-01-24 23:42:44.000000 borgmatic-1.8.8/tests/unit/borg/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16121 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)    23624 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)    22531 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1577 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2560 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/borg/test_version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.076576 borgmatic-1.8.8/tests/unit/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/unit/commands/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.076576 borgmatic-1.8.8/tests/unit/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      226 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/commands/completion/test_actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)      431 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/commands/completion/test_bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4616 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/commands/completion/test_fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)    17204 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    60271 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/commands/test_borgmatic.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.079909 borgmatic-1.8.8/tests/unit/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/unit/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      694 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/config/test_checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8085 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/config/test_collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2068 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/config/test_constants.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3090 2023-12-26 05:49:05.000000 borgmatic-1.8.8/tests/unit/config/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5029 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1587 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/config/test_load.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7115 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/config/test_normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5231 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7311 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-01-31 18:55:04.083243 borgmatic-1.8.8/tests/unit/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.8/tests/unit/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6382 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_apprise.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4238 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/hooks/test_command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3726 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3162 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4490 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3002 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11731 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3192 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_loki.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19565 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_mariadb.py
--rw-r--r--   0 witten    (1000) witten    (1000)    17395 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/hooks/test_mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19490 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7411 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2303 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/hooks/test_pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    39869 2024-01-31 18:42:00.000000 borgmatic-1.8.8/tests/unit/hooks/test_postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7930 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/hooks/test_sqlite.py
--rw-r--r--   0 witten    (1000) witten    (1000)    22253 2024-01-24 22:25:14.000000 borgmatic-1.8.8/tests/unit/test_execute.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16323 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/test_logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1852 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/test_signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1426 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tests/unit/test_verbosity.py
--rw-r--r--   0 witten    (1000) witten    (1000)      829 2023-12-26 05:59:57.000000 borgmatic-1.8.8/tox.ini
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.445958 borgmatic-1.8.9/
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.8.9/.dockerignore
+-rw-r--r--   0 witten    (1000) witten    (1000)     1624 2023-12-26 05:49:05.000000 borgmatic-1.8.9/.eleventy.js
+-rw-r--r--   0 witten    (1000) witten    (1000)       12 2023-12-26 05:48:44.000000 borgmatic-1.8.9/.flake8
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.409290 borgmatic-1.8.9/.gitea/
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.412624 borgmatic-1.8.9/.gitea/issue_template/
+-rw-r--r--   0 witten    (1000) witten    (1000)     2113 2023-12-26 05:59:57.000000 borgmatic-1.8.9/.gitea/issue_template/bug_template.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)       27 2023-12-26 05:59:57.000000 borgmatic-1.8.9/.gitea/issue_template/config.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)      334 2023-12-26 05:59:57.000000 borgmatic-1.8.9/.gitea/issue_template/feature_template.yaml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.412624 borgmatic-1.8.9/.gitea/workflows/
+-rw-r--r--   0 witten    (1000) witten    (1000)      770 2024-03-08 18:54:55.000000 borgmatic-1.8.9/.gitea/workflows/build.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)      105 2023-05-12 23:35:39.000000 borgmatic-1.8.9/.gitignore
+-rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.8.9/AUTHORS
+-rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.8.9/LICENSE
+-rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.8.9/MANIFEST.in
+-rw-r--r--   0 witten    (1000) witten    (1000)    72140 2024-03-11 20:27:02.000000 borgmatic-1.8.9/NEWS
+-rw-r--r--   0 witten    (1000) witten    (1000)      920 2024-03-11 20:28:10.445958 borgmatic-1.8.9/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     6648 2024-03-07 03:55:43.000000 borgmatic-1.8.9/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      658 2023-12-26 05:59:57.000000 borgmatic-1.8.9/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.412624 borgmatic-1.8.9/borgmatic/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.415957 borgmatic-1.8.9/borgmatic/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:46:46.000000 borgmatic-1.8.9/borgmatic/actions/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      327 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1190 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      878 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1322 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1914 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/compact.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.415957 borgmatic-1.8.9/borgmatic/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3698 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/actions/config/bootstrap.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1622 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/config/generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      858 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/config/validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3869 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/actions/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      863 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/export_key.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1521 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1962 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1571 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      398 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/json.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1709 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1385 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1380 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1091 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13507 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1228 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1162 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      705 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/actions/transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.419290 borgmatic-1.8.9/borgmatic/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2465 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1434 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15943 2024-02-16 03:12:50.000000 borgmatic-1.8.9/borgmatic/borg/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1855 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    20188 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1995 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2412 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/export_key.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2628 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5954 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1368 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/borg/feature.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4088 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/borg/flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3731 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8719 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2996 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3368 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3810 2024-03-11 18:22:45.000000 borgmatic-1.8.9/borgmatic/borg/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2197 2024-01-24 23:37:17.000000 borgmatic-1.8.9/borgmatic/borg/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5539 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/borg/state.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2191 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      673 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1046 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/borg/version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.419290 borgmatic-1.8.9/borgmatic/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/commands/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    53949 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/commands/arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    33527 2024-03-09 01:30:51.000000 borgmatic-1.8.9/borgmatic/commands/borgmatic.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.419290 borgmatic-1.8.9/borgmatic/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1382 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/completion/actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2390 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/completion/bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6785 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/completion/fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/commands/validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.419290 borgmatic-1.8.9/borgmatic/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      322 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/config/checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2210 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/config/collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2170 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/config/constants.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1573 2024-01-07 06:49:02.000000 borgmatic-1.8.9/borgmatic/config/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10993 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/config/generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15578 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/config/load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11373 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/config/normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4486 2024-02-16 05:03:28.000000 borgmatic-1.8.9/borgmatic/config/override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    70736 2024-03-11 19:34:43.000000 borgmatic-1.8.9/borgmatic/config/schema.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     7318 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/config/validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    16771 2024-01-24 23:37:17.000000 borgmatic-1.8.9/borgmatic/execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.422624 borgmatic-1.8.9/borgmatic/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/borgmatic/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3551 2024-03-10 22:53:25.000000 borgmatic-1.8.9/borgmatic/hooks/apprise.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3302 2024-03-08 18:54:55.000000 borgmatic-1.8.9/borgmatic/hooks/command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1929 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1810 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3315 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2460 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3366 2024-03-10 23:00:38.000000 borgmatic-1.8.9/borgmatic/hooks/healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2650 2024-03-10 23:00:39.000000 borgmatic-1.8.9/borgmatic/hooks/logs.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4405 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/loki.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9648 2024-03-03 22:27:48.000000 borgmatic-1.8.9/borgmatic/hooks/mariadb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7251 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/hooks/mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      199 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/monitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9607 2024-03-03 22:27:48.000000 borgmatic-1.8.9/borgmatic/hooks/mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3218 2024-03-11 19:35:04.000000 borgmatic-1.8.9/borgmatic/hooks/ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2606 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/hooks/pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12643 2024-01-31 18:41:59.000000 borgmatic-1.8.9/borgmatic/hooks/postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4921 2024-01-24 22:25:14.000000 borgmatic-1.8.9/borgmatic/hooks/sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7357 2024-03-04 21:46:28.000000 borgmatic-1.8.9/borgmatic/logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1120 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      586 2023-12-26 05:59:57.000000 borgmatic-1.8.9/borgmatic/verbosity.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.445958 borgmatic-1.8.9/borgmatic.egg-info/
+-rw-r--r--   0 witten    (1000) witten    (1000)      920 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     9297 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/SOURCES.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)        1 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/dependency_links.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)      200 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/entry_points.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)      100 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/requires.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2024-03-11 20:28:10.000000 borgmatic-1.8.9/borgmatic.egg-info/top_level.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.422624 borgmatic-1.8.9/docs/
+-rw-r--r--   0 witten    (1000) witten    (1000)     1544 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/Dockerfile
+-rw-r--r--   0 witten    (1000) witten    (1000)     6648 2024-03-07 03:55:43.000000 borgmatic-1.8.9/docs/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      672 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.422624 borgmatic-1.8.9/docs/_data/
+-rw-r--r--   0 witten    (1000) witten    (1000)      112 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_data/borgmatic.js
+-rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/_data/layout.json
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.422624 borgmatic-1.8.9/docs/_includes/
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/_includes/asciinema.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.425957 borgmatic-1.8.9/docs/_includes/components/
+-rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/_includes/components/external-links.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/_includes/components/info-blocks.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     5125 2023-12-26 05:48:44.000000 borgmatic-1.8.9/docs/_includes/components/lists.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     1788 2023-12-26 05:48:44.000000 borgmatic-1.8.9/docs/_includes/components/minilink.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      219 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_includes/components/suggestion-link.html
+-rw-r--r--   0 witten    (1000) witten    (1000)     1849 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_includes/components/toc.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/_includes/header.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)    26314 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_includes/index.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.425957 borgmatic-1.8.9/docs/_includes/layouts/
+-rw-r--r--   0 witten    (1000) witten    (1000)      909 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_includes/layouts/base.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     1184 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/_includes/layouts/main.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     3039 2023-05-12 23:35:39.000000 borgmatic-1.8.9/docs/_includes/prism-theme.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      422 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/docker-compose.yaml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.425957 borgmatic-1.8.9/docs/how-to/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5252 2024-03-11 17:38:31.000000 borgmatic-1.8.9/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    17635 2024-02-09 23:34:14.000000 borgmatic-1.8.9/docs/how-to/backup-your-databases.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     2820 2024-01-24 22:25:14.000000 borgmatic-1.8.9/docs/how-to/customize-warnings-and-errors.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     8724 2023-12-28 17:53:07.000000 borgmatic-1.8.9/docs/how-to/deal-with-very-large-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6888 2024-03-11 02:14:14.000000 borgmatic-1.8.9/docs/how-to/develop-on-borgmatic.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6826 2024-02-09 23:34:15.000000 borgmatic-1.8.9/docs/how-to/extract-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       77 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/how-to/index.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6531 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/how-to/inspect-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     2165 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/how-to/make-backups-redundant.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    20919 2024-01-24 22:25:14.000000 borgmatic-1.8.9/docs/how-to/make-per-application-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    18959 2024-03-11 19:33:59.000000 borgmatic-1.8.9/docs/how-to/monitor-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     4149 2023-12-30 23:48:52.000000 borgmatic-1.8.9/docs/how-to/provide-your-passwords.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.8.9/docs/how-to/restore-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     5925 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/how-to/run-arbitrary-borg-commands.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.8.9/docs/how-to/run-preparation-steps-before-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    15708 2024-03-04 21:46:46.000000 borgmatic-1.8.9/docs/how-to/set-up-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     7316 2024-01-24 22:25:14.000000 borgmatic-1.8.9/docs/how-to/upgrade.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.425957 borgmatic-1.8.9/docs/reference/
+-rw-r--r--   0 witten    (1000) witten    (1000)      853 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/reference/command-line.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      757 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/reference/configuration.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       80 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/reference/index.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     2358 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/reference/source-code.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.429291 borgmatic-1.8.9/docs/static/
+-rw-r--r--   0 witten    (1000) witten    (1000)   160907 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/static/apprise.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/borgbase.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/borgmatic.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/borgmatic.svg
+-rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/cronhub.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/cronitor.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/healthchecks.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    15536 2023-12-26 05:59:57.000000 borgmatic-1.8.9/docs/static/loki.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/mariadb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    12839 2023-05-12 23:35:39.000000 borgmatic-1.8.9/docs/static/mongodb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/mysql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10266 2023-05-12 23:35:39.000000 borgmatic-1.8.9/docs/static/ntfy.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    20107 2023-05-12 23:35:39.000000 borgmatic-1.8.9/docs/static/pagerduty.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.8.9/docs/static/postgresql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4668 2023-12-26 05:48:44.000000 borgmatic-1.8.9/docs/static/sqlite.png
+-rw-r--r--   0 witten    (1000) witten    (1000)       64 2023-04-15 02:33:57.000000 borgmatic-1.8.9/pyproject.toml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.409290 borgmatic-1.8.9/sample/
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.429291 borgmatic-1.8.9/sample/cron/
+-rw-r--r--   0 witten    (1000) witten    (1000)      183 2023-05-12 23:35:39.000000 borgmatic-1.8.9/sample/cron/borgmatic
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.429291 borgmatic-1.8.9/sample/systemd/
+-rw-r--r--   0 witten    (1000) witten    (1000)      499 2023-12-26 05:59:57.000000 borgmatic-1.8.9/sample/systemd/borgmatic-user.service
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.9/sample/systemd/borgmatic-user.timer
+-rw-r--r--   0 witten    (1000) witten    (1000)     2574 2023-12-26 05:59:57.000000 borgmatic-1.8.9/sample/systemd/borgmatic.service
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.9/sample/systemd/borgmatic.timer
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/scripts/
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      259 2023-12-26 05:59:57.000000 borgmatic-1.8.9/scripts/dev-docs
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2023-05-12 23:35:39.000000 borgmatic-1.8.9/scripts/find-unsupported-borg-options
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.8.9/scripts/push
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     1685 2023-12-26 05:59:57.000000 borgmatic-1.8.9/scripts/release
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      828 2024-03-07 05:24:41.000000 borgmatic-1.8.9/scripts/run-end-to-end-tests
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     1290 2024-03-06 16:27:03.000000 borgmatic-1.8.9/scripts/run-full-tests
+-rw-r--r--   0 witten    (1000) witten    (1000)      505 2024-03-11 20:28:10.445958 borgmatic-1.8.9/setup.cfg
+-rw-r--r--   0 witten    (1000) witten    (1000)     1349 2024-03-11 20:26:53.000000 borgmatic-1.8.9/setup.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      537 2024-01-24 22:25:14.000000 borgmatic-1.8.9/test_requirements.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/end-to-end/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/end-to-end/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1666 2024-03-07 02:39:14.000000 borgmatic-1.8.9/tests/end-to-end/docker-compose.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     2981 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      268 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_completion.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19474 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_database.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      588 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      358 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_invalid_flag.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1980 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1630 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/end-to-end/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/integration/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/actions/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/actions/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1088 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/actions/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/borg/test_commands.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      546 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/integration/borg/test_feature.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/integration/commands/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.432624 borgmatic-1.8.9/tests/integration/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      811 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/completion/test_actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/completion/test_bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/completion/test_fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    24013 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      432 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/integration/commands/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/commands/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.435958 borgmatic-1.8.9/tests/integration/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/integration/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8839 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    44398 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/integration/config/test_load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1810 2024-02-16 05:08:36.000000 borgmatic-1.8.9/tests/integration/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1142 2023-12-29 04:06:02.000000 borgmatic-1.8.9/tests/integration/config/test_schema.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7876 2024-02-16 05:02:53.000000 borgmatic-1.8.9/tests/integration/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.435958 borgmatic-1.8.9/tests/integration/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)      855 2024-03-10 16:50:06.000000 borgmatic-1.8.9/tests/integration/hooks/test_apprise.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      870 2024-03-10 16:50:01.000000 borgmatic-1.8.9/tests/integration/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3144 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/integration/hooks/test_loki.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13671 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/integration/test_execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.435958 borgmatic-1.8.9/tests/unit/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/unit/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.435958 borgmatic-1.8.9/tests/unit/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:46:46.000000 borgmatic-1.8.9/tests/unit/actions/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.439291 borgmatic-1.8.9/tests/unit/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)     6690 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/config/test_bootstrap.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1305 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      599 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/config/test_validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      390 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      821 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2847 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3049 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9107 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/actions/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      670 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_export_key.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      967 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1074 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2085 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      889 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_json.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2084 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      824 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2609 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1748 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    20005 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1575 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1526 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      630 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/actions/test_transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.439291 borgmatic-1.8.9/tests/unit/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/unit/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12673 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4204 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    46706 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7282 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)   133420 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2075 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9727 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_export_key.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12008 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    22446 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7120 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/borg/test_flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19581 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/borg/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    27870 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12356 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    16640 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    14097 2024-03-11 18:23:53.000000 borgmatic-1.8.9/tests/unit/borg/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    16121 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    23624 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    22531 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1577 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2560 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/borg/test_version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.439291 borgmatic-1.8.9/tests/unit/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/unit/commands/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.439291 borgmatic-1.8.9/tests/unit/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      226 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/commands/completion/test_actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      431 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/commands/completion/test_bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4616 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/commands/completion/test_fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    17204 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    60271 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/commands/test_borgmatic.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.442625 borgmatic-1.8.9/tests/unit/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/unit/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      694 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/config/test_checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8085 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/config/test_collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2068 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/config/test_constants.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3090 2023-12-26 05:49:05.000000 borgmatic-1.8.9/tests/unit/config/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5029 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1587 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/config/test_load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7115 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/config/test_normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5231 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7311 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2024-03-11 20:28:10.445958 borgmatic-1.8.9/tests/unit/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-08-24 17:57:25.000000 borgmatic-1.8.9/tests/unit/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12203 2024-03-10 07:14:05.000000 borgmatic-1.8.9/tests/unit/hooks/test_apprise.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4238 2024-03-08 18:54:55.000000 borgmatic-1.8.9/tests/unit/hooks/test_command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3726 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3162 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4490 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3002 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10229 2024-03-10 01:12:55.000000 borgmatic-1.8.9/tests/unit/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3728 2024-03-10 20:15:32.000000 borgmatic-1.8.9/tests/unit/hooks/test_logs.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3192 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_loki.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    22437 2024-03-03 22:27:48.000000 borgmatic-1.8.9/tests/unit/hooks/test_mariadb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    17395 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/hooks/test_mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    22221 2024-03-03 22:27:48.000000 borgmatic-1.8.9/tests/unit/hooks/test_mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8856 2024-03-11 19:42:01.000000 borgmatic-1.8.9/tests/unit/hooks/test_ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2303 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/hooks/test_pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    39869 2024-01-31 18:42:00.000000 borgmatic-1.8.9/tests/unit/hooks/test_postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7930 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/hooks/test_sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    22253 2024-01-24 22:25:14.000000 borgmatic-1.8.9/tests/unit/test_execute.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    18961 2024-03-04 21:46:28.000000 borgmatic-1.8.9/tests/unit/test_logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1852 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/test_signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1426 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tests/unit/test_verbosity.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      829 2023-12-26 05:59:57.000000 borgmatic-1.8.9/tox.ini
```

### Comparing `borgmatic-1.8.8/.drone.yml` & `borgmatic-1.8.9/tests/end-to-end/docker-compose.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,65 @@
----
-kind: pipeline
-name: python-3-8-alpine-3-13
-
+version: '3'
 services:
-  - name: postgresql
+  postgresql:
     image: docker.io/postgres:13.1-alpine
     environment:
       POSTGRES_PASSWORD: test
       POSTGRES_DB: test
-  - name: postgresql2
+  postgresql2:
     image: docker.io/postgres:13.1-alpine
     environment:
       POSTGRES_PASSWORD: test2
       POSTGRES_DB: test
-    commands:
-      - docker-entrypoint.sh -p 5433
-  - name: mariadb
+    command: docker-entrypoint.sh -p 5433
+  mariadb:
     image: docker.io/mariadb:10.11.4
     environment:
       MARIADB_ROOT_PASSWORD: test
       MARIADB_DATABASE: test
-  - name: mariadb2
+  mariadb2:
     image: docker.io/mariadb:10.11.4
     environment:
       MARIADB_ROOT_PASSWORD: test2
       MARIADB_DATABASE: test
-    commands:
-      - docker-entrypoint.sh --port=3307
-  - name: not-actually-mysql
+    command: docker-entrypoint.sh --port=3307
+  not-actually-mysql:
     image: docker.io/mariadb:10.11.4
     environment:
       MARIADB_ROOT_PASSWORD: test
       MARIADB_DATABASE: test
-  - name: not-actually-mysql2
+  not-actually-mysql2:
     image: docker.io/mariadb:10.11.4
     environment:
       MARIADB_ROOT_PASSWORD: test2
       MARIADB_DATABASE: test
-    commands:
-      - docker-entrypoint.sh --port=3307
-  - name: mongodb
+    command: docker-entrypoint.sh --port=3307
+  mongodb:
     image: docker.io/mongo:5.0.5
     environment:
       MONGO_INITDB_ROOT_USERNAME: root
       MONGO_INITDB_ROOT_PASSWORD: test
-  - name: mongodb2
+  mongodb2:
     image: docker.io/mongo:5.0.5
     environment:
       MONGO_INITDB_ROOT_USERNAME: root2
       MONGO_INITDB_ROOT_PASSWORD: test2
-    commands:
-      - docker-entrypoint.sh --port=27018
-
-clone:
-  skip_verify: true
-
-steps:
-- name: build
-  image: docker.io/alpine:3.13
-  environment:
-    TEST_CONTAINER: true
-  pull: always
-  commands:
-    - scripts/run-full-tests
----
-kind: pipeline
-name: documentation
-type: exec
-
-platform:
-  os: linux
-  arch: amd64
-
-clone:
-  skip_verify: true
-
-steps:
-- name: build
-  environment:
-    USERNAME:
-      from_secret: docker_username
-    PASSWORD:
-      from_secret: docker_password
-    IMAGE_NAME: projects.torsion.org/borgmatic-collective/borgmatic:docs
-  commands:
-    - podman login --username "$USERNAME" --password "$PASSWORD" projects.torsion.org
-    - podman build --tag "$IMAGE_NAME" --file docs/Dockerfile --storage-opt "overlay.mount_program=/usr/bin/fuse-overlayfs" .
-    - podman push "$IMAGE_NAME"
-
-trigger:
-  repo:
-    - borgmatic-collective/borgmatic
-  branch:
-    - main
+    command: docker-entrypoint.sh --port=27018
+  tests:
+    image: docker.io/alpine:3.13
+    environment:
+      TEST_CONTAINER: true
+    volumes:
+      - "../..:/app"
+    tmpfs:
+      - "/app/borgmatic.egg-info"
+      - "/app/build"
+    tty: true
+    working_dir: /app
+    entrypoint: /app/scripts/run-full-tests
+    depends_on:
+      - postgresql
+      - postgresql2
+      - mariadb
+      - mariadb2
+      - mongodb
+      - mongodb2
```

### Comparing `borgmatic-1.8.8/.eleventy.js` & `borgmatic-1.8.9/.eleventy.js`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/.gitea/issue_template/bug_template.yaml` & `borgmatic-1.8.9/.gitea/issue_template/bug_template.yaml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/AUTHORS` & `borgmatic-1.8.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/LICENSE` & `borgmatic-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/NEWS` & `borgmatic-1.8.9/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+1.8.9
+ * #311: Add custom dump/restore command options for MySQL and MariaDB.
+ * #811: Add an "access_token" option to the ntfy monitoring hook for authenticating
+   without username/password.
+ * #827: When the "--json" flag is given, suppress console escape codes so as not to
+   interfere with JSON output.
+ * #829: Fix "--override" values containing deprecated section headers not actually overriding
+   configuration options under deprecated section headers.
+ * #835: Add support for the NO_COLOR environment variable. See the documentation for more
+   information:
+   https://torsion.org/borgmatic/docs/how-to/set-up-backups/#colored-output
+ * #839: Add log sending for the Apprise logging hook, enabled by default. See the documentation for
+   more information:
+   https://torsion.org/borgmatic/docs/how-to/monitor-your-backups/#apprise-hook
+ * #839: Document a potentially breaking shell quoting edge case within error hooks:
+   https://torsion.org/borgmatic/docs/how-to/monitor-your-backups/#error-hooks
+ * #840: When running the "rcreate" action and the repository already exists but with a different
+   encryption mode than requested, error.
+ * Switch from Drone to Gitea Actions for continuous integration.
+ * Rename scripts/run-end-to-end-dev-tests to scripts/run-end-to-end-tests and use it in both dev
+   and CI for better dev-CI parity.
+ * Clarify documentation about restoring a database: borgmatic does not create the database upon
+   restore.
+
 1.8.8
  * #370: For the PostgreSQL hook, pass the "PGSSLMODE" environment variable through to Borg when the
    database's configuration omits the "ssl_mode" option.
  * #818: Allow the "--repository" flag to match across multiple configuration files.
  * #820: Fix broken repository detection in the "rcreate" action with Borg 1.4. The issue did not
    occur with other versions of Borg.
  * #822: Fix broken escaping logic in the PostgreSQL hook's "pg_dump_command" option.
```

### Comparing `borgmatic-1.8.8/PKG-INFO` & `borgmatic-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.8.8
+Version: 1.8.9
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.8.8/README.md` & `borgmatic-1.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,10 +150,7 @@
 [register](https://projects.torsion.org/user/sign_up?invite_code=borgmatic)
 first. We also accept Pull Requests on GitHub, if that's more your thing. In
 general, contributions are very welcome. We don't bite!
 
 Also, please check out the [borgmatic development
 how-to](https://torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/) for
 info on cloning source code, running tests, etc.
-
-<a href="https://build.torsion.org/borgmatic-collective/borgmatic" alt="build status">![Build Status](https://build.torsion.org/api/badges/borgmatic-collective/borgmatic/status.svg?ref=refs/heads/main)</a>
-
```

#### html2text {}

```diff
@@ -50,9 +50,8 @@
 projects.torsion.org/borgmatic-collective/borgmatic/pulls) or open an [issue]
 (https://projects.torsion.org/borgmatic-collective/borgmatic/issues) to discuss
 your idea. Note that you'll need to [register](https://projects.torsion.org/
 user/sign_up?invite_code=borgmatic) first. We also accept Pull Requests on
 GitHub, if that's more your thing. In general, contributions are very welcome.
 We don't bite! Also, please check out the [borgmatic development how-to](https:
 //torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/) for info on cloning
-source code, running tests, etc. _!_[_B_u_i_l_d_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_b_u_i_l_d_._t_o_r_s_i_o_n_._o_r_g_/_a_p_i_/
-_b_a_d_g_e_s_/_b_o_r_g_m_a_t_i_c_-_c_o_l_l_e_c_t_i_v_e_/_b_o_r_g_m_a_t_i_c_/_s_t_a_t_u_s_._s_v_g_?_r_e_f_=_r_e_f_s_/_h_e_a_d_s_/_m_a_i_n_)
+source code, running tests, etc.
```

### Comparing `borgmatic-1.8.8/SECURITY.md` & `borgmatic-1.8.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/borg.py` & `borgmatic-1.8.9/borgmatic/actions/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/break_lock.py` & `borgmatic-1.8.9/borgmatic/actions/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/check.py` & `borgmatic-1.8.9/borgmatic/actions/check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/compact.py` & `borgmatic-1.8.9/borgmatic/actions/compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/config/bootstrap.py` & `borgmatic-1.8.9/borgmatic/actions/config/bootstrap.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/config/generate.py` & `borgmatic-1.8.9/borgmatic/actions/config/generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/config/validate.py` & `borgmatic-1.8.9/borgmatic/actions/config/validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/create.py` & `borgmatic-1.8.9/borgmatic/actions/create.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/export_key.py` & `borgmatic-1.8.9/borgmatic/actions/export_key.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/export_tar.py` & `borgmatic-1.8.9/borgmatic/actions/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/extract.py` & `borgmatic-1.8.9/borgmatic/actions/extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/info.py` & `borgmatic-1.8.9/borgmatic/actions/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/list.py` & `borgmatic-1.8.9/borgmatic/actions/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/mount.py` & `borgmatic-1.8.9/borgmatic/actions/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/prune.py` & `borgmatic-1.8.9/borgmatic/actions/prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/rcreate.py` & `borgmatic-1.8.9/borgmatic/actions/rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/restore.py` & `borgmatic-1.8.9/borgmatic/actions/restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/rinfo.py` & `borgmatic-1.8.9/borgmatic/actions/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/rlist.py` & `borgmatic-1.8.9/borgmatic/actions/rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/actions/transfer.py` & `borgmatic-1.8.9/borgmatic/actions/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/borg.py` & `borgmatic-1.8.9/borgmatic/borg/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/break_lock.py` & `borgmatic-1.8.9/borgmatic/borg/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/check.py` & `borgmatic-1.8.9/borgmatic/borg/check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/compact.py` & `borgmatic-1.8.9/borgmatic/borg/compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/create.py` & `borgmatic-1.8.9/borgmatic/borg/create.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/environment.py` & `borgmatic-1.8.9/borgmatic/borg/environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/export_key.py` & `borgmatic-1.8.9/borgmatic/borg/export_key.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/export_tar.py` & `borgmatic-1.8.9/borgmatic/borg/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/extract.py` & `borgmatic-1.8.9/borgmatic/borg/extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/feature.py` & `borgmatic-1.8.9/borgmatic/borg/feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/flags.py` & `borgmatic-1.8.9/borgmatic/borg/flags.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/info.py` & `borgmatic-1.8.9/borgmatic/borg/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/list.py` & `borgmatic-1.8.9/borgmatic/borg/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/mount.py` & `borgmatic-1.8.9/borgmatic/borg/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/prune.py` & `borgmatic-1.8.9/borgmatic/borg/prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/rcreate.py` & `borgmatic-1.8.9/borgmatic/borg/rcreate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import json
 import logging
 import subprocess
 
 from borgmatic.borg import environment, feature, flags, rinfo
 from borgmatic.execute import DO_NOT_CAPTURE, execute_command
 
 logger = logging.getLogger(__name__)
@@ -27,25 +28,38 @@
     remote_path=None,
 ):
     '''
     Given a dry-run flag, a local or remote repository path, a configuration dict, the local Borg
     version, a Borg encryption mode, the path to another repo whose key material should be reused,
     whether the repository should be append-only, and the storage quota to use, create the
     repository. If the repository already exists, then log and skip creation.
+
+    Raise ValueError if the requested encryption mode does not match that of the repository.
+    Raise json.decoder.JSONDecodeError if the "borg info" JSON outputcannot be decoded.
+    Raise subprocess.CalledProcessError if "borg info" returns an error exit code.
     '''
     try:
-        rinfo.display_repository_info(
-            repository_path,
-            config,
-            local_borg_version,
-            argparse.Namespace(json=True),
-            global_arguments,
-            local_path,
-            remote_path,
+        info_data = json.loads(
+            rinfo.display_repository_info(
+                repository_path,
+                config,
+                local_borg_version,
+                argparse.Namespace(json=True),
+                global_arguments,
+                local_path,
+                remote_path,
+            )
         )
+        repository_encryption_mode = info_data.get('encryption', {}).get('mode')
+
+        if repository_encryption_mode != encryption_mode:
+            raise ValueError(
+                f'Requested encryption mode "{encryption_mode}" does not match existing repository encryption mode "{repository_encryption_mode}"'
+            )
+
         logger.info(f'{repository_path}: Repository already exists. Skipping creation.')
         return
     except subprocess.CalledProcessError as error:
         if error.returncode not in RINFO_REPOSITORY_NOT_FOUND_EXIT_CODES:
             raise
 
     lock_wait = config.get('lock_wait')
```

### Comparing `borgmatic-1.8.8/borgmatic/borg/rinfo.py` & `borgmatic-1.8.9/borgmatic/borg/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/rlist.py` & `borgmatic-1.8.9/borgmatic/borg/rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/transfer.py` & `borgmatic-1.8.9/borgmatic/borg/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/umount.py` & `borgmatic-1.8.9/borgmatic/borg/umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/borg/version.py` & `borgmatic-1.8.9/borgmatic/borg/version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/commands/arguments.py` & `borgmatic-1.8.9/borgmatic/commands/arguments.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/commands/borgmatic.py` & `borgmatic-1.8.9/borgmatic/commands/borgmatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                     error,
                 )
                 encountered_error = error
                 error_repository = repository['path']
 
     try:
         if monitoring_hooks_are_activated:
-            # send logs irrespective of error
+            # Send logs irrespective of error.
             dispatch.call_hooks(
                 'ping_monitor',
                 config,
                 config_filename,
                 monitor.MONITOR_HOOK_NAMES,
                 monitor.State.LOG,
                 monitoring_log_level,
@@ -868,26 +868,25 @@
     configuration_parse_errors = (
         (max(log.levelno for log in parse_logs) >= logging.CRITICAL) if parse_logs else False
     )
 
     any_json_flags = any(
         getattr(sub_arguments, 'json', False) for sub_arguments in arguments.values()
     )
-    colorama.init(
-        autoreset=True,
-        strip=not should_do_markup(global_arguments.no_color or any_json_flags, configs),
-    )
+    color_enabled = should_do_markup(global_arguments.no_color or any_json_flags, configs)
+    colorama.init(autoreset=color_enabled, strip=not color_enabled)
     try:
         configure_logging(
             verbosity_to_log_level(global_arguments.verbosity),
             verbosity_to_log_level(global_arguments.syslog_verbosity),
             verbosity_to_log_level(global_arguments.log_file_verbosity),
             verbosity_to_log_level(global_arguments.monitoring_verbosity),
             global_arguments.log_file,
             global_arguments.log_file_format,
+            color_enabled=color_enabled,
         )
     except (FileNotFoundError, PermissionError) as error:
         configure_logging(logging.CRITICAL)
         logger.critical(f'Error configuring logging: {error}')
         exit_with_help_link()
 
     summary_logs = (
```

### Comparing `borgmatic-1.8.8/borgmatic/commands/completion/actions.py` & `borgmatic-1.8.9/borgmatic/commands/completion/actions.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/commands/completion/bash.py` & `borgmatic-1.8.9/borgmatic/commands/completion/bash.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/commands/completion/fish.py` & `borgmatic-1.8.9/borgmatic/commands/completion/fish.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/collect.py` & `borgmatic-1.8.9/borgmatic/config/collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/constants.py` & `borgmatic-1.8.9/borgmatic/config/constants.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/environment.py` & `borgmatic-1.8.9/borgmatic/config/environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/generate.py` & `borgmatic-1.8.9/borgmatic/config/generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/load.py` & `borgmatic-1.8.9/borgmatic/config/load.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/normalize.py` & `borgmatic-1.8.9/borgmatic/config/normalize.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/config/override.py` & `borgmatic-1.8.9/borgmatic/config/override.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return ()
 
     parsed_overrides = []
 
     for raw_override in raw_overrides:
         try:
             raw_keys, value = raw_override.split('=', 1)
-            keys = strip_section_names(tuple(raw_keys.split('.')))
+            keys = tuple(raw_keys.split('.'))
             option_type = type_for_option(schema, keys)
 
             parsed_overrides.append(
                 (
                     keys,
                     convert_value_type(value, option_type),
                 )
@@ -123,12 +123,17 @@
 
 
 def apply_overrides(config, schema, raw_overrides):
     '''
     Given a configuration dict, a corresponding configuration schema dict, and a sequence of
     configuration file override strings in the form of "option.suboption=value", parse each override
     and set it into the configuration dict.
+
+    Set the overrides into the configuration both with and without deprecated section names (if
+    used), so that the overrides work regardless of whether the configuration is also using
+    deprecated section names.
     '''
     overrides = parse_overrides(raw_overrides, schema)
 
     for keys, value in overrides:
         set_values(config, keys, value)
+        set_values(config, strip_section_names(keys), value)
```

### Comparing `borgmatic-1.8.8/borgmatic/config/schema.yaml` & `borgmatic-1.8.9/borgmatic/config/schema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -967,14 +967,28 @@
                 password:
                     type: string
                     description: |
                         Password with which to connect to the database. Omitting
                         a password will only work if MariaDB is configured to
                         trust the configured username without a password.
                     example: trustsome1
+                mariadb_dump_command:
+                    type: string
+                    description: |
+                        Command to use instead of "mariadb-dump". This can be
+                        used to run a specific mariadb_dump version (e.g., one
+                        inside a running container). Defaults to "mariadb-dump".
+                    example: docker exec mariadb_container mariadb-dump
+                mariadb_command:
+                    type: string
+                    description: |
+                        Command to run instead of "mariadb". This can be used to
+                        run a specific mariadb version (e.g., one inside a
+                        running container). Defaults to "mariadb".
+                    example: docker exec mariadb_container mariadb           
                 restore_password:
                     type: string
                     description: |
                         Password with which to connect to the restore database.
                         Defaults to the "password" option.
                     example: trustsome1
                 format:
@@ -1083,14 +1097,28 @@
                     example: trustsome1
                 restore_password:
                     type: string
                     description: |
                         Password with which to connect to the restore database.
                         Defaults to the "password" option.
                     example: trustsome1
+                mysql_dump_command:
+                    type: string
+                    description: |
+                        Command to use instead of "mysqldump". This can be used
+                        to run a specific mysql_dump version (e.g., one inside a
+                        running container). Defaults to "mysqldump".
+                    example: docker exec mysql_container mysqldump
+                mysql_command:
+                    type: string
+                    description: |
+                        Command to run instead of "mysql". This can be used to
+                        run a specific mysql version (e.g., one inside a running
+                        container). Defaults to "mysql".
+                    example: docker exec mysql_container mysql
                 format:
                     type: string
                     enum: ['sql']
                     description: |
                         Database dump output format. Currently only "sql" is
                         supported. Defaults to "sql" for a single database. Or,
                         when database name is "all" and format is blank, dumps
@@ -1286,14 +1314,20 @@
                     The username used for authentication.
                 example: testuser
             password:
                 type: string
                 description: |
                     The password used for authentication.
                 example: fakepassword
+            access_token:
+                type: string
+                description: |
+                    An ntfy access token to authenticate with instead of
+                    username/password.
+                example: tk_AgQdq7mVBoFD37zQVN29RhuMzNIz2
             start:
                 type: object
                 properties:
                     title:
                         type: string
                         description: |
                             The title of the message.
@@ -1400,14 +1434,27 @@
                     services and their configuration can be found at
                     https://github.com/caronc/apprise/wiki.
                 example:
                     - url: "kodi://user@hostname"
                       label: kodi
                     - url: "line://Token@User"
                       label: line
+            send_logs:
+                type: boolean
+                description: |
+                    Send borgmatic logs to Apprise services as part the
+                    "finish", "fail", and "log" states. Defaults to true.
+                example: false
+            logs_size_limit:
+                type: integer
+                description: |
+                    Number of bytes of borgmatic logs to send to Apprise
+                    services. Set to 0 to send all logs and disable this
+                    truncation. Defaults to 1500.
+                example: 100000
             start:
                 type: object
                 required: ['body']
                 properties:
                     title:
                         type: string
                         description: |
@@ -1445,29 +1492,46 @@
                             title is sent.
                         example: Ping!
                     body:
                         type: string
                         description: |
                             Specify the message body.
                         example: Your backups have failed.
+            log:
+                type: object
+                required: ['body']
+                properties:
+                    title:
+                        type: string
+                        description: |
+                            Specify the message title. If left unspecified, no
+                            title is sent.
+                        example: Ping!
+                    body:
+                        type: string
+                        description: |
+                            Specify the message body.
+                        example: Here is some info about your backups.
             states:
                 type: array
                 items:
                     type: string
                     enum:
                         - start
                         - finish
                         - fail
+                        - log
                     uniqueItems: true
                 description: |
-                    List of one or more monitoring states to ping for: "start",
-                    "finish", and/or "fail". Defaults to pinging for failure
-                    only. For each selected state, corresponding configuration
-                    for the message title and body should be given. If any is
-                    left unspecified, a generic message is emitted instead.
+                    List of one or more monitoring states to ping for:
+                    "start", "finish", "fail", and/or "log". Defaults to
+                    pinging for failure only. For each selected state,
+                    corresponding configuration for the message title and body
+                    should be given. If any is left unspecified, a generic
+                    message is emitted instead.
                 example:
                     - start
                     - finish
 
     healthchecks:
         type: object
         required: ['ping_url']
```

### Comparing `borgmatic-1.8.8/borgmatic/config/validate.py` & `borgmatic-1.8.9/borgmatic/config/validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/execute.py` & `borgmatic-1.8.9/borgmatic/execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/apprise.py` & `borgmatic-1.8.9/borgmatic/hooks/pagerduty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,81 @@
+import datetime
+import json
 import logging
-import operator
+import platform
+
+import requests
+
+from borgmatic.hooks import monitor
 
 logger = logging.getLogger(__name__)
 
+EVENTS_API_URL = 'https://events.pagerduty.com/v2/enqueue'
+
 
 def initialize_monitor(
-    ping_url, config, config_filename, monitoring_log_level, dry_run
+    integration_key, config, config_filename, monitoring_log_level, dry_run
 ):  # pragma: no cover
     '''
     No initialization is necessary for this monitor.
     '''
     pass
 
 
 def ping_monitor(hook_config, config, config_filename, state, monitoring_log_level, dry_run):
     '''
-    Ping the configured Apprise service URLs. Use the given configuration filename in any log
-    entries. If this is a dry run, then don't actually ping anything.
+    If this is an error state, create a PagerDuty event with the configured integration key. Use
+    the given configuration filename in any log entries. If this is a dry run, then don't actually
+    create an event.
     '''
-    try:
-        import apprise
-        from apprise import NotifyFormat, NotifyType
-    except ImportError:  # pragma: no cover
-        logger.warning('Unable to import Apprise in monitoring hook')
+    if state != monitor.State.FAIL:
+        logger.debug(
+            f'{config_filename}: Ignoring unsupported monitoring {state.name.lower()} in PagerDuty hook',
+        )
         return
 
-    state_to_notify_type = {
-        'start': NotifyType.INFO,
-        'finish': NotifyType.SUCCESS,
-        'fail': NotifyType.FAILURE,
-        'log': NotifyType.INFO,
-    }
-
-    run_states = hook_config.get('states', ['fail'])
-
-    if state.name.lower() not in run_states:
-        return
-
-    state_config = hook_config.get(
-        state.name.lower(),
-        {
-            'title': f'A borgmatic {state.name} event happened',
-            'body': f'A borgmatic {state.name} event happened',
-        },
-    )
-
-    if not hook_config.get('services'):
-        logger.info(f'{config_filename}: No Apprise services to ping')
-        return
-
-    dry_run_string = ' (dry run; not actually pinging)' if dry_run else ''
-    labels_string = ', '.join(map(operator.itemgetter('label'), hook_config.get('services')))
-    logger.info(f'{config_filename}: Pinging Apprise services: {labels_string}{dry_run_string}')
-
-    apprise_object = apprise.Apprise()
-    apprise_object.add(list(map(operator.itemgetter('url'), hook_config.get('services'))))
+    dry_run_label = ' (dry run; not actually sending)' if dry_run else ''
+    logger.info(f'{config_filename}: Sending failure event to PagerDuty {dry_run_label}')
 
     if dry_run:
         return
 
-    result = apprise_object.notify(
-        title=state_config.get('title', ''),
-        body=state_config.get('body'),
-        body_format=NotifyFormat.TEXT,
-        notify_type=state_to_notify_type[state.name.lower()],
+    hostname = platform.node()
+    local_timestamp = (
+        datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc).astimezone().isoformat()
+    )
+    payload = json.dumps(
+        {
+            'routing_key': hook_config['integration_key'],
+            'event_action': 'trigger',
+            'payload': {
+                'summary': f'backup failed on {hostname}',
+                'severity': 'error',
+                'source': hostname,
+                'timestamp': local_timestamp,
+                'component': 'borgmatic',
+                'group': 'backups',
+                'class': 'backup failure',
+                'custom_details': {
+                    'hostname': hostname,
+                    'configuration filename': config_filename,
+                    'server time': local_timestamp,
+                },
+            },
+        }
     )
+    logger.debug(f'{config_filename}: Using PagerDuty payload: {payload}')
 
-    if result is False:
-        logger.warning(f'{config_filename}: Error sending some Apprise notifications')
+    logging.getLogger('urllib3').setLevel(logging.ERROR)
+    try:
+        response = requests.post(EVENTS_API_URL, data=payload.encode('utf-8'))
+        if not response.ok:
+            response.raise_for_status()
+    except requests.exceptions.RequestException as error:
+        logger.warning(f'{config_filename}: PagerDuty error: {error}')
 
 
 def destroy_monitor(
     ping_url_or_uuid, config, config_filename, monitoring_log_level, dry_run
 ):  # pragma: no cover
     '''
     No destruction is necessary for this monitor.
```

### Comparing `borgmatic-1.8.8/borgmatic/hooks/command.py` & `borgmatic-1.8.9/borgmatic/hooks/command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/cronhub.py` & `borgmatic-1.8.9/borgmatic/hooks/cronhub.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/cronitor.py` & `borgmatic-1.8.9/borgmatic/hooks/cronitor.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/dispatch.py` & `borgmatic-1.8.9/borgmatic/hooks/dispatch.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/dump.py` & `borgmatic-1.8.9/borgmatic/hooks/dump.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/loki.py` & `borgmatic-1.8.9/borgmatic/hooks/loki.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/mariadb.py` & `borgmatic-1.8.9/borgmatic/hooks/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import logging
 import os
+import shlex
 
 from borgmatic.execute import (
     execute_command,
     execute_command_and_capture_output,
     execute_command_with_processes,
 )
 from borgmatic.hooks import dump
@@ -13,15 +14,15 @@
 
 
 def make_dump_path(config):  # pragma: no cover
     '''
     Make the dump path from the given configuration dict and the name of this hook.
     '''
     return dump.make_data_source_dump_path(
-        config.get('borgmatic_source_directory'), 'mariadb_databases'
+        config.get('borgmatic_source_directory'), 'mysql_databases'
     )
 
 
 SYSTEM_DATABASE_NAMES = ('information_schema', 'mysql', 'performance_schema', 'sys')
 
 
 def database_names_to_dump(database, extra_environment, log_prefix, dry_run):
@@ -31,25 +32,28 @@
     excluding any system databases that will cause problems during restore.
     '''
     if database['name'] != 'all':
         return (database['name'],)
     if dry_run:
         return ()
 
+    mysql_show_command = tuple(
+        shlex.quote(part) for part in shlex.split(database.get('mysql_command') or 'mysql')
+    )
     show_command = (
-        ('mariadb',)
+        mysql_show_command
         + (tuple(database['list_options'].split(' ')) if 'list_options' in database else ())
         + (('--host', database['hostname']) if 'hostname' in database else ())
         + (('--port', str(database['port'])) if 'port' in database else ())
         + (('--protocol', 'tcp') if 'hostname' in database or 'port' in database else ())
         + (('--user', database['username']) if 'username' in database else ())
         + ('--skip-column-names', '--batch')
         + ('--execute', 'show schemas')
     )
-    logger.debug(f'{log_prefix}: Querying for "all" MariaDB databases to dump')
+    logger.debug(f'{log_prefix}: Querying for "all" MySQL databases to dump')
     show_output = execute_command_and_capture_output(
         show_command, extra_environment=extra_environment
     )
 
     return tuple(
         show_name
         for show_name in show_output.strip().splitlines()
@@ -57,47 +61,50 @@
     )
 
 
 def execute_dump_command(
     database, log_prefix, dump_path, database_names, extra_environment, dry_run, dry_run_label
 ):
     '''
-    Kick off a dump for the given MariaDB database (provided as a configuration dict) to a named
-    pipe constructed from the given dump path and database name. Use the given log prefix in any
-    log entries.
+    Kick off a dump for the given MySQL/MariaDB database (provided as a configuration dict) to a
+    named pipe constructed from the given dump path and database name. Use the given log prefix in
+    any log entries.
 
     Return a subprocess.Popen instance for the dump process ready to spew to a named pipe. But if
     this is a dry run, then don't actually dump anything and return None.
     '''
     database_name = database['name']
     dump_filename = dump.make_data_source_dump_filename(
         dump_path, database['name'], database.get('hostname')
     )
 
     if os.path.exists(dump_filename):
         logger.warning(
-            f'{log_prefix}: Skipping duplicate dump of MariaDB database "{database_name}" to {dump_filename}'
+            f'{log_prefix}: Skipping duplicate dump of MySQL database "{database_name}" to {dump_filename}'
         )
         return None
 
+    mysql_dump_command = tuple(
+        shlex.quote(part) for part in shlex.split(database.get('mysql_dump_command') or 'mysqldump')
+    )
     dump_command = (
-        ('mariadb-dump',)
+        mysql_dump_command
         + (tuple(database['options'].split(' ')) if 'options' in database else ())
         + (('--add-drop-database',) if database.get('add_drop_database', True) else ())
         + (('--host', database['hostname']) if 'hostname' in database else ())
         + (('--port', str(database['port'])) if 'port' in database else ())
         + (('--protocol', 'tcp') if 'hostname' in database or 'port' in database else ())
         + (('--user', database['username']) if 'username' in database else ())
         + ('--databases',)
         + database_names
         + ('--result-file', dump_filename)
     )
 
     logger.debug(
-        f'{log_prefix}: Dumping MariaDB database "{database_name}" to {dump_filename}{dry_run_label}'
+        f'{log_prefix}: Dumping MySQL database "{database_name}" to {dump_filename}{dry_run_label}'
     )
     if dry_run:
         return None
 
     dump.create_named_pipe_for_dump(dump_filename)
 
     return execute_command(
@@ -105,39 +112,38 @@
         extra_environment=extra_environment,
         run_to_completion=False,
     )
 
 
 def dump_data_sources(databases, config, log_prefix, dry_run):
     '''
-    Dump the given MariaDB databases to a named pipe. The databases are supplied as a sequence of
-    dicts, one dict describing each database as per the configuration schema. Use the given
-    configuration dict to construct the destination path and the given log prefix in any log
-    entries.
+    Dump the given MySQL/MariaDB databases to a named pipe. The databases are supplied as a sequence
+    of dicts, one dict describing each database as per the configuration schema. Use the given
+    configuration dict to construct the destination path and the given log prefix in any log entries.
 
     Return a sequence of subprocess.Popen instances for the dump processes ready to spew to a named
     pipe. But if this is a dry run, then don't actually dump anything and return an empty sequence.
     '''
     dry_run_label = ' (dry run; not actually dumping anything)' if dry_run else ''
     processes = []
 
-    logger.info(f'{log_prefix}: Dumping MariaDB databases{dry_run_label}')
+    logger.info(f'{log_prefix}: Dumping MySQL databases{dry_run_label}')
 
     for database in databases:
         dump_path = make_dump_path(config)
         extra_environment = {'MYSQL_PWD': database['password']} if 'password' in database else None
         dump_database_names = database_names_to_dump(
             database, extra_environment, log_prefix, dry_run
         )
 
         if not dump_database_names:
             if dry_run:
                 continue
 
-            raise ValueError('Cannot find any MariaDB databases to dump.')
+            raise ValueError('Cannot find any MySQL databases to dump.')
 
         if database['name'] == 'all' and database.get('format'):
             for dump_name in dump_database_names:
                 renamed_database = copy.copy(database)
                 renamed_database['name'] = dump_name
                 processes.append(
                     execute_dump_command(
@@ -168,15 +174,15 @@
 
 def remove_data_source_dumps(databases, config, log_prefix, dry_run):  # pragma: no cover
     '''
     Remove all database dump files for this hook regardless of the given databases. Use the given
     configuration dict to construct the destination path and the log prefix in any log entries. If
     this is a dry run, then don't actually remove anything.
     '''
-    dump.remove_data_source_dumps(make_dump_path(config), 'MariaDB', log_prefix, dry_run)
+    dump.remove_data_source_dumps(make_dump_path(config), 'MySQL', log_prefix, dry_run)
 
 
 def make_data_source_dump_pattern(databases, config, log_prefix, name=None):  # pragma: no cover
     '''
     Given a sequence of configurations dicts, a configuration dict, a prefix to log with, and a
     database name to match, return the corresponding glob patterns to match the database dump in an
     archive.
@@ -204,29 +210,33 @@
     username = connection_params['username'] or data_source.get(
         'restore_username', data_source.get('username')
     )
     password = connection_params['password'] or data_source.get(
         'restore_password', data_source.get('password')
     )
 
+    mysql_restore_command = tuple(
+        shlex.quote(part) for part in shlex.split(data_source.get('mysql_command') or 'mysql')
+    )
     restore_command = (
-        ('mariadb', '--batch')
+        mysql_restore_command
+        + ('--batch',)
         + (
             tuple(data_source['restore_options'].split(' '))
             if 'restore_options' in data_source
             else ()
         )
         + (('--host', hostname) if hostname else ())
         + (('--port', str(port)) if port else ())
         + (('--protocol', 'tcp') if hostname or port else ())
         + (('--user', username) if username else ())
     )
     extra_environment = {'MYSQL_PWD': password} if password else None
 
-    logger.debug(f"{log_prefix}: Restoring MariaDB database {data_source['name']}{dry_run_label}")
+    logger.debug(f"{log_prefix}: Restoring MySQL database {data_source['name']}{dry_run_label}")
     if dry_run:
         return
 
     # Don't give Borg local path so as to error on warnings, as "borg extract" only gives a warning
     # if the restore paths don't exist in the archive.
     execute_command_with_processes(
         restore_command,
```

### Comparing `borgmatic-1.8.8/borgmatic/hooks/mongodb.py` & `borgmatic-1.8.9/borgmatic/hooks/mongodb.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/mysql.py` & `borgmatic-1.8.9/borgmatic/hooks/mariadb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import logging
 import os
+import shlex
 
 from borgmatic.execute import (
     execute_command,
     execute_command_and_capture_output,
     execute_command_with_processes,
 )
 from borgmatic.hooks import dump
@@ -13,15 +14,15 @@
 
 
 def make_dump_path(config):  # pragma: no cover
     '''
     Make the dump path from the given configuration dict and the name of this hook.
     '''
     return dump.make_data_source_dump_path(
-        config.get('borgmatic_source_directory'), 'mysql_databases'
+        config.get('borgmatic_source_directory'), 'mariadb_databases'
     )
 
 
 SYSTEM_DATABASE_NAMES = ('information_schema', 'mysql', 'performance_schema', 'sys')
 
 
 def database_names_to_dump(database, extra_environment, log_prefix, dry_run):
@@ -31,25 +32,28 @@
     excluding any system databases that will cause problems during restore.
     '''
     if database['name'] != 'all':
         return (database['name'],)
     if dry_run:
         return ()
 
+    mariadb_show_command = tuple(
+        shlex.quote(part) for part in shlex.split(database.get('mariadb_command') or 'mariadb')
+    )
     show_command = (
-        ('mysql',)
+        mariadb_show_command
         + (tuple(database['list_options'].split(' ')) if 'list_options' in database else ())
         + (('--host', database['hostname']) if 'hostname' in database else ())
         + (('--port', str(database['port'])) if 'port' in database else ())
         + (('--protocol', 'tcp') if 'hostname' in database or 'port' in database else ())
         + (('--user', database['username']) if 'username' in database else ())
         + ('--skip-column-names', '--batch')
         + ('--execute', 'show schemas')
     )
-    logger.debug(f'{log_prefix}: Querying for "all" MySQL databases to dump')
+    logger.debug(f'{log_prefix}: Querying for "all" MariaDB databases to dump')
     show_output = execute_command_and_capture_output(
         show_command, extra_environment=extra_environment
     )
 
     return tuple(
         show_name
         for show_name in show_output.strip().splitlines()
@@ -57,47 +61,51 @@
     )
 
 
 def execute_dump_command(
     database, log_prefix, dump_path, database_names, extra_environment, dry_run, dry_run_label
 ):
     '''
-    Kick off a dump for the given MySQL/MariaDB database (provided as a configuration dict) to a
-    named pipe constructed from the given dump path and database name. Use the given log prefix in
-    any log entries.
+    Kick off a dump for the given MariaDB database (provided as a configuration dict) to a named
+    pipe constructed from the given dump path and database name. Use the given log prefix in any
+    log entries.
 
     Return a subprocess.Popen instance for the dump process ready to spew to a named pipe. But if
     this is a dry run, then don't actually dump anything and return None.
     '''
     database_name = database['name']
     dump_filename = dump.make_data_source_dump_filename(
         dump_path, database['name'], database.get('hostname')
     )
 
     if os.path.exists(dump_filename):
         logger.warning(
-            f'{log_prefix}: Skipping duplicate dump of MySQL database "{database_name}" to {dump_filename}'
+            f'{log_prefix}: Skipping duplicate dump of MariaDB database "{database_name}" to {dump_filename}'
         )
         return None
 
+    mariadb_dump_command = tuple(
+        shlex.quote(part)
+        for part in shlex.split(database.get('mariadb_dump_command') or 'mariadb-dump')
+    )
     dump_command = (
-        ('mysqldump',)
+        mariadb_dump_command
         + (tuple(database['options'].split(' ')) if 'options' in database else ())
         + (('--add-drop-database',) if database.get('add_drop_database', True) else ())
         + (('--host', database['hostname']) if 'hostname' in database else ())
         + (('--port', str(database['port'])) if 'port' in database else ())
         + (('--protocol', 'tcp') if 'hostname' in database or 'port' in database else ())
         + (('--user', database['username']) if 'username' in database else ())
         + ('--databases',)
         + database_names
         + ('--result-file', dump_filename)
     )
 
     logger.debug(
-        f'{log_prefix}: Dumping MySQL database "{database_name}" to {dump_filename}{dry_run_label}'
+        f'{log_prefix}: Dumping MariaDB database "{database_name}" to {dump_filename}{dry_run_label}'
     )
     if dry_run:
         return None
 
     dump.create_named_pipe_for_dump(dump_filename)
 
     return execute_command(
@@ -105,38 +113,39 @@
         extra_environment=extra_environment,
         run_to_completion=False,
     )
 
 
 def dump_data_sources(databases, config, log_prefix, dry_run):
     '''
-    Dump the given MySQL/MariaDB databases to a named pipe. The databases are supplied as a sequence
-    of dicts, one dict describing each database as per the configuration schema. Use the given
-    configuration dict to construct the destination path and the given log prefix in any log entries.
+    Dump the given MariaDB databases to a named pipe. The databases are supplied as a sequence of
+    dicts, one dict describing each database as per the configuration schema. Use the given
+    configuration dict to construct the destination path and the given log prefix in any log
+    entries.
 
     Return a sequence of subprocess.Popen instances for the dump processes ready to spew to a named
     pipe. But if this is a dry run, then don't actually dump anything and return an empty sequence.
     '''
     dry_run_label = ' (dry run; not actually dumping anything)' if dry_run else ''
     processes = []
 
-    logger.info(f'{log_prefix}: Dumping MySQL databases{dry_run_label}')
+    logger.info(f'{log_prefix}: Dumping MariaDB databases{dry_run_label}')
 
     for database in databases:
         dump_path = make_dump_path(config)
         extra_environment = {'MYSQL_PWD': database['password']} if 'password' in database else None
         dump_database_names = database_names_to_dump(
             database, extra_environment, log_prefix, dry_run
         )
 
         if not dump_database_names:
             if dry_run:
                 continue
 
-            raise ValueError('Cannot find any MySQL databases to dump.')
+            raise ValueError('Cannot find any MariaDB databases to dump.')
 
         if database['name'] == 'all' and database.get('format'):
             for dump_name in dump_database_names:
                 renamed_database = copy.copy(database)
                 renamed_database['name'] = dump_name
                 processes.append(
                     execute_dump_command(
@@ -167,15 +176,15 @@
 
 def remove_data_source_dumps(databases, config, log_prefix, dry_run):  # pragma: no cover
     '''
     Remove all database dump files for this hook regardless of the given databases. Use the given
     configuration dict to construct the destination path and the log prefix in any log entries. If
     this is a dry run, then don't actually remove anything.
     '''
-    dump.remove_data_source_dumps(make_dump_path(config), 'MySQL', log_prefix, dry_run)
+    dump.remove_data_source_dumps(make_dump_path(config), 'MariaDB', log_prefix, dry_run)
 
 
 def make_data_source_dump_pattern(databases, config, log_prefix, name=None):  # pragma: no cover
     '''
     Given a sequence of configurations dicts, a configuration dict, a prefix to log with, and a
     database name to match, return the corresponding glob patterns to match the database dump in an
     archive.
@@ -203,29 +212,33 @@
     username = connection_params['username'] or data_source.get(
         'restore_username', data_source.get('username')
     )
     password = connection_params['password'] or data_source.get(
         'restore_password', data_source.get('password')
     )
 
+    mariadb_restore_command = tuple(
+        shlex.quote(part) for part in shlex.split(data_source.get('mariadb_command') or 'mariadb')
+    )
     restore_command = (
-        ('mysql', '--batch')
+        mariadb_restore_command
+        + ('--batch',)
         + (
             tuple(data_source['restore_options'].split(' '))
             if 'restore_options' in data_source
             else ()
         )
         + (('--host', hostname) if hostname else ())
         + (('--port', str(port)) if port else ())
         + (('--protocol', 'tcp') if hostname or port else ())
         + (('--user', username) if username else ())
     )
     extra_environment = {'MYSQL_PWD': password} if password else None
 
-    logger.debug(f"{log_prefix}: Restoring MySQL database {data_source['name']}{dry_run_label}")
+    logger.debug(f"{log_prefix}: Restoring MariaDB database {data_source['name']}{dry_run_label}")
     if dry_run:
         return
 
     # Don't give Borg local path so as to error on warnings, as "borg extract" only gives a warning
     # if the restore paths don't exist in the archive.
     execute_command_with_processes(
         restore_command,
```

### Comparing `borgmatic-1.8.8/borgmatic/hooks/ntfy.py` & `borgmatic-1.8.9/borgmatic/hooks/ntfy.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,17 +46,24 @@
             'X-Message': state_config.get('message'),
             'X-Priority': state_config.get('priority'),
             'X-Tags': state_config.get('tags'),
         }
 
         username = hook_config.get('username')
         password = hook_config.get('password')
-
+        access_token = hook_config.get('access_token')
         auth = None
-        if (username and password) is not None:
+
+        if access_token is not None:
+            if username or password:
+                logger.warning(
+                    f'{config_filename}: ntfy access_token is set but so is username/password, only using access_token'
+                )
+            auth = requests.auth.HTTPBasicAuth('', access_token)
+        elif (username and password) is not None:
             auth = requests.auth.HTTPBasicAuth(username, password)
             logger.info(f'{config_filename}: Using basic auth with user {username} for ntfy')
         elif username is not None:
             logger.warning(
                 f'{config_filename}: Password missing for ntfy authentication, defaulting to no auth'
             )
         elif password is not None:
```

### Comparing `borgmatic-1.8.8/borgmatic/hooks/pagerduty.py` & `borgmatic-1.8.9/borgmatic/hooks/healthchecks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-import datetime
-import json
 import logging
-import platform
 
 import requests
 
+import borgmatic.hooks.logs
 from borgmatic.hooks import monitor
 
 logger = logging.getLogger(__name__)
 
-EVENTS_API_URL = 'https://events.pagerduty.com/v2/enqueue'
+MONITOR_STATE_TO_HEALTHCHECKS = {
+    monitor.State.START: 'start',
+    monitor.State.FINISH: None,  # Healthchecks doesn't append to the URL for the finished state.
+    monitor.State.FAIL: 'fail',
+    monitor.State.LOG: 'log',
+}
 
+DEFAULT_PING_BODY_LIMIT_BYTES = 1500
+HANDLER_IDENTIFIER = 'healthchecks'
 
-def initialize_monitor(
-    integration_key, config, config_filename, monitoring_log_level, dry_run
-):  # pragma: no cover
+
+def initialize_monitor(hook_config, config, config_filename, monitoring_log_level, dry_run):
     '''
-    No initialization is necessary for this monitor.
+    Add a handler to the root logger that stores in memory the most recent logs emitted. That way,
+    we can send them all to Healthchecks upon a finish or failure state. But skip this if the
+    "send_logs" option is false.
     '''
-    pass
+    if hook_config.get('send_logs') is False:
+        return
 
+    ping_body_limit = max(
+        hook_config.get('ping_body_limit', DEFAULT_PING_BODY_LIMIT_BYTES)
+        - len(borgmatic.hooks.logs.PAYLOAD_TRUNCATION_INDICATOR),
+        0,
+    )
 
-def ping_monitor(hook_config, config, config_filename, state, monitoring_log_level, dry_run):
-    '''
-    If this is an error state, create a PagerDuty event with the configured integration key. Use
-    the given configuration filename in any log entries. If this is a dry run, then don't actually
-    create an event.
-    '''
-    if state != monitor.State.FAIL:
-        logger.debug(
-            f'{config_filename}: Ignoring unsupported monitoring {state.name.lower()} in PagerDuty hook',
+    borgmatic.hooks.logs.add_handler(
+        borgmatic.hooks.logs.Forgetful_buffering_handler(
+            HANDLER_IDENTIFIER, ping_body_limit, monitoring_log_level
         )
-        return
+    )
 
-    dry_run_label = ' (dry run; not actually sending)' if dry_run else ''
-    logger.info(f'{config_filename}: Sending failure event to PagerDuty {dry_run_label}')
 
-    if dry_run:
-        return
-
-    hostname = platform.node()
-    local_timestamp = (
-        datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc).astimezone().isoformat()
-    )
-    payload = json.dumps(
-        {
-            'routing_key': hook_config['integration_key'],
-            'event_action': 'trigger',
-            'payload': {
-                'summary': f'backup failed on {hostname}',
-                'severity': 'error',
-                'source': hostname,
-                'timestamp': local_timestamp,
-                'component': 'borgmatic',
-                'group': 'backups',
-                'class': 'backup failure',
-                'custom_details': {
-                    'hostname': hostname,
-                    'configuration filename': config_filename,
-                    'server time': local_timestamp,
-                },
-            },
-        }
+def ping_monitor(hook_config, config, config_filename, state, monitoring_log_level, dry_run):
+    '''
+    Ping the configured Healthchecks URL or UUID, modified with the monitor.State. Use the given
+    configuration filename in any log entries, and log to Healthchecks with the giving log level.
+    If this is a dry run, then don't actually ping anything.
+    '''
+    ping_url = (
+        hook_config['ping_url']
+        if hook_config['ping_url'].startswith('http')
+        else f"https://hc-ping.com/{hook_config['ping_url']}"
     )
-    logger.debug(f'{config_filename}: Using PagerDuty payload: {payload}')
+    dry_run_label = ' (dry run; not actually pinging)' if dry_run else ''
+
+    if 'states' in hook_config and state.name.lower() not in hook_config['states']:
+        logger.info(
+            f'{config_filename}: Skipping Healthchecks {state.name.lower()} ping due to configured states'
+        )
+        return
 
-    logging.getLogger('urllib3').setLevel(logging.ERROR)
-    try:
-        response = requests.post(EVENTS_API_URL, data=payload.encode('utf-8'))
-        if not response.ok:
-            response.raise_for_status()
-    except requests.exceptions.RequestException as error:
-        logger.warning(f'{config_filename}: PagerDuty error: {error}')
+    healthchecks_state = MONITOR_STATE_TO_HEALTHCHECKS.get(state)
+    if healthchecks_state:
+        ping_url = f'{ping_url}/{healthchecks_state}'
+
+    logger.info(f'{config_filename}: Pinging Healthchecks {state.name.lower()}{dry_run_label}')
+    logger.debug(f'{config_filename}: Using Healthchecks ping URL {ping_url}')
+
+    if state in (monitor.State.FINISH, monitor.State.FAIL, monitor.State.LOG):
+        payload = borgmatic.hooks.logs.format_buffered_logs_for_payload(HANDLER_IDENTIFIER)
+    else:
+        payload = ''
+
+    if not dry_run:
+        logging.getLogger('urllib3').setLevel(logging.ERROR)
+        try:
+            response = requests.post(
+                ping_url, data=payload.encode('utf-8'), verify=hook_config.get('verify_tls', True)
+            )
+            if not response.ok:
+                response.raise_for_status()
+        except requests.exceptions.RequestException as error:
+            logger.warning(f'{config_filename}: Healthchecks error: {error}')
 
 
-def destroy_monitor(
-    ping_url_or_uuid, config, config_filename, monitoring_log_level, dry_run
-):  # pragma: no cover
+def destroy_monitor(hook_config, config, config_filename, monitoring_log_level, dry_run):
     '''
-    No destruction is necessary for this monitor.
+    Remove the monitor handler that was added to the root logger. This prevents the handler from
+    getting reused by other instances of this monitor.
     '''
-    pass
+    borgmatic.hooks.logs.remove_handler(HANDLER_IDENTIFIER)
```

### Comparing `borgmatic-1.8.8/borgmatic/hooks/postgresql.py` & `borgmatic-1.8.9/borgmatic/hooks/postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/hooks/sqlite.py` & `borgmatic-1.8.9/borgmatic/hooks/sqlite.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/logger.py` & `borgmatic-1.8.9/borgmatic/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     '''
     if no_color:
         return False
 
     if any(config.get('output', {}).get('color') is False for config in configs.values()):
         return False
 
+    no_color_env = os.environ.get('NO_COLOR', None)
+    if no_color_env is not None:
+        return False
+
     py_colors = os.environ.get('PY_COLORS', None)
 
     if py_colors is not None:
         return to_bool(py_colors)
 
     return interactive_console()
 
@@ -155,18 +159,19 @@
 def configure_logging(
     console_log_level,
     syslog_log_level=None,
     log_file_log_level=None,
     monitoring_log_level=None,
     log_file=None,
     log_file_format=None,
+    color_enabled=True,
 ):
     '''
     Configure logging to go to both the console and (syslog or log file). Use the given log levels,
-    respectively.
+    respectively. If color is enabled, set up log formatting accordingly.
 
     Raise FileNotFoundError or PermissionError if the log file could not be opened for writing.
     '''
     add_custom_log_levels()
 
     if syslog_log_level is None:
         syslog_log_level = logging.DISABLED
@@ -187,15 +192,18 @@
             logging.ERROR: console_error_handler,
             logging.WARN: console_error_handler,
             logging.ANSWER: console_standard_handler,
             logging.INFO: console_standard_handler,
             logging.DEBUG: console_standard_handler,
         }
     )
-    console_handler.setFormatter(Console_color_formatter())
+
+    if color_enabled:
+        console_handler.setFormatter(Console_color_formatter())
+
     console_handler.setLevel(console_log_level)
 
     handlers = [console_handler]
 
     if syslog_log_level != logging.DISABLED:
         syslog_path = None
```

### Comparing `borgmatic-1.8.8/borgmatic/signals.py` & `borgmatic-1.8.9/borgmatic/signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic/verbosity.py` & `borgmatic-1.8.9/borgmatic/verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/borgmatic.egg-info/PKG-INFO` & `borgmatic-1.8.9/borgmatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.8.8
+Version: 1.8.9
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.8.8/borgmatic.egg-info/SOURCES.txt` & `borgmatic-1.8.9/borgmatic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .dockerignore
-.drone.yml
 .eleventy.js
 .flake8
 .gitignore
 AUTHORS
 LICENSE
 MANIFEST.in
 NEWS
@@ -13,14 +12,15 @@
 setup.cfg
 setup.py
 test_requirements.txt
 tox.ini
 .gitea/issue_template/bug_template.yaml
 .gitea/issue_template/config.yaml
 .gitea/issue_template/feature_template.yaml
+.gitea/workflows/build.yaml
 borgmatic/__init__.py
 borgmatic/execute.py
 borgmatic/logger.py
 borgmatic/signals.py
 borgmatic/verbosity.py
 borgmatic.egg-info/PKG-INFO
 borgmatic.egg-info/SOURCES.txt
@@ -99,14 +99,15 @@
 borgmatic/hooks/apprise.py
 borgmatic/hooks/command.py
 borgmatic/hooks/cronhub.py
 borgmatic/hooks/cronitor.py
 borgmatic/hooks/dispatch.py
 borgmatic/hooks/dump.py
 borgmatic/hooks/healthchecks.py
+borgmatic/hooks/logs.py
 borgmatic/hooks/loki.py
 borgmatic/hooks/mariadb.py
 borgmatic/hooks/mongodb.py
 borgmatic/hooks/monitor.py
 borgmatic/hooks/mysql.py
 borgmatic/hooks/ntfy.py
 borgmatic/hooks/pagerduty.py
@@ -172,23 +173,22 @@
 sample/systemd/borgmatic-user.timer
 sample/systemd/borgmatic.service
 sample/systemd/borgmatic.timer
 scripts/dev-docs
 scripts/find-unsupported-borg-options
 scripts/push
 scripts/release
-scripts/run-end-to-end-dev-tests
+scripts/run-end-to-end-tests
 scripts/run-full-tests
 tests/__init__.py
 tests/end-to-end/__init__.py
 tests/end-to-end/docker-compose.yaml
 tests/end-to-end/test_borgmatic.py
 tests/end-to-end/test_completion.py
 tests/end-to-end/test_database.py
-tests/end-to-end/test_dev_parity_with_build_server.py
 tests/end-to-end/test_generate_config.py
 tests/end-to-end/test_invalid_flag.py
 tests/end-to-end/test_override.py
 tests/end-to-end/test_validate_config.py
 tests/integration/__init__.py
 tests/integration/test_execute.py
 tests/integration/actions/__init__.py
@@ -207,14 +207,15 @@
 tests/integration/commands/completion/test_fish.py
 tests/integration/config/__init__.py
 tests/integration/config/test_generate.py
 tests/integration/config/test_load.py
 tests/integration/config/test_override.py
 tests/integration/config/test_schema.py
 tests/integration/config/test_validate.py
+tests/integration/hooks/test_apprise.py
 tests/integration/hooks/test_healthchecks.py
 tests/integration/hooks/test_loki.py
 tests/unit/__init__.py
 tests/unit/test_execute.py
 tests/unit/test_logger.py
 tests/unit/test_signals.py
 tests/unit/test_verbosity.py
@@ -283,14 +284,15 @@
 tests/unit/hooks/test_apprise.py
 tests/unit/hooks/test_command.py
 tests/unit/hooks/test_cronhub.py
 tests/unit/hooks/test_cronitor.py
 tests/unit/hooks/test_dispatch.py
 tests/unit/hooks/test_dump.py
 tests/unit/hooks/test_healthchecks.py
+tests/unit/hooks/test_logs.py
 tests/unit/hooks/test_loki.py
 tests/unit/hooks/test_mariadb.py
 tests/unit/hooks/test_mongodb.py
 tests/unit/hooks/test_mysql.py
 tests/unit/hooks/test_ntfy.py
 tests/unit/hooks/test_pagerduty.py
 tests/unit/hooks/test_postgresql.py
```

### Comparing `borgmatic-1.8.8/docs/Dockerfile` & `borgmatic-1.8.9/docs/Dockerfile`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/README.md` & `borgmatic-1.8.9/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,10 +150,7 @@
 [register](https://projects.torsion.org/user/sign_up?invite_code=borgmatic)
 first. We also accept Pull Requests on GitHub, if that's more your thing. In
 general, contributions are very welcome. We don't bite!
 
 Also, please check out the [borgmatic development
 how-to](https://torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/) for
 info on cloning source code, running tests, etc.
-
-<a href="https://build.torsion.org/borgmatic-collective/borgmatic" alt="build status">![Build Status](https://build.torsion.org/api/badges/borgmatic-collective/borgmatic/status.svg?ref=refs/heads/main)</a>
-
```

#### html2text {}

```diff
@@ -50,9 +50,8 @@
 projects.torsion.org/borgmatic-collective/borgmatic/pulls) or open an [issue]
 (https://projects.torsion.org/borgmatic-collective/borgmatic/issues) to discuss
 your idea. Note that you'll need to [register](https://projects.torsion.org/
 user/sign_up?invite_code=borgmatic) first. We also accept Pull Requests on
 GitHub, if that's more your thing. In general, contributions are very welcome.
 We don't bite! Also, please check out the [borgmatic development how-to](https:
 //torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/) for info on cloning
-source code, running tests, etc. _!_[_B_u_i_l_d_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_b_u_i_l_d_._t_o_r_s_i_o_n_._o_r_g_/_a_p_i_/
-_b_a_d_g_e_s_/_b_o_r_g_m_a_t_i_c_-_c_o_l_l_e_c_t_i_v_e_/_b_o_r_g_m_a_t_i_c_/_s_t_a_t_u_s_._s_v_g_?_r_e_f_=_r_e_f_s_/_h_e_a_d_s_/_m_a_i_n_)
+source code, running tests, etc.
```

### Comparing `borgmatic-1.8.8/docs/SECURITY.md` & `borgmatic-1.8.9/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/components/info-blocks.css` & `borgmatic-1.8.9/docs/_includes/components/info-blocks.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/components/lists.css` & `borgmatic-1.8.9/docs/_includes/components/lists.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/components/minilink.css` & `borgmatic-1.8.9/docs/_includes/components/minilink.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/components/toc.css` & `borgmatic-1.8.9/docs/_includes/components/toc.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/index.css` & `borgmatic-1.8.9/docs/_includes/index.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/layouts/base.njk` & `borgmatic-1.8.9/docs/_includes/layouts/base.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/layouts/main.njk` & `borgmatic-1.8.9/docs/_includes/layouts/main.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/_includes/prism-theme.css` & `borgmatic-1.8.9/docs/_includes/prism-theme.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md` & `borgmatic-1.8.9/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md` & `borgmatic-1.8.9/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/backup-your-databases.md` & `borgmatic-1.8.9/docs/how-to/backup-your-databases.md`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,18 @@
 cleanup hooks as a work-around with other database systems. Also, please [file
 a ticket](https://torsion.org/borgmatic/#issues) for additional database
 systems that you'd like supported.
 
 
 ## Database restoration
 
+When you want to replace an existing database with its backed-up contents, you
+can restore it with borgmatic. Note that the database must already exist;
+borgmatic does not currently create a database upon restore.
+
 To restore a database dump from an archive, use the `borgmatic restore`
 action. But the first step is to figure out which archive to restore from. A
 good way to do that is to use the `rlist` action:
 
 ```bash
 borgmatic rlist
 ```
```

### Comparing `borgmatic-1.8.8/docs/how-to/customize-warnings-and-errors.md` & `borgmatic-1.8.9/docs/how-to/customize-warnings-and-errors.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/deal-with-very-large-backups.md` & `borgmatic-1.8.9/docs/how-to/deal-with-very-large-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/develop-on-borgmatic.md` & `borgmatic-1.8.9/docs/how-to/develop-on-borgmatic.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,22 @@
 
 ```bash
 cd borgmatic
 pipx ensurepath
 pipx install --editable .
 ```
 
+Or to work on the [Apprise
+hook](https://torsion.org/borgmatic/docs/how-to/monitor-your-backups/#apprise-hook),
+change that last line to:
+
+```bash
+pipx install --editable .[Apprise]
+```
+
 To get oriented with the borgmatic source code, have a look at the [source
 code reference](https://torsion.org/borgmatic/docs/reference/source-code/).
 
 
 ## Automated tests
 
 Assuming you've cloned the borgmatic source code as described above and you're
@@ -88,22 +96,22 @@
 ### End-to-end tests
 
 borgmatic additionally includes some end-to-end tests that integration test
 with Borg and supported databases for a few representative scenarios. These
 tests don't run by default when running `tox`, because they're relatively slow
 and depend on containers for runtime dependencies. These tests do run on the
 continuous integration (CI) server, and running them on your developer machine
-is the closest thing to CI-test parity.
+is the closest thing to dev-CI parity.
 
 If you would like to run the full test suite, first install Docker (or Podman;
 see below) and [Docker Compose](https://docs.docker.com/compose/install/).
 Then run:
 
 ```bash
-scripts/run-end-to-end-dev-tests
+scripts/run-end-to-end-tests
 ```
 
 This script assumes you have permission to run `docker`. If you don't, then
 you may need to run with `sudo`.
 
 
 #### Podman
@@ -137,27 +145,35 @@
  * For strings, prefer single quotes over double quotes.
  * Limit all lines to a maximum of 100 characters.
  * Use trailing commas within multiline values or argument lists.
  * For multiline constructs, put opening and closing delimiters on lines
    separate from their contents.
  * Within multiline constructs, use standard four-space indentation. Don't align
    indentation with an opening delimiter.
+ * In general, spell out words in variable names instead of shortening them.
+   So, think `index` instead of `idx`. There are some notable exceptions to
+   this though (like `config`).
 
 borgmatic code uses the [Black](https://black.readthedocs.io/en/stable/) code
 formatter, the [Flake8](http://flake8.pycqa.org/en/latest/) code checker, and
 the [isort](https://github.com/timothycrosley/isort) import orderer, so
 certain code style requirements will be enforced when running automated tests.
 See the Black, Flake8, and isort documentation for more information.
 
+
 ## Continuous integration
 
-Each pull request triggers a continuous integration build which runs the test
-suite. You can view these builds on
-[build.torsion.org](https://build.torsion.org/borgmatic-collective/borgmatic),
-and they're also linked from the commits list on each pull request.
+Each commit to
+[main](https://projects.torsion.org/borgmatic-collective/borgmatic/branches)
+triggers [a continuous integration
+build](https://projects.torsion.org/borgmatic-collective/borgmatic/actions)
+which runs the test suite and updates
+[documentation](https://torsion.org/borgmatic/). These builds are also linked
+from the [commits for the main
+branch](https://projects.torsion.org/borgmatic-collective/borgmatic/commits/branch/main).
 
 ## Documentation development
 
 Updates to borgmatic's documentation are welcome. It's formatted in Markdown
 and located in the `docs/` directory in borgmatic's source, plus the
 `README.md` file at the root.
```

### Comparing `borgmatic-1.8.8/docs/how-to/extract-a-backup.md` & `borgmatic-1.8.9/docs/how-to/extract-a-backup.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/inspect-your-backups.md` & `borgmatic-1.8.9/docs/how-to/inspect-your-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/make-backups-redundant.md` & `borgmatic-1.8.9/docs/how-to/make-backups-redundant.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/make-per-application-backups.md` & `borgmatic-1.8.9/docs/how-to/make-per-application-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/monitor-your-backups.md` & `borgmatic-1.8.9/docs/how-to/monitor-your-backups.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 The `on_error` hook supports interpolating particular runtime variables into
 the hook command. Here's an example that assumes you provide a separate shell
 script to handle the alerting:
 
 ```yaml
 on_error:
-    - send-text-message.sh "{configuration_filename}" "{repository}"
+    - send-text-message.sh {configuration_filename} {repository}
 ```
 
 In this example, when the error occurs, borgmatic interpolates runtime values
 into the hook command: the borgmatic configuration filename and the path of
 the repository. Here's the full set of supported variables you can use here:
 
  * `configuration_filename`: borgmatic configuration filename in which the
@@ -120,14 +120,35 @@
 `compact`, or `check` actions/hooks in which an error occurs and not other
 actions. borgmatic does not run `on_error` hooks if an error occurs within a
 `before_everything` or `after_everything` hook. For more about hooks, see the
 [borgmatic hooks
 documentation](https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/),
 especially the security information.
 
+<span class="minilink minilink-addedin">New in version 1.8.7</span> borgmatic
+automatically escapes these interpolated values to prevent shell injection
+attacks. One implication of this change is that you shouldn't wrap the
+interpolated values in your own quotes, as that will interfere with the
+quoting performed by borgmatic and result in your command receiving incorrect
+arguments. For instance, this won't work:
+
+
+```yaml
+on_error:
+    # Don't do this! It won't work, as the {error} value is already quoted.
+    - send-text-message.sh "Uh oh: {error}"
+```
+
+Do this instead:
+
+```yaml
+on_error:
+    - send-text-message.sh {error}
+```
+
 
 ## Healthchecks hook
 
 [Healthchecks](https://healthchecks.io/) is a service that provides "instant
 alerts when your cron jobs fail silently," and borgmatic has built-in
 integration with it. Once you create a Healthchecks account and project on
 their site, all you need to do is configure borgmatic with the unique "Ping
@@ -145,15 +166,15 @@
 With this configuration, borgmatic pings your Healthchecks project when a
 backup begins, ends, or errors, but only when any of the `create`, `prune`,
 `compact`, or `check` actions are run.
 
 Then, if the actions complete successfully, borgmatic notifies Healthchecks of
 the success and includes borgmatic logs in the payload data sent to
 Healthchecks. This means that borgmatic logs show up in the Healthchecks UI,
-although be aware that Healthchecks currently has a 10-kilobyte limit for the
+although be aware that Healthchecks currently has a 100-kilobyte limit for the
 logs in each ping.
 
 If an error occurs during any action or hook, borgmatic notifies Healthchecks,
 also tacking on logs including the error itself. But the logs are only
 included for errors that occur when a `create`, `prune`, `compact`, or `check`
 action is run.
 
@@ -273,30 +294,30 @@
 [ntfy](https://ntfy.sh) is a free, simple, service (either hosted or
 self-hosted) which offers simple pub/sub push notifications to multiple
 platforms including [web](https://ntfy.sh/stats),
 [Android](https://play.google.com/store/apps/details?id=io.heckel.ntfy) and
 [iOS](https://apps.apple.com/us/app/ntfy/id1625396347).
 
 Since push notifications for regular events might soon become quite annoying,
-this hook only fires on any errors by default in order to instantly alert you to issues.
-The `states` list can override this.
-
-As ntfy is unauthenticated, it isn't a suitable channel for any private information
-so the default messages are intentionally generic. These can be overridden, depending
-on your risk assessment. Each `state` can have its own custom messages, priorities and tags
-or, if none are provided, will use the default.
+this hook only fires on any errors by default in order to instantly alert you
+to issues. The `states` list can override this. Each state can have its own
+custom messages, priorities and tags or, if none are provided, will use the
+default.
 
-An example configuration is shown here, with all the available options, including
-[priorities](https://ntfy.sh/docs/publish/#message-priority) and
+An example configuration is shown here with all the available options,
+including [priorities](https://ntfy.sh/docs/publish/#message-priority) and
 [tags](https://ntfy.sh/docs/publish/#tags-emojis):
 
 ```yaml
 ntfy:
     topic: my-unique-topic
     server: https://ntfy.my-domain.com
+    username: myuser
+    password: secret
+
     start:
         title: A borgmatic backup started
         message: Watch this space...
         tags: borgmatic
         priority: min
     finish:
         title: A borgmatic backup completed successfully
@@ -313,14 +334,24 @@
         - finish
         - fail
 ```
 
 <span class="minilink minilink-addedin">Prior to version 1.8.0</span> Put
 the `ntfy:` option in the `hooks:` section of your configuration.
 
+<span class="minilink minilink-addedin">New in version 1.8.9</span> Instead of
+`username`/`password`, you can specify an [ntfy access
+token](https://docs.ntfy.sh/config/#access-tokens):
+
+```yaml
+ntfy:
+    topic: my-unique-topic
+    server: https://ntfy.my-domain.com
+    access_token: tk_AgQdq7mVBoFD37zQVN29RhuMzNIz2
+````
 
 ## Loki hook
 
 <span class="minilink minilink-addedin">New in version 1.8.3</span> [Grafana
 Loki](https://grafana.com/oss/loki/) is a "horizontally scalable, highly
 available, multi-tenant log aggregation system inspired by Prometheus."
 borgmatic has built-in integration with Loki, sending both backup status and
@@ -381,15 +412,15 @@
 
 Depending on how you installed borgmatic, it may not have come with Apprise.
 For instance, if you originally [installed borgmatic with
 pipx](https://torsion.org/borgmatic/docs/how-to/set-up-backups/#installation),
 run the following to install Apprise so borgmatic can use it:
 
 ```bash
-sudo pipx install --editable --force borgmatic[Apprise]
+sudo pipx install --force borgmatic[Apprise]
 ```
 
 Omit `sudo` if borgmatic is installed as a non-root user.
 
 Once Apprise is installed, configure borgmatic to notify one or more [Apprise
 services](https://github.com/caronc/apprise/wiki). For example:
 
@@ -425,14 +456,45 @@
         body: Your backups have failed.
     states:
         - start
         - finish
         - fail
 ```
 
+<span class="minilink minilink-addedin">New in version 1.8.9</span> borgmatic
+logs are automatically included in the body data sent to your Apprise services
+when a backup finishes or fails.
+
+You can customize the verbosity of the logs that are sent with borgmatic's
+`--monitoring-verbosity` flag. The `--list` and `--stats` flags may also be of
+use. See `borgmatic create --help` for more information.
+
+If you don't want any logs sent, you can disable this feature by setting
+`send_logs` to `false`:
+
+```yaml
+apprise:
+    services:
+        - url: gotify://hostname/token
+          label: gotify
+    send_logs: false
+```
+
+Or to limit the size of logs sent to Apprise services:
+
+```yaml
+apprise:
+    services:
+        - url: gotify://hostname/token
+          label: gotify
+    logs_size_limit: 500
+```
+
+This may be necessary for some services that reject large requests.
+
 See the [configuration
 reference](https://torsion.org/borgmatic/docs/reference/configuration/) for
 details.
 
 
 ## Scripting borgmatic
```

### Comparing `borgmatic-1.8.8/docs/how-to/provide-your-passwords.md` & `borgmatic-1.8.9/docs/how-to/provide-your-passwords.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/run-arbitrary-borg-commands.md` & `borgmatic-1.8.9/docs/how-to/run-arbitrary-borg-commands.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/how-to/set-up-backups.md` & `borgmatic-1.8.9/docs/how-to/set-up-backups.md`

 * *Files 0% similar despite different names*

```diff
@@ -402,16 +402,17 @@
 ```
 
 ### Colored output
 
 borgmatic produces colored terminal output by default. It is disabled when a
 non-interactive terminal is detected (like a cron job), or when you use the
 `--json` flag. Otherwise, you can disable it by passing the `--no-color` flag,
-setting the environment variable `PY_COLORS=False`, or setting the `color`
-option to `false` in the `output` section of configuration.
+setting the environment variables `PY_COLORS=False` or `NO_COLOR=True`, or
+setting the `color` option to `false` in the `output` section of
+configuration.
 
 
 ## Troubleshooting
 
 ### "found character that cannot start any token" error
 
 If you run borgmatic and see an error looking something like this, it probably
```

#### html2text {}

```diff
@@ -179,23 +179,24 @@
 and open a new shell) so the completions take effect. #### fish To add
 completions for fish, install the completions file globally: ```fish borgmatic
 --fish-completion | sudo tee /usr/share/fish/vendor_completions.d/
 borgmatic.fish source /usr/share/fish/vendor_completions.d/borgmatic.fish ```
 ### Colored output borgmatic produces colored terminal output by default. It is
 disabled when a non-interactive terminal is detected (like a cron job), or when
 you use the `--json` flag. Otherwise, you can disable it by passing the `--no-
-color` flag, setting the environment variable `PY_COLORS=False`, or setting the
-`color` option to `false` in the `output` section of configuration. ##
-Troubleshooting ### "found character that cannot start any token" error If you
-run borgmatic and see an error looking something like this, it probably means
-you've used tabs instead of spaces: ``` test.yaml: Error parsing configuration
-file An error occurred while parsing a configuration file at config.yaml: while
-scanning for the next token found character that cannot start any token in
-"config.yaml", line 230, column 1 ``` YAML does not allow tabs. So to fix this,
-replace any tabs in your configuration file with the requisite number of
-spaces. ### libyaml compilation errors borgmatic depends on a Python YAML
-library (ruamel.yaml) that will optionally use a C YAML library (libyaml) if
-present. But if it's not installed, then when installing or upgrading
-borgmatic, you may see errors about compiling the YAML library. If so, not to
-worry. borgmatic should install and function correctly even without the C YAML
-library. And borgmatic won't be any faster with the C library present, so you
-don't need to go out of your way to install it.
+color` flag, setting the environment variables `PY_COLORS=False` or
+`NO_COLOR=True`, or setting the `color` option to `false` in the `output`
+section of configuration. ## Troubleshooting ### "found character that cannot
+start any token" error If you run borgmatic and see an error looking something
+like this, it probably means you've used tabs instead of spaces: ``` test.yaml:
+Error parsing configuration file An error occurred while parsing a
+configuration file at config.yaml: while scanning for the next token found
+character that cannot start any token in "config.yaml", line 230, column 1 ```
+YAML does not allow tabs. So to fix this, replace any tabs in your
+configuration file with the requisite number of spaces. ### libyaml compilation
+errors borgmatic depends on a Python YAML library (ruamel.yaml) that will
+optionally use a C YAML library (libyaml) if present. But if it's not
+installed, then when installing or upgrading borgmatic, you may see errors
+about compiling the YAML library. If so, not to worry. borgmatic should install
+and function correctly even without the C YAML library. And borgmatic won't be
+any faster with the C library present, so you don't need to go out of your way
+to install it.
```

### Comparing `borgmatic-1.8.8/docs/how-to/upgrade.md` & `borgmatic-1.8.9/docs/how-to/upgrade.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/reference/command-line.md` & `borgmatic-1.8.9/docs/reference/command-line.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/reference/configuration.md` & `borgmatic-1.8.9/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/reference/source-code.md` & `borgmatic-1.8.9/docs/reference/source-code.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/apprise.png` & `borgmatic-1.8.9/docs/static/apprise.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/borgbase.png` & `borgmatic-1.8.9/docs/static/borgbase.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/borgmatic.png` & `borgmatic-1.8.9/docs/static/borgmatic.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/borgmatic.svg` & `borgmatic-1.8.9/docs/static/borgmatic.svg`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/cronhub.png` & `borgmatic-1.8.9/docs/static/cronhub.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/cronitor.png` & `borgmatic-1.8.9/docs/static/cronitor.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/healthchecks.png` & `borgmatic-1.8.9/docs/static/healthchecks.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/loki.png` & `borgmatic-1.8.9/docs/static/loki.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/mariadb.png` & `borgmatic-1.8.9/docs/static/mariadb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/mongodb.png` & `borgmatic-1.8.9/docs/static/mongodb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/mysql.png` & `borgmatic-1.8.9/docs/static/mysql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/ntfy.png` & `borgmatic-1.8.9/docs/static/ntfy.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/pagerduty.png` & `borgmatic-1.8.9/docs/static/pagerduty.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/postgresql.png` & `borgmatic-1.8.9/docs/static/postgresql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/docs/static/sqlite.png` & `borgmatic-1.8.9/docs/static/sqlite.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/sample/systemd/borgmatic.service` & `borgmatic-1.8.9/sample/systemd/borgmatic.service`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/scripts/find-unsupported-borg-options` & `borgmatic-1.8.9/scripts/find-unsupported-borg-options`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/scripts/release` & `borgmatic-1.8.9/scripts/release`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/scripts/run-full-tests` & `borgmatic-1.8.9/scripts/run-full-tests`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/sh
 
 # This script installs test dependencies and runs all tests, including end-to-end tests. It
 # is designed to run inside a test container, and presumes that other test infrastructure like
 # databases are already running. Therefore, on a developer machine, you should not run this script
-# directly. Instead, run scripts/run-end-to-end-dev-tests
+# directly. Instead, run scripts/run-end-to-end-tests
 #
 # For more information, see:
 # https://torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/
 
 set -e
 
 if [ -z "$TEST_CONTAINER" ]; then
@@ -21,12 +21,9 @@
     py3-ruamel.yaml py3-ruamel.yaml.clib py3-yaml bash sqlite fish
 # If certain dependencies of black are available in this version of Alpine, install them.
 apk add --no-cache py3-typed-ast py3-regex || true
 python3 -m pip install --no-cache --upgrade pip==22.2.2 setuptools==64.0.1
 pip3 install --ignore-installed tox==4.11.3
 export COVERAGE_FILE=/tmp/.coverage
 
-if [ "$1" != "--end-to-end-only" ]; then
-    tox --workdir /tmp/.tox --sitepackages
-fi
-
+tox --workdir /tmp/.tox --sitepackages
 tox --workdir /tmp/.tox --sitepackages -e end-to-end
```

### Comparing `borgmatic-1.8.8/setup.py` & `borgmatic-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '1.8.8'
+VERSION = '1.8.9'
 
 
 setup(
     name='borgmatic',
     version=VERSION,
     description='Simple, configuration-driven backup software for servers and workstations',
     author='Dan Helfman',
```

### Comparing `borgmatic-1.8.8/test_requirements.txt` & `borgmatic-1.8.9/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/end-to-end/test_borgmatic.py` & `borgmatic-1.8.9/tests/end-to-end/test_borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/end-to-end/test_database.py` & `borgmatic-1.8.9/tests/end-to-end/test_database.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/end-to-end/test_generate_config.py` & `borgmatic-1.8.9/tests/end-to-end/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/end-to-end/test_override.py` & `borgmatic-1.8.9/tests/end-to-end/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/end-to-end/test_validate_config.py` & `borgmatic-1.8.9/tests/end-to-end/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/actions/config/test_validate.py` & `borgmatic-1.8.9/tests/integration/actions/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/borg/test_commands.py` & `borgmatic-1.8.9/tests/integration/borg/test_commands.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/borg/test_feature.py` & `borgmatic-1.8.9/tests/integration/borg/test_feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/commands/completion/test_actions.py` & `borgmatic-1.8.9/tests/integration/commands/completion/test_actions.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/commands/test_arguments.py` & `borgmatic-1.8.9/tests/integration/commands/test_arguments.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/config/test_generate.py` & `borgmatic-1.8.9/tests/integration/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/config/test_load.py` & `borgmatic-1.8.9/tests/integration/config/test_load.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/config/test_override.py` & `borgmatic-1.8.9/tests/integration/config/test_override.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,28 +25,32 @@
 
 
 def test_apply_overrides_updates_config():
     raw_overrides = [
         'section.key=value1',
         'other_section.thing=value2',
         'section.nested.key=value3',
+        'location.no_longer_in_location=value4',
         'new.foo=bar',
         'new.mylist=[baz]',
         'new.nonlist=[quux]',
     ]
     config = {
         'section': {'key': 'value', 'other': 'other_value'},
         'other_section': {'thing': 'thing_value'},
+        'no_longer_in_location': 'because_location_is_deprecated',
     }
     schema = {
         'properties': {
             'new': {'properties': {'mylist': {'type': 'array'}, 'nonlist': {'type': 'string'}}}
         }
     }
 
     module.apply_overrides(config, schema, raw_overrides)
 
     assert config == {
         'section': {'key': 'value1', 'other': 'other_value', 'nested': {'key': 'value3'}},
         'other_section': {'thing': 'value2'},
         'new': {'foo': 'bar', 'mylist': ['baz'], 'nonlist': '[quux]'},
+        'location': {'no_longer_in_location': 'value4'},
+        'no_longer_in_location': 'value4',
     }
```

### Comparing `borgmatic-1.8.8/tests/integration/config/test_schema.py` & `borgmatic-1.8.9/tests/integration/config/test_schema.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/config/test_validate.py` & `borgmatic-1.8.9/tests/integration/config/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             - path: hostname.borg
 
         local_path: borg1
         '''
     )
 
     config, config_paths, logs = module.parse_configuration(
-        '/tmp/config.yaml', '/tmp/schema.yaml', overrides=['location.local_path=borg2']
+        '/tmp/config.yaml', '/tmp/schema.yaml', overrides=['local_path=borg2']
     )
 
     assert config == {
         'source_directories': ['/home'],
         'repositories': [{'path': 'hostname.borg'}],
         'local_path': 'borg2',
     }
```

### Comparing `borgmatic-1.8.8/tests/integration/hooks/test_loki.py` & `borgmatic-1.8.9/tests/integration/hooks/test_loki.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/integration/test_execute.py` & `borgmatic-1.8.9/tests/integration/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/config/test_bootstrap.py` & `borgmatic-1.8.9/tests/unit/actions/config/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/config/test_generate.py` & `borgmatic-1.8.9/tests/unit/actions/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/config/test_validate.py` & `borgmatic-1.8.9/tests/unit/actions/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_borg.py` & `borgmatic-1.8.9/tests/unit/actions/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_break_lock.py` & `borgmatic-1.8.9/tests/unit/actions/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_check.py` & `borgmatic-1.8.9/tests/unit/actions/test_check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_compact.py` & `borgmatic-1.8.9/tests/unit/actions/test_compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_create.py` & `borgmatic-1.8.9/tests/unit/actions/test_create.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_export_key.py` & `borgmatic-1.8.9/tests/unit/actions/test_export_key.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_export_tar.py` & `borgmatic-1.8.9/tests/unit/actions/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_extract.py` & `borgmatic-1.8.9/tests/unit/actions/test_extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_info.py` & `borgmatic-1.8.9/tests/unit/actions/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_json.py` & `borgmatic-1.8.9/tests/unit/actions/test_json.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_list.py` & `borgmatic-1.8.9/tests/unit/actions/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_mount.py` & `borgmatic-1.8.9/tests/unit/actions/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_prune.py` & `borgmatic-1.8.9/tests/unit/actions/test_prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_rcreate.py` & `borgmatic-1.8.9/tests/unit/actions/test_rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_restore.py` & `borgmatic-1.8.9/tests/unit/actions/test_restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_rinfo.py` & `borgmatic-1.8.9/tests/unit/actions/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_rlist.py` & `borgmatic-1.8.9/tests/unit/actions/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/actions/test_transfer.py` & `borgmatic-1.8.9/tests/unit/actions/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_borg.py` & `borgmatic-1.8.9/tests/unit/borg/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_break_lock.py` & `borgmatic-1.8.9/tests/unit/borg/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_check.py` & `borgmatic-1.8.9/tests/unit/borg/test_check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_compact.py` & `borgmatic-1.8.9/tests/unit/borg/test_compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_create.py` & `borgmatic-1.8.9/tests/unit/borg/test_create.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_environment.py` & `borgmatic-1.8.9/tests/unit/borg/test_environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_export_key.py` & `borgmatic-1.8.9/tests/unit/borg/test_export_key.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_export_tar.py` & `borgmatic-1.8.9/tests/unit/borg/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_extract.py` & `borgmatic-1.8.9/tests/unit/borg/test_extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_flags.py` & `borgmatic-1.8.9/tests/unit/borg/test_flags.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_info.py` & `borgmatic-1.8.9/tests/unit/borg/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_list.py` & `borgmatic-1.8.9/tests/unit/borg/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_mount.py` & `borgmatic-1.8.9/tests/unit/borg/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_prune.py` & `borgmatic-1.8.9/tests/unit/borg/test_prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_rcreate.py` & `borgmatic-1.8.9/tests/unit/borg/test_rcreate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from ..test_verbosity import insert_logging_mock
 
 RINFO_SOME_UNKNOWN_EXIT_CODE = -999
 RCREATE_COMMAND = ('borg', 'rcreate', '--encryption', 'repokey')
 
 
 def insert_rinfo_command_found_mock():
-    flexmock(module.rinfo).should_receive('display_repository_info')
+    flexmock(module.rinfo).should_receive('display_repository_info').and_return(
+        '{"encryption": {"mode": "repokey"}}'
+    )
 
 
 def insert_rinfo_command_not_found_mock():
     flexmock(module.rinfo).should_receive('display_repository_info').and_raise(
         subprocess.CalledProcessError(sorted(module.RINFO_REPOSITORY_NOT_FOUND_EXIT_CODES)[0], [])
     )
 
@@ -116,14 +118,35 @@
         config={},
         local_borg_version='2.3.4',
         global_arguments=flexmock(log_json=False),
         encryption_mode='repokey',
     )
 
 
+def test_create_repository_errors_when_repository_with_differing_encryption_mode_already_exists():
+    insert_rinfo_command_found_mock()
+    flexmock(module.feature).should_receive('available').and_return(True)
+    flexmock(module.flags).should_receive('make_repository_flags').and_return(
+        (
+            '--repo',
+            'repo',
+        )
+    )
+
+    with pytest.raises(ValueError):
+        module.create_repository(
+            dry_run=False,
+            repository_path='repo',
+            config={},
+            local_borg_version='2.3.4',
+            global_arguments=flexmock(log_json=False),
+            encryption_mode='repokey-blake2',
+        )
+
+
 def test_create_repository_raises_for_unknown_rinfo_command_error():
     flexmock(module.rinfo).should_receive('display_repository_info').and_raise(
         subprocess.CalledProcessError(RINFO_SOME_UNKNOWN_EXIT_CODE, [])
     )
 
     with pytest.raises(subprocess.CalledProcessError):
         module.create_repository(
```

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_rinfo.py` & `borgmatic-1.8.9/tests/unit/borg/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_rlist.py` & `borgmatic-1.8.9/tests/unit/borg/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_transfer.py` & `borgmatic-1.8.9/tests/unit/borg/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_umount.py` & `borgmatic-1.8.9/tests/unit/borg/test_umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/borg/test_version.py` & `borgmatic-1.8.9/tests/unit/borg/test_version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/commands/completion/test_fish.py` & `borgmatic-1.8.9/tests/unit/commands/completion/test_fish.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/commands/test_arguments.py` & `borgmatic-1.8.9/tests/unit/commands/test_arguments.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/commands/test_borgmatic.py` & `borgmatic-1.8.9/tests/unit/commands/test_borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_checks.py` & `borgmatic-1.8.9/tests/unit/config/test_checks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_collect.py` & `borgmatic-1.8.9/tests/unit/config/test_collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_constants.py` & `borgmatic-1.8.9/tests/unit/config/test_constants.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_environment.py` & `borgmatic-1.8.9/tests/unit/config/test_environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_generate.py` & `borgmatic-1.8.9/tests/unit/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_load.py` & `borgmatic-1.8.9/tests/unit/config/test_load.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_normalize.py` & `borgmatic-1.8.9/tests/unit/config/test_normalize.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_override.py` & `borgmatic-1.8.9/tests/unit/config/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/config/test_validate.py` & `borgmatic-1.8.9/tests/unit/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_command.py` & `borgmatic-1.8.9/tests/unit/hooks/test_command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_cronhub.py` & `borgmatic-1.8.9/tests/unit/hooks/test_cronhub.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_cronitor.py` & `borgmatic-1.8.9/tests/unit/hooks/test_cronitor.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_dispatch.py` & `borgmatic-1.8.9/tests/unit/hooks/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_dump.py` & `borgmatic-1.8.9/tests/unit/hooks/test_dump.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_healthchecks.py` & `borgmatic-1.8.9/tests/unit/hooks/test_healthchecks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,145 +1,83 @@
 from flexmock import flexmock
 
 from borgmatic.hooks import healthchecks as module
 
 
-def test_forgetful_buffering_handler_emit_collects_log_records():
-    handler = module.Forgetful_buffering_handler(byte_capacity=100, log_level=1)
-    handler.emit(flexmock(getMessage=lambda: 'foo'))
-    handler.emit(flexmock(getMessage=lambda: 'bar'))
-
-    assert handler.buffer == ['foo\n', 'bar\n']
-    assert not handler.forgot
-
-
-def test_forgetful_buffering_handler_emit_collects_log_records_with_zero_byte_capacity():
-    handler = module.Forgetful_buffering_handler(byte_capacity=0, log_level=1)
-    handler.emit(flexmock(getMessage=lambda: 'foo'))
-    handler.emit(flexmock(getMessage=lambda: 'bar'))
-
-    assert handler.buffer == ['foo\n', 'bar\n']
-    assert not handler.forgot
-
-
-def test_forgetful_buffering_handler_emit_forgets_log_records_when_capacity_reached():
-    handler = module.Forgetful_buffering_handler(byte_capacity=len('foo\nbar\n'), log_level=1)
-    handler.emit(flexmock(getMessage=lambda: 'foo'))
-    assert handler.buffer == ['foo\n']
-    handler.emit(flexmock(getMessage=lambda: 'bar'))
-    assert handler.buffer == ['foo\n', 'bar\n']
-    handler.emit(flexmock(getMessage=lambda: 'baz'))
-    assert handler.buffer == ['bar\n', 'baz\n']
-    handler.emit(flexmock(getMessage=lambda: 'quux'))
-    assert handler.buffer == ['quux\n']
-    assert handler.forgot
-
-
-def test_format_buffered_logs_for_payload_flattens_log_buffer():
-    handler = module.Forgetful_buffering_handler(byte_capacity=100, log_level=1)
-    handler.buffer = ['foo\n', 'bar\n']
-    logger = flexmock(handlers=[handler])
-    logger.should_receive('removeHandler')
-    flexmock(module.logging).should_receive('getLogger').and_return(logger)
-
-    payload = module.format_buffered_logs_for_payload()
-
-    assert payload == 'foo\nbar\n'
-
-
-def test_format_buffered_logs_for_payload_inserts_truncation_indicator_when_logs_forgotten():
-    handler = module.Forgetful_buffering_handler(byte_capacity=100, log_level=1)
-    handler.buffer = ['foo\n', 'bar\n']
-    handler.forgot = True
-    logger = flexmock(handlers=[handler])
-    logger.should_receive('removeHandler')
-    flexmock(module.logging).should_receive('getLogger').and_return(logger)
-
-    payload = module.format_buffered_logs_for_payload()
-
-    assert payload == '...\nfoo\nbar\n'
-
-
-def test_format_buffered_logs_for_payload_without_handler_produces_empty_payload():
-    logger = flexmock(handlers=[module.logging.Handler()])
-    logger.should_receive('removeHandler')
-    flexmock(module.logging).should_receive('getLogger').and_return(logger)
-
-    payload = module.format_buffered_logs_for_payload()
-
-    assert payload == ''
-
-
 def mock_logger():
     logger = flexmock()
     logger.should_receive('addHandler')
     logger.should_receive('removeHandler')
     flexmock(module.logging).should_receive('getLogger').and_return(logger)
 
 
 def test_initialize_monitor_creates_log_handler_with_ping_body_limit():
     ping_body_limit = 100
     monitoring_log_level = 1
 
     mock_logger()
-    flexmock(module).should_receive('Forgetful_buffering_handler').with_args(
-        ping_body_limit - len(module.PAYLOAD_TRUNCATION_INDICATOR), monitoring_log_level
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').with_args(
+        module.HANDLER_IDENTIFIER,
+        ping_body_limit - len(module.borgmatic.hooks.logs.PAYLOAD_TRUNCATION_INDICATOR),
+        monitoring_log_level,
     ).once()
 
     module.initialize_monitor(
         {'ping_body_limit': ping_body_limit}, {}, 'test.yaml', monitoring_log_level, dry_run=False
     )
 
 
 def test_initialize_monitor_creates_log_handler_with_default_ping_body_limit():
     monitoring_log_level = 1
 
     mock_logger()
-    flexmock(module).should_receive('Forgetful_buffering_handler').with_args(
-        module.DEFAULT_PING_BODY_LIMIT_BYTES - len(module.PAYLOAD_TRUNCATION_INDICATOR),
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').with_args(
+        module.HANDLER_IDENTIFIER,
+        module.DEFAULT_PING_BODY_LIMIT_BYTES
+        - len(module.borgmatic.hooks.logs.PAYLOAD_TRUNCATION_INDICATOR),
         monitoring_log_level,
     ).once()
 
     module.initialize_monitor({}, {}, 'test.yaml', monitoring_log_level, dry_run=False)
 
 
 def test_initialize_monitor_creates_log_handler_with_zero_ping_body_limit():
     ping_body_limit = 0
     monitoring_log_level = 1
 
     mock_logger()
-    flexmock(module).should_receive('Forgetful_buffering_handler').with_args(
-        ping_body_limit, monitoring_log_level
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').with_args(
+        module.HANDLER_IDENTIFIER, ping_body_limit, monitoring_log_level
     ).once()
 
     module.initialize_monitor(
         {'ping_body_limit': ping_body_limit}, {}, 'test.yaml', monitoring_log_level, dry_run=False
     )
 
 
 def test_initialize_monitor_creates_log_handler_when_send_logs_true():
     mock_logger()
-    flexmock(module).should_receive('Forgetful_buffering_handler').once()
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').once()
 
     module.initialize_monitor(
         {'send_logs': True}, {}, 'test.yaml', monitoring_log_level=1, dry_run=False
     )
 
 
 def test_initialize_monitor_bails_when_send_logs_false():
     mock_logger()
-    flexmock(module).should_receive('Forgetful_buffering_handler').never()
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
 
     module.initialize_monitor(
         {'send_logs': False}, {}, 'test.yaml', monitoring_log_level=1, dry_run=False
     )
 
 
 def test_ping_monitor_hits_ping_url_for_start_state():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com'}
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/start', data=''.encode('utf-8'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
@@ -150,15 +88,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_hits_ping_url_for_finish_state():
     hook_config = {'ping_url': 'https://example.com'}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com', data=payload.encode('utf-8'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
         {},
@@ -168,15 +109,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_hits_ping_url_for_fail_state():
     hook_config = {'ping_url': 'https://example.com'}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/fail', data=payload.encode('utf'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
         {},
@@ -186,15 +130,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_hits_ping_url_for_log_state():
     hook_config = {'ping_url': 'https://example.com'}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/log', data=payload.encode('utf'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
         {},
@@ -204,15 +151,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_with_ping_uuid_hits_corresponding_url():
     hook_config = {'ping_url': 'abcd-efgh-ijkl-mnop'}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         f"https://hc-ping.com/{hook_config['ping_url']}",
         data=payload.encode('utf-8'),
         verify=True,
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
@@ -224,15 +174,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_skips_ssl_verification_when_verify_tls_false():
     hook_config = {'ping_url': 'https://example.com', 'verify_tls': False}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com', data=payload.encode('utf-8'), verify=False
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
         {},
@@ -242,15 +195,18 @@
         dry_run=False,
     )
 
 
 def test_ping_monitor_executes_ssl_verification_when_verify_tls_true():
     hook_config = {'ping_url': 'https://example.com', 'verify_tls': True}
     payload = 'data'
-    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.borgmatic.hooks.logs).should_receive('get_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive(
+        'format_buffered_logs_for_payload'
+    ).and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com', data=payload.encode('utf-8'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
         {},
@@ -258,45 +214,45 @@
         state=module.monitor.State.FINISH,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
 def test_ping_monitor_dry_run_does_not_hit_ping_url():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com'}
     flexmock(module.requests).should_receive('post').never()
 
     module.ping_monitor(
         hook_config,
         {},
         'config.yaml',
         state=module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=True,
     )
 
 
 def test_ping_monitor_does_not_hit_ping_url_when_states_not_matching():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com', 'states': ['finish']}
     flexmock(module.requests).should_receive('post').never()
 
     module.ping_monitor(
         hook_config,
         {},
         'config.yaml',
         state=module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=True,
     )
 
 
 def test_ping_monitor_hits_ping_url_when_states_matching():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com', 'states': ['start', 'finish']}
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/start', data=''.encode('utf-8'), verify=True
     ).and_return(flexmock(ok=True))
 
     module.ping_monitor(
         hook_config,
@@ -305,15 +261,15 @@
         state=module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
 def test_ping_monitor_with_connection_error_logs_warning():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com'}
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/start', data=''.encode('utf-8'), verify=True
     ).and_raise(module.requests.exceptions.ConnectionError)
     flexmock(module.logger).should_receive('warning').once()
 
     module.ping_monitor(
@@ -323,15 +279,15 @@
         state=module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
 def test_ping_monitor_with_other_error_logs_warning():
-    flexmock(module).should_receive('Forgetful_buffering_handler')
+    flexmock(module.borgmatic.hooks.logs).should_receive('Forgetful_buffering_handler').never()
     hook_config = {'ping_url': 'https://example.com'}
     response = flexmock(ok=False)
     response.should_receive('raise_for_status').and_raise(
         module.requests.exceptions.RequestException
     )
     flexmock(module.requests).should_receive('post').with_args(
         'https://example.com/start', data=''.encode('utf-8'), verify=True
```

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_loki.py` & `borgmatic-1.8.9/tests/unit/hooks/test_loki.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_mariadb.py` & `borgmatic-1.8.9/tests/unit/hooks/test_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 import pytest
 from flexmock import flexmock
 
-from borgmatic.hooks import mariadb as module
+from borgmatic.hooks import mysql as module
 
 
 def test_database_names_to_dump_passes_through_name():
     extra_environment = flexmock()
     log_prefix = ''
 
     names = module.database_names_to_dump(
@@ -25,19 +25,19 @@
     names = module.database_names_to_dump(
         {'name': 'all'}, extra_environment, log_prefix, dry_run=True
     )
 
     assert names == ()
 
 
-def test_database_names_to_dump_queries_mariadb_for_database_names():
+def test_database_names_to_dump_queries_mysql_for_database_names():
     extra_environment = flexmock()
     log_prefix = ''
     flexmock(module).should_receive('execute_command_and_capture_output').with_args(
-        ('mariadb', '--skip-column-names', '--batch', '--execute', 'show schemas'),
+        ('mysql', '--skip-column-names', '--batch', '--execute', 'show schemas'),
         extra_environment=extra_environment,
     ).and_return('foo\nbar\nmysql\n').once()
 
     names = module.database_names_to_dump(
         {'name': 'all'}, extra_environment, log_prefix, dry_run=False
     )
 
@@ -121,40 +121,61 @@
             dry_run=object,
             dry_run_label=object,
         ).and_return(process).once()
 
     assert module.dump_data_sources(databases, {}, 'test.yaml', dry_run=False) == processes
 
 
-def test_database_names_to_dump_runs_mariadb_with_list_options():
-    database = {'name': 'all', 'list_options': '--defaults-extra-file=mariadb.cnf'}
+def test_database_names_to_dump_runs_mysql_with_list_options():
+    database = {'name': 'all', 'list_options': '--defaults-extra-file=my.cnf'}
     flexmock(module).should_receive('execute_command_and_capture_output').with_args(
         (
-            'mariadb',
-            '--defaults-extra-file=mariadb.cnf',
+            'mysql',
+            '--defaults-extra-file=my.cnf',
             '--skip-column-names',
             '--batch',
             '--execute',
             'show schemas',
         ),
         extra_environment=None,
     ).and_return(('foo\nbar')).once()
 
     assert module.database_names_to_dump(database, None, 'test.yaml', '') == ('foo', 'bar')
 
 
-def test_execute_dump_command_runs_mariadb_dump():
+def test_database_names_to_dump_runs_non_default_mysql_with_list_options():
+    database = {
+        'name': 'all',
+        'list_options': '--defaults-extra-file=my.cnf',
+        'mysql_command': 'custom_mysql',
+    }
+    flexmock(module).should_receive('execute_command_and_capture_output').with_args(
+        extra_environment=None,
+        full_command=(
+            'custom_mysql',  # Custom MySQL command
+            '--defaults-extra-file=my.cnf',
+            '--skip-column-names',
+            '--batch',
+            '--execute',
+            'show schemas',
+        ),
+    ).and_return(('foo\nbar')).once()
+
+    assert module.database_names_to_dump(database, None, 'test.yaml', '') == ('foo', 'bar')
+
+
+def test_execute_dump_command_runs_mysqldump():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mariadb-dump',
+            'mysqldump',
             '--add-drop-database',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
         extra_environment=None,
@@ -171,23 +192,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mariadb_dump_without_add_drop_database():
+def test_execute_dump_command_runs_mysqldump_without_add_drop_database():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mariadb-dump',
+            'mysqldump',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
         extra_environment=None,
         run_to_completion=False,
@@ -203,23 +224,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mariadb_dump_with_hostname_and_port():
+def test_execute_dump_command_runs_mysqldump_with_hostname_and_port():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mariadb-dump',
+            'mysqldump',
             '--add-drop-database',
             '--host',
             'database.example.org',
             '--port',
             '5433',
             '--protocol',
             'tcp',
@@ -242,23 +263,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mariadb_dump_with_username_and_password():
+def test_execute_dump_command_runs_mysqldump_with_username_and_password():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mariadb-dump',
+            'mysqldump',
             '--add-drop-database',
             '--user',
             'root',
             '--databases',
             'foo',
             '--result-file',
             'dump',
@@ -277,23 +298,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mariadb_dump_with_options():
+def test_execute_dump_command_runs_mysqldump_with_options():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mariadb-dump',
+            'mysqldump',
             '--stuff=such',
             '--add-drop-database',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
@@ -311,15 +332,51 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_with_duplicate_dump_skips_mariadb_dump():
+def test_execute_dump_command_runs_non_default_mysqldump():
+    process = flexmock()
+    flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
+    flexmock(module.os.path).should_receive('exists').and_return(False)
+    flexmock(module.dump).should_receive('create_named_pipe_for_dump')
+
+    flexmock(module).should_receive('execute_command').with_args(
+        (
+            'custom_mysqldump',  # Custom MySQL dump command
+            '--add-drop-database',
+            '--databases',
+            'foo',
+            '--result-file',
+            'dump',
+        ),
+        extra_environment=None,
+        run_to_completion=False,
+    ).and_return(process).once()
+
+    assert (
+        module.execute_dump_command(
+            database={
+                'name': 'foo',
+                'mysql_dump_command': 'custom_mysqldump',
+            },  # Custom MySQL dump command specified
+            log_prefix='log',
+            dump_path=flexmock(),
+            database_names=('foo',),
+            extra_environment=None,
+            dry_run=False,
+            dry_run_label='',
+        )
+        == process
+    )
+
+
+def test_execute_dump_command_with_duplicate_dump_skips_mysqldump():
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(True)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump').never()
     flexmock(module).should_receive('execute_command').never()
 
     assert (
         module.execute_dump_command(
@@ -331,15 +388,15 @@
             dry_run=True,
             dry_run_label='SO DRY',
         )
         is None
     )
 
 
-def test_execute_dump_command_with_dry_run_skips_mariadb_dump():
+def test_execute_dump_command_with_dry_run_skips_mysqldump():
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').never()
 
     assert (
@@ -375,20 +432,20 @@
         'databases/localhost/all'
     )
     flexmock(module).should_receive('database_names_to_dump').and_return(())
 
     assert module.dump_data_sources(databases, {}, 'test.yaml', dry_run=True) == []
 
 
-def test_restore_data_source_dump_runs_mariadb_to_restore():
+def test_restore_data_source_dump_runs_mysql_to_restore():
     hook_config = [{'name': 'foo'}, {'name': 'bar'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mariadb', '--batch'),
+        ('mysql', '--batch'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment=None,
     ).once()
 
     module.restore_data_source_dump(
@@ -403,20 +460,48 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mariadb_with_options():
+def test_restore_data_source_dump_runs_mysql_with_options():
     hook_config = [{'name': 'foo', 'restore_options': '--harder'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mariadb', '--batch', '--harder'),
+        ('mysql', '--batch', '--harder'),
+        processes=[extract_process],
+        output_log_level=logging.DEBUG,
+        input_file=extract_process.stdout,
+        extra_environment=None,
+    ).once()
+
+    module.restore_data_source_dump(
+        hook_config,
+        {},
+        'test.yaml',
+        data_source=hook_config[0],
+        dry_run=False,
+        extract_process=extract_process,
+        connection_params={
+            'hostname': None,
+            'port': None,
+            'username': None,
+            'password': None,
+        },
+    )
+
+
+def test_restore_data_source_dump_runs_non_default_mysql_with_options():
+    hook_config = [{'name': 'foo', 'mysql_command': 'custom_mysql', 'restore_options': '--harder'}]
+    extract_process = flexmock(stdout=flexmock())
+
+    flexmock(module).should_receive('execute_command_with_processes').with_args(
+        ('custom_mysql', '--batch', '--harder'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment=None,
     ).once()
 
     module.restore_data_source_dump(
@@ -431,21 +516,21 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mariadb_with_hostname_and_port():
+def test_restore_data_source_dump_runs_mysql_with_hostname_and_port():
     hook_config = [{'name': 'foo', 'hostname': 'database.example.org', 'port': 5433}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mariadb',
+            'mysql',
             '--batch',
             '--host',
             'database.example.org',
             '--port',
             '5433',
             '--protocol',
             'tcp',
@@ -468,20 +553,20 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mariadb_with_username_and_password():
+def test_restore_data_source_dump_runs_mysql_with_username_and_password():
     hook_config = [{'name': 'foo', 'username': 'root', 'password': 'trustsome1'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mariadb', '--batch', '--user', 'root'),
+        ('mysql', '--batch', '--user', 'root'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment={'MYSQL_PWD': 'trustsome1'},
     ).once()
 
     module.restore_data_source_dump(
@@ -512,15 +597,15 @@
             'restore_password': 'restorepassword',
         }
     ]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mariadb',
+            'mysql',
             '--batch',
             '--host',
             'clihost',
             '--port',
             'cliport',
             '--protocol',
             'tcp',
@@ -533,15 +618,15 @@
         extra_environment={'MYSQL_PWD': 'clipassword'},
     ).once()
 
     module.restore_data_source_dump(
         hook_config,
         {},
         'test.yaml',
-        data_source=hook_config[0],
+        data_source={'name': 'foo'},
         dry_run=False,
         extract_process=extract_process,
         connection_params={
             'hostname': 'clihost',
             'port': 'cliport',
             'username': 'cliusername',
             'password': 'clipassword',
@@ -563,15 +648,15 @@
             'restore_port': 'restoreport',
         }
     ]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mariadb',
+            'mysql',
             '--batch',
             '--host',
             'restorehost',
             '--port',
             'restoreport',
             '--protocol',
             'tcp',
```

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_mongodb.py` & `borgmatic-1.8.9/tests/unit/hooks/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_mysql.py` & `borgmatic-1.8.9/tests/unit/hooks/test_mariadb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 import pytest
 from flexmock import flexmock
 
-from borgmatic.hooks import mysql as module
+from borgmatic.hooks import mariadb as module
 
 
 def test_database_names_to_dump_passes_through_name():
     extra_environment = flexmock()
     log_prefix = ''
 
     names = module.database_names_to_dump(
@@ -25,19 +25,19 @@
     names = module.database_names_to_dump(
         {'name': 'all'}, extra_environment, log_prefix, dry_run=True
     )
 
     assert names == ()
 
 
-def test_database_names_to_dump_queries_mysql_for_database_names():
+def test_database_names_to_dump_queries_mariadb_for_database_names():
     extra_environment = flexmock()
     log_prefix = ''
     flexmock(module).should_receive('execute_command_and_capture_output').with_args(
-        ('mysql', '--skip-column-names', '--batch', '--execute', 'show schemas'),
+        ('mariadb', '--skip-column-names', '--batch', '--execute', 'show schemas'),
         extra_environment=extra_environment,
     ).and_return('foo\nbar\nmysql\n').once()
 
     names = module.database_names_to_dump(
         {'name': 'all'}, extra_environment, log_prefix, dry_run=False
     )
 
@@ -121,40 +121,61 @@
             dry_run=object,
             dry_run_label=object,
         ).and_return(process).once()
 
     assert module.dump_data_sources(databases, {}, 'test.yaml', dry_run=False) == processes
 
 
-def test_database_names_to_dump_runs_mysql_with_list_options():
-    database = {'name': 'all', 'list_options': '--defaults-extra-file=my.cnf'}
+def test_database_names_to_dump_runs_mariadb_with_list_options():
+    database = {'name': 'all', 'list_options': '--defaults-extra-file=mariadb.cnf'}
     flexmock(module).should_receive('execute_command_and_capture_output').with_args(
         (
-            'mysql',
-            '--defaults-extra-file=my.cnf',
+            'mariadb',
+            '--defaults-extra-file=mariadb.cnf',
             '--skip-column-names',
             '--batch',
             '--execute',
             'show schemas',
         ),
         extra_environment=None,
     ).and_return(('foo\nbar')).once()
 
     assert module.database_names_to_dump(database, None, 'test.yaml', '') == ('foo', 'bar')
 
 
-def test_execute_dump_command_runs_mysqldump():
+def test_database_names_to_dump_runs_non_default_mariadb_with_list_options():
+    database = {
+        'name': 'all',
+        'list_options': '--defaults-extra-file=mariadb.cnf',
+        'mariadb_command': 'custom_mariadb',
+    }
+    flexmock(module).should_receive('execute_command_and_capture_output').with_args(
+        extra_environment=None,
+        full_command=(
+            'custom_mariadb',  # Custom MariaDB command
+            '--defaults-extra-file=mariadb.cnf',
+            '--skip-column-names',
+            '--batch',
+            '--execute',
+            'show schemas',
+        ),
+    ).and_return(('foo\nbar')).once()
+
+    assert module.database_names_to_dump(database, None, 'test.yaml', '') == ('foo', 'bar')
+
+
+def test_execute_dump_command_runs_mariadb_dump():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mysqldump',
+            'mariadb-dump',
             '--add-drop-database',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
         extra_environment=None,
@@ -171,23 +192,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mysqldump_without_add_drop_database():
+def test_execute_dump_command_runs_mariadb_dump_without_add_drop_database():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mysqldump',
+            'mariadb-dump',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
         extra_environment=None,
         run_to_completion=False,
@@ -203,23 +224,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mysqldump_with_hostname_and_port():
+def test_execute_dump_command_runs_mariadb_dump_with_hostname_and_port():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mysqldump',
+            'mariadb-dump',
             '--add-drop-database',
             '--host',
             'database.example.org',
             '--port',
             '5433',
             '--protocol',
             'tcp',
@@ -242,23 +263,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mysqldump_with_username_and_password():
+def test_execute_dump_command_runs_mariadb_dump_with_username_and_password():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mysqldump',
+            'mariadb-dump',
             '--add-drop-database',
             '--user',
             'root',
             '--databases',
             'foo',
             '--result-file',
             'dump',
@@ -277,23 +298,23 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_runs_mysqldump_with_options():
+def test_execute_dump_command_runs_mariadb_dump_with_options():
     process = flexmock()
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').with_args(
         (
-            'mysqldump',
+            'mariadb-dump',
             '--stuff=such',
             '--add-drop-database',
             '--databases',
             'foo',
             '--result-file',
             'dump',
         ),
@@ -311,15 +332,53 @@
             dry_run=False,
             dry_run_label='',
         )
         == process
     )
 
 
-def test_execute_dump_command_with_duplicate_dump_skips_mysqldump():
+def test_execute_dump_command_runs_non_default_mariadb_dump_with_options():
+    process = flexmock()
+    flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
+    flexmock(module.os.path).should_receive('exists').and_return(False)
+    flexmock(module.dump).should_receive('create_named_pipe_for_dump')
+
+    flexmock(module).should_receive('execute_command').with_args(
+        (
+            'custom_mariadb_dump',  # Custom MariaDB dump command
+            '--stuff=such',
+            '--add-drop-database',
+            '--databases',
+            'foo',
+            '--result-file',
+            'dump',
+        ),
+        extra_environment=None,
+        run_to_completion=False,
+    ).and_return(process).once()
+
+    assert (
+        module.execute_dump_command(
+            database={
+                'name': 'foo',
+                'mariadb_dump_command': 'custom_mariadb_dump',
+                'options': '--stuff=such',
+            },  # Custom MariaDB dump command specified
+            log_prefix='log',
+            dump_path=flexmock(),
+            database_names=('foo',),
+            extra_environment=None,
+            dry_run=False,
+            dry_run_label='',
+        )
+        == process
+    )
+
+
+def test_execute_dump_command_with_duplicate_dump_skips_mariadb_dump():
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(True)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump').never()
     flexmock(module).should_receive('execute_command').never()
 
     assert (
         module.execute_dump_command(
@@ -331,15 +390,15 @@
             dry_run=True,
             dry_run_label='SO DRY',
         )
         is None
     )
 
 
-def test_execute_dump_command_with_dry_run_skips_mysqldump():
+def test_execute_dump_command_with_dry_run_skips_mariadb_dump():
     flexmock(module.dump).should_receive('make_data_source_dump_filename').and_return('dump')
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.dump).should_receive('create_named_pipe_for_dump')
 
     flexmock(module).should_receive('execute_command').never()
 
     assert (
@@ -375,20 +434,20 @@
         'databases/localhost/all'
     )
     flexmock(module).should_receive('database_names_to_dump').and_return(())
 
     assert module.dump_data_sources(databases, {}, 'test.yaml', dry_run=True) == []
 
 
-def test_restore_data_source_dump_runs_mysql_to_restore():
+def test_restore_data_source_dump_runs_mariadb_to_restore():
     hook_config = [{'name': 'foo'}, {'name': 'bar'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mysql', '--batch'),
+        ('mariadb', '--batch'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment=None,
     ).once()
 
     module.restore_data_source_dump(
@@ -403,20 +462,50 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mysql_with_options():
+def test_restore_data_source_dump_runs_mariadb_with_options():
     hook_config = [{'name': 'foo', 'restore_options': '--harder'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mysql', '--batch', '--harder'),
+        ('mariadb', '--batch', '--harder'),
+        processes=[extract_process],
+        output_log_level=logging.DEBUG,
+        input_file=extract_process.stdout,
+        extra_environment=None,
+    ).once()
+
+    module.restore_data_source_dump(
+        hook_config,
+        {},
+        'test.yaml',
+        data_source=hook_config[0],
+        dry_run=False,
+        extract_process=extract_process,
+        connection_params={
+            'hostname': None,
+            'port': None,
+            'username': None,
+            'password': None,
+        },
+    )
+
+
+def test_restore_data_source_dump_runs_non_default_mariadb_with_options():
+    hook_config = [
+        {'name': 'foo', 'restore_options': '--harder', 'mariadb_command': 'custom_mariadb'}
+    ]
+    extract_process = flexmock(stdout=flexmock())
+
+    flexmock(module).should_receive('execute_command_with_processes').with_args(
+        ('custom_mariadb', '--batch', '--harder'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment=None,
     ).once()
 
     module.restore_data_source_dump(
@@ -431,21 +520,21 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mysql_with_hostname_and_port():
+def test_restore_data_source_dump_runs_mariadb_with_hostname_and_port():
     hook_config = [{'name': 'foo', 'hostname': 'database.example.org', 'port': 5433}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mysql',
+            'mariadb',
             '--batch',
             '--host',
             'database.example.org',
             '--port',
             '5433',
             '--protocol',
             'tcp',
@@ -468,20 +557,20 @@
             'port': None,
             'username': None,
             'password': None,
         },
     )
 
 
-def test_restore_data_source_dump_runs_mysql_with_username_and_password():
+def test_restore_data_source_dump_runs_mariadb_with_username_and_password():
     hook_config = [{'name': 'foo', 'username': 'root', 'password': 'trustsome1'}]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
-        ('mysql', '--batch', '--user', 'root'),
+        ('mariadb', '--batch', '--user', 'root'),
         processes=[extract_process],
         output_log_level=logging.DEBUG,
         input_file=extract_process.stdout,
         extra_environment={'MYSQL_PWD': 'trustsome1'},
     ).once()
 
     module.restore_data_source_dump(
@@ -512,15 +601,15 @@
             'restore_password': 'restorepassword',
         }
     ]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mysql',
+            'mariadb',
             '--batch',
             '--host',
             'clihost',
             '--port',
             'cliport',
             '--protocol',
             'tcp',
@@ -533,15 +622,15 @@
         extra_environment={'MYSQL_PWD': 'clipassword'},
     ).once()
 
     module.restore_data_source_dump(
         hook_config,
         {},
         'test.yaml',
-        data_source={'name': 'foo'},
+        data_source=hook_config[0],
         dry_run=False,
         extract_process=extract_process,
         connection_params={
             'hostname': 'clihost',
             'port': 'cliport',
             'username': 'cliusername',
             'password': 'clipassword',
@@ -563,15 +652,15 @@
             'restore_port': 'restoreport',
         }
     ]
     extract_process = flexmock(stdout=flexmock())
 
     flexmock(module).should_receive('execute_command_with_processes').with_args(
         (
-            'mysql',
+            'mariadb',
             '--batch',
             '--host',
             'restorehost',
             '--port',
             'restoreport',
             '--protocol',
             'tcp',
```

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_ntfy.py` & `borgmatic-1.8.9/tests/unit/hooks/test_ntfy.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,60 @@
         'config.yaml',
         borgmatic.hooks.monitor.State.FAIL,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
-def test_ping_monitor_with_auth_hits_hosted_ntfy_on_fail():
+def test_ping_monitor_with_access_token_hits_hosted_ntfy_on_fail():
+    hook_config = {
+        'topic': topic,
+        'access_token': 'abc123',
+    }
+    flexmock(module.requests).should_receive('post').with_args(
+        f'{default_base_url}/{topic}',
+        headers=return_default_message_headers(borgmatic.hooks.monitor.State.FAIL),
+        auth=module.requests.auth.HTTPBasicAuth('', 'abc123'),
+    ).and_return(flexmock(ok=True)).once()
+
+    module.ping_monitor(
+        hook_config,
+        {},
+        'config.yaml',
+        borgmatic.hooks.monitor.State.FAIL,
+        monitoring_log_level=1,
+        dry_run=False,
+    )
+
+
+def test_ping_monitor_with_username_password_and_access_token_ignores_username_password():
+    hook_config = {
+        'topic': topic,
+        'username': 'testuser',
+        'password': 'fakepassword',
+        'access_token': 'abc123',
+    }
+    flexmock(module.requests).should_receive('post').with_args(
+        f'{default_base_url}/{topic}',
+        headers=return_default_message_headers(borgmatic.hooks.monitor.State.FAIL),
+        auth=module.requests.auth.HTTPBasicAuth('', 'abc123'),
+    ).and_return(flexmock(ok=True)).once()
+    flexmock(module.logger).should_receive('warning').once()
+
+    module.ping_monitor(
+        hook_config,
+        {},
+        'config.yaml',
+        borgmatic.hooks.monitor.State.FAIL,
+        monitoring_log_level=1,
+        dry_run=False,
+    )
+
+
+def test_ping_monitor_with_username_password_hits_hosted_ntfy_on_fail():
     hook_config = {
         'topic': topic,
         'username': 'testuser',
         'password': 'fakepassword',
     }
     flexmock(module.requests).should_receive('post').with_args(
         f'{default_base_url}/{topic}',
@@ -70,15 +115,15 @@
         'config.yaml',
         borgmatic.hooks.monitor.State.FAIL,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
-def test_ping_monitor_auth_with_no_username_warning():
+def test_ping_monitor_with_password_but_no_username_warns():
     hook_config = {'topic': topic, 'password': 'fakepassword'}
     flexmock(module.requests).should_receive('post').with_args(
         f'{default_base_url}/{topic}',
         headers=return_default_message_headers(borgmatic.hooks.monitor.State.FAIL),
         auth=None,
     ).and_return(flexmock(ok=True)).once()
     flexmock(module.logger).should_receive('warning').once()
@@ -89,15 +134,15 @@
         'config.yaml',
         borgmatic.hooks.monitor.State.FAIL,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
-def test_ping_monitor_auth_with_no_password_warning():
+def test_ping_monitor_with_username_but_no_password_warns():
     hook_config = {'topic': topic, 'username': 'testuser'}
     flexmock(module.requests).should_receive('post').with_args(
         f'{default_base_url}/{topic}',
         headers=return_default_message_headers(borgmatic.hooks.monitor.State.FAIL),
         auth=None,
     ).and_return(flexmock(ok=True)).once()
     flexmock(module.logger).should_receive('warning').once()
```

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_pagerduty.py` & `borgmatic-1.8.9/tests/unit/hooks/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_postgresql.py` & `borgmatic-1.8.9/tests/unit/hooks/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/hooks/test_sqlite.py` & `borgmatic-1.8.9/tests/unit/hooks/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/test_execute.py` & `borgmatic-1.8.9/tests/unit/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/test_logger.py` & `borgmatic-1.8.9/tests/unit/test_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,59 +65,92 @@
             },
         )
         is False
     )
 
 
 def test_should_do_markup_respects_PY_COLORS_environment_variable():
-    flexmock(module.os.environ).should_receive('get').and_return('True')
+    flexmock(module.os.environ).should_receive('get').with_args('PY_COLORS', None).and_return(
+        'True'
+    )
+    flexmock(module.os.environ).should_receive('get').with_args('NO_COLOR', None).and_return(None)
+
     flexmock(module).should_receive('to_bool').and_return(True)
 
     assert module.should_do_markup(no_color=False, configs={}) is True
 
 
 def test_should_do_markup_prefers_no_color_value_to_config_value():
     assert (
         module.should_do_markup(no_color=True, configs={'foo.yaml': {'output': {'color': True}}})
         is False
     )
 
 
-def test_should_do_markup_prefers_config_value_to_PY_COLORS():
+def test_should_do_markup_prefers_config_value_to_environment_variables():
     flexmock(module.os.environ).should_receive('get').and_return('True')
     flexmock(module).should_receive('to_bool').and_return(True)
 
     assert (
         module.should_do_markup(no_color=False, configs={'foo.yaml': {'output': {'color': False}}})
         is False
     )
 
 
-def test_should_do_markup_prefers_no_color_value_to_PY_COLORS():
+def test_should_do_markup_prefers_no_color_value_to_environment_variables():
     flexmock(module.os.environ).should_receive('get').and_return('True')
     flexmock(module).should_receive('to_bool').and_return(True)
 
     assert module.should_do_markup(no_color=True, configs={}) is False
 
 
 def test_should_do_markup_respects_interactive_console_value():
     flexmock(module.os.environ).should_receive('get').and_return(None)
     flexmock(module).should_receive('interactive_console').and_return(True)
 
     assert module.should_do_markup(no_color=False, configs={}) is True
 
 
 def test_should_do_markup_prefers_PY_COLORS_to_interactive_console_value():
-    flexmock(module.os.environ).should_receive('get').and_return('True')
+    flexmock(module.os.environ).should_receive('get').with_args('PY_COLORS', None).and_return(
+        'True'
+    )
+    flexmock(module.os.environ).should_receive('get').with_args('NO_COLOR', None).and_return(None)
     flexmock(module).should_receive('to_bool').and_return(True)
     flexmock(module).should_receive('interactive_console').and_return(False)
 
     assert module.should_do_markup(no_color=False, configs={}) is True
 
 
+def test_should_do_markup_prefers_NO_COLOR_to_interactive_console_value():
+    flexmock(module.os.environ).should_receive('get').with_args('PY_COLORS', None).and_return(None)
+    flexmock(module.os.environ).should_receive('get').with_args('NO_COLOR', None).and_return('True')
+    flexmock(module).should_receive('interactive_console').and_return(False)
+
+    assert module.should_do_markup(no_color=False, configs={}) is False
+
+
+def test_should_do_markup_respects_NO_COLOR_environment_variable():
+    flexmock(module.os.environ).should_receive('get').with_args('NO_COLOR', None).and_return('True')
+    flexmock(module.os.environ).should_receive('get').with_args('PY_COLORS', None).and_return(None)
+
+    assert module.should_do_markup(no_color=False, configs={}) is False
+
+
+def test_should_do_markup_prefers_NO_COLOR_to_PY_COLORS():
+    flexmock(module.os.environ).should_receive('get').with_args('PY_COLORS', None).and_return(
+        'True'
+    )
+    flexmock(module.os.environ).should_receive('get').with_args('NO_COLOR', None).and_return(
+        'SomeValue'
+    )
+
+    assert module.should_do_markup(no_color=False, configs={}) is False
+
+
 def test_multi_stream_handler_logs_to_handler_for_log_level():
     error_handler = flexmock()
     error_handler.should_receive('emit').once()
     info_handler = flexmock()
 
     multi_handler = module.Multi_stream_handler(
         {module.logging.ERROR: error_handler, module.logging.INFO: info_handler}
@@ -173,19 +206,17 @@
 
     module.add_logging_level('PLAID', 99)
 
 
 def test_configure_logging_with_syslog_log_level_probes_for_log_socket_on_linux():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
     flexmock(module).should_receive('Console_color_formatter')
     flexmock(module).should_receive('interactive_console').and_return(False)
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').with_args('/dev/log').and_return(True)
     syslog_handler = logging.handlers.SysLogHandler()
@@ -195,19 +226,17 @@
 
     module.configure_logging(logging.INFO, syslog_log_level=logging.DEBUG)
 
 
 def test_configure_logging_with_syslog_log_level_probes_for_log_socket_on_macos():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
     flexmock(module).should_receive('Console_color_formatter')
     flexmock(module).should_receive('interactive_console').and_return(False)
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').with_args('/dev/log').and_return(False)
     flexmock(module.os.path).should_receive('exists').with_args('/var/run/syslog').and_return(True)
@@ -218,19 +247,17 @@
 
     module.configure_logging(logging.INFO, syslog_log_level=logging.DEBUG)
 
 
 def test_configure_logging_with_syslog_log_level_probes_for_log_socket_on_freebsd():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
     flexmock(module).should_receive('Console_color_formatter')
     flexmock(module).should_receive('interactive_console').and_return(False)
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').with_args('/dev/log').and_return(False)
     flexmock(module.os.path).should_receive('exists').with_args('/var/run/syslog').and_return(False)
@@ -242,55 +269,49 @@
 
     module.configure_logging(logging.INFO, syslog_log_level=logging.DEBUG)
 
 
 def test_configure_logging_without_syslog_log_level_skips_syslog():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
     flexmock(module).should_receive('Console_color_formatter')
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.INFO, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').never()
     flexmock(module.logging.handlers).should_receive('SysLogHandler').never()
 
     module.configure_logging(console_log_level=logging.INFO)
 
 
 def test_configure_logging_skips_syslog_if_not_found():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
     flexmock(module).should_receive('Console_color_formatter')
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.INFO, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.logging.handlers).should_receive('SysLogHandler').never()
 
     module.configure_logging(console_log_level=logging.INFO, syslog_log_level=logging.DEBUG)
 
 
 def test_configure_logging_skips_log_file_if_log_file_logging_is_disabled():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).DISABLED = module.DISABLED
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
 
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.INFO, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').never()
     flexmock(module.logging.handlers).should_receive('SysLogHandler').never()
     flexmock(module.logging.handlers).should_receive('WatchedFileHandler').never()
@@ -299,19 +320,17 @@
         console_log_level=logging.INFO, log_file_log_level=logging.DISABLED, log_file='/tmp/logfile'
     )
 
 
 def test_configure_logging_to_log_file_instead_of_syslog():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
 
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').never()
     flexmock(module.logging.handlers).should_receive('SysLogHandler').never()
     file_handler = logging.handlers.WatchedFileHandler('/tmp/logfile')
@@ -326,19 +345,17 @@
         log_file='/tmp/logfile',
     )
 
 
 def test_configure_logging_to_both_log_file_and_syslog():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
 
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').with_args('/dev/log').and_return(True)
     syslog_handler = logging.handlers.SysLogHandler()
     flexmock(module.logging.handlers).should_receive('SysLogHandler').with_args(
@@ -359,19 +376,17 @@
 
 def test_configure_logging_to_log_file_formats_with_custom_log_format():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
     flexmock(module.logging).should_receive('Formatter').with_args(
         '{message}', style='{'  # noqa: FS003
     ).once()
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
 
     flexmock(module).should_receive('interactive_console').and_return(False)
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.DEBUG, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').with_args('/dev/log').and_return(True)
     flexmock(module.logging.handlers).should_receive('SysLogHandler').never()
@@ -387,20 +402,34 @@
         log_file_format='{message}',  # noqa: FS003
     )
 
 
 def test_configure_logging_skips_log_file_if_argument_is_none():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.ANSWER
-    flexmock(module).should_receive('Multi_stream_handler').and_return(
-        flexmock(
-            setFormatter=lambda formatter: None, setLevel=lambda level: None, level=logging.INFO
-        )
-    )
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').once()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
 
     flexmock(module.logging).should_receive('basicConfig').with_args(
         level=logging.INFO, handlers=list
     )
     flexmock(module.os.path).should_receive('exists').and_return(False)
     flexmock(module.logging.handlers).should_receive('WatchedFileHandler').never()
 
     module.configure_logging(console_log_level=logging.INFO, log_file=None)
+
+
+def test_configure_logging_skips_console_color_formatter_if_color_disabled():
+    flexmock(module).should_receive('add_custom_log_levels')
+    flexmock(module.logging).ANSWER = module.ANSWER
+    multi_stream_handler = flexmock(setLevel=lambda level: None, level=logging.INFO)
+    multi_stream_handler.should_receive('setFormatter').never()
+    flexmock(module).should_receive('Multi_stream_handler').and_return(multi_stream_handler)
+
+    flexmock(module.logging).should_receive('basicConfig').with_args(
+        level=logging.INFO, handlers=list
+    )
+    flexmock(module.os.path).should_receive('exists').and_return(False)
+    flexmock(module.logging.handlers).should_receive('WatchedFileHandler').never()
+
+    module.configure_logging(console_log_level=logging.INFO, log_file=None, color_enabled=False)
```

### Comparing `borgmatic-1.8.8/tests/unit/test_signals.py` & `borgmatic-1.8.9/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tests/unit/test_verbosity.py` & `borgmatic-1.8.9/tests/unit/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.8/tox.ini` & `borgmatic-1.8.9/tox.ini`

 * *Files identical despite different names*

