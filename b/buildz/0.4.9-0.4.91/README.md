# Comparing `tmp/buildz-0.4.9.tar.gz` & `tmp/buildz-0.4.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.9.tar", last modified: Sun Apr  7 19:01:44 2024, max compression
+gzip compressed data, was "buildz-0.4.91.tar", last modified: Tue Apr 16 14:14:44 2024, max compression
```

## Comparing `buildz-0.4.9.tar` & `buildz-0.4.91.tar`

### file list

```diff
@@ -1,132 +1,154 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.567186 buildz-0.4.9/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.9/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1896 2024-04-07 19:01:44.567186 buildz-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2024-04-07 18:00:18.000000 buildz-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.489056 buildz-0.4.9/buildz/
--rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.9/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.9/buildz/__main__.py
--rw-rw-rw-   0        0        0     1771 2024-04-02 17:23:58.000000 buildz-0.4.9/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.504685 buildz-0.4.9/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.504685 buildz-0.4.9/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.9/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.9/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.504685 buildz-0.4.9/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.4.9/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.9/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.504685 buildz-0.4.9/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.9/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.9/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.9/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.9/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.9/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.9/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.9/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.4.9/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.9/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.9/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      542 2024-04-02 16:54:56.000000 buildz-0.4.9/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.9/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.9/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.9/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.9/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.9/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.9/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.9/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.9/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.9/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.9/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.9/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.520322 buildz-0.4.9/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.9/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.9/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    12673 2024-04-02 14:42:14.000000 buildz-0.4.9/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.535934 buildz-0.4.9/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.9/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.9/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.9/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.551560 buildz-0.4.9/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.9/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.9/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.9/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.9/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.9/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.9/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.9/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.9/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.9/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.9/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.9/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.9/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.9/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1931 2024-04-07 18:52:48.000000 buildz-0.4.9/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.551560 buildz-0.4.9/buildz/tz/
--rw-rw-rw-   0        0        0      306 2024-04-07 18:50:02.000000 buildz-0.4.9/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.4.9/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.551560 buildz-0.4.9/buildz/xf/
--rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.9/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.9/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.551560 buildz-0.4.9/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.9/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.9/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.567186 buildz-0.4.9/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.9/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.9/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.9/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.9/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.9/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.9/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.9/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.9/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.9/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.9/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.9/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.9/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.9/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.9/buildz/xf/loader/pos.py
--rw-rw-rw-   0        0        0     1921 2024-04-02 14:13:24.000000 buildz-0.4.9/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.9/buildz/xf/read.py
--rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.9/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.567186 buildz-0.4.9/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.9/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.9/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.567186 buildz-0.4.9/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.9/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.9/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.9/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.9/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.9/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.9/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.9/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.9/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:01:44.504685 buildz-0.4.9/buildz.egg-info/
--rw-rw-rw-   0        0        0     1896 2024-04-07 19:01:44.000000 buildz-0.4.9/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2976 2024-04-07 19:01:44.000000 buildz-0.4.9/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 19:01:44.000000 buildz-0.4.9/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-07 19:01:44.000000 buildz-0.4.9/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 19:01:44.567186 buildz-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-07 19:01:19.000000 buildz-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.463063 buildz-0.4.91/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.91/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.91/MANIFEST.in
+-rw-rw-rw-   0        0        0     2706 2024-04-16 14:14:44.463063 buildz-0.4.91/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.4.91/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.897421 buildz-0.4.91/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.4.91/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.91/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.4.91/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.927921 buildz-0.4.91/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.937433 buildz-0.4.91/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.91/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.91/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.945025 buildz-0.4.91/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.4.91/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.91/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.960673 buildz-0.4.91/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.976337 buildz-0.4.91/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.91/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.91/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.91/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.91/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.91/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.006075 buildz-0.4.91/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.91/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.91/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.4.91/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.91/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.91/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.4.91/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.008084 buildz-0.4.91/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.91/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.91/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.91/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.008084 buildz-0.4.91/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.91/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.91/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.024110 buildz-0.4.91/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.91/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.91/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.91/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.91/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.039740 buildz-0.4.91/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.91/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.91/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.055524 buildz-0.4.91/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.91/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.91/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    12673 2024-04-16 13:23:38.000000 buildz-0.4.91/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.134876 buildz-0.4.91/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.91/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.91/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.214026 buildz-0.4.91/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.91/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.91/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.91/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.91/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.91/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.91/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.91/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.91/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1931 2024-04-07 18:52:48.000000 buildz-0.4.91/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.221451 buildz-0.4.91/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.4.91/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.4.91/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.247866 buildz-0.4.91/buildz/xf/
+-rw-rw-rw-   0        0        0      210 2024-04-16 13:29:45.000000 buildz-0.4.91/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.4.91/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.91/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.280399 buildz-0.4.91/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.4.91/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.4.91/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.318389 buildz-0.4.91/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.91/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.4.91/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.91/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.91/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.91/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.4.91/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.4.91/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.4.91/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.91/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.4.91/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.91/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.4.91/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.4.91/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.4.91/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.357098 buildz-0.4.91/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.4.91/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.4.91/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.404072 buildz-0.4.91/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.4.91/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.4.91/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.4.91/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.4.91/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.4.91/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.4.91/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.4.91/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.4.91/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.4.91/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.4.91/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.91/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.4.91/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     2838 2024-04-16 10:04:19.000000 buildz-0.4.91/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.4.91/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1687 2024-04-16 14:12:03.000000 buildz-0.4.91/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0     2009 2024-04-10 16:50:01.000000 buildz-0.4.91/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.4.91/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2525 2024-04-16 13:29:30.000000 buildz-0.4.91/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.4.91/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.91/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.430238 buildz-0.4.91/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.91/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.91/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.461697 buildz-0.4.91/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.91/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.91/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.91/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.91/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.91/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.91/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.91/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.4.91/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.922962 buildz-0.4.91/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2706 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3526 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:14:44.463063 buildz-0.4.91/setup.cfg
+-rw-rw-rw-   0        0        0      771 2024-04-16 13:30:05.000000 buildz-0.4.91/setup.py
```

### Comparing `buildz-0.4.9/LICENSE` & `buildz-0.4.91/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/PKG-INFO` & `buildz-0.4.91/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: buildz
-Version: 0.4.9
-Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
-Home-page: https://github.com/buildCodeZ/buildz
-Author: Zzz
-Author-email: 1309458652@qq.com
-License: Apache License 2.0
-Keywords: buildz
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # buildz
 ```
 1，在json格式基础上加了点东西，让配置文件写起来更简单，模块在buildz.xf下
 2，基于xf格式写了个ioc控制反转配置文件读取的程序，模块在buildz.ioc下
 3，其他工具模块：
     buildz.fz: 文件夹查找
     buildz.pyz: 简化python __import__调用
@@ -24,22 +11,26 @@
 代码关系:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
     buildz.ioc需要buildz.xf和buildz.pyz
     buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
+PS: 对比了下json.loads（修改了下json的scanner.py，让它在纯python下运行，不然json.loads会更快）和目前的xf.loads(buildz.xf.readz.loads)的速度，xf.loads比json.loads慢7倍，可能是读字符串更频繁，方法调用更多（为了代码更结构化和容易修改），其实有一版更慢(buildz.xf.read.loads，废弃代码，后面看情况删掉)，慢100倍，因为只考虑结构化，没考虑列表增减开销
+
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
     buildz.argx: read command argument in special format
     buildz.demo: example codes to use buildz, run "python -m buildz" will use this module
 code relationship:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
     buildz.ioc use buildz.xf and buildz.pyz
     buildz.tz: some tools, only contains "myerse diff algorithm" now
     buildz.demo use all other modules
 
 run python -m buildz to see help
+
+PS: testing speed on json.loads(has modified scanner.py in json module to make it purely run on Python, which make it run slower) and xf.loads(real func is buildz.xf.readz.loads), xf.loads takes 7 times longer than json.loads, it may cost by more func calls and more string cutting and reading(to make codes more structuring and easier to update)
 ```
```

### Comparing `buildz-0.4.9/buildz/demo/ioc/deal.py` & `buildz-0.4.91/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/ioc/help.py` & `buildz-0.4.91/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/myers/deal.py` & `buildz-0.4.91/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/res/conf/main.js` & `buildz-0.4.91/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/res/help/ioc.js` & `buildz-0.4.91/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/res/help/myers.js` & `buildz-0.4.91/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/res/help/search.js` & `buildz-0.4.91/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/res/help/xf.js` & `buildz-0.4.91/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/search/deal.py` & `buildz-0.4.91/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/demo/test.py` & `buildz-0.4.91/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/fz/dirz.py` & `buildz-0.4.91/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/fz/fio.py` & `buildz-0.4.91/buildz/fz/fio.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/fz/lsf.py` & `buildz-0.4.91/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc/base.py` & `buildz-0.4.91/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc/conf.py` & `buildz-0.4.91/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc/confs.py` & `buildz-0.4.91/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/base.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/call.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/calls.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.4.91/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/env.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/join.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/list.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/map.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/obj.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/ref.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/val.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/ioc/ioc_deal/var.py` & `buildz-0.4.91/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/pyz.py` & `buildz-0.4.91/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/tz/myers_diff.py` & `buildz-0.4.91/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/file.py` & `buildz-0.4.91/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/base.py` & `buildz-0.4.91/buildz/xf/loader/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 
 class BaseDeal:
+    def has_prev(self):
+        return 1
+    def has_deal(self):
+        return 1
     def sp(self):
         return super(self.__class__, self)
     def regist(self, mgs):
         if self._id is None:
             self._id = mgs.regist()
     def id(self):
         return self._id
```

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/listz.py` & `buildz-0.4.91/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/lr.py` & `buildz-0.4.91/buildz/xf/loader/deal/lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             return False
         if self.same(self.left, cl):
             buffer.pop_read(self.ll)
             rm = buffer.full()
             if len(rm.strip())>0:
                 pos.update(rm)
                 raise exp.FormatExp(self.err("unexcept char before <lr> left symbol"), pos.get(), rm)
+            buffer.clean()
             pos.update(cl)
             queue.append(item.PrevItem(cl, pos.get(), self.id(), left = 1))
         else:
             buffer.pop_read(self.lr)
             rm = buffer.full()
             buffer.clean()
             pos.update(rm)
```

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/lrval.py` & `buildz-0.4.91/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/mapz.py` & `buildz-0.4.91/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/nextz.py` & `buildz-0.4.91/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/reval.py` & `buildz-0.4.91/buildz/xf/loader/deal/reval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from .. import base
 from .. import item
 from .. import exp
 from . import lr
 import re
 class ValDeal(base.BaseDeal):
+    def has_prev(self):
+        return 0
+    def has_deal(self):
+        return 1
     """
         正则表达式匹配
     """
     def init(self, pt, fc):
         st = self.like("^", pt)
         ed = self.like("$", pt)
         if pt[0]!=st:
```

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/setz.py` & `buildz-0.4.91/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/spt.py` & `buildz-0.4.91/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/deal/strz.py` & `buildz-0.4.91/buildz/xf/loader/deal/strz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from .. import base
 from .. import item
 from .. import exp
 from ... import file
 import json
 class PrevStrDeal(base.BaseDeal):
+    def has_prev(self):
+        return 1
+    def has_deal(self):
+        return 0
     def init(self, left = '"', right= '"', single_line = False, note = False, translate = False):
         self.left = left
         self.right = right
         self.ll = len(left)
         self.lr = len(right)
         self.single_line = single_line
         self.note = note
@@ -67,14 +71,15 @@
                 c = buffer.read(1,1)
                 if len(c)==0:
                     pos.update(tmp)
                     raise exp.FormatExp("unexcept file end while reading string", pos.get())
                 tmp += c
                 continue
             ctmp+=c
+        buffer.clean()
         xtmp = tmp[:-self.lr]
         if not self.note and self.single_line and xtmp.find(self.like("\n", xtmp))>=0:
             print("left:",self.left, "right:", self.right)
             raise exp.FormatExp("contain enter in single line string", pos.get(), tmp)
         if self.translate:
             xtmp = self.do_translate(xtmp)
         curr_pos = pos.get()
```

### Comparing `buildz-0.4.9/buildz/xf/loader/item.py` & `buildz-0.4.91/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/loader/mg.py` & `buildz-0.4.91/buildz/xf/loader/mg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 
 from . import buffer
 from . import base
 from . import pos
 from . import exp
+from ..stack import Stack
 class Manager:
     def fcs(self, fc, *args, **maps):
         return fc(*self.cs(*args), **maps)
     def add_fc(self, fc, *args, **maps):
         obj = self.fcs(fc, *args, **maps)
         self.add(obj)
         return self
     def cs(self, *args):
         return [self.c(k) for k in args]
     def c(self, s):
         if self.bts:
             s = s.encode(self.code)
         return s
+    # 上面这些没用
     def add(self,obj):
         #obj.init()
         obj.regist(self)
-        self.prevs.append(obj.prev)
-        self.deals.append(obj.deal)
+        if obj.has_prev():
+            self.prevs.append(obj.prev)
+        if obj.has_deal():
+            self.deals.append(obj.deal)
         return self
     def do(self, fcs, *argv, **maps):
         for fc in fcs:
             if fc(*argv, **maps):
                 return True
         return False
     def regist(self):
@@ -32,29 +36,47 @@
         self.index+=1
         return "id_"+str(id)
     def __init__(self):
         self.index = 0
         self.deals = []
         self.prevs = []
     def load(self, reader):
-        buff = buffer.Buffer(reader)
+        if type(reader) in [str, bytes]:
+            #print(f"try str, {len(reader)}")
+            buff = buffer.StrBuffer(reader)
+            s = reader.replace(" ", "")
+            queue = Stack(len(s)+1)
+        else:
+            buff = buffer.Buffer(reader)
+            queue = []
         _pos = pos.PosCal()
-        queue = []
         self.pos = _pos
         self.buffer = buff
         self.queue = queue
+        import time
+        crr = time.time()
         while self.do(self.prevs, buff, queue, _pos):
             pass
-        stack = []
+        now = time.time()
+        #print(f"prev time: {now - crr}, prevs: {len(self.prevs)}, queue: {len(queue)}")
+        #stack = []
+        stack = Stack(len(queue))
+        #stack = []
+        crr = time.time()
+        ns = 0
         while self.do(self.deals, queue, stack):
+            ns = max(len(stack), ns)
             pass
+        now = time.time()
+        #print(f"deal time: {now - crr}, deals: {len(self.deals)}, stack: {ns}")
         if len(stack)==0:
             raise Exception("ERROR not data")
         for _item in stack:
             if not _item.check(is_val=1):
+                print(f"err item: {_item}")
                 raise exp.FormatExp("format error found", _item.pos)
         if len(stack)==1:
             return stack[0].val
         else:
             return [it.val for it in stack]
 
 pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildz-0.4.9/buildz/xf/loader/pos.py` & `buildz-0.4.91/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/mapz.py` & `buildz-0.4.91/buildz/xf/mapz.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,20 @@
             v = obj[k]
         rst.append(v)
     if len(rst)==1:
         rst = rst[0]
     return rst
 
 pass
+def s(obj, **maps):
+    for k in maps:
+        v = maps[k]
+        obj[k] = v
 
+pass
 def sets(maps, keys, val):
     if type(keys) != list:
         keys = [keys]
     for key in keys[:-1]:
         if key not in maps:
             maps[key] = {}
         maps = maps[key]
```

### Comparing `buildz-0.4.9/buildz/xf/read.py` & `buildz-0.4.91/buildz/xf/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,10 +77,10 @@
     #     lr = lr.encode()
     #     ls = ls.encode()
     # x = s.strip()
     # if len(x)>0 and x[0] not in ls:
     #     s = lr[0]+s+lr[1]
     mgs = build()
     input = buffer.BufferInput(s)
-    return mgs.load(input)
+    return mgs.load(s)
 
 pass
```

### Comparing `buildz-0.4.9/buildz/xf/write.py` & `buildz-0.4.91/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/base.py` & `buildz-0.4.91/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/conf.py` & `buildz-0.4.91/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/deal/listz.py` & `buildz-0.4.91/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/deal/mapz.py` & `buildz-0.4.91/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/deal/strz.py` & `buildz-0.4.91/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/itemz.py` & `buildz-0.4.91/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz/xf/writer/mg.py` & `buildz-0.4.91/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.9/buildz.egg-info/PKG-INFO` & `buildz-0.4.91/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.9
+Version: 0.4.91
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
@@ -24,22 +24,26 @@
 代码关系:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
     buildz.ioc需要buildz.xf和buildz.pyz
     buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
+PS: 对比了下json.loads（修改了下json的scanner.py，让它在纯python下运行，不然json.loads会更快）和目前的xf.loads(buildz.xf.readz.loads)的速度，xf.loads比json.loads慢7倍，可能是读字符串更频繁，方法调用更多（为了代码更结构化和容易修改），其实有一版更慢(buildz.xf.read.loads，废弃代码，后面看情况删掉)，慢100倍，因为只考虑结构化，没考虑列表增减开销
+
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
     buildz.argx: read command argument in special format
     buildz.demo: example codes to use buildz, run "python -m buildz" will use this module
 code relationship:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
     buildz.ioc use buildz.xf and buildz.pyz
     buildz.tz: some tools, only contains "myerse diff algorithm" now
     buildz.demo use all other modules
 
 run python -m buildz to see help
+
+PS: testing speed on json.loads(has modified scanner.py in json module to make it purely run on Python, which make it run slower) and xf.loads(real func is buildz.xf.readz.loads), xf.loads takes 7 times longer than json.loads, it may cost by more func calls and more string cutting and reading(to make codes more structuring and easier to update)
 ```
```

### Comparing `buildz-0.4.9/buildz.egg-info/SOURCES.txt` & `buildz-0.4.91/buildz.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -72,17 +72,20 @@
 buildz/ioc/ioc_deal/conf/obj_set_lists.js
 buildz/ioc/ioc_deal/conf/ovar_lists.js
 buildz/ioc/ioc_deal/conf/ref_lists.js
 buildz/ioc/ioc_deal/conf/var_lists.js
 buildz/tz/__init__.py
 buildz/tz/myers_diff.py
 buildz/xf/__init__.py
+buildz/xf/__main__.py
 buildz/xf/file.py
 buildz/xf/mapz.py
 buildz/xf/read.py
+buildz/xf/readz.py
+buildz/xf/stack.py
 buildz/xf/write.py
 buildz/xf/xargs.py
 buildz/xf/loader/base.py
 buildz/xf/loader/buffer.py
 buildz/xf/loader/exp.py
 buildz/xf/loader/item.py
 buildz/xf/loader/mg.py
@@ -93,14 +96,31 @@
 buildz/xf/loader/deal/mapz.py
 buildz/xf/loader/deal/nextz.py
 buildz/xf/loader/deal/reval.py
 buildz/xf/loader/deal/setz.py
 buildz/xf/loader/deal/spc.py
 buildz/xf/loader/deal/spt.py
 buildz/xf/loader/deal/strz.py
+buildz/xf/loaderz/base.py
+buildz/xf/loaderz/buffer.py
+buildz/xf/loaderz/exp.py
+buildz/xf/loaderz/item.py
+buildz/xf/loaderz/mg.py
+buildz/xf/loaderz/pos.py
+buildz/xf/loaderz/test.py
+buildz/xf/loaderz/deal/listz.py
+buildz/xf/loaderz/deal/lr.py
+buildz/xf/loaderz/deal/lrval.py
+buildz/xf/loaderz/deal/mapz.py
+buildz/xf/loaderz/deal/nextz.py
+buildz/xf/loaderz/deal/reval.py
+buildz/xf/loaderz/deal/setz.py
+buildz/xf/loaderz/deal/spc.py
+buildz/xf/loaderz/deal/spt.py
+buildz/xf/loaderz/deal/strz.py
 buildz/xf/writer/base.py
 buildz/xf/writer/conf.py
 buildz/xf/writer/itemz.py
 buildz/xf/writer/mg.py
 buildz/xf/writer/deal/jsonval.py
 buildz/xf/writer/deal/listz.py
 buildz/xf/writer/deal/mapz.py
```

### Comparing `buildz-0.4.9/setup.py` & `buildz-0.4.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.9',
+    version = '0.4.91',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

