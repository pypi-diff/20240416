# Comparing `tmp/Tailbone-0.9.90.tar.gz` & `tmp/tailbone-0.9.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tailbone-0.9.90.tar", last modified: Mon Apr  1 23:28:51 2024, max compression
+gzip compressed data, was "tailbone-0.9.91.tar", last modified: Mon Apr 15 15:57:40 2024, max compression
```

## Comparing `Tailbone-0.9.90.tar` & `tailbone-0.9.91.tar`

### file list

```diff
@@ -1,516 +1,513 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/
--rw-r--r--   0 lance     (1000) lance     (1000)   159981 2024-04-01 23:28:19.000000 Tailbone-0.9.90/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 Tailbone-0.9.90/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 Tailbone-0.9.90/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-01 23:28:51.293865 Tailbone-0.9.90/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 Tailbone-0.9.90/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/Tailbone.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)    14878 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      272 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)      448 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        9 2024-04-01 23:28:51.000000 Tailbone-0.9.90/Tailbone.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     2128 2024-04-01 23:28:51.293865 Tailbone-0.9.90/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 20:02:32.000000 Tailbone-0.9.90/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/
--rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       49 2024-04-01 23:28:24.000000 Tailbone-0.9.90/tailbone/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/api/
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 Tailbone-0.9.90/tailbone/api/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7865 2023-05-17 04:11:43.000000 Tailbone-0.9.90/tailbone/api/auth.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/api/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 Tailbone-0.9.90/tailbone/api/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12760 2023-11-02 00:42:53.000000 Tailbone-0.9.90/tailbone/api/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7150 2023-11-15 15:46:15.000000 Tailbone-0.9.90/tailbone/api/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 Tailbone-0.9.90/tailbone/api/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11602 2023-09-17 22:23:51.000000 Tailbone-0.9.90/tailbone/api/batch/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20393 2023-11-02 00:43:37.000000 Tailbone-0.9.90/tailbone/api/batch/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5099 2023-05-17 04:34:48.000000 Tailbone-0.9.90/tailbone/api/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4643 2023-06-17 03:15:35.000000 Tailbone-0.9.90/tailbone/api/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 Tailbone-0.9.90/tailbone/api/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1202 2023-05-20 00:29:29.000000 Tailbone-0.9.90/tailbone/api/essentials.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 Tailbone-0.9.90/tailbone/api/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21938 2023-10-08 17:24:00.000000 Tailbone-0.9.90/tailbone/api/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 Tailbone-0.9.90/tailbone/api/master2.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 Tailbone-0.9.90/tailbone/api/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7461 2023-09-02 15:55:47.000000 Tailbone-0.9.90/tailbone/api/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 Tailbone-0.9.90/tailbone/api/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2181 2023-05-03 00:13:09.000000 Tailbone-0.9.90/tailbone/api/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 Tailbone-0.9.90/tailbone/api/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 Tailbone-0.9.90/tailbone/api/workorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11334 2023-10-24 01:35:10.000000 Tailbone-0.9.90/tailbone/app.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 Tailbone-0.9.90/tailbone/asgi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6324 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 Tailbone-0.9.90/tailbone/beaker.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 Tailbone-0.9.90/tailbone/cleanup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2931 2023-11-02 00:44:30.000000 Tailbone-0.9.90/tailbone/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 Tailbone-0.9.90/tailbone/db.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9796 2023-12-01 00:13:00.000000 Tailbone-0.9.90/tailbone/diffs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 Tailbone-0.9.90/tailbone/exceptions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)     1107 2023-09-17 00:47:36.000000 Tailbone-0.9.90/tailbone/forms/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 Tailbone-0.9.90/tailbone/forms/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)    49488 2024-03-26 17:53:16.000000 Tailbone-0.9.90/tailbone/forms/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2361 2023-08-29 21:08:45.000000 Tailbone-0.9.90/tailbone/forms/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7041 2023-10-09 20:50:24.000000 Tailbone-0.9.90/tailbone/forms/types.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20440 2023-12-02 01:47:37.000000 Tailbone-0.9.90/tailbone/forms/widgets.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 Tailbone-0.9.90/tailbone/grids/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    70611 2024-03-26 16:48:40.000000 Tailbone-0.9.90/tailbone/grids/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    40585 2023-12-11 19:49:51.000000 Tailbone-0.9.90/tailbone/grids/filters.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 Tailbone-0.9.90/tailbone/handler.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1883 2023-05-05 02:26:43.000000 Tailbone-0.9.90/tailbone/helpers.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29626 2023-10-29 20:45:59.000000 Tailbone-0.9.90/tailbone/menus.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 Tailbone-0.9.90/tailbone/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 Tailbone-0.9.90/tailbone/providers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.253864 Tailbone-0.9.90/tailbone/reports/
--rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/reports/inventory_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/reports/ordering_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/scaffolds.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.257864 Tailbone-0.9.90/tailbone/static/
--rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/static/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.257864 Tailbone-0.9.90/tailbone/static/css/
--rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 Tailbone-0.9.90/tailbone/static/css/base.css
--rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 Tailbone-0.9.90/tailbone/static/css/codehilite.css
--rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 Tailbone-0.9.90/tailbone/static/css/diffs.css
--rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 Tailbone-0.9.90/tailbone/static/css/filters.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 Tailbone-0.9.90/tailbone/static/css/forms.css
--rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 Tailbone-0.9.90/tailbone/static/css/grids.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1173 2023-02-02 22:24:46.000000 Tailbone-0.9.90/tailbone/static/css/grids.rowstatus.css
--rw-r--r--   0 lance     (1000) lance     (1000)     2671 2023-10-25 15:44:50.000000 Tailbone-0.9.90/tailbone/static/css/layout.css
--rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/css/normalize.css
--rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 Tailbone-0.9.90/tailbone/static/css/perms.css
--rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 Tailbone-0.9.90/tailbone/static/css/progress.css
--rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/static/css/purchases.css
--rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/static/css/schedule_print.css
--rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 Tailbone-0.9.90/tailbone/static/css/timesheet.css
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.257864 Tailbone-0.9.90/tailbone/static/files/
--rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 Tailbone-0.9.90/tailbone/static/files/newproduct_template.xlsx
--rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 Tailbone-0.9.90/tailbone/static/files/vendor_catalog_template.xlsx
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.257864 Tailbone-0.9.90/tailbone/static/img/
--rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/Hymenocephalus_italicus.jpg
--rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/delete.png
--rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/edit.png
--rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/home_logo.png
--rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/loading.gif
--rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/static/img/product.png
--rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/rattail.ico
--rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 Tailbone-0.9.90/tailbone/static/img/save.png
--rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/sort_arrow_down.png
--rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/sort_arrow_up.png
--rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 Tailbone-0.9.90/tailbone/static/img/testing.png
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 Tailbone-0.9.90/tailbone/static/img/view.png
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.257864 Tailbone-0.9.90/tailbone/static/js/
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 Tailbone-0.9.90/tailbone/static/js/debounce.js
--rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/static/js/numeric.js
--rw-r--r--   0 lance     (1000) lance     (1000)     9498 2023-10-26 01:03:48.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.autocomplete.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.datepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     4561 2023-06-16 17:21:44.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.grid.js
--rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.message_recipients.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.numericinput.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.oncebutton.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1403 2023-09-17 00:42:09.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.timepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1427 2023-06-06 16:53:17.000000 Tailbone-0.9.90/tailbone/static/js/tailbone.feedback.js
--rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/static/robots.txt
--rw-r--r--   0 lance     (1000) lance     (1000)    10327 2023-11-01 13:09:36.000000 Tailbone-0.9.90/tailbone/subscribers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/
--rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 Tailbone-0.9.90/tailbone/templates/about.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/appinfo/
--rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 Tailbone-0.9.90/tailbone/templates/appinfo/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3270 2023-10-24 14:53:32.000000 Tailbone-0.9.90/tailbone/templates/appinfo/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6314 2023-02-03 05:54:56.000000 Tailbone-0.9.90/tailbone/templates/appsettings.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 Tailbone-0.9.90/tailbone/templates/autocomplete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    33683 2023-11-17 23:00:34.000000 Tailbone-0.9.90/tailbone/templates/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 Tailbone-0.9.90/tailbone/templates/base_meta.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/batch/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 Tailbone-0.9.90/tailbone/templates/batch/edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/batch/importer/
--rw-r--r--   0 lance     (1000) lance     (1000)     2387 2023-02-03 05:42:46.000000 Tailbone-0.9.90/tailbone/templates/batch/importer/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 Tailbone-0.9.90/tailbone/templates/batch/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/batch/inventory/
--rw-r--r--   0 lance     (1000) lance     (1000)    10312 2023-10-06 20:50:38.000000 Tailbone-0.9.90/tailbone/templates/batch/inventory/desktop_form.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/batch/newproduct/
--rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 Tailbone-0.9.90/tailbone/templates/batch/newproduct/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.261864 Tailbone-0.9.90/tailbone/templates/batch/pos/
--rw-r--r--   0 lance     (1000) lance     (1000)      285 2023-10-07 04:17:54.000000 Tailbone-0.9.90/tailbone/templates/batch/pos/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/batch/pricing/
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 Tailbone-0.9.90/tailbone/templates/batch/pricing/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/
--rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      247 2022-01-06 20:44:32.000000 Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11873 2023-02-03 05:50:11.000000 Tailbone-0.9.90/tailbone/templates/batch/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 Tailbone-0.9.90/tailbone/templates/batch/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 Tailbone-0.9.90/tailbone/templates/change_password.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 Tailbone-0.9.90/tailbone/templates/configure-menus.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 Tailbone-0.9.90/tailbone/templates/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/customers/
--rw-r--r--   0 lance     (1000) lance     (1000)     3775 2023-06-11 18:38:46.000000 Tailbone-0.9.90/tailbone/templates/customers/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/customers/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 Tailbone-0.9.90/tailbone/templates/customers/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1215 2023-10-12 04:47:13.000000 Tailbone-0.9.90/tailbone/templates/customers/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     6522 2023-10-25 00:29:26.000000 Tailbone-0.9.90/tailbone/templates/custorders/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    92495 2023-10-26 14:28:39.000000 Tailbone-0.9.90/tailbone/templates/custorders/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/custorders/items/
--rw-r--r--   0 lance     (1000) lance     (1000)    16046 2023-09-12 17:35:33.000000 Tailbone-0.9.90/tailbone/templates/custorders/items/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       81 2023-09-10 19:59:06.000000 Tailbone-0.9.90/tailbone/templates/custorders/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/datasync/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.265864 Tailbone-0.9.90/tailbone/templates/datasync/changes/
--rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 Tailbone-0.9.90/tailbone/templates/datasync/changes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 Tailbone-0.9.90/tailbone/templates/datasync/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 Tailbone-0.9.90/tailbone/templates/datasync/status.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/deform/
--rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 Tailbone-0.9.90/tailbone/templates/deform/autocomplete_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 Tailbone-0.9.90/tailbone/templates/deform/cases_units.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 Tailbone-0.9.90/tailbone/templates/deform/checkbox.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 Tailbone-0.9.90/tailbone/templates/deform/checkbox_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 Tailbone-0.9.90/tailbone/templates/deform/checked_password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 Tailbone-0.9.90/tailbone/templates/deform/date_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 Tailbone-0.9.90/tailbone/templates/deform/date_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      543 2023-09-17 01:00:05.000000 Tailbone-0.9.90/tailbone/templates/deform/datetime_falafel.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 Tailbone-0.9.90/tailbone/templates/deform/file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 Tailbone-0.9.90/tailbone/templates/deform/message_recipients_buefy.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 Tailbone-0.9.90/tailbone/templates/deform/multi_file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/deform/numberinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 Tailbone-0.9.90/tailbone/templates/deform/numericinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 Tailbone-0.9.90/tailbone/templates/deform/password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 Tailbone-0.9.90/tailbone/templates/deform/percentinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 Tailbone-0.9.90/tailbone/templates/deform/permissions.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 Tailbone-0.9.90/tailbone/templates/deform/problem_report_days.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 Tailbone-0.9.90/tailbone/templates/deform/select.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1177 2023-08-08 19:10:04.000000 Tailbone-0.9.90/tailbone/templates/deform/select_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/deform/select_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 Tailbone-0.9.90/tailbone/templates/deform/select_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      550 2023-03-23 15:17:29.000000 Tailbone-0.9.90/tailbone/templates/deform/textarea.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 Tailbone-0.9.90/tailbone/templates/deform/textinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      230 2023-09-26 00:21:51.000000 Tailbone-0.9.90/tailbone/templates/deform/time_falafel.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 Tailbone-0.9.90/tailbone/templates/deform/time_jquery.pt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/departments/
--rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 Tailbone-0.9.90/tailbone/templates/departments/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      551 2023-10-09 05:16:53.000000 Tailbone-0.9.90/tailbone/templates/diff.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/email-bounces/
--rw-r--r--   0 lance     (1000) lance     (1000)     1659 2023-09-08 15:46:55.000000 Tailbone-0.9.90/tailbone/templates/email-bounces/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/employees/
--rw-r--r--   0 lance     (1000) lance     (1000)      626 2023-06-11 04:11:26.000000 Tailbone-0.9.90/tailbone/templates/employees/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 Tailbone-0.9.90/tailbone/templates/employees/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/exception.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1493 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/templates/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2779 2023-06-17 19:13:31.000000 Tailbone-0.9.90/tailbone/templates/formposter.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)     7047 2023-10-05 18:09:53.000000 Tailbone-0.9.90/tailbone/templates/forms/deform_buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       67 2023-02-03 05:36:08.000000 Tailbone-0.9.90/tailbone/templates/forms/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      265 2022-08-09 03:19:59.000000 Tailbone-0.9.90/tailbone/templates/forms/util.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 Tailbone-0.9.90/tailbone/templates/generate_feature.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/generated-projects/
--rw-r--r--   0 lance     (1000) lance     (1000)      582 2023-05-04 18:51:55.000000 Tailbone-0.9.90/tailbone/templates/generated-projects/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 Tailbone-0.9.90/tailbone/templates/grids/b-table.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    28295 2023-10-11 03:10:01.000000 Tailbone-0.9.90/tailbone/templates/grids/buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1573 2019-05-06 23:17:43.000000 Tailbone-0.9.90/tailbone/templates/grids/filters.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1898 2023-10-11 03:10:01.000000 Tailbone-0.9.90/tailbone/templates/grids/filters_buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/grids/nav.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 Tailbone-0.9.90/tailbone/templates/home.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/ifps-plu-codes/
--rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 Tailbone-0.9.90/tailbone/templates/ifps-plu-codes/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.269864 Tailbone-0.9.90/tailbone/templates/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 Tailbone-0.9.90/tailbone/templates/importing/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 Tailbone-0.9.90/tailbone/templates/importing/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 Tailbone-0.9.90/tailbone/templates/importing/runjob.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 Tailbone-0.9.90/tailbone/templates/importing/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.249864 Tailbone-0.9.90/tailbone/templates/labels/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/labels/profiles/
--rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/templates/labels/profiles/create.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/templates/labels/profiles/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 Tailbone-0.9.90/tailbone/templates/labels/profiles/printer.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 Tailbone-0.9.90/tailbone/templates/labels/profiles/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 Tailbone-0.9.90/tailbone/templates/login.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/luigi/
--rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 Tailbone-0.9.90/tailbone/templates/luigi/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 Tailbone-0.9.90/tailbone/templates/luigi/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/master/
--rw-r--r--   0 lance     (1000) lance     (1000)     1376 2023-02-03 05:30:32.000000 Tailbone-0.9.90/tailbone/templates/master/clone.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 Tailbone-0.9.90/tailbone/templates/master/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 Tailbone-0.9.90/tailbone/templates/master/create.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/templates/master/create_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1401 2023-02-03 05:26:22.000000 Tailbone-0.9.90/tailbone/templates/master/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      226 2023-10-10 02:06:31.000000 Tailbone-0.9.90/tailbone/templates/master/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 Tailbone-0.9.90/tailbone/templates/master/edit_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 Tailbone-0.9.90/tailbone/templates/master/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 Tailbone-0.9.90/tailbone/templates/master/import_file.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    25083 2023-09-15 18:45:55.000000 Tailbone-0.9.90/tailbone/templates/master/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5560 2023-06-19 02:20:45.000000 Tailbone-0.9.90/tailbone/templates/master/merge.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1033 2023-02-03 22:16:07.000000 Tailbone-0.9.90/tailbone/templates/master/versions.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11299 2023-10-23 20:28:04.000000 Tailbone-0.9.90/tailbone/templates/master/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 Tailbone-0.9.90/tailbone/templates/master/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1413 2023-10-10 15:07:41.000000 Tailbone-0.9.90/tailbone/templates/master/view_version.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/members/
--rw-r--r--   0 lance     (1000) lance     (1000)     2342 2023-08-26 14:11:45.000000 Tailbone-0.9.90/tailbone/templates/members/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      262 2023-06-14 19:01:14.000000 Tailbone-0.9.90/tailbone/templates/members/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 Tailbone-0.9.90/tailbone/templates/menu.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/messages/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/messages/archive/
--rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 Tailbone-0.9.90/tailbone/templates/messages/archive/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1777 2023-03-23 15:22:59.000000 Tailbone-0.9.90/tailbone/templates/messages/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/messages/inbox/
--rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 Tailbone-0.9.90/tailbone/templates/messages/inbox/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 Tailbone-0.9.90/tailbone/templates/messages/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 Tailbone-0.9.90/tailbone/templates/messages/recipients.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/messages/sent/
--rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 Tailbone-0.9.90/tailbone/templates/messages/sent/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 Tailbone-0.9.90/tailbone/templates/messages/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 Tailbone-0.9.90/tailbone/templates/multi_file_upload.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.273864 Tailbone-0.9.90/tailbone/templates/ordering/
--rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 Tailbone-0.9.90/tailbone/templates/ordering/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 Tailbone-0.9.90/tailbone/templates/ordering/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 Tailbone-0.9.90/tailbone/templates/ordering/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1813 2023-08-28 02:36:03.000000 Tailbone-0.9.90/tailbone/templates/page.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 Tailbone-0.9.90/tailbone/templates/page_help.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/people/
--rw-r--r--   0 lance     (1000) lance     (1000)     1296 2023-06-17 19:36:29.000000 Tailbone-0.9.90/tailbone/templates/people/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 Tailbone-0.9.90/tailbone/templates/people/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/people/merge-requests/
--rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 Tailbone-0.9.90/tailbone/templates/people/merge-requests/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1106 2023-02-03 05:39:41.000000 Tailbone-0.9.90/tailbone/templates/people/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    84972 2024-04-01 23:03:00.000000 Tailbone-0.9.90/tailbone/templates/people/view_profile_buefy.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/poser/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/poser/reports/
--rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 Tailbone-0.9.90/tailbone/templates/poser/reports/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 Tailbone-0.9.90/tailbone/templates/poser/setup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/poser/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 Tailbone-0.9.90/tailbone/templates/poser/views/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/principal/
--rw-r--r--   0 lance     (1000) lance     (1000)     7974 2023-10-18 22:35:09.000000 Tailbone-0.9.90/tailbone/templates/principal/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      319 2023-10-18 21:45:40.000000 Tailbone-0.9.90/tailbone/templates/principal/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/products/
--rw-r--r--   0 lance     (1000) lance     (1000)     3760 2024-03-26 17:53:16.000000 Tailbone-0.9.90/tailbone/templates/products/batch.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-08-25 13:40:55.000000 Tailbone-0.9.90/tailbone/templates/products/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 Tailbone-0.9.90/tailbone/templates/products/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11948 2023-10-26 15:05:27.000000 Tailbone-0.9.90/tailbone/templates/products/lookup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/products/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     4913 2023-10-27 01:41:10.000000 Tailbone-0.9.90/tailbone/templates/products/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13299 2023-02-11 03:23:43.000000 Tailbone-0.9.90/tailbone/templates/products/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/progress.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/purchases/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/purchases/batches/
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 Tailbone-0.9.90/tailbone/templates/purchases/batches/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/purchases/batches/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.277865 Tailbone-0.9.90/tailbone/templates/purchases/credits/
--rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 Tailbone-0.9.90/tailbone/templates/purchases/credits/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/purchases/receiving_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/purchases/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/receiving/
--rw-r--r--   0 lance     (1000) lance     (1000)     7668 2023-09-17 23:19:14.000000 Tailbone-0.9.90/tailbone/templates/receiving/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 Tailbone-0.9.90/tailbone/templates/receiving/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1495 2023-02-03 05:31:39.000000 Tailbone-0.9.90/tailbone/templates/receiving/declare_credit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1400 2023-02-03 05:32:35.000000 Tailbone-0.9.90/tailbone/templates/receiving/receive_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 Tailbone-0.9.90/tailbone/templates/receiving/transform_unit_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13336 2023-11-02 01:52:57.000000 Tailbone-0.9.90/tailbone/templates/receiving/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    21718 2023-07-07 22:11:23.000000 Tailbone-0.9.90/tailbone/templates/receiving/view_row.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/reports/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/reports/generated/
--rw-r--r--   0 lance     (1000) lance     (1000)     1817 2023-02-03 05:22:38.000000 Tailbone-0.9.90/tailbone/templates/reports/generated/choose.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 Tailbone-0.9.90/tailbone/templates/reports/generated/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 Tailbone-0.9.90/tailbone/templates/reports/generated/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      691 2023-02-03 05:22:09.000000 Tailbone-0.9.90/tailbone/templates/reports/generated/generate.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 Tailbone-0.9.90/tailbone/templates/reports/generated/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/reports/inventory.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/reports/ordering.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/reports/problems/
--rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 Tailbone-0.9.90/tailbone/templates/reports/problems/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/roles/
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 Tailbone-0.9.90/tailbone/templates/roles/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 Tailbone-0.9.90/tailbone/templates/roles/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      407 2023-03-25 18:02:44.000000 Tailbone-0.9.90/tailbone/templates/roles/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 Tailbone-0.9.90/tailbone/templates/roles/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      867 2023-06-14 19:26:51.000000 Tailbone-0.9.90/tailbone/templates/roles/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.249864 Tailbone-0.9.90/tailbone/templates/settings/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/settings/email/
--rw-r--r--   0 lance     (1000) lance     (1000)     4605 2023-08-31 04:30:54.000000 Tailbone-0.9.90/tailbone/templates/settings/email/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 Tailbone-0.9.90/tailbone/templates/settings/email/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3005 2023-08-31 04:29:03.000000 Tailbone-0.9.90/tailbone/templates/settings/email/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 Tailbone-0.9.90/tailbone/templates/shifts/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/shifts/schedule.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 Tailbone-0.9.90/tailbone/templates/shifts/schedule_edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/shifts/schedule_print.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/shifts/schedule_print_employee.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 Tailbone-0.9.90/tailbone/templates/shifts/timesheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 Tailbone-0.9.90/tailbone/templates/shifts/timesheet_edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/tables/
--rw-r--r--   0 lance     (1000) lance     (1000)    31927 2023-05-13 02:23:37.000000 Tailbone-0.9.90/tailbone/templates/tables/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      307 2023-05-13 01:29:02.000000 Tailbone-0.9.90/tailbone/templates/tables/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      245 2023-05-13 01:31:53.000000 Tailbone-0.9.90/tailbone/templates/tables/migrations.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/tempmon/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.281865 Tailbone-0.9.90/tailbone/templates/tempmon/appliances/
--rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 Tailbone-0.9.90/tailbone/templates/tempmon/appliances/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 Tailbone-0.9.90/tailbone/templates/tempmon/appliances/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/tempmon/clients/
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.90/tailbone/templates/tempmon/clients/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-10-05 17:49:24.000000 Tailbone-0.9.90/tailbone/templates/tempmon/clients/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 Tailbone-0.9.90/tailbone/templates/tempmon/dashboard.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/tempmon/probes/
--rw-r--r--   0 lance     (1000) lance     (1000)     3664 2023-07-07 22:38:34.000000 Tailbone-0.9.90/tailbone/templates/tempmon/probes/graph.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 Tailbone-0.9.90/tailbone/templates/tempmon/probes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2738 2023-10-05 17:29:42.000000 Tailbone-0.9.90/tailbone/templates/tempmon/probes/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/tempmon/readings/
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.90/tailbone/templates/tempmon/readings/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.249864 Tailbone-0.9.90/tailbone/templates/themes/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/themes/falafel/
--rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/themes/falafel/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/themes/falafel/progress.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/themes/falafel/upgrade.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.249864 Tailbone-0.9.90/tailbone/templates/trainwreck/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/
--rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/rollover.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/view_row.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/units-of-measure/
--rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 Tailbone-0.9.90/tailbone/templates/units-of-measure/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/upgrade.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/upgrades/
--rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 Tailbone-0.9.90/tailbone/templates/upgrades/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     9414 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/templates/upgrades/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/users/
--rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/templates/users/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1314 2022-02-15 02:30:15.000000 Tailbone-0.9.90/tailbone/templates/users/preferences.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4517 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/templates/users/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 Tailbone-0.9.90/tailbone/templates/util.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 Tailbone-0.9.90/tailbone/templates/vendors/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.249864 Tailbone-0.9.90/tailbone/templates/views/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/views/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 Tailbone-0.9.90/tailbone/templates/views/model/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.285865 Tailbone-0.9.90/tailbone/templates/workorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 Tailbone-0.9.90/tailbone/templates/workorders/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 Tailbone-0.9.90/tailbone/tweens.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13431 2023-11-12 03:25:41.000000 Tailbone-0.9.90/tailbone/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 Tailbone-0.9.90/tailbone/views/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/asgi/
--rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-06-09 19:22:50.000000 Tailbone-0.9.90/tailbone/views/asgi/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 Tailbone-0.9.90/tailbone/views/asgi/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 Tailbone-0.9.90/tailbone/views/asgi/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9533 2023-12-13 18:05:29.000000 Tailbone-0.9.90/tailbone/views/auth.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/views/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    59583 2023-11-06 00:30:51.000000 Tailbone-0.9.90/tailbone/views/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 Tailbone-0.9.90/tailbone/views/batch/delproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6215 2023-05-05 01:11:45.000000 Tailbone-0.9.90/tailbone/views/batch/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9978 2024-03-27 18:10:54.000000 Tailbone-0.9.90/tailbone/views/batch/importer.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19323 2023-10-06 20:52:44.000000 Tailbone-0.9.90/tailbone/views/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 Tailbone-0.9.90/tailbone/views/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6695 2023-08-31 01:01:47.000000 Tailbone-0.9.90/tailbone/views/batch/newproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9511 2023-10-20 15:10:15.000000 Tailbone-0.9.90/tailbone/views/batch/pos.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12439 2024-03-26 17:53:16.000000 Tailbone-0.9.90/tailbone/views/batch/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9366 2023-05-05 02:26:03.000000 Tailbone-0.9.90/tailbone/views/batch/product.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15017 2023-05-30 18:24:14.000000 Tailbone-0.9.90/tailbone/views/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 Tailbone-0.9.90/tailbone/views/batch/vendorinvoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7059 2023-10-18 23:04:31.000000 Tailbone-0.9.90/tailbone/views/bouncer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 Tailbone-0.9.90/tailbone/views/brands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 Tailbone-0.9.90/tailbone/views/categories.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13198 2023-06-17 21:09:24.000000 Tailbone-0.9.90/tailbone/views/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6188 2023-06-17 20:49:58.000000 Tailbone-0.9.90/tailbone/views/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 Tailbone-0.9.90/tailbone/views/customergroups.py
--rw-r--r--   0 lance     (1000) lance     (1000)    32367 2023-10-25 17:19:50.000000 Tailbone-0.9.90/tailbone/views/customers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 Tailbone-0.9.90/tailbone/views/custorders/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 Tailbone-0.9.90/tailbone/views/custorders/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 Tailbone-0.9.90/tailbone/views/custorders/creating.py
--rw-r--r--   0 lance     (1000) lance     (1000)    26154 2023-09-12 17:39:23.000000 Tailbone-0.9.90/tailbone/views/custorders/items.py
--rw-r--r--   0 lance     (1000) lance     (1000)    45521 2023-10-25 19:05:36.000000 Tailbone-0.9.90/tailbone/views/custorders/orders.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16525 2023-06-01 16:37:13.000000 Tailbone-0.9.90/tailbone/views/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7660 2023-12-22 17:40:34.000000 Tailbone-0.9.90/tailbone/views/departments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 Tailbone-0.9.90/tailbone/views/depositlinks.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19409 2023-10-30 03:22:01.000000 Tailbone-0.9.90/tailbone/views/email.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14156 2023-10-18 22:53:40.000000 Tailbone-0.9.90/tailbone/views/employees.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2229 2023-05-05 15:39:16.000000 Tailbone-0.9.90/tailbone/views/essentials.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 Tailbone-0.9.90/tailbone/views/exports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 Tailbone-0.9.90/tailbone/views/families.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4000 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/views/features.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 Tailbone-0.9.90/tailbone/views/filemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1384 2023-09-10 18:50:16.000000 Tailbone-0.9.90/tailbone/views/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 Tailbone-0.9.90/tailbone/views/ifps.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21962 2023-05-10 01:24:53.000000 Tailbone-0.9.90/tailbone/views/importing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 Tailbone-0.9.90/tailbone/views/inventory.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/labels/
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/views/labels/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1326 2023-09-10 18:50:26.000000 Tailbone-0.9.90/tailbone/views/labels/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 Tailbone-0.9.90/tailbone/views/labels/profiles.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 Tailbone-0.9.90/tailbone/views/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)   227934 2023-12-02 01:42:13.000000 Tailbone-0.9.90/tailbone/views/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)    18131 2023-12-01 00:19:11.000000 Tailbone-0.9.90/tailbone/views/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 Tailbone-0.9.90/tailbone/views/menus.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20543 2023-10-18 23:06:19.000000 Tailbone-0.9.90/tailbone/views/messages.py
--rw-r--r--   0 lance     (1000) lance     (1000)    76212 2024-04-01 23:03:37.000000 Tailbone-0.9.90/tailbone/views/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 Tailbone-0.9.90/tailbone/views/permissions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/poser/
--rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 Tailbone-0.9.90/tailbone/views/poser/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 Tailbone-0.9.90/tailbone/views/poser/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 Tailbone-0.9.90/tailbone/views/poser/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 Tailbone-0.9.90/tailbone/views/poser/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6493 2023-10-18 22:32:13.000000 Tailbone-0.9.90/tailbone/views/principal.py
--rw-r--r--   0 lance     (1000) lance     (1000)   102631 2024-03-26 17:53:16.000000 Tailbone-0.9.90/tailbone/views/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 Tailbone-0.9.90/tailbone/views/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15358 2023-05-20 00:45:29.000000 Tailbone-0.9.90/tailbone/views/projects.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.289865 Tailbone-0.9.90/tailbone/views/purchases/
--rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/views/purchases/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13572 2023-10-18 23:17:47.000000 Tailbone-0.9.90/tailbone/views/purchases/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6915 2023-09-17 23:22:43.000000 Tailbone-0.9.90/tailbone/views/purchases/credits.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tailbone/views/purchasing/
--rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 Tailbone-0.9.90/tailbone/views/purchasing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    34215 2023-10-18 23:01:26.000000 Tailbone-0.9.90/tailbone/views/purchasing/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12698 2023-06-27 23:18:35.000000 Tailbone-0.9.90/tailbone/views/purchasing/costing.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19718 2023-10-17 20:25:52.000000 Tailbone-0.9.90/tailbone/views/purchasing/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)    89420 2023-12-20 17:53:56.000000 Tailbone-0.9.90/tailbone/views/purchasing/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 Tailbone-0.9.90/tailbone/views/reportcodes.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29977 2023-10-06 15:11:24.000000 Tailbone-0.9.90/tailbone/views/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20040 2023-02-03 06:30:15.000000 Tailbone-0.9.90/tailbone/views/roles.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16700 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/views/settings.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tailbone/views/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 Tailbone-0.9.90/tailbone/views/shifts/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6797 2023-10-18 23:14:40.000000 Tailbone-0.9.90/tailbone/views/shifts/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21935 2023-10-04 16:45:12.000000 Tailbone-0.9.90/tailbone/views/shifts/lib.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 Tailbone-0.9.90/tailbone/views/shifts/schedule.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 Tailbone-0.9.90/tailbone/views/shifts/timesheet.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 Tailbone-0.9.90/tailbone/views/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 Tailbone-0.9.90/tailbone/views/subdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16028 2023-05-13 02:22:15.000000 Tailbone-0.9.90/tailbone/views/tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2103 2023-10-07 02:23:35.000000 Tailbone-0.9.90/tailbone/views/taxes.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tailbone/views/tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 Tailbone-0.9.90/tailbone/views/tempmon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 Tailbone-0.9.90/tailbone/views/tempmon/appliances.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9593 2023-10-05 18:08:20.000000 Tailbone-0.9.90/tailbone/views/tempmon/clients.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3486 2023-04-21 17:01:56.000000 Tailbone-0.9.90/tailbone/views/tempmon/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 Tailbone-0.9.90/tailbone/views/tempmon/dashboard.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11672 2023-10-18 23:08:32.000000 Tailbone-0.9.90/tailbone/views/tempmon/probes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4062 2023-10-18 23:16:37.000000 Tailbone-0.9.90/tailbone/views/tempmon/readings.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2076 2023-10-19 22:38:32.000000 Tailbone-0.9.90/tailbone/views/tenders.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tailbone/views/trainwreck/
--rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 Tailbone-0.9.90/tailbone/views/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15019 2023-09-20 23:03:33.000000 Tailbone-0.9.90/tailbone/views/trainwreck/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 Tailbone-0.9.90/tailbone/views/trainwreck/defaults.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2409 2023-10-07 01:55:59.000000 Tailbone-0.9.90/tailbone/views/typical.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 Tailbone-0.9.90/tailbone/views/uoms.py
--rw-r--r--   0 lance     (1000) lance     (1000)    25047 2023-05-19 00:56:33.000000 Tailbone-0.9.90/tailbone/views/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)    27921 2023-05-15 13:10:42.000000 Tailbone-0.9.90/tailbone/views/users.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tailbone/views/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-02-23 01:01:50.000000 Tailbone-0.9.90/tailbone/views/vendors/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:49.000000 Tailbone-0.9.90/tailbone/views/vendors/catalogs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7783 2023-10-24 22:43:48.000000 Tailbone-0.9.90/tailbone/views/vendors/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:41.000000 Tailbone-0.9.90/tailbone/views/vendors/invoices.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4738 2023-02-23 04:40:20.000000 Tailbone-0.9.90/tailbone/views/vendors/samplefiles.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 Tailbone-0.9.90/tailbone/views/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6966 2023-10-18 23:16:11.000000 Tailbone-0.9.90/tailbone/views/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-09-02 20:50:35.000000 Tailbone-0.9.90/tailbone/views/workorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3747 2023-05-17 02:25:47.000000 Tailbone-0.9.90/tailbone/webapi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1511 2022-08-24 23:26:54.000000 Tailbone-0.9.90/tasks.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-01 23:28:51.293865 Tailbone-0.9.90/tests/
--rw-rw-r--   0 lance     (1000) lance     (1000)     1057 2023-05-25 19:55:35.000000 Tailbone-0.9.90/tests/test_app.py
--rw-r--r--   0 lance     (1000) lance     (1000)      191 2013-09-10 19:45:40.000000 Tailbone-0.9.90/tests/test_helpers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.276757 tailbone-0.9.91/
+-rw-r--r--   0 lance     (1000) lance     (1000)   160360 2024-04-15 15:56:22.000000 tailbone-0.9.91/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 tailbone-0.9.91/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 tailbone-0.9.91/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-15 15:57:40.276757 tailbone-0.9.91/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 tailbone-0.9.91/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.276757 tailbone-0.9.91/Tailbone.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)    14749 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      272 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)      448 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        9 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2128 2024-04-15 15:57:40.276757 tailbone-0.9.91/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 20:02:32.000000 tailbone-0.9.91/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       49 2024-04-15 15:56:39.000000 tailbone-0.9.91/tailbone/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/api/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 tailbone-0.9.91/tailbone/api/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7865 2023-05-17 04:11:43.000000 tailbone-0.9.91/tailbone/api/auth.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/api/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 tailbone-0.9.91/tailbone/api/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12760 2023-11-02 00:42:53.000000 tailbone-0.9.91/tailbone/api/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7150 2023-11-15 15:46:15.000000 tailbone-0.9.91/tailbone/api/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 tailbone-0.9.91/tailbone/api/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11993 2024-04-11 18:51:54.000000 tailbone-0.9.91/tailbone/api/batch/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20740 2024-04-11 19:12:25.000000 tailbone-0.9.91/tailbone/api/batch/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5099 2023-05-17 04:34:48.000000 tailbone-0.9.91/tailbone/api/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4643 2023-06-17 03:15:35.000000 tailbone-0.9.91/tailbone/api/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 tailbone-0.9.91/tailbone/api/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1202 2023-05-20 00:29:29.000000 tailbone-0.9.91/tailbone/api/essentials.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 tailbone-0.9.91/tailbone/api/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21938 2023-10-08 17:24:00.000000 tailbone-0.9.91/tailbone/api/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 tailbone-0.9.91/tailbone/api/master2.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 tailbone-0.9.91/tailbone/api/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7461 2023-09-02 15:55:47.000000 tailbone-0.9.91/tailbone/api/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 tailbone-0.9.91/tailbone/api/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2181 2023-05-03 00:13:09.000000 tailbone-0.9.91/tailbone/api/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 tailbone-0.9.91/tailbone/api/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 tailbone-0.9.91/tailbone/api/workorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11334 2023-10-24 01:35:10.000000 tailbone-0.9.91/tailbone/app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 tailbone-0.9.91/tailbone/asgi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6324 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 tailbone-0.9.91/tailbone/beaker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 tailbone-0.9.91/tailbone/cleanup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2366 2024-04-13 14:19:43.000000 tailbone-0.9.91/tailbone/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 tailbone-0.9.91/tailbone/db.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9796 2023-12-01 00:13:00.000000 tailbone-0.9.91/tailbone/diffs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 tailbone-0.9.91/tailbone/exceptions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1107 2023-09-17 00:47:36.000000 tailbone-0.9.91/tailbone/forms/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 tailbone-0.9.91/tailbone/forms/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    49572 2024-04-15 01:24:25.000000 tailbone-0.9.91/tailbone/forms/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2361 2023-08-29 21:08:45.000000 tailbone-0.9.91/tailbone/forms/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7041 2023-10-09 20:50:24.000000 tailbone-0.9.91/tailbone/forms/types.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20432 2024-04-15 01:23:41.000000 tailbone-0.9.91/tailbone/forms/widgets.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 tailbone-0.9.91/tailbone/grids/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    70674 2024-04-15 01:45:42.000000 tailbone-0.9.91/tailbone/grids/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    40585 2023-12-11 19:49:51.000000 tailbone-0.9.91/tailbone/grids/filters.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 tailbone-0.9.91/tailbone/handler.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1883 2023-05-05 02:26:43.000000 tailbone-0.9.91/tailbone/helpers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29626 2023-10-29 20:45:59.000000 tailbone-0.9.91/tailbone/menus.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 tailbone-0.9.91/tailbone/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 tailbone-0.9.91/tailbone/providers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/reports/
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/reports/inventory_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/reports/ordering_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/scaffolds.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/css/
+-rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 tailbone-0.9.91/tailbone/static/css/base.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 tailbone-0.9.91/tailbone/static/css/codehilite.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 tailbone-0.9.91/tailbone/static/css/diffs.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/filters.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/forms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 tailbone-0.9.91/tailbone/static/css/grids.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1167 2024-04-15 01:28:38.000000 tailbone-0.9.91/tailbone/static/css/grids.rowstatus.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     2671 2023-10-25 15:44:50.000000 tailbone-0.9.91/tailbone/static/css/layout.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/css/normalize.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 tailbone-0.9.91/tailbone/static/css/perms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/progress.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/css/purchases.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/static/css/schedule_print.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 tailbone-0.9.91/tailbone/static/css/timesheet.css
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/files/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 tailbone-0.9.91/tailbone/static/files/newproduct_template.xlsx
+-rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 tailbone-0.9.91/tailbone/static/files/vendor_catalog_template.xlsx
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/img/
+-rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/Hymenocephalus_italicus.jpg
+-rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/delete.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/edit.png
+-rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/home_logo.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/loading.gif
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/static/img/product.png
+-rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/rattail.ico
+-rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 tailbone-0.9.91/tailbone/static/img/save.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/sort_arrow_down.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/sort_arrow_up.png
+-rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 tailbone-0.9.91/tailbone/static/img/testing.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/view.png
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/static/js/
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 tailbone-0.9.91/tailbone/static/js/debounce.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/js/numeric.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     9498 2023-10-26 01:03:48.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.autocomplete.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.datepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     4561 2023-06-16 17:21:44.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.grid.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.message_recipients.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.numericinput.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.oncebutton.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1403 2023-09-17 00:42:09.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.timepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1427 2023-06-06 16:53:17.000000 tailbone-0.9.91/tailbone/static/js/tailbone.feedback.js
+-rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/robots.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)    10220 2024-04-15 01:55:42.000000 tailbone-0.9.91/tailbone/subscribers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/
+-rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 tailbone-0.9.91/tailbone/templates/about.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/appinfo/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 tailbone-0.9.91/tailbone/templates/appinfo/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3270 2023-10-24 14:53:32.000000 tailbone-0.9.91/tailbone/templates/appinfo/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6317 2024-04-14 23:27:37.000000 tailbone-0.9.91/tailbone/templates/appsettings.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 tailbone-0.9.91/tailbone/templates/autocomplete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    33683 2023-11-17 23:00:34.000000 tailbone-0.9.91/tailbone/templates/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 tailbone-0.9.91/tailbone/templates/base_meta.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/batch/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 tailbone-0.9.91/tailbone/templates/batch/edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/importer/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2381 2024-04-15 00:15:19.000000 tailbone-0.9.91/tailbone/templates/batch/importer/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 tailbone-0.9.91/tailbone/templates/batch/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/inventory/
+-rw-r--r--   0 lance     (1000) lance     (1000)    10321 2024-04-15 00:11:34.000000 tailbone-0.9.91/tailbone/templates/batch/inventory/desktop_form.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/newproduct/
+-rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 tailbone-0.9.91/tailbone/templates/batch/newproduct/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/pos/
+-rw-r--r--   0 lance     (1000) lance     (1000)      285 2023-10-07 04:17:54.000000 tailbone-0.9.91/tailbone/templates/batch/pos/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/pricing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 tailbone-0.9.91/tailbone/templates/batch/pricing/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      241 2024-04-15 00:15:22.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11890 2024-04-15 00:15:17.000000 tailbone-0.9.91/tailbone/templates/batch/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 tailbone-0.9.91/tailbone/templates/batch/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 tailbone-0.9.91/tailbone/templates/change_password.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 tailbone-0.9.91/tailbone/templates/configure-menus.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 tailbone-0.9.91/tailbone/templates/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/customers/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3775 2023-06-11 18:38:46.000000 tailbone-0.9.91/tailbone/templates/customers/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/customers/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 tailbone-0.9.91/tailbone/templates/customers/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1096 2024-04-15 01:26:15.000000 tailbone-0.9.91/tailbone/templates/customers/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6522 2023-10-25 00:29:26.000000 tailbone-0.9.91/tailbone/templates/custorders/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    92495 2023-10-26 14:28:39.000000 tailbone-0.9.91/tailbone/templates/custorders/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/custorders/items/
+-rw-r--r--   0 lance     (1000) lance     (1000)    16040 2024-04-15 00:15:26.000000 tailbone-0.9.91/tailbone/templates/custorders/items/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       81 2023-09-10 19:59:06.000000 tailbone-0.9.91/tailbone/templates/custorders/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/datasync/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/datasync/changes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 tailbone-0.9.91/tailbone/templates/datasync/changes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 tailbone-0.9.91/tailbone/templates/datasync/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 tailbone-0.9.91/tailbone/templates/datasync/status.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/deform/
+-rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 tailbone-0.9.91/tailbone/templates/deform/autocomplete_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 tailbone-0.9.91/tailbone/templates/deform/cases_units.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 tailbone-0.9.91/tailbone/templates/deform/checkbox.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 tailbone-0.9.91/tailbone/templates/deform/checkbox_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 tailbone-0.9.91/tailbone/templates/deform/checked_password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 tailbone-0.9.91/tailbone/templates/deform/date_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 tailbone-0.9.91/tailbone/templates/deform/date_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      543 2023-09-17 01:00:05.000000 tailbone-0.9.91/tailbone/templates/deform/datetime_falafel.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 tailbone-0.9.91/tailbone/templates/deform/file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 tailbone-0.9.91/tailbone/templates/deform/message_recipients.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 tailbone-0.9.91/tailbone/templates/deform/multi_file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/deform/numberinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 tailbone-0.9.91/tailbone/templates/deform/numericinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 tailbone-0.9.91/tailbone/templates/deform/password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 tailbone-0.9.91/tailbone/templates/deform/percentinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 tailbone-0.9.91/tailbone/templates/deform/permissions.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 tailbone-0.9.91/tailbone/templates/deform/problem_report_days.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 tailbone-0.9.91/tailbone/templates/deform/select.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1177 2023-08-08 19:10:04.000000 tailbone-0.9.91/tailbone/templates/deform/select_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/deform/select_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 tailbone-0.9.91/tailbone/templates/deform/select_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      550 2023-03-23 15:17:29.000000 tailbone-0.9.91/tailbone/templates/deform/textarea.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 tailbone-0.9.91/tailbone/templates/deform/textinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      230 2023-09-26 00:21:51.000000 tailbone-0.9.91/tailbone/templates/deform/time_falafel.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 tailbone-0.9.91/tailbone/templates/deform/time_jquery.pt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/departments/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 tailbone-0.9.91/tailbone/templates/departments/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      551 2023-10-09 05:16:53.000000 tailbone-0.9.91/tailbone/templates/diff.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/email-bounces/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1659 2023-09-08 15:46:55.000000 tailbone-0.9.91/tailbone/templates/email-bounces/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/employees/
+-rw-r--r--   0 lance     (1000) lance     (1000)      626 2023-06-11 04:11:26.000000 tailbone-0.9.91/tailbone/templates/employees/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 tailbone-0.9.91/tailbone/templates/employees/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/exception.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1506 2024-04-15 00:15:12.000000 tailbone-0.9.91/tailbone/templates/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2779 2023-06-17 19:13:31.000000 tailbone-0.9.91/tailbone/templates/formposter.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7053 2024-04-15 00:03:36.000000 tailbone-0.9.91/tailbone/templates/forms/deform.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 tailbone-0.9.91/tailbone/templates/generate_feature.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/generated-projects/
+-rw-r--r--   0 lance     (1000) lance     (1000)      582 2023-05-04 18:51:55.000000 tailbone-0.9.91/tailbone/templates/generated-projects/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 tailbone-0.9.91/tailbone/templates/grids/b-table.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    28542 2024-04-15 01:40:53.000000 tailbone-0.9.91/tailbone/templates/grids/complete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1898 2023-10-11 03:10:01.000000 tailbone-0.9.91/tailbone/templates/grids/filters.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/grids/nav.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 tailbone-0.9.91/tailbone/templates/home.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/ifps-plu-codes/
+-rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 tailbone-0.9.91/tailbone/templates/ifps-plu-codes/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 tailbone-0.9.91/tailbone/templates/importing/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 tailbone-0.9.91/tailbone/templates/importing/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 tailbone-0.9.91/tailbone/templates/importing/runjob.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 tailbone-0.9.91/tailbone/templates/importing/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.248757 tailbone-0.9.91/tailbone/templates/labels/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/labels/profiles/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/create.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/printer.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 tailbone-0.9.91/tailbone/templates/login.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/luigi/
+-rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 tailbone-0.9.91/tailbone/templates/luigi/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 tailbone-0.9.91/tailbone/templates/luigi/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/master/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1364 2024-04-15 00:15:10.000000 tailbone-0.9.91/tailbone/templates/master/clone.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 tailbone-0.9.91/tailbone/templates/master/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 tailbone-0.9.91/tailbone/templates/master/create.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/master/create_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2024-04-15 00:15:05.000000 tailbone-0.9.91/tailbone/templates/master/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      226 2023-10-10 02:06:31.000000 tailbone-0.9.91/tailbone/templates/master/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 tailbone-0.9.91/tailbone/templates/master/edit_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 tailbone-0.9.91/tailbone/templates/master/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 tailbone-0.9.91/tailbone/templates/master/import_file.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    25086 2024-04-13 15:01:04.000000 tailbone-0.9.91/tailbone/templates/master/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5560 2023-06-19 02:20:45.000000 tailbone-0.9.91/tailbone/templates/master/merge.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1036 2024-04-13 15:00:59.000000 tailbone-0.9.91/tailbone/templates/master/versions.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11305 2024-04-13 15:00:53.000000 tailbone-0.9.91/tailbone/templates/master/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 tailbone-0.9.91/tailbone/templates/master/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1413 2023-10-10 15:07:41.000000 tailbone-0.9.91/tailbone/templates/master/view_version.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/members/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2342 2023-08-26 14:11:45.000000 tailbone-0.9.91/tailbone/templates/members/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      262 2023-06-14 19:01:14.000000 tailbone-0.9.91/tailbone/templates/members/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/templates/menu.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/archive/
+-rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 tailbone-0.9.91/tailbone/templates/messages/archive/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1777 2023-03-23 15:22:59.000000 tailbone-0.9.91/tailbone/templates/messages/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/inbox/
+-rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 tailbone-0.9.91/tailbone/templates/messages/inbox/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 tailbone-0.9.91/tailbone/templates/messages/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 tailbone-0.9.91/tailbone/templates/messages/recipients.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/sent/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/messages/sent/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 tailbone-0.9.91/tailbone/templates/messages/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 tailbone-0.9.91/tailbone/templates/multi_file_upload.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/ordering/
+-rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 tailbone-0.9.91/tailbone/templates/ordering/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 tailbone-0.9.91/tailbone/templates/ordering/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 tailbone-0.9.91/tailbone/templates/ordering/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1813 2023-08-28 02:36:03.000000 tailbone-0.9.91/tailbone/templates/page.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 tailbone-0.9.91/tailbone/templates/page_help.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/people/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1296 2023-06-17 19:36:29.000000 tailbone-0.9.91/tailbone/templates/people/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 tailbone-0.9.91/tailbone/templates/people/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/people/merge-requests/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 tailbone-0.9.91/tailbone/templates/people/merge-requests/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1100 2024-04-15 00:14:52.000000 tailbone-0.9.91/tailbone/templates/people/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    84948 2024-04-15 00:33:25.000000 tailbone-0.9.91/tailbone/templates/people/view_profile.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/reports/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 tailbone-0.9.91/tailbone/templates/poser/reports/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 tailbone-0.9.91/tailbone/templates/poser/setup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 tailbone-0.9.91/tailbone/templates/poser/views/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/principal/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7971 2024-04-14 23:38:53.000000 tailbone-0.9.91/tailbone/templates/principal/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      319 2023-10-18 21:45:40.000000 tailbone-0.9.91/tailbone/templates/principal/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/products/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3763 2024-04-15 00:12:29.000000 tailbone-0.9.91/tailbone/templates/products/batch.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-08-25 13:40:55.000000 tailbone-0.9.91/tailbone/templates/products/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 tailbone-0.9.91/tailbone/templates/products/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11948 2023-10-26 15:05:27.000000 tailbone-0.9.91/tailbone/templates/products/lookup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/products/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4913 2023-10-27 01:41:10.000000 tailbone-0.9.91/tailbone/templates/products/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13263 2024-04-15 00:33:50.000000 tailbone-0.9.91/tailbone/templates/products/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/progress.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/batches/
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 tailbone-0.9.91/tailbone/templates/purchases/batches/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/batches/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/credits/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 tailbone-0.9.91/tailbone/templates/purchases/credits/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/receiving_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/receiving/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7668 2023-09-17 23:19:14.000000 tailbone-0.9.91/tailbone/templates/receiving/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 tailbone-0.9.91/tailbone/templates/receiving/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1415 2024-04-15 00:18:30.000000 tailbone-0.9.91/tailbone/templates/receiving/declare_credit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-15 00:18:40.000000 tailbone-0.9.91/tailbone/templates/receiving/receive_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 tailbone-0.9.91/tailbone/templates/receiving/transform_unit_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13336 2023-11-02 01:52:57.000000 tailbone-0.9.91/tailbone/templates/receiving/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    21718 2023-07-07 22:11:23.000000 tailbone-0.9.91/tailbone/templates/receiving/view_row.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/reports/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/reports/generated/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1811 2024-04-15 00:15:00.000000 tailbone-0.9.91/tailbone/templates/reports/generated/choose.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 tailbone-0.9.91/tailbone/templates/reports/generated/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 tailbone-0.9.91/tailbone/templates/reports/generated/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      685 2024-04-15 00:14:55.000000 tailbone-0.9.91/tailbone/templates/reports/generated/generate.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 tailbone-0.9.91/tailbone/templates/reports/generated/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/reports/inventory.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/reports/ordering.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/reports/problems/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 tailbone-0.9.91/tailbone/templates/reports/problems/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/roles/
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 tailbone-0.9.91/tailbone/templates/roles/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 tailbone-0.9.91/tailbone/templates/roles/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      407 2023-03-25 18:02:44.000000 tailbone-0.9.91/tailbone/templates/roles/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 tailbone-0.9.91/tailbone/templates/roles/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      754 2024-04-15 01:27:32.000000 tailbone-0.9.91/tailbone/templates/roles/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/settings/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/settings/email/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4605 2023-08-31 04:30:54.000000 tailbone-0.9.91/tailbone/templates/settings/email/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 tailbone-0.9.91/tailbone/templates/settings/email/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2993 2024-04-15 00:15:31.000000 tailbone-0.9.91/tailbone/templates/settings/email/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 tailbone-0.9.91/tailbone/templates/shifts/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_print.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_print_employee.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 tailbone-0.9.91/tailbone/templates/shifts/timesheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 tailbone-0.9.91/tailbone/templates/shifts/timesheet_edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tables/
+-rw-r--r--   0 lance     (1000) lance     (1000)    31927 2023-05-13 02:23:37.000000 tailbone-0.9.91/tailbone/templates/tables/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      307 2023-05-13 01:29:02.000000 tailbone-0.9.91/tailbone/templates/tables/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      245 2023-05-13 01:31:53.000000 tailbone-0.9.91/tailbone/templates/tables/migrations.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/appliances/
+-rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 tailbone-0.9.91/tailbone/templates/tempmon/appliances/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 tailbone-0.9.91/tailbone/templates/tempmon/appliances/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/clients/
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.91/tailbone/templates/tempmon/clients/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-10-05 17:49:24.000000 tailbone-0.9.91/tailbone/templates/tempmon/clients/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 tailbone-0.9.91/tailbone/templates/tempmon/dashboard.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/probes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3664 2023-07-07 22:38:34.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/graph.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2738 2023-10-05 17:29:42.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/readings/
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.91/tailbone/templates/tempmon/readings/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/themes/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/themes/falafel/
+-rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/progress.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/upgrade.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/trainwreck/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/rollover.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/view_row.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/units-of-measure/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 tailbone-0.9.91/tailbone/templates/units-of-measure/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/upgrade.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/upgrades/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 tailbone-0.9.91/tailbone/templates/upgrades/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     9408 2024-04-15 00:15:24.000000 tailbone-0.9.91/tailbone/templates/upgrades/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/users/
+-rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/users/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-14 23:56:36.000000 tailbone-0.9.91/tailbone/templates/users/preferences.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4517 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/templates/users/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 tailbone-0.9.91/tailbone/templates/util.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 tailbone-0.9.91/tailbone/templates/vendors/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/views/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/views/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 tailbone-0.9.91/tailbone/templates/views/model/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/workorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 tailbone-0.9.91/tailbone/templates/workorders/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 tailbone-0.9.91/tailbone/tweens.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13431 2023-11-12 03:25:41.000000 tailbone-0.9.91/tailbone/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 tailbone-0.9.91/tailbone/views/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/asgi/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-06-09 19:22:50.000000 tailbone-0.9.91/tailbone/views/asgi/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 tailbone-0.9.91/tailbone/views/asgi/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 tailbone-0.9.91/tailbone/views/asgi/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9533 2023-12-13 18:05:29.000000 tailbone-0.9.91/tailbone/views/auth.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    59664 2024-04-15 01:48:34.000000 tailbone-0.9.91/tailbone/views/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 tailbone-0.9.91/tailbone/views/batch/delproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6098 2024-04-14 23:51:02.000000 tailbone-0.9.91/tailbone/views/batch/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9880 2024-04-15 01:55:22.000000 tailbone-0.9.91/tailbone/views/batch/importer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19323 2023-10-06 20:52:44.000000 tailbone-0.9.91/tailbone/views/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 tailbone-0.9.91/tailbone/views/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6695 2023-08-31 01:01:47.000000 tailbone-0.9.91/tailbone/views/batch/newproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9505 2024-04-15 00:34:44.000000 tailbone-0.9.91/tailbone/views/batch/pos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12439 2024-03-26 17:53:16.000000 tailbone-0.9.91/tailbone/views/batch/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9258 2024-04-14 23:44:49.000000 tailbone-0.9.91/tailbone/views/batch/product.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15017 2023-05-30 18:24:14.000000 tailbone-0.9.91/tailbone/views/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 tailbone-0.9.91/tailbone/views/batch/vendorinvoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7059 2023-10-18 23:04:31.000000 tailbone-0.9.91/tailbone/views/bouncer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 tailbone-0.9.91/tailbone/views/brands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 tailbone-0.9.91/tailbone/views/categories.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13198 2023-06-17 21:09:24.000000 tailbone-0.9.91/tailbone/views/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6188 2023-06-17 20:49:58.000000 tailbone-0.9.91/tailbone/views/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 tailbone-0.9.91/tailbone/views/customergroups.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    31934 2024-04-15 01:54:49.000000 tailbone-0.9.91/tailbone/views/customers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 tailbone-0.9.91/tailbone/views/custorders/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 tailbone-0.9.91/tailbone/views/custorders/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 tailbone-0.9.91/tailbone/views/custorders/creating.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    26148 2024-04-15 00:35:12.000000 tailbone-0.9.91/tailbone/views/custorders/items.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    45521 2023-10-25 19:05:36.000000 tailbone-0.9.91/tailbone/views/custorders/orders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16525 2023-06-01 16:37:13.000000 tailbone-0.9.91/tailbone/views/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7781 2024-04-15 00:32:55.000000 tailbone-0.9.91/tailbone/views/departments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 tailbone-0.9.91/tailbone/views/depositlinks.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19409 2023-10-30 03:22:01.000000 tailbone-0.9.91/tailbone/views/email.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14156 2023-10-18 22:53:40.000000 tailbone-0.9.91/tailbone/views/employees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2229 2023-05-05 15:39:16.000000 tailbone-0.9.91/tailbone/views/essentials.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 tailbone-0.9.91/tailbone/views/exports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 tailbone-0.9.91/tailbone/views/families.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4000 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/views/features.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 tailbone-0.9.91/tailbone/views/filemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1384 2023-09-10 18:50:16.000000 tailbone-0.9.91/tailbone/views/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 tailbone-0.9.91/tailbone/views/ifps.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21962 2023-05-10 01:24:53.000000 tailbone-0.9.91/tailbone/views/importing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 tailbone-0.9.91/tailbone/views/inventory.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/labels/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/labels/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1326 2023-09-10 18:50:26.000000 tailbone-0.9.91/tailbone/views/labels/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 tailbone-0.9.91/tailbone/views/labels/profiles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 tailbone-0.9.91/tailbone/views/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)   228233 2024-04-14 23:07:56.000000 tailbone-0.9.91/tailbone/views/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    18131 2023-12-01 00:19:11.000000 tailbone-0.9.91/tailbone/views/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 tailbone-0.9.91/tailbone/views/menus.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20417 2024-04-15 01:47:46.000000 tailbone-0.9.91/tailbone/views/messages.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    75831 2024-04-15 01:45:58.000000 tailbone-0.9.91/tailbone/views/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 tailbone-0.9.91/tailbone/views/permissions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/poser/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 tailbone-0.9.91/tailbone/views/poser/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 tailbone-0.9.91/tailbone/views/poser/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 tailbone-0.9.91/tailbone/views/poser/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 tailbone-0.9.91/tailbone/views/poser/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6454 2024-04-14 23:38:57.000000 tailbone-0.9.91/tailbone/views/principal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)   102892 2024-04-15 01:46:20.000000 tailbone-0.9.91/tailbone/views/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 tailbone-0.9.91/tailbone/views/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15358 2023-05-20 00:45:29.000000 tailbone-0.9.91/tailbone/views/projects.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/purchases/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/purchases/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13572 2023-10-18 23:17:47.000000 tailbone-0.9.91/tailbone/views/purchases/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6915 2023-09-17 23:22:43.000000 tailbone-0.9.91/tailbone/views/purchases/credits.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/purchasing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 tailbone-0.9.91/tailbone/views/purchasing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    34167 2024-04-15 00:36:07.000000 tailbone-0.9.91/tailbone/views/purchasing/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12698 2023-06-27 23:18:35.000000 tailbone-0.9.91/tailbone/views/purchasing/costing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19673 2024-04-14 23:29:26.000000 tailbone-0.9.91/tailbone/views/purchasing/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    89356 2024-04-15 00:37:38.000000 tailbone-0.9.91/tailbone/views/purchasing/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 tailbone-0.9.91/tailbone/views/reportcodes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29907 2024-04-15 00:32:35.000000 tailbone-0.9.91/tailbone/views/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20099 2024-04-15 00:39:14.000000 tailbone-0.9.91/tailbone/views/roles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16580 2024-04-15 01:25:01.000000 tailbone-0.9.91/tailbone/views/settings.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/shifts/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6797 2023-10-18 23:14:40.000000 tailbone-0.9.91/tailbone/views/shifts/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    22006 2024-04-14 23:49:25.000000 tailbone-0.9.91/tailbone/views/shifts/lib.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 tailbone-0.9.91/tailbone/views/shifts/schedule.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 tailbone-0.9.91/tailbone/views/shifts/timesheet.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 tailbone-0.9.91/tailbone/views/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/views/subdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15898 2024-04-14 23:09:45.000000 tailbone-0.9.91/tailbone/views/tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2103 2023-10-07 02:23:35.000000 tailbone-0.9.91/tailbone/views/taxes.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 tailbone-0.9.91/tailbone/views/tempmon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 tailbone-0.9.91/tailbone/views/tempmon/appliances.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9593 2023-10-05 18:08:20.000000 tailbone-0.9.91/tailbone/views/tempmon/clients.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3480 2024-04-15 00:40:07.000000 tailbone-0.9.91/tailbone/views/tempmon/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 tailbone-0.9.91/tailbone/views/tempmon/dashboard.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11672 2023-10-18 23:08:32.000000 tailbone-0.9.91/tailbone/views/tempmon/probes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4062 2023-10-18 23:16:37.000000 tailbone-0.9.91/tailbone/views/tempmon/readings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2076 2023-10-19 22:38:32.000000 tailbone-0.9.91/tailbone/views/tenders.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/trainwreck/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 tailbone-0.9.91/tailbone/views/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14860 2024-04-15 00:40:27.000000 tailbone-0.9.91/tailbone/views/trainwreck/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 tailbone-0.9.91/tailbone/views/trainwreck/defaults.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2409 2023-10-07 01:55:59.000000 tailbone-0.9.91/tailbone/views/typical.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 tailbone-0.9.91/tailbone/views/uoms.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    24918 2024-04-15 01:52:07.000000 tailbone-0.9.91/tailbone/views/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    27763 2024-04-15 00:33:08.000000 tailbone-0.9.91/tailbone/views/users.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-02-23 01:01:50.000000 tailbone-0.9.91/tailbone/views/vendors/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:49.000000 tailbone-0.9.91/tailbone/views/vendors/catalogs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7783 2023-10-24 22:43:48.000000 tailbone-0.9.91/tailbone/views/vendors/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:41.000000 tailbone-0.9.91/tailbone/views/vendors/invoices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4738 2023-02-23 04:40:20.000000 tailbone-0.9.91/tailbone/views/vendors/samplefiles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 tailbone-0.9.91/tailbone/views/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6966 2023-10-18 23:16:11.000000 tailbone-0.9.91/tailbone/views/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-09-02 20:50:35.000000 tailbone-0.9.91/tailbone/views/workorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3747 2023-05-17 02:25:47.000000 tailbone-0.9.91/tailbone/webapi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1445 2024-04-15 15:57:32.000000 tailbone-0.9.91/tasks.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tests/
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1057 2023-05-25 19:55:35.000000 tailbone-0.9.91/tests/test_app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      191 2013-09-10 19:45:40.000000 tailbone-0.9.91/tests/test_helpers.py
```

### Comparing `Tailbone-0.9.90/CHANGES.rst` & `tailbone-0.9.91/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 
 CHANGELOG
 =========
 
 Unreleased
 ----------
 
+
+0.9.91 (2024-04-15)
+-------------------
+
+* Avoid uncaught error when updating order batch row quantities.
+
+* Try to return JSON error when receiving API call fails.
+
+* Avoid error for tax field when creating new department.
+
+* Show toast msg instead of silent error, when grid fetch fails.
+
+* Remove most references to "buefy" name in class methods, template
+  filenames etc.
+
+
 0.9.90 (2024-04-01)
 -------------------
 
 * Add basic CRUD for Person "preferred first name".
 
 
 0.9.89 (2024-03-27)
```

### Comparing `Tailbone-0.9.90/COPYING.txt` & `tailbone-0.9.91/COPYING.txt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/PKG-INFO` & `tailbone-0.9.91/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.90
+Version: 0.9.91
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `Tailbone-0.9.90/Tailbone.egg-info/PKG-INFO` & `tailbone-0.9.91/Tailbone.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.90
+Version: 0.9.91
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `Tailbone-0.9.90/Tailbone.egg-info/SOURCES.txt` & `tailbone-0.9.91/Tailbone.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 tailbone/templates/deform/checkbox.pt
 tailbone/templates/deform/checkbox_dynamic.pt
 tailbone/templates/deform/checked_password.pt
 tailbone/templates/deform/date_jquery.pt
 tailbone/templates/deform/date_plain.pt
 tailbone/templates/deform/datetime_falafel.pt
 tailbone/templates/deform/file_upload.pt
-tailbone/templates/deform/message_recipients_buefy.pt
+tailbone/templates/deform/message_recipients.pt
 tailbone/templates/deform/multi_file_upload.pt
 tailbone/templates/deform/numberinput.pt
 tailbone/templates/deform/numericinput.pt
 tailbone/templates/deform/password.pt
 tailbone/templates/deform/percentinput.pt
 tailbone/templates/deform/permissions.pt
 tailbone/templates/deform/problem_report_days.pt
@@ -178,22 +178,19 @@
 tailbone/templates/deform/textinput.pt
 tailbone/templates/deform/time_falafel.pt
 tailbone/templates/deform/time_jquery.pt
 tailbone/templates/departments/view.mako
 tailbone/templates/email-bounces/view.mako
 tailbone/templates/employees/configure.mako
 tailbone/templates/employees/view.mako
-tailbone/templates/forms/deform_buefy.mako
-tailbone/templates/forms/form.mako
-tailbone/templates/forms/util.mako
+tailbone/templates/forms/deform.mako
 tailbone/templates/generated-projects/create.mako
 tailbone/templates/grids/b-table.mako
-tailbone/templates/grids/buefy.mako
+tailbone/templates/grids/complete.mako
 tailbone/templates/grids/filters.mako
-tailbone/templates/grids/filters_buefy.mako
 tailbone/templates/grids/nav.mako
 tailbone/templates/ifps-plu-codes/index.mako
 tailbone/templates/importing/configure.mako
 tailbone/templates/importing/index.mako
 tailbone/templates/importing/runjob.mako
 tailbone/templates/importing/view.mako
 tailbone/templates/labels/profiles/create.mako
@@ -228,15 +225,15 @@
 tailbone/templates/messages/sent/index.mako
 tailbone/templates/ordering/create.mako
 tailbone/templates/ordering/view.mako
 tailbone/templates/ordering/worksheet.mako
 tailbone/templates/people/configure.mako
 tailbone/templates/people/index.mako
 tailbone/templates/people/view.mako
-tailbone/templates/people/view_profile_buefy.mako
+tailbone/templates/people/view_profile.mako
 tailbone/templates/people/merge-requests/view.mako
 tailbone/templates/poser/setup.mako
 tailbone/templates/poser/reports/view.mako
 tailbone/templates/poser/views/configure.mako
 tailbone/templates/principal/find_by_perm.mako
 tailbone/templates/principal/index.mako
 tailbone/templates/products/batch.mako
```

### Comparing `Tailbone-0.9.90/setup.cfg` & `tailbone-0.9.91/setup.cfg`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/setup.py` & `tailbone-0.9.91/setup.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/__init__.py` & `tailbone-0.9.91/tailbone/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/__init__.py` & `tailbone-0.9.91/tailbone/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/auth.py` & `tailbone-0.9.91/tailbone/api/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/batch/__init__.py` & `tailbone-0.9.91/tailbone/api/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/batch/core.py` & `tailbone-0.9.91/tailbone/api/batch/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/batch/inventory.py` & `tailbone-0.9.91/tailbone/api/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/batch/labels.py` & `tailbone-0.9.91/tailbone/api/batch/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/batch/ordering.py` & `tailbone-0.9.91/tailbone/api/batch/ordering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -24,26 +24,31 @@
 Tailbone Web API - Ordering Batches
 
 These views expose the basic CRUD interface to "ordering" batches, for the web
 API.
 """
 
 import datetime
+import logging
 
-from rattail.db import model
-from rattail.util import pretty_quantity
+import sqlalchemy as sa
+
+from rattail.db.model import PurchaseBatch, PurchaseBatchRow
 
 from cornice import Service
 
 from tailbone.api.batch import APIBatchView, APIBatchRowView
 
 
+log = logging.getLogger(__name__)
+
+
 class OrderingBatchViews(APIBatchView):
 
-    model_class = model.PurchaseBatch
+    model_class = PurchaseBatch
     default_handler_spec = 'rattail.batch.purchase:PurchaseBatchHandler'
     route_prefix = 'orderingbatchviews'
     permission_prefix = 'ordering'
     collection_url_prefix = '/ordering-batches'
     object_url_prefix = '/ordering-batch'
     supports_toggle_complete = True
     supports_execute = True
@@ -51,20 +56,21 @@
     def base_query(self):
         """
         Modifies the default logic as follows:
 
         Adds a condition to the query, to ensure only purchase batches with
         "ordering" mode are returned.
         """
-        query = super(OrderingBatchViews, self).base_query()
+        model = self.model
+        query = super().base_query()
         query = query.filter(model.PurchaseBatch.mode == self.enum.PURCHASE_BATCH_MODE_ORDERING)
         return query
 
     def normalize(self, batch):
-        data = super(OrderingBatchViews, self).normalize(batch)
+        data = super().normalize(batch)
 
         data['vendor_uuid'] = batch.vendor.uuid
         data['vendor_display'] = str(batch.vendor)
 
         data['department_uuid'] = batch.department_uuid
         data['department_display'] = str(batch.department) if batch.department else None
 
@@ -77,15 +83,15 @@
         """
         Modifies the default logic as follows:
 
         Sets the mode to "ordering" for the new batch.
         """
         data = dict(data)
         data['mode'] = self.enum.PURCHASE_BATCH_MODE_ORDERING
-        batch = super(OrderingBatchViews, self).create_object(data)
+        batch = super().create_object(data)
         return batch
 
     def worksheet(self):
         """
         Returns primary data for the Ordering Worksheet view.
         """
         batch = self.get_object()
@@ -217,26 +223,27 @@
         worksheet.add_view('GET', 'worksheet', klass=cls,
                            permission='{}.worksheet'.format(permission_prefix))
         config.add_cornice_service(worksheet)
 
 
 class OrderingBatchRowViews(APIBatchRowView):
 
-    model_class = model.PurchaseBatchRow
+    model_class = PurchaseBatchRow
     default_handler_spec = 'rattail.batch.purchase:PurchaseBatchHandler'
     route_prefix = 'ordering.rows'
     permission_prefix = 'ordering'
     collection_url_prefix = '/ordering-batch-rows'
     object_url_prefix = '/ordering-batch-row'
     supports_quick_entry = True
     editable = True
 
     def normalize(self, row):
+        data = super().normalize(row)
+        app = self.get_rattail_app()
         batch = row.batch
-        data = super(OrderingBatchRowViews, self).normalize(row)
 
         data['item_id'] = row.item_id
         data['upc'] = str(row.upc)
         data['upc_pretty'] = row.upc.pretty() if row.upc else None
         data['brand_name'] = row.brand_name
         data['description'] = row.description
         data['size'] = row.size
@@ -248,16 +255,16 @@
 
         # unit_uom can vary by product
         data['unit_uom'] = 'LB' if row.product and row.product.weighed else 'EA'
 
         data['case_quantity'] = row.case_quantity
         data['cases_ordered'] = row.cases_ordered
         data['units_ordered'] = row.units_ordered
-        data['cases_ordered_display'] = pretty_quantity(row.cases_ordered or 0, empty_zero=False)
-        data['units_ordered_display'] = pretty_quantity(row.units_ordered or 0, empty_zero=False)
+        data['cases_ordered_display'] = app.render_quantity(row.cases_ordered or 0, empty_zero=False)
+        data['units_ordered_display'] = app.render_quantity(row.units_ordered or 0, empty_zero=False)
 
         data['po_unit_cost'] = row.po_unit_cost
         data['po_unit_cost_display'] = "${:0.2f}".format(row.po_unit_cost) if row.po_unit_cost is not None else None
         data['po_total_calculated'] = row.po_total_calculated
         data['po_total_calculated_display'] = "${:0.2f}".format(row.po_total_calculated) if row.po_total_calculated is not None else None
         data['status_code'] = row.status_code
         data['status_display'] = row.STATUS.get(row.status_code, str(row.status_code))
@@ -277,15 +284,25 @@
         method of the batch handler.
 
         Note that the "normal" logic for this method is not invoked at all.
         """
         if not self.batch_handler.is_mutable(row.batch):
             return {'error': "Batch is not mutable"}
 
-        self.batch_handler.update_row_quantity(row, **data)
+        try:
+            self.batch_handler.update_row_quantity(row, **data)
+            self.Session.flush()
+        except Exception as error:
+            log.warning("update_row_quantity failed", exc_info=True)
+            if isinstance(error, sa.exc.DataError) and hasattr(error, 'orig'):
+                error = str(error.orig)
+            else:
+                error = str(error)
+            return {'error': error}
+
         return row
 
 
 def defaults(config, **kwargs):
     base = globals()
 
     OrderingBatchViews = kwargs.get('OrderingBatchViews', base['OrderingBatchViews'])
```

### Comparing `Tailbone-0.9.90/tailbone/api/batch/receiving.py` & `tailbone-0.9.91/tailbone/api/batch/receiving.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,14 +23,15 @@
 """
 Tailbone Web API - Receiving Batches
 """
 
 import logging
 
 import humanize
+import sqlalchemy as sa
 
 from rattail.db import model
 from rattail.util import pretty_quantity
 
 from cornice import Service
 from deform import widget as dfwidget
 
@@ -436,17 +437,25 @@
         row = self.Session.get(model.PurchaseBatchRow, form.validated['row'])
         if row is not self.get_object():
             return {'error': "Specified row does not match the route!"}
 
         # handler takes care of the row receiving logic for us
         kwargs = dict(form.validated)
         del kwargs['row']
-        self.batch_handler.receive_row(row, **kwargs)
+        try:
+            self.batch_handler.receive_row(row, **kwargs)
+            self.Session.flush()
+        except Exception as error:
+            log.warning("receive() failed", exc_info=True)
+            if isinstance(error, sa.exc.DataError) and hasattr(error, 'orig'):
+                error = str(error.orig)
+            else:
+                error = str(error)
+            return {'error': error}
 
-        self.Session.flush()
         return self._get(obj=row)
 
     @classmethod
     def defaults(cls, config):
         cls._defaults(config)
         cls._batch_row_defaults(config)
         cls._receiving_batch_row_defaults(config)
```

### Comparing `Tailbone-0.9.90/tailbone/api/common.py` & `tailbone-0.9.91/tailbone/api/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/core.py` & `tailbone-0.9.91/tailbone/api/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/customers.py` & `tailbone-0.9.91/tailbone/api/customers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/essentials.py` & `tailbone-0.9.91/tailbone/api/essentials.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/labels.py` & `tailbone-0.9.91/tailbone/api/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/master.py` & `tailbone-0.9.91/tailbone/api/master.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/master2.py` & `tailbone-0.9.91/tailbone/api/master2.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/people.py` & `tailbone-0.9.91/tailbone/api/people.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/products.py` & `tailbone-0.9.91/tailbone/api/products.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/upgrades.py` & `tailbone-0.9.91/tailbone/api/upgrades.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/users.py` & `tailbone-0.9.91/tailbone/api/users.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/vendors.py` & `tailbone-0.9.91/tailbone/api/vendors.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/api/workorders.py` & `tailbone-0.9.91/tailbone/api/workorders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/app.py` & `tailbone-0.9.91/tailbone/app.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/asgi.py` & `tailbone-0.9.91/tailbone/asgi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/auth.py` & `tailbone-0.9.91/tailbone/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/beaker.py` & `tailbone-0.9.91/tailbone/beaker.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/cleanup.py` & `tailbone-0.9.91/tailbone/cleanup.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/config.py` & `tailbone-0.9.91/tailbone/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -57,33 +57,14 @@
     return config.get('tailbone', 'csrf_token_name', default='_csrf')
 
 
 def csrf_header_name(config):
     return config.get('tailbone', 'csrf_header_name', default='X-CSRF-TOKEN')
 
 
-def get_buefy_version(config):
-    warnings.warn("get_buefy_version() is deprecated; please use "
-                  "tailbone.util.get_libver() instead",
-                  DeprecationWarning, stacklevel=2)
-
-    version = config.get('tailbone', 'libver.buefy')
-    if version:
-        return version
-
-    return config.get('tailbone', 'buefy_version',
-                      default='latest')
-
-
-def get_buefy_0_8(config, version=None):
-    warnings.warn("get_buefy_0_8() is no longer supported",
-                  DeprecationWarning, stacklevel=2)
-    return False
-
-
 def global_help_url(config):
     return config.get('tailbone', 'global_help_url')
 
 
 def protected_usernames(config):
     return config.getlist('tailbone', 'protected_usernames')
```

### Comparing `Tailbone-0.9.90/tailbone/db.py` & `tailbone-0.9.91/tailbone/db.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/diffs.py` & `tailbone-0.9.91/tailbone/diffs.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/exceptions.py` & `tailbone-0.9.91/tailbone/exceptions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/forms/__init__.py` & `tailbone-0.9.91/tailbone/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/forms/common.py` & `tailbone-0.9.91/tailbone/forms/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/forms/core.py` & `tailbone-0.9.91/tailbone/forms/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -29,35 +29,34 @@
 import logging
 import warnings
 from collections import OrderedDict
 
 import sqlalchemy as sa
 from sqlalchemy import orm
 from sqlalchemy.ext.associationproxy import AssociationProxy, ASSOCIATION_PROXY
+from wuttjamaican.util import UNSPECIFIED
 
-from rattail.time import localtime
-from rattail.util import prettify, pretty_boolean, pretty_quantity
-from rattail.core import UNSPECIFIED
+from rattail.util import prettify, pretty_boolean
 from rattail.db.util import get_fieldnames
 
 import colander
 import deform
 from colanderalchemy import SQLAlchemySchemaNode
 from colanderalchemy.schema import _creation_order
 from deform import widget as dfwidget
 from pyramid_deform import SessionFileUploadTempStore
 from pyramid.renderers import render
 from webhelpers2.html import tags, HTML
 
 from tailbone.db import Session
 from tailbone.util import raw_datetime, get_form_data, render_markdown
-from . import types
-from .widgets import (ReadonlyWidget, PlainDateWidget,
-                      JQueryDateWidget, JQueryTimeWidget,
-                      MultiFileUploadWidget)
+from tailbone.forms import types
+from tailbone.forms.widgets import (ReadonlyWidget, PlainDateWidget,
+                                    JQueryDateWidget, JQueryTimeWidget,
+                                    MultiFileUploadWidget)
 from tailbone.exceptions import TailboneJSONFieldError
 
 
 log = logging.getLogger(__name__)
 
 
 def get_association_proxy(mapper, field):
@@ -221,24 +220,24 @@
                     for column in next_prop.columns:
                         if isinstance(column.type, sa.LargeBinary):
                             excludes.append(next_prop.key)
 
         if excludes:
             overrides['excludes'] = excludes
 
-        return super(CustomSchemaNode, self).get_schema_from_relationship(prop, overrides)
+        return super().get_schema_from_relationship(prop, overrides)
 
     def dictify(self, obj):
         """ Return a dictified version of `obj` using schema information.
 
         .. note::
            This method was copied from upstream and modified to add automatic
            handling of "association proxy" fields.
         """
-        dict_ = super(CustomSchemaNode, self).dictify(obj)
+        dict_ = super().dictify(obj)
         for node in self:
 
             name = node.name
             if name not in dict_:
                 # we're only processing association proxy fields here
                 if not self.supported_association_proxy(name):
                     continue
@@ -790,20 +789,19 @@
         text = self.helptext[key]
         text = text.replace('"', '&quot;')
         return HTML.literal(text)
 
     def set_vuejs_field_converter(self, field, converter):
         self.vuejs_field_converters[field] = converter
 
-    def render(self, template=None, **kwargs):
-        if not template:
-            template = '/forms/form.mako'
-        context = kwargs
-        context['form'] = self
-        return render(template, context)
+    def render(self, **kwargs):
+        warnings.warn("Form.render() is deprecated (for now?); "
+                      "please use Form.render_deform() instead",
+                      DeprecationWarning, stacklevel=2)
+        return self.render_deform(**kwargs)
 
     def make_deform_form(self):
         if not hasattr(self, 'deform_form'):
 
             schema = self.make_schema()
 
             # TODO: we are still also doing this when making the schema, but
@@ -837,22 +835,22 @@
 
             self.deform_form = form
 
         return self.deform_form
 
     def render_deform(self, dform=None, template=None, **kwargs):
         if not template:
-            template = '/forms/deform_buefy.mako'
+            template = '/forms/deform.mako'
 
         if dform is None:
             dform = self.make_deform_form()
 
         # TODO: would perhaps be nice to leverage deform's default rendering
         # someday..? i.e. using Chameleon *.pt templates
-        # return form.render()
+        # return dform.render()
 
         context = kwargs
         context['form'] = self
         context['dform'] = dform
         context.setdefault('can_edit_help', self.can_edit_help)
         if context['can_edit_help']:
             context.setdefault('edit_help_url', self.edit_help_url)
@@ -964,20 +962,20 @@
            </tailbone-form>
         """
         kwargs = dict(self.vuejs_component_kwargs)
         if self.can_edit_help:
             kwargs.setdefault(':configure-fields-help', 'configureFieldsHelp')
         return HTML.tag(self.component, **kwargs)
 
-    def render_buefy_field(self, fieldname, bfield_attrs={}):
+    def render_field_complete(self, fieldname, bfield_attrs={}):
         """
-        Render the given field in a Buefy-compatible way.  Note that
-        this is meant to render *editable* fields, i.e. showing a
-        widget, unless the field input is hidden.  In other words it's
-        not for "readonly" fields.
+        Render the given field completely, i.e. with ``<b-field>``
+        wrapper.  Note that this is meant to render *editable* fields,
+        i.e. showing a widget, unless the field input is hidden.  In
+        other words it's not for "readonly" fields.
         """
         dform = self.make_deform_form()
         field = dform[fieldname] if fieldname in dform else None
 
         include = bool(field)
         if self.readonly or (not field and fieldname in self.readonly_fields):
             include = True
@@ -1128,15 +1126,16 @@
             return ""
         return raw_datetime(self.request.rattail_config, value)
 
     def render_datetime_local(self, record, field_name):
         value = self.obtain_value(record, field_name)
         if value is None:
             return ""
-        value = localtime(self.request.rattail_config, value)
+        app = self.get_rattail_app()
+        value = app.localtime(value)
         return raw_datetime(self.request.rattail_config, value)
 
     def render_duration(self, record, field_name):
         seconds = self.obtain_value(record, field_name)
         if seconds is None:
             return ""
         app = self.request.rattail_config.get_app()
@@ -1157,15 +1156,16 @@
         except ValueError:
             return str(value)
 
     def render_quantity(self, obj, field):
         value = self.obtain_value(obj, field)
         if value is None:
             return ""
-        return pretty_quantity(value)
+        app = self.get_rattail_app()
+        return app.render_quantity(value)
 
     def render_percent(self, obj, field):
         app = self.request.rattail_config.get_app()
         value = self.obtain_value(obj, field)
         return app.render_percent(value, places=3)
 
     def render_gpc(self, obj, field):
```

### Comparing `Tailbone-0.9.90/tailbone/forms/receiving.py` & `tailbone-0.9.91/tailbone/forms/receiving.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/forms/types.py` & `tailbone-0.9.91/tailbone/forms/types.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/forms/widgets.py` & `tailbone-0.9.91/tailbone/forms/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -53,19 +53,19 @@
 class NumberInputWidget(dfwidget.TextInputWidget):
     template = 'numberinput'
     autocomplete = 'off'
 
 
 class NumericInputWidget(NumberInputWidget):
     """
-    This widget only supports Buefy themes for now.  It uses a
-    ``<numeric-input>`` component, which will leverage the ``numeric.js``
-    functions to ensure user doesn't enter any non-numeric values.  Note that
-    this still uses a normal "text" input on the HTML side, as opposed to a
-    "number" input, since the latter is a bit ugly IMHO.
+    This widget uses a ``<numeric-input>`` component, which will
+    leverage the ``numeric.js`` functions to ensure user doesn't enter
+    any non-numeric values.  Note that this still uses a normal "text"
+    input on the HTML side, as opposed to a "number" input, since the
+    latter is a bit ugly IMHO.
     """
     template = 'numericinput'
     allow_enter = True
 
 
 class PercentInputWidget(dfwidget.TextInputWidget):
     """
@@ -149,14 +149,15 @@
     """
     This checkbox widget can be "dynamic" in the sense that form logic can
     control its value and state.
     """
     template = 'checkbox_dynamic'
 
 
+# TODO: deprecate / remove this
 class PlainSelectWidget(dfwidget.SelectWidget):
     template = 'select_plain'
 
 
 class CustomSelectWidget(dfwidget.SelectWidget):
     """
     This widget is mostly for convenience.  You can set extra kwargs for the
```

### Comparing `Tailbone-0.9.90/tailbone/grids/__init__.py` & `tailbone-0.9.91/tailbone/grids/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/grids/core.py` & `tailbone-0.9.91/tailbone/grids/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1329,60 +1329,60 @@
         if self.sortable:
             data = self.sort_data(data)
         if self.pageable:
             self.pager = self.paginate_data(data)
             data = self.pager
         return data
 
-    def render_complete(self, template='/grids/buefy.mako', **kwargs):
+    def render_complete(self, template='/grids/complete.mako', **kwargs):
         """
-        Render the complete grid, including filters.
-        """
-        context = kwargs
-        context['grid'] = self
-        context['request'] = self.request
-        context.setdefault('allow_save_defaults', True)
-        context.setdefault('view_click_handler', self.get_view_click_handler())
-        return render(template, context)
-
-    def render_buefy(self, template='/grids/buefy.mako', **kwargs):
-        """
-        Render the Buefy grid, complete with filters.  Note that this also
+        Render the grid, complete with filters.  Note that this also
         includes the context menu items and grid tools.
         """
         if 'grid_columns' not in kwargs:
-            kwargs['grid_columns'] = self.get_buefy_columns()
+            kwargs['grid_columns'] = self.get_table_columns()
 
         if 'grid_data' not in kwargs:
-            kwargs['grid_data'] = self.get_buefy_data()
+            kwargs['grid_data'] = self.get_table_data()
 
         if 'static_data' not in kwargs:
             kwargs['static_data'] = self.has_static_data()
 
         if self.filterable and 'filters_data' not in kwargs:
             kwargs['filters_data'] = self.get_filters_data()
 
         if self.filterable and 'filters_sequence' not in kwargs:
             kwargs['filters_sequence'] = self.get_filters_sequence()
 
-        return self.render_complete(template=template, **kwargs)
+        context = kwargs
+        context['grid'] = self
+        context['request'] = self.request
+        context.setdefault('allow_save_defaults', True)
+        context.setdefault('view_click_handler', self.get_view_click_handler())
+        return render(template, context)
 
-    def render_buefy_table_element(self, template='/grids/b-table.mako',
-                                   data_prop='gridData', empty_labels=False,
-                                   **kwargs):
+    def render_buefy(self, **kwargs):
+        warnings.warn("Grid.render_buefy() is deprecated; "
+                      "please use Grid.render_complete() instead",
+                      DeprecationWarning, stacklevel=2)
+        return self.render_complete(**kwargs)
+
+    def render_table_element(self, template='/grids/b-table.mako',
+                             data_prop='gridData', empty_labels=False,
+                             **kwargs):
         """
         This is intended for ad-hoc "small" grids with static data.  Renders
         just a ``<b-table>`` element instead of the typical "full" grid.
         """
         context = dict(kwargs)
         context['grid'] = self
         context['data_prop'] = data_prop
         context['empty_labels'] = empty_labels
         if 'grid_columns' not in context:
-            context['grid_columns'] = self.get_buefy_columns()
+            context['grid_columns'] = self.get_table_columns()
         context.setdefault('paginated', False)
         if context['paginated']:
             context.setdefault('per_page', 20)
         context['view_click_handler'] = self.get_view_click_handler()
         return render(template, context)
 
     def get_view_click_handler(self):
@@ -1433,15 +1433,15 @@
         Returns a list of filter keys (strings) in the sequence with which they
         should be displayed in the UI.
         """
         return list(self.filters)
 
     def get_filters_data(self):
         """
-        Returns a dict of current filters data, for use with Buefy grid view.
+        Returns a dict of current filters data, for use with index view.
         """
         data = {}
         for filtr in self.filters.values():
 
             valueless = [v for v in filtr.valueless_verbs
                          if v in filtr.verbs]
 
@@ -1569,18 +1569,18 @@
         data is represented as a SQLAlchemy query.
         """
         # TODO: should make this smarter?
         if isinstance(self.data, list):
             return True
         return False
 
-    def get_buefy_columns(self):
+    def get_table_columns(self):
         """
-        Return a list of dicts representing all grid columns.  Meant for use
-        with Buefy table.
+        Return a list of dicts representing all grid columns.  Meant
+        for use with the client-side JS table.
         """
         columns = []
         for name in self.columns:
             columns.append({
                 'field': name,
                 'label': self.get_label(name),
                 'sortable': self.sortable and name in self.sorters,
@@ -1594,17 +1594,18 @@
         if self.row_uuid_getter:
             return self.row_uuid_getter(rowobj)
 
         # otherwise fallback to normal uuid, if present
         if hasattr(rowobj, 'uuid'):
             return rowobj.uuid
 
-    def get_buefy_data(self):
+    def get_table_data(self):
         """
-        Returns a list of data rows for the grid, for use with Buefy table.
+        Returns a list of data rows for the grid, for use with
+        client-side JS table.
         """
         # filter / sort / paginate to get "visible" data
         raw_data = self.make_visible_data()
         data = []
         status_map = {}
         checked = []
 
@@ -1632,16 +1633,16 @@
 
             # sometimes we need to include some "raw" data columns in our
             # result set, even though the column is not displayed as part of
             # the grid.  this can be used for front-end editing of row data for
             # instance, when the "display" version is different than raw data.
             # here is the hack we use for that.
             columns = list(self.columns)
-            if hasattr(self, 'buefy_data_columns'):
-                columns.extend(self.buefy_data_columns)
+            if hasattr(self, 'raw_data_columns'):
+                columns.extend(self.raw_data_columns)
 
             # iterate over data fields
             for name in columns:
 
                 # leverage configured rendering logic where applicable;
                 # otherwise use "raw" data value as string
                 if self.renderers and name in self.renderers:
@@ -1698,15 +1699,15 @@
             results['total_items'] = count
 
         return results
 
     def set_action_urls(self, row, rowobj, i):
         """
         Pre-generate all action URLs for the given data row.  Meant for use
-        with Buefy table, since we can't generate URLs from JS.
+        with client-side table, since we can't generate URLs from JS.
         """
         for action in (self.main_actions + self.more_actions):
             url = action.get_url(rowobj, i)
             row['_action_url_{}'.format(action.key)] = url
 
     def is_linked(self, name):
         """
```

### Comparing `Tailbone-0.9.90/tailbone/grids/filters.py` & `tailbone-0.9.91/tailbone/grids/filters.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/handler.py` & `tailbone-0.9.91/tailbone/handler.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/helpers.py` & `tailbone-0.9.91/tailbone/helpers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/menus.py` & `tailbone-0.9.91/tailbone/menus.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/progress.py` & `tailbone-0.9.91/tailbone/progress.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/providers.py` & `tailbone-0.9.91/tailbone/providers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/reports/inventory_worksheet.mako` & `tailbone-0.9.91/tailbone/reports/inventory_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/reports/ordering_worksheet.mako` & `tailbone-0.9.91/tailbone/reports/ordering_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/scaffolds.py` & `tailbone-0.9.91/tailbone/scaffolds.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/__init__.py` & `tailbone-0.9.91/tailbone/static/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/codehilite.css` & `tailbone-0.9.91/tailbone/static/css/codehilite.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/diffs.css` & `tailbone-0.9.91/tailbone/static/css/diffs.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/forms.css` & `tailbone-0.9.91/tailbone/static/css/forms.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/grids.css` & `tailbone-0.9.91/tailbone/static/css/grids.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/grids.rowstatus.css` & `tailbone-0.9.91/tailbone/static/css/grids.rowstatus.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 /********************************************************************************
  * grids.rowstatus.css
  *
- * Add "row status" styles for Buefy grid tables.
+ * Add "row status" styles for grid tables.
  ********************************************************************************/
 
 /**************************************************
  * grid rows with "warning" status
  **************************************************/
 
 tr.warning {
```

### Comparing `Tailbone-0.9.90/tailbone/static/css/layout.css` & `tailbone-0.9.91/tailbone/static/css/layout.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/normalize.css` & `tailbone-0.9.91/tailbone/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/perms.css` & `tailbone-0.9.91/tailbone/static/css/perms.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/progress.css` & `tailbone-0.9.91/tailbone/static/css/progress.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/css/timesheet.css` & `tailbone-0.9.91/tailbone/static/css/timesheet.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/files/newproduct_template.xlsx` & `tailbone-0.9.91/tailbone/static/files/newproduct_template.xlsx`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/files/vendor_catalog_template.xlsx` & `tailbone-0.9.91/tailbone/static/files/vendor_catalog_template.xlsx`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/Hymenocephalus_italicus.jpg` & `tailbone-0.9.91/tailbone/static/img/Hymenocephalus_italicus.jpg`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/delete.png` & `tailbone-0.9.91/tailbone/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/edit.png` & `tailbone-0.9.91/tailbone/static/img/edit.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/home_logo.png` & `tailbone-0.9.91/tailbone/static/img/home_logo.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/loading.gif` & `tailbone-0.9.91/tailbone/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/product.png` & `tailbone-0.9.91/tailbone/static/img/product.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/rattail.ico` & `tailbone-0.9.91/tailbone/static/img/rattail.ico`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/save.png` & `tailbone-0.9.91/tailbone/static/img/save.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/testing.png` & `tailbone-0.9.91/tailbone/static/img/testing.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/img/view.png` & `tailbone-0.9.91/tailbone/static/img/view.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/debounce.js` & `tailbone-0.9.91/tailbone/static/js/debounce.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/numeric.js` & `tailbone-0.9.91/tailbone/static/js/numeric.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.autocomplete.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.autocomplete.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.datepicker.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.datepicker.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.grid.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.grid.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.message_recipients.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.message_recipients.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.numericinput.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.numericinput.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.oncebutton.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.oncebutton.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.buefy.timepicker.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.timepicker.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/static/js/tailbone.feedback.js` & `tailbone-0.9.91/tailbone/static/js/tailbone.feedback.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/subscribers.py` & `tailbone-0.9.91/tailbone/subscribers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -174,17 +174,14 @@
         # background color may be set per-request, by some apps
         if hasattr(request, 'background_color') and request.background_color:
             renderer_globals['background_color'] = request.background_color
         else: # otherwise we use the one from config
             renderer_globals['background_color'] = request.rattail_config.get(
                 'tailbone', 'background_color')
 
-        # TODO: remove this hack once nothing references it
-        renderer_globals['buefy_0_8'] = False
-
         # maybe set custom stylesheet
         css = None
         if request.user:
             css = request.rattail_config.get('tailbone.{}'.format(request.user.uuid),
                                              'buefy_css')
         if not css:
             css = request.rattail_config.get('tailbone', 'theme.falafel.buefy_css')
```

### Comparing `Tailbone-0.9.90/tailbone/templates/appinfo/configure.mako` & `tailbone-0.9.91/tailbone/templates/appinfo/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/appinfo/index.mako` & `tailbone-0.9.91/tailbone/templates/appinfo/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/appsettings.mako` & `tailbone-0.9.91/tailbone/templates/appsettings.mako`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
   </script>
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   <script type="text/javascript">
 
-    ThisPageData.groups = ${json.dumps(buefy_data)|n}
+    ThisPageData.groups = ${json.dumps(settings_data)|n}
     ThisPageData.showingGroup = ${json.dumps(current_group or '')|n}
 
   </script>
 </%def>
 
 <%def name="make_this_page_component()">
   ${parent.make_this_page_component()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/autocomplete.mako` & `tailbone-0.9.91/tailbone/templates/autocomplete.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/base.mako` & `tailbone-0.9.91/tailbone/templates/base.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/base_meta.mako` & `tailbone-0.9.91/tailbone/templates/base_meta.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/importer/view_row.mako` & `tailbone-0.9.91/tailbone/templates/batch/importer/view_row.mako`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
            </tr>
         % endfor
       </tbody>
     </table>
 % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <tailbone-form></tailbone-form>
     <br />
     ${self.field_diff_table()}
   </div>
 </%def>
```

#### html2text {}

```diff
@@ -11,11 +11,11 @@
 % elif instance.status_code in (enum.IMPORTER_BATCH_ROW_STATUS_UPDATE,
 enum.IMPORTER_BATCH_ROW_STATUS_NOCHANGE):
 ffiieelldd nnaammee oolldd vvaalluuee nneeww vvaalluuee
 % elif instance.status_code == enum.IMPORTER_BATCH_ROW_STATUS_DELETE:
 ffiieelldd nnaammee oolldd vvaalluuee                       nneeww vvaalluuee
 ${field}   ${repr(diff_old_values[field])}  
 % endif
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 
 ${self.field_diff_table()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/index.mako` & `tailbone-0.9.91/tailbone/templates/batch/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/inventory/desktop_form.mako` & `tailbone-0.9.91/tailbone/templates/batch/inventory/desktop_form.mako`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         % endif
 
       </div>
     </div>
   </nav>
 </%def>
 
-<%def name="render_form()">
+<%def name="render_form_template()">
   <script type="text/x-template" id="${form.component}-template">
     <div class="product-info">
 
       ${h.form(form.action_url, **{'@submit': 'handleSubmit'})}
       ${h.csrf_token(request)}
 
       ${h.hidden('product', **{':value': 'productInfo.uuid'})}
```

#### html2text {}

```diff
@@ -4,10 +4,10 @@
 Batch
 % if not batch.executed and master.has_perm('edit'): ${h.form
 (master.get_action_url('toggle_complete', batch), **{'@submit':
 'toggleCompleteSubmitting = true'})} ${h.csrf_token(request)} ${h.hidden
 ('complete', value='true')}
 disabled="toggleCompleteSubmitting"> {{ toggleCompleteSubmitting ? "Working,
 please wait..." : "Mark Complete" }} ${h.end_form()} % endif
-def> <%def name="render_form()">
+def> <%def name="render_form_template()">
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/pricing/configure.mako` & `tailbone-0.9.91/tailbone/templates/batch/pricing/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/configure.mako` & `tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/vendorcatalog/create.mako` & `tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/batch/view.mako` & `tailbone-0.9.91/tailbone/templates/batch/view.mako`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,18 @@
       % else:
           <p>TODO: batch cannot be executed..?</p>
       % endif
     </div>
   </div>
 </%def>
 
-<%def name="render_form()">
+<%def name="render_form_template()">
   ## TODO: should use self.render_form_buttons()
-  ## ${form.render(form_id='batch-form', buttons=capture(self.render_form_buttons))|n}
-  ${form.render(form_id='batch-form', buttons=capture(buttons))|n}
+  ## ${form.render_deform(form_id='batch-form', buttons=capture(self.render_form_buttons))|n}
+  ${form.render_deform(form_id='batch-form', buttons=capture(buttons))|n}
 </%def>
 
 <%def name="render_this_page()">
   ${parent.render_this_page()}
 
   % if master.has_worksheet_file and master.allow_worksheet(batch) and master.has_perm('worksheet'):
       <b-modal has-modal-card
@@ -202,15 +202,15 @@
       ${upload_worksheet_form.render_deform(buttons=False, form_kwargs={'ref': 'actualUploadForm'})|n}
   % endif
   % if master.handler.executable(batch) and master.has_perm('execute'):
       ${execute_form.render_deform(form_kwargs={'ref': 'actualExecuteForm'}, buttons=False)|n}
   % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <${form.component} @show-upload="showUploadDialog = true">
     </${form.component}>
   </div>
 </%def>
 
 <%def name="render_row_grid_tools()">
```

#### html2text {}

```diff
@@ -37,18 +37,18 @@
 click="submitExecuteBatch()" icon-left="arrow-circle-right" text="Execute
 Batch">
 % endif % else:
 TODO: batch *may* be executed, but not by *you*
 % endif % else:
 TODO: batch cannot be executed..?
 % endif
-def> <%def name="render_form()"> ## TODO: should use self.render_form_buttons()
-## ${form.render(form_id='batch-form', buttons=capture
-(self.render_form_buttons))|n} ${form.render(form_id='batch-form',
-buttons=capture(buttons))|n}
+def> <%def name="render_form_template()"> ## TODO: should use
+self.render_form_buttons() ## ${form.render_deform(form_id='batch-form',
+buttons=capture(self.render_form_buttons))|n} ${form.render_deform
+(form_id='batch-form', buttons=capture(buttons))|n}
 def> <%def name="render_this_page()"> ${parent.render_this_page()} % if
 master.has_worksheet_file and master.allow_worksheet(batch) and master.has_perm
 ('worksheet'):
 Upload Worksheet
 This will update the batch data with the worksheet file you provide.  Please be
 certain to use the right one!
 
@@ -61,15 +61,15 @@
 def> <%def name="render_this_page_template()"> $
 {parent.render_this_page_template()} % if master.has_worksheet_file and
 master.allow_worksheet(batch) and master.has_perm('worksheet'): $
 {upload_worksheet_form.render_deform(buttons=False, form_kwargs={'ref':
 'actualUploadForm'})|n} % endif % if master.handler.executable(batch) and
 master.has_perm('execute'): ${execute_form.render_deform(form_kwargs={'ref':
 'actualExecuteForm'}, buttons=False)|n} % endif
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 <${form.component} @show-upload="showUploadDialog = true">
 {form.component}>
 def> <%def name="render_row_grid_tools()"> ${parent.render_row_grid_tools()} %
 if master.rows_bulk_deletable and not batch.executed and master.has_perm
 ('delete_rows'):
 click="deleteResultsInit()" :disabled="!total" icon-pack="fas" icon-
 left="trash"> Delete Results
```

### Comparing `Tailbone-0.9.90/tailbone/templates/configure-menus.mako` & `tailbone-0.9.91/tailbone/templates/configure-menus.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/configure.mako` & `tailbone-0.9.91/tailbone/templates/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/customers/configure.mako` & `tailbone-0.9.91/tailbone/templates/customers/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/customers/pending/view.mako` & `tailbone-0.9.91/tailbone/templates/customers/pending/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/customers/view.mako` & `tailbone-0.9.91/tailbone/templates/customers/view.mako`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <%def name="object_helpers()">
   ${parent.object_helpers()}
   % if show_profiles_helper and show_profiles_people:
       ${view_profiles_helper(show_profiles_people)}
   % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <tailbone-form @detach-person="detachPerson">
     </tailbone-form>
   </div>
 </%def>
 
 <%def name="modify_this_page_vars()">
@@ -24,17 +24,15 @@
     ${form.component_studly}Data.shoppers = ${json.dumps(shoppers_data)|n}
     % endif
     % if expose_people:
     ${form.component_studly}Data.peopleData = ${json.dumps(people_data)|n}
     % endif
 
     ThisPage.methods.detachPerson = function(url) {
-        ## TODO: this should require POST, but we will add that once
-        ## we can assume a Buefy theme is present, to avoid having to
-        ## implement the logic in old jquery...
+        ## TODO: this should require POST! but for now we just redirect..
         if (confirm("Are you sure you want to detach this person from this customer account?")) {
             location.href = url
         }
     }
 
   </script>
 </%def>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 ## -*- coding: utf-8; -*- <%inherit file="/master/view.mako" /> <%namespace
 file="/util.mako" import="view_profiles_helper" /> <%def name="object_helpers
 ()"> ${parent.object_helpers()} % if show_profiles_helper and
 show_profiles_people: ${view_profiles_helper(show_profiles_people)} % endif
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 detach-person="detachPerson">
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/custorders/configure.mako` & `tailbone-0.9.91/tailbone/templates/custorders/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/custorders/create.mako` & `tailbone-0.9.91/tailbone/templates/custorders/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/custorders/items/view.mako` & `tailbone-0.9.91/tailbone/templates/custorders/items/view.mako`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/master/view.mako" />
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <${form.component} ref="mainForm"
                        % if master.has_perm('confirm_price'):
                        @confirm-price="showConfirmPrice"
                        % endif
                        % if master.has_perm('change_status'):
                        @change-status="showChangeStatus"
```

### Comparing `Tailbone-0.9.90/tailbone/templates/datasync/changes/index.mako` & `tailbone-0.9.91/tailbone/templates/datasync/changes/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/datasync/configure.mako` & `tailbone-0.9.91/tailbone/templates/datasync/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/datasync/status.mako` & `tailbone-0.9.91/tailbone/templates/datasync/status.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/autocomplete_jquery.pt` & `tailbone-0.9.91/tailbone/templates/deform/autocomplete_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/cases_units.pt` & `tailbone-0.9.91/tailbone/templates/deform/cases_units.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/checkbox_dynamic.pt` & `tailbone-0.9.91/tailbone/templates/deform/checkbox_dynamic.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/checked_password.pt` & `tailbone-0.9.91/tailbone/templates/deform/checked_password.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/date_jquery.pt` & `tailbone-0.9.91/tailbone/templates/deform/date_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/date_plain.pt` & `tailbone-0.9.91/tailbone/templates/deform/date_plain.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/datetime_falafel.pt` & `tailbone-0.9.91/tailbone/templates/deform/datetime_falafel.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/file_upload.pt` & `tailbone-0.9.91/tailbone/templates/deform/file_upload.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/message_recipients_buefy.pt` & `tailbone-0.9.91/tailbone/templates/deform/message_recipients.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/numberinput.pt` & `tailbone-0.9.91/tailbone/templates/deform/numberinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/password.pt` & `tailbone-0.9.91/tailbone/templates/deform/password.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/percentinput.pt` & `tailbone-0.9.91/tailbone/templates/deform/percentinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/permissions.pt` & `tailbone-0.9.91/tailbone/templates/deform/permissions.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/problem_report_days.pt` & `tailbone-0.9.91/tailbone/templates/deform/problem_report_days.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/select.pt` & `tailbone-0.9.91/tailbone/templates/deform/select.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/select_dynamic.pt` & `tailbone-0.9.91/tailbone/templates/deform/select_dynamic.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/select_jquery.pt` & `tailbone-0.9.91/tailbone/templates/deform/select_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/select_plain.pt` & `tailbone-0.9.91/tailbone/templates/deform/select_plain.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/textarea.pt` & `tailbone-0.9.91/tailbone/templates/deform/textarea.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/textinput.pt` & `tailbone-0.9.91/tailbone/templates/deform/textinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/deform/time_jquery.pt` & `tailbone-0.9.91/tailbone/templates/deform/time_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/diff.mako` & `tailbone-0.9.91/tailbone/templates/diff.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/email-bounces/view.mako` & `tailbone-0.9.91/tailbone/templates/email-bounces/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/employees/configure.mako` & `tailbone-0.9.91/tailbone/templates/employees/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/exception.mako` & `tailbone-0.9.91/tailbone/templates/exception.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/form.mako` & `tailbone-0.9.91/tailbone/templates/form.mako`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/page.mako" />
 
 <%def name="object_helpers()"></%def>
 
 <%def name="render_form_buttons()"></%def>
 
-<%def name="render_form()">
-  ${form.render(buttons=capture(self.render_form_buttons))|n}
+<%def name="render_form_template()">
+  ${form.render_deform(buttons=capture(self.render_form_buttons))|n}
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     ${form.render_vuejs_component()}
   </div>
 </%def>
 
 <%def name="page_content()">
   <div class="form-wrapper">
     <br />
-    ${self.render_buefy_form()}
+    ${self.render_form()}
   </div>
 </%def>
 
 <%def name="render_this_page()">
   <div style="display: flex; justify-content: space-between;">
 
     <div class="this-page-content">
@@ -45,15 +45,15 @@
   </div>
 </%def>
 
 <%def name="before_object_helpers()"></%def>
 
 <%def name="render_this_page_template()">
   % if form is not Undefined:
-      ${self.render_form()}
+      ${self.render_form_template()}
   % endif
   ${parent.render_this_page_template()}
 </%def>
 
 <%def name="finalize_this_page_vars()">
   ${parent.finalize_this_page_vars()}
   % if form is not Undefined:
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 ## -*- coding: utf-8; -*- <%inherit file="/page.mako" /> <%def
 name="object_helpers()">
 def> <%def name="render_form_buttons()">
-def> <%def name="render_form()"> ${form.render(buttons=capture
+def> <%def name="render_form_template()"> ${form.render_deform(buttons=capture
 (self.render_form_buttons))|n}
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 ${form.render_vuejs_component()}
 def> <%def name="page_content()">
 
-${self.render_buefy_form()}
+${self.render_form()}
 def> <%def name="render_this_page()">
 ${self.page_content()}
 ${before_object_helpers()}
 ${self.object_helpers()}
     * ${self.context_menu_items()}
 def> <%def name="before_object_helpers()">
 def> <%def name="render_this_page_template()"> % if form is not Undefined: $
-{self.render_form()} % endif ${parent.render_this_page_template()}
+{self.render_form_template()} % endif ${parent.render_this_page_template()}
 def> <%def name="finalize_this_page_vars()"> ${parent.finalize_this_page_vars
 ()} % if form is not Undefined:
 % endif
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/formposter.mako` & `tailbone-0.9.91/tailbone/templates/formposter.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/forms/deform_buefy.mako` & `tailbone-0.9.91/tailbone/templates/forms/deform.mako`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     % elif form.grouping:
         % for group in form.grouping:
             <nav class="panel">
               <p class="panel-heading">${group}</p>
               <div class="panel-block">
                 <div>
                   % for field in form.grouping[group]:
-                      ${form.render_buefy_field(field)}
+                      ${form.render_field_complete(field)}
                   % endfor
                 </div>
               </div>
             </nav>
         % endfor
     % else:
         % for field in form.fields:
-            ${form.render_buefy_field(field)}
+            ${form.render_field_complete(field)}
         % endfor
     % endif
   </section>
 
   % if buttons:
       <br />
       ${buttons|n}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/generate_feature.mako` & `tailbone-0.9.91/tailbone/templates/generate_feature.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/generated-projects/create.mako` & `tailbone-0.9.91/tailbone/templates/generated-projects/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/grids/b-table.mako` & `tailbone-0.9.91/tailbone/templates/grids/b-table.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/grids/buefy.mako` & `tailbone-0.9.91/tailbone/templates/grids/complete.mako`

 * *Files 3% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     <div style="display: flex; justify-content: space-between; margin-bottom: 0.5em;">
 
       <div style="display: flex; flex-direction: column; justify-content: space-between;">
         <div></div>
         <div class="filters">
           % if grid.filterable:
               ## TODO: stop using |n filter
-              ${grid.render_filters(template='/grids/filters_buefy.mako', allow_save_defaults=allow_save_defaults)|n}
+              ${grid.render_filters(allow_save_defaults=allow_save_defaults)|n}
           % endif
         </div>
       </div>
 
       <div style="display: flex; flex-direction: column; justify-content: space-between;">
 
         <div class="context-menu">
@@ -167,17 +167,14 @@
 
     <b-table
        :data="visibleData"
        ## :columns="columns"
        :loading="loading"
        :row-class="getRowClass"
 
-       ## TODO: this should be more configurable, maybe auto-detect based
-       ## on buefy version??  probably cannot do that, but this feature
-       ## is only supported with buefy 0.8.13 and newer
        % if request.rattail_config.getbool('tailbone', 'sticky_headers'):
        sticky-header
        height="600px"
        % endif
 
        :checkable="checkable"
 
@@ -580,24 +577,36 @@
                   params = new URLSearchParams(this.getBasicParams())
                   params.append('partial', true)
                   params = params.toString()
               }
 
               this.loading = true
               this.$http.get(`${'$'}{this.ajaxDataUrl}?${'$'}{params}`).then(({ data }) => {
-                  ${grid.component_studly}CurrentData = data.data
-                  this.data = ${grid.component_studly}CurrentData
-                  this.rowStatusMap = data.row_status_map
-                  this.total = data.total_items
-                  this.firstItem = data.first_item
-                  this.lastItem = data.last_item
-                  this.loading = false
-                  this.checkedRows = this.locateCheckedRows(data.checked_rows)
-                  if (success) {
-                      success()
+                  if (!data.error) {
+                      ${grid.component_studly}CurrentData = data.data
+                      this.data = ${grid.component_studly}CurrentData
+                      this.rowStatusMap = data.row_status_map
+                      this.total = data.total_items
+                      this.firstItem = data.first_item
+                      this.lastItem = data.last_item
+                      this.loading = false
+                      this.checkedRows = this.locateCheckedRows(data.checked_rows)
+                      if (success) {
+                          success()
+                      }
+                  } else {
+                      this.$buefy.toast.open({
+                          message: data.error,
+                          type: 'is-danger',
+                          duration: 2000, // 4 seconds
+                      })
+                      this.loading = false
+                      if (failure) {
+                          failure()
+                      }
                   }
               })
               .catch((error) => {
                   this.data = []
                   this.total = 0
                   this.loading = false
                   if (failure) {
```

### Comparing `Tailbone-0.9.90/tailbone/templates/grids/filters_buefy.mako` & `tailbone-0.9.91/tailbone/templates/grids/filters.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/grids/nav.mako` & `tailbone-0.9.91/tailbone/templates/grids/nav.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/home.mako` & `tailbone-0.9.91/tailbone/templates/home.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/importing/configure.mako` & `tailbone-0.9.91/tailbone/templates/importing/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/importing/runjob.mako` & `tailbone-0.9.91/tailbone/templates/importing/runjob.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/importing/view.mako` & `tailbone-0.9.91/tailbone/templates/importing/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/labels/profiles/edit.mako` & `tailbone-0.9.91/tailbone/templates/labels/profiles/edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/labels/profiles/view.mako` & `tailbone-0.9.91/tailbone/templates/labels/profiles/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/login.mako` & `tailbone-0.9.91/tailbone/templates/login.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/luigi/configure.mako` & `tailbone-0.9.91/tailbone/templates/luigi/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/luigi/index.mako` & `tailbone-0.9.91/tailbone/templates/luigi/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/clone.mako` & `tailbone-0.9.91/tailbone/templates/master/clone.mako`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/form.mako" />
 
 <%def name="title()">Clone ${model_title}: ${instance_title}</%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <br />
   <b-notification :closable="false">
     You are about to clone the following ${model_title} as a new record:
   </b-notification>
-  ${parent.render_buefy_form()}
+  ${parent.render_form()}
 </%def>
 
 <%def name="render_form_buttons()">
   <br />
   <b-notification :closable="false">
     Are you sure about this?
   </b-notification>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ## -*- coding: utf-8; -*- <%inherit file="/form.mako" /> <%def name="title
 ()">Clone ${model_title}: ${instance_title}
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 closable="false"> You are about to clone the following ${model_title} as a new
-record: ${parent.render_buefy_form()}
+record: ${parent.render_form()}
 def> <%def name="render_form_buttons()">
 closable="false"> Are you sure about this?
 ${h.form(request.current_route_url(), **{'@submit': 'submitForm'})} $
 {h.csrf_token(request)} ${h.hidden('clone', value='clone')}
 disabled="formSubmitting"> {{ submitButtonText }}
 ${h.end_form()}
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/master/configure.mako` & `tailbone-0.9.91/tailbone/templates/master/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/delete.mako` & `tailbone-0.9.91/tailbone/templates/master/delete.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/form.mako" />
 
 <%def name="title()">Delete ${model_title}: ${instance_title}</%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <br />
   <b-notification type="is-danger" :closable="false">
     You are about to delete the following ${model_title} and all associated data:
   </b-notification>
-  ${parent.render_buefy_form()}
+  ${parent.render_form()}
 </%def>
 
 <%def name="render_form_buttons()">
   <br />
   <b-notification type="is-danger" :closable="false">
     Are you sure about this?
   </b-notification>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ## -*- coding: utf-8; -*- <%inherit file="/form.mako" /> <%def name="title
 ()">Delete ${model_title}: ${instance_title}
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 closable="false"> You are about to delete the following ${model_title} and all
-associated data: ${parent.render_buefy_form()}
+associated data: ${parent.render_form()}
 def> <%def name="render_form_buttons()">
 closable="false"> Are you sure about this?
 ${h.form(request.current_route_url(), **{'@submit': 'submitForm'})} $
 {h.csrf_token(request)}
 disabled="formSubmitting"> {{ formButtonText }}
 ${h.end_form()}
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/master/edit_row.mako` & `tailbone-0.9.91/tailbone/templates/master/edit_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/form.mako` & `tailbone-0.9.91/tailbone/templates/master/form.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/index.mako` & `tailbone-0.9.91/tailbone/templates/master/index.mako`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
   ${self.page_content()}
 </%def>
 
 <%def name="render_this_page_template()">
   ${parent.render_this_page_template()}
 
   ## TODO: stop using |n filter
-  ${grid.render_buefy(tools=capture(self.grid_tools).strip(), context_menu=capture(self.context_menu_items).strip())|n}
+  ${grid.render_complete(tools=capture(self.grid_tools).strip(), context_menu=capture(self.context_menu_items).strip())|n}
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   <script type="text/javascript">
 
     % if master.supports_grid_totals:
```

### Comparing `Tailbone-0.9.90/tailbone/templates/master/merge.mako` & `tailbone-0.9.91/tailbone/templates/master/merge.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/versions.mako` & `tailbone-0.9.91/tailbone/templates/master/versions.mako`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   </script>
 </%def>
 
 <%def name="render_this_page_template()">
   ${parent.render_this_page_template()}
 
   ## TODO: stop using |n filter
-  ${grid.render_buefy()|n}
+  ${grid.render_complete()|n}
 </%def>
 
 <%def name="page_content()">
   <tailbone-grid :csrftoken="csrftoken">
   </tailbone-grid>
 </%def>
```

#### html2text {}

```diff
@@ -7,11 +7,11 @@
 {instance_title} Â» history
 def> <%def name="content_title()"> Version History
 def> <%def name="render_this_page()"> ${self.page_content()}
 def> <%def name="make_this_page_component()"> ${parent.make_this_page_component
 ()}
 def> <%def name="render_this_page_template()"> $
 {parent.render_this_page_template()} ## TODO: stop using |n filter $
-{grid.render_buefy()|n}
+{grid.render_complete()|n}
 def> <%def name="page_content()">
 csrftoken="csrftoken">
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/master/view.mako` & `tailbone-0.9.91/tailbone/templates/master/view.mako`

 * *Files 1% similar despite different names*

```diff
@@ -224,19 +224,19 @@
 <%def name="render_row_grid_component()">
   <tailbone-grid ref="rowGrid" id="rowGrid"></tailbone-grid>
 </%def>
 
 <%def name="render_this_page_template()">
   % if master.has_rows:
       ## TODO: stop using |n filter
-      ${rows_grid.render_buefy(allow_save_defaults=False, tools=capture(self.render_row_grid_tools))|n}
+      ${rows_grid.render_complete(allow_save_defaults=False, tools=capture(self.render_row_grid_tools))|n}
   % endif
   ${parent.render_this_page_template()}
   % if expose_versions:
-      ${versions_grid.render_buefy()|n}
+      ${versions_grid.render_complete()|n}
   % endif
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   % if expose_versions:
       <script type="text/javascript">
```

#### html2text {}

```diff
@@ -55,18 +55,18 @@
 [field].before}" v-show="viewVersionShowAllFields || version.values
 [field].after != version.values[field].before">
 {{ field }}
 active.sync="viewVersionLoading" :is-full-page="false">
 % endif
 def> <%def name="render_row_grid_component()">
 def> <%def name="render_this_page_template()"> % if master.has_rows: ## TODO:
-stop using |n filter ${rows_grid.render_buefy(allow_save_defaults=False,
+stop using |n filter ${rows_grid.render_complete(allow_save_defaults=False,
 tools=capture(self.render_row_grid_tools))|n} % endif $
 {parent.render_this_page_template()} % if expose_versions: $
-{versions_grid.render_buefy()|n} % endif
+{versions_grid.render_complete()|n} % endif
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()} %
 if expose_versions:
 % endif
 def> <%def name="modify_whole_page_vars()"> ${parent.modify_whole_page_vars()}
 def> <%def name="finalize_this_page_vars()"> ${parent.finalize_this_page_vars
 ()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/master/view_row.mako` & `tailbone-0.9.91/tailbone/templates/master/view_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/master/view_version.mako` & `tailbone-0.9.91/tailbone/templates/master/view_version.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/members/configure.mako` & `tailbone-0.9.91/tailbone/templates/members/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/menu.mako` & `tailbone-0.9.91/tailbone/templates/menu.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/messages/create.mako` & `tailbone-0.9.91/tailbone/templates/messages/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/messages/index.mako` & `tailbone-0.9.91/tailbone/templates/messages/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/messages/recipients.mako` & `tailbone-0.9.91/tailbone/templates/messages/recipients.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/messages/view.mako` & `tailbone-0.9.91/tailbone/templates/messages/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/multi_file_upload.mako` & `tailbone-0.9.91/tailbone/templates/multi_file_upload.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/ordering/view.mako` & `tailbone-0.9.91/tailbone/templates/ordering/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/ordering/worksheet.mako` & `tailbone-0.9.91/tailbone/templates/ordering/worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/page.mako` & `tailbone-0.9.91/tailbone/templates/page.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/page_help.mako` & `tailbone-0.9.91/tailbone/templates/page_help.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/people/configure.mako` & `tailbone-0.9.91/tailbone/templates/people/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/people/index.mako` & `tailbone-0.9.91/tailbone/templates/people/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/people/merge-requests/view.mako` & `tailbone-0.9.91/tailbone/templates/people/merge-requests/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/people/view.mako` & `tailbone-0.9.91/tailbone/templates/people/view.mako`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <%namespace file="/util.mako" import="view_profiles_helper" />
 
 <%def name="object_helpers()">
   ${parent.object_helpers()}
   ${view_profiles_helper([instance])}
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <tailbone-form v-on:make-user="makeUser"></tailbone-form>
   </div>
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 ## -*- coding: utf-8; -*- <%inherit file="/master/view.mako" /> <%namespace
 file="/util.mako" import="view_profiles_helper" /> <%def name="object_helpers
 ()"> ${parent.object_helpers()} ${view_profiles_helper([instance])}
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
 def> <%def name="page_content()"> ${parent.page_content()} % if not
 instance.users and request.has_perm('users.create'): ${h.form(url
 ('people.make_user'), ref='makeUserForm')} ${h.csrf_token(request)} ${h.hidden
 ('person_uuid', value=instance.uuid)} ${h.end_form()} % endif
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/people/view_profile_buefy.mako` & `tailbone-0.9.91/tailbone/templates/people/view_profile.mako`

 * *Files 0% similar despite different names*

```diff
@@ -1399,18 +1399,18 @@
               type="is-boxed"
               @input="activeTabChanged">
         ${self.render_profile_tabs()}
       </b-tabs>
 
       % if request.has_perm('people_profile.view_versions'):
 
-          ${revisions_grid.render_buefy_table_element(data_prop='revisions',
-                                                      show_footer=True,
-                                                      vshow='viewingHistory',
-                                                      loading='gettingRevisions')|n}
+          ${revisions_grid.render_table_element(data_prop='revisions',
+                                                show_footer=True,
+                                                vshow='viewingHistory',
+                                                loading='gettingRevisions')|n}
 
           <b-modal :active.sync="showingRevisionDialog">
 
             <div class="card">
               <div class="card-content">
 
                 <div style="display: flex; justify-content: space-between;">
```

### Comparing `Tailbone-0.9.90/tailbone/templates/poser/reports/view.mako` & `tailbone-0.9.91/tailbone/templates/poser/reports/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/poser/setup.mako` & `tailbone-0.9.91/tailbone/templates/poser/setup.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/poser/views/configure.mako` & `tailbone-0.9.91/tailbone/templates/poser/views/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/principal/find_by_perm.mako` & `tailbone-0.9.91/tailbone/templates/principal/find_by_perm.mako`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,16 @@
   </script>
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   <script type="text/javascript">
 
-    ThisPageData.permissionGroups = ${json.dumps(buefy_perms)|n}
-    ThisPageData.sortedGroups = ${json.dumps(buefy_sorted_groups)|n}
+    ThisPageData.permissionGroups = ${json.dumps(perms_data)|n}
+    ThisPageData.sortedGroups = ${json.dumps(sorted_groups_data)|n}
 
   </script>
 </%def>
 
 <%def name="make_this_page_component()">
   ${parent.make_this_page_component()}
   <script type="text/javascript">
@@ -109,15 +109,15 @@
         template: '#find-principals-template',
         props: {
             permissionGroups: Object,
             sortedGroups: Array
         },
         data() {
             return {
-                groupPermissions: ${json.dumps(buefy_perms.get(selected_group, {}).get('permissions', []))|n},
+                groupPermissions: ${json.dumps(perms_data.get(selected_group, {}).get('permissions', []))|n},
                 permissionGroupTerm: '',
                 permissionTerm: '',
                 selectedGroup: ${json.dumps(selected_group)|n},
                 selectedPermission: ${json.dumps(selected_permission)|n},
                 selectedPermissionLabel: ${json.dumps(selected_permission_label or '')|n},
                 formSubmitting: false,
             }
```

### Comparing `Tailbone-0.9.90/tailbone/templates/products/batch.mako` & `tailbone-0.9.91/tailbone/templates/products/batch.mako`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,25 @@
       Cancel
     </b-button>
   </div>
 
   ${h.end_form()}
 </%def>
 
-<%def name="render_form()">
+<%def name="render_form_template()">
   <script type="text/x-template" id="${form.component}-template">
     ${self.render_form_innards()}
   </script>
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   <script type="text/javascript">
 
-    ## TODO: ugh, an awful lot of duplicated code here (from /forms/deform_buefy.mako)
+    ## TODO: ugh, an awful lot of duplicated code here (from /forms/deform.mako)
 
     let ${form.component_studly} = {
         template: '#${form.component}-template',
         methods: {
 
             ## TODO: deprecate / remove the latter option here
             % if form.auto_disable_save or form.auto_disable:
```

#### html2text {}

```diff
@@ -13,10 +13,10 @@
 dform['notes'])} % for key, pform in six.iteritems(params_forms):
 % for field in pform.make_deform_form(): ${render_deform_field(pform, field)} %
 endfor
 % endfor
 disabled="${form.component_studly}Submitting"> {{ $
 {form.component_studly}ButtonText }} Cancel
 ${h.end_form()}
-def> <%def name="render_form()">
+def> <%def name="render_form_template()">
 def> <%def name="modify_this_page_vars()"> ${parent.modify_this_page_vars()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/products/configure.mako` & `tailbone-0.9.91/tailbone/templates/products/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/products/index.mako` & `tailbone-0.9.91/tailbone/templates/products/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/products/lookup.mako` & `tailbone-0.9.91/tailbone/templates/products/lookup.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/products/pending/view.mako` & `tailbone-0.9.91/tailbone/templates/products/pending/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/products/view.mako` & `tailbone-0.9.91/tailbone/templates/products/view.mako`

 * *Files 2% similar despite different names*

```diff
@@ -104,28 +104,28 @@
 </%def>
 
 <%def name="render_movement_fields(form)">
     ${form.render_field_readonly('last_sold')}
 </%def>
 
 <%def name="lookup_codes_grid()">
-  ${lookup_codes['grid'].render_buefy_table_element(data_prop='lookupCodesData')|n}
+  ${lookup_codes['grid'].render_table_element(data_prop='lookupCodesData')|n}
 </%def>
 
 <%def name="lookup_codes_panel()">
   <nav class="panel">
     <p class="panel-heading">Additional Lookup Codes</p>
     <div class="panel-block">
       ${self.lookup_codes_grid()}
     </div>
   </nav>
 </%def>
 
 <%def name="sources_grid()">
-  ${vendor_sources['grid'].render_buefy_table_element(data_prop='vendorSourcesData')|n}
+  ${vendor_sources['grid'].render_table_element(data_prop='vendorSourcesData')|n}
 </%def>
 
 <%def name="sources_panel()">
   <nav class="panel">
     <p class="panel-heading">
       Vendor Sources
       % if request.rattail_config.versioning_enabled() and master.has_perm('versions'):
@@ -171,15 +171,15 @@
         <div class="modal-card">
           <header class="modal-card-head">
             <p class="modal-card-title">
               Regular Price History
             </p>
           </header>
           <section class="modal-card-body">
-            ${regular_price_history_grid.render_buefy_table_element(data_prop='regularPriceHistoryData', loading='regularPriceHistoryLoading', paginated=True, per_page=10)|n}
+            ${regular_price_history_grid.render_table_element(data_prop='regularPriceHistoryData', loading='regularPriceHistoryLoading', paginated=True, per_page=10)|n}
           </section>
           <footer class="modal-card-foot">
             <b-button @click="showingPriceHistory_regular = false">
               Close
             </b-button>
           </footer>
         </div>
@@ -190,15 +190,15 @@
         <div class="modal-card">
           <header class="modal-card-head">
             <p class="modal-card-title">
               Current Price History
             </p>
           </header>
           <section class="modal-card-body">
-            ${current_price_history_grid.render_buefy_table_element(data_prop='currentPriceHistoryData', loading='currentPriceHistoryLoading', paginated=True, per_page=10)|n}
+            ${current_price_history_grid.render_table_element(data_prop='currentPriceHistoryData', loading='currentPriceHistoryLoading', paginated=True, per_page=10)|n}
           </section>
           <footer class="modal-card-foot">
             <b-button @click="showingPriceHistory_current = false">
               Close
             </b-button>
           </footer>
         </div>
@@ -209,15 +209,15 @@
         <div class="modal-card">
           <header class="modal-card-head">
             <p class="modal-card-title">
               Suggested Price History
             </p>
           </header>
           <section class="modal-card-body">
-            ${suggested_price_history_grid.render_buefy_table_element(data_prop='suggestedPriceHistoryData', loading='suggestedPriceHistoryLoading', paginated=True, per_page=10)|n}
+            ${suggested_price_history_grid.render_table_element(data_prop='suggestedPriceHistoryData', loading='suggestedPriceHistoryLoading', paginated=True, per_page=10)|n}
           </section>
           <footer class="modal-card-foot">
             <b-button @click="showingPriceHistory_suggested = false">
               Close
             </b-button>
           </footer>
         </div>
@@ -228,15 +228,15 @@
         <div class="modal-card">
           <header class="modal-card-head">
             <p class="modal-card-title">
               Cost History
             </p>
           </header>
           <section class="modal-card-body">
-            ${cost_history_grid.render_buefy_table_element(data_prop='costHistoryData', loading='costHistoryLoading', paginated=True, per_page=10)|n}
+            ${cost_history_grid.render_table_element(data_prop='costHistoryData', loading='costHistoryLoading', paginated=True, per_page=10)|n}
           </section>
           <footer class="modal-card-foot">
             <b-button @click="showingCostHistory = false">
               Close
             </b-button>
           </footer>
         </div>
@@ -285,15 +285,15 @@
 
     ThisPageData.vendorSourcesData = ${json.dumps(vendor_sources['data'])|n}
     ThisPageData.lookupCodesData = ${json.dumps(lookup_codes['data'])|n}
 
     % if request.rattail_config.versioning_enabled() and master.has_perm('versions'):
 
         ThisPageData.showingPriceHistory_regular = false
-        ThisPageData.regularPriceHistoryDataRaw = ${json.dumps(regular_price_history_grid.get_buefy_data()['data'])|n}
+        ThisPageData.regularPriceHistoryDataRaw = ${json.dumps(regular_price_history_grid.get_table_data()['data'])|n}
         ThisPageData.regularPriceHistoryLoading = false
 
         ThisPage.computed.regularPriceHistoryData = function() {
             let data = []
             this.regularPriceHistoryDataRaw.forEach(raw => {
                 data.push({
                     price: raw.price_display,
@@ -314,15 +314,15 @@
             this.$http.get(url, {params: params}).then(response => {
                 this.regularPriceHistoryDataRaw = response.data
                 this.regularPriceHistoryLoading = false
             })
         }
 
         ThisPageData.showingPriceHistory_current = false
-        ThisPageData.currentPriceHistoryDataRaw = ${json.dumps(current_price_history_grid.get_buefy_data()['data'])|n}
+        ThisPageData.currentPriceHistoryDataRaw = ${json.dumps(current_price_history_grid.get_table_data()['data'])|n}
         ThisPageData.currentPriceHistoryLoading = false
 
         ThisPage.computed.currentPriceHistoryData = function() {
             let data = []
             this.currentPriceHistoryDataRaw.forEach(raw => {
                 data.push({
                     price: raw.price_display,
@@ -344,15 +344,15 @@
             this.$http.get(url, {params: params}).then(response => {
                 this.currentPriceHistoryDataRaw = response.data
                 this.currentPriceHistoryLoading = false
             })
         }
 
         ThisPageData.showingPriceHistory_suggested = false
-        ThisPageData.suggestedPriceHistoryDataRaw = ${json.dumps(suggested_price_history_grid.get_buefy_data()['data'])|n}
+        ThisPageData.suggestedPriceHistoryDataRaw = ${json.dumps(suggested_price_history_grid.get_table_data()['data'])|n}
         ThisPageData.suggestedPriceHistoryLoading = false
 
         ThisPage.computed.suggestedPriceHistoryData = function() {
             let data = []
             this.suggestedPriceHistoryDataRaw.forEach(raw => {
                 data.push({
                     price: raw.price_display,
@@ -373,15 +373,15 @@
             this.$http.get(url, {params: params}).then(response => {
                 this.suggestedPriceHistoryDataRaw = response.data
                 this.suggestedPriceHistoryLoading = false
             })
         }
 
         ThisPageData.showingCostHistory = false
-        ThisPageData.costHistoryDataRaw = ${json.dumps(cost_history_grid.get_buefy_data()['data'])|n}
+        ThisPageData.costHistoryDataRaw = ${json.dumps(cost_history_grid.get_table_data()['data'])|n}
         ThisPageData.costHistoryLoading = false
 
         ThisPage.computed.costHistoryData = function() {
             let data = []
             this.costHistoryDataRaw.forEach(raw => {
                 data.push({
                     cost: raw.cost_display,
```

#### html2text {}

```diff
@@ -34,20 +34,20 @@
 ['flag']: ${form.render_field_readonly(field)} % endfor
 def> <%def name="movement_panel()">
 Movement
 ${self.render_movement_fields(form)}
 def> <%def name="render_movement_fields(form)"> ${form.render_field_readonly
 ('last_sold')}
 def> <%def name="lookup_codes_grid()"> ${lookup_codes
-['grid'].render_buefy_table_element(data_prop='lookupCodesData')|n}
+['grid'].render_table_element(data_prop='lookupCodesData')|n}
 def> <%def name="lookup_codes_panel()">
 Additional Lookup Codes
 ${self.lookup_codes_grid()}
-def> <%def name="sources_grid()"> ${vendor_sources
-['grid'].render_buefy_table_element(data_prop='vendorSourcesData')|n}
+def> <%def name="sources_grid()"> ${vendor_sources['grid'].render_table_element
+(data_prop='vendorSourcesData')|n}
 def> <%def name="sources_panel()">
 Vendor Sources % if request.rattail_config.versioning_enabled() and
 master.has_perm('versions'): click.prevent="showCostHistory()"> (view cost
 history)
 % endif
 ${self.sources_grid()}
 def> <%def name="notes_panel()">
@@ -58,33 +58,33 @@
 ${form.render_field_readonly('ingredients')}
 def> <%def name="extra_left_panels()">
 def> <%def name="extra_right_panels()">
 def> <%def name="render_this_page()"> ${parent.render_this_page()} % if
 request.rattail_config.versioning_enabled() and master.has_perm('versions'):
 active.sync="showingPriceHistory_regular" has-modal-card>
 Regular Price History
-${regular_price_history_grid.render_buefy_table_element
+${regular_price_history_grid.render_table_element
 (data_prop='regularPriceHistoryData', loading='regularPriceHistoryLoading',
 paginated=True, per_page=10)|n}
 click="showingPriceHistory_regular = false"> Close
 active.sync="showingPriceHistory_current" has-modal-card>
 Current Price History
-${current_price_history_grid.render_buefy_table_element
+${current_price_history_grid.render_table_element
 (data_prop='currentPriceHistoryData', loading='currentPriceHistoryLoading',
 paginated=True, per_page=10)|n}
 click="showingPriceHistory_current = false"> Close
 active.sync="showingPriceHistory_suggested" has-modal-card>
 Suggested Price History
-${suggested_price_history_grid.render_buefy_table_element
+${suggested_price_history_grid.render_table_element
 (data_prop='suggestedPriceHistoryData', loading='suggestedPriceHistoryLoading',
 paginated=True, per_page=10)|n}
 click="showingPriceHistory_suggested = false"> Close
 active.sync="showingCostHistory" has-modal-card>
 Cost History
-${cost_history_grid.render_buefy_table_element(data_prop='costHistoryData',
+${cost_history_grid.render_table_element(data_prop='costHistoryData',
 loading='costHistoryLoading', paginated=True, per_page=10)|n}
 click="showingCostHistory = false"> Close
 % endif
 def> <%def name="page_content()">
 Product
 ${self.render_main_fields(form)}
 % if image_url: ${h.image(image_url, "Product Image", id='product-image',
```

### Comparing `Tailbone-0.9.90/tailbone/templates/progress.mako` & `tailbone-0.9.91/tailbone/templates/progress.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/purchases/credits/index.mako` & `tailbone-0.9.91/tailbone/templates/purchases/credits/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/purchases/receiving_worksheet.mako` & `tailbone-0.9.91/tailbone/templates/purchases/receiving_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/purchases/view.mako` & `tailbone-0.9.91/tailbone/templates/purchases/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/receiving/configure.mako` & `tailbone-0.9.91/tailbone/templates/receiving/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/receiving/declare_credit.mako` & `tailbone-0.9.91/tailbone/templates/receiving/declare_credit.mako`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/form.mako" />
-<%namespace file="/forms/util.mako" import="render_buefy_field" />
 
 <%def name="title()">Declare Credit for Row #${row.sequence}</%def>
 
 <%def name="context_menu_items()">
   ${parent.context_menu_items()}
   % if master.rows_viewable and master.has_perm('view'):
       <li>${h.link_to("View this {}".format(row_model_title), row_action_url('view', row))}</li>
   % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
 
   <p class="block">
     Please select the "state" of the product, and enter the
     appropriate quantity.
   </p>
 
   <p class="block">
@@ -27,27 +26,27 @@
   </p>
 
   <p class="block">
     Please see ${h.link_to("Receive Row", url('{}.receive_row'.format(route_prefix), uuid=batch.uuid, row_uuid=row.uuid))}
     if you need to "receive" instead of "convert" the product.
   </p>
 
-  ${parent.render_buefy_form()}
+  ${parent.render_form()}
 
 </%def>
 
-<%def name="buefy_form_body()">
+<%def name="form_body()">
 
-  ${render_buefy_field(dform['credit_type'])}
+  ${form.render_field_complete('credit_type')}
 
-  ${render_buefy_field(dform['quantity'])}
+  ${form.render_field_complete('quantity')}
 
-  ${render_buefy_field(dform['expiration_date'], bfield_kwargs={'v-show': "field_model_credit_type == 'expired'"})}
+  ${form.render_field_complete('expiration_date', bfield_attrs={'v-show': "field_model_credit_type == 'expired'"})}
 
 </%def>
 
-<%def name="render_form()">
-  ${form.render_deform(buttons=capture(self.render_form_buttons), form_body=capture(self.buefy_form_body))|n}
+<%def name="render_form_template()">
+  ${form.render_deform(buttons=capture(self.render_form_buttons), form_body=capture(self.form_body))|n}
 </%def>
 
 
 ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/receiving/receive_row.mako` & `tailbone-0.9.91/tailbone/templates/receiving/receive_row.mako`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/form.mako" />
-<%namespace file="/forms/util.mako" import="render_buefy_field" />
 
 <%def name="title()">Receive for Row #${row.sequence}</%def>
 
 <%def name="context_menu_items()">
   ${parent.context_menu_items()}
   % if master.rows_viewable and master.has_perm('view'):
       <li>${h.link_to("View this {}".format(row_model_title), row_action_url('view', row))}</li>
   % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
 
   <p class="block">
     Please select the "state" of the product, and enter the appropriate
     quantity.
   </p>
 
   <p class="block">
@@ -24,27 +23,27 @@
   </p>
 
   <p class="block">
     Please see ${h.link_to("Declare Credit", url('{}.declare_credit'.format(route_prefix), uuid=batch.uuid, row_uuid=row.uuid))}
     if you need to "convert" some already-received amount, into a credit.
   </p>
 
-  ${parent.render_buefy_form()}
+  ${parent.render_form()}
 
 </%def>
 
-<%def name="buefy_form_body()">
+<%def name="form_body()">
 
-  ${render_buefy_field(dform['mode'])}
+  ${form.render_field_complete('mode')}
 
-  ${render_buefy_field(dform['quantity'])}
+  ${form.render_field_complete('quantity')}
 
-  ${render_buefy_field(dform['expiration_date'], bfield_kwargs={'v-show': "field_model_mode == 'expired'"})}
+  ${form.render_field_complete('expiration_date', bfield_attrs={'v-show': "field_model_mode == 'expired'"})}
 
 </%def>
 
-<%def name="render_form()">
-  ${form.render_deform(buttons=capture(self.render_form_buttons), form_body=capture(self.buefy_form_body))|n}
+<%def name="render_form_template()">
+  ${form.render_deform(buttons=capture(self.render_form_buttons), form_body=capture(self.form_body))|n}
 </%def>
 
 
 ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/receiving/view.mako` & `tailbone-0.9.91/tailbone/templates/receiving/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/receiving/view_row.mako` & `tailbone-0.9.91/tailbone/templates/receiving/view_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/generated/choose.mako` & `tailbone-0.9.91/tailbone/templates/reports/generated/choose.mako`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             margin-top: 2em;
         }
     % endif
 
   </style>
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <p>Please select the type of report you wish to generate.</p>
     <br />
     <div style="display: flex;">
       <tailbone-form v-on:report-change="reportChanged"></tailbone-form>
       <div id="report-description">{{ reportDescription }}</div>
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 ## -*- coding: utf-8; -*- <%inherit file="/master/create.mako" /> <%def
 name="extra_styles()"> ${parent.extra_styles()}
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 Please select the type of report you wish to generate.
 
 {{ reportDescription }}
 def> <%def name="page_content()"> % if use_form: ${parent.page_content()} %
 else:
 
 Please select the type of report you wish to generate.
```

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/generated/configure.mako` & `tailbone-0.9.91/tailbone/templates/reports/generated/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/generated/generate.mako` & `tailbone-0.9.91/tailbone/templates/reports/generated/generate.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/master/form.mako" />
 
 <%def name="title()">${index_title} &raquo; ${report.name}</%def>
 
 <%def name="content_title()">New Report:&nbsp; ${report.name}</%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <p class="block">
       ${report.__doc__}
     </p>
     % if report.help_url:
         <p class="block">
           <b-button icon-pack="fas"
```

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/generated/view.mako` & `tailbone-0.9.91/tailbone/templates/reports/generated/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/inventory.mako` & `tailbone-0.9.91/tailbone/templates/reports/inventory.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/ordering.mako` & `tailbone-0.9.91/tailbone/templates/reports/ordering.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/reports/problems/view.mako` & `tailbone-0.9.91/tailbone/templates/reports/problems/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/roles/create.mako` & `tailbone-0.9.91/tailbone/templates/roles/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/roles/edit.mako` & `tailbone-0.9.91/tailbone/templates/roles/edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/settings/email/configure.mako` & `tailbone-0.9.91/tailbone/templates/settings/email/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/settings/email/index.mako` & `tailbone-0.9.91/tailbone/templates/settings/email/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/settings/email/view.mako` & `tailbone-0.9.91/tailbone/templates/settings/email/view.mako`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## -*- coding: utf-8; -*-
 <%inherit file="/master/view.mako" />
 
-<%def name="render_buefy_form()">
-  ${parent.render_buefy_form()}
+<%def name="render_form()">
+  ${parent.render_form()}
   <email-preview-tools></email-preview-tools>
 </%def>
 
 <%def name="render_this_page_template()">
   ${parent.render_this_page_template()}
   <script type="text/x-template" id="email-preview-tools-template">
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 ## -*- coding: utf-8; -*- <%inherit file="/master/view.mako" /> <%def
-name="render_buefy_form()"> ${parent.render_buefy_form()}
+name="render_form()"> ${parent.render_form()}
 def> <%def name="render_this_page_template()"> $
 {parent.render_this_page_template()}
 def> <%def name="make_this_page_component()"> ${parent.make_this_page_component
 ()}
 def> ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/base.mako` & `tailbone-0.9.91/tailbone/templates/shifts/base.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/schedule.mako` & `tailbone-0.9.91/tailbone/templates/shifts/schedule.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/schedule_edit.mako` & `tailbone-0.9.91/tailbone/templates/shifts/schedule_edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/schedule_print.mako` & `tailbone-0.9.91/tailbone/templates/shifts/schedule_print.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/schedule_print_employee.mako` & `tailbone-0.9.91/tailbone/templates/shifts/schedule_print_employee.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/timesheet.mako` & `tailbone-0.9.91/tailbone/templates/shifts/timesheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/shifts/timesheet_edit.mako` & `tailbone-0.9.91/tailbone/templates/shifts/timesheet_edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tables/create.mako` & `tailbone-0.9.91/tailbone/templates/tables/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tempmon/appliances/index.mako` & `tailbone-0.9.91/tailbone/templates/tempmon/appliances/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tempmon/clients/view.mako` & `tailbone-0.9.91/tailbone/templates/tempmon/clients/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tempmon/dashboard.mako` & `tailbone-0.9.91/tailbone/templates/tempmon/dashboard.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tempmon/probes/graph.mako` & `tailbone-0.9.91/tailbone/templates/tempmon/probes/graph.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/tempmon/probes/view.mako` & `tailbone-0.9.91/tailbone/templates/tempmon/probes/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/configure.mako` & `tailbone-0.9.91/tailbone/templates/trainwreck/transactions/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/trainwreck/transactions/rollover.mako` & `tailbone-0.9.91/tailbone/templates/trainwreck/transactions/rollover.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/units-of-measure/index.mako` & `tailbone-0.9.91/tailbone/templates/units-of-measure/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/upgrade.mako` & `tailbone-0.9.91/tailbone/templates/upgrade.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/upgrades/configure.mako` & `tailbone-0.9.91/tailbone/templates/upgrades/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/upgrades/view.mako` & `tailbone-0.9.91/tailbone/templates/upgrades/view.mako`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
   % if master.has_perm('execute'):
       ${h.form(master.get_action_url('declare_failure', instance), ref='declareFailureForm')}
       ${h.csrf_token(request)}
       ${h.end_form()}
   % endif
 </%def>
 
-<%def name="render_buefy_form()">
+<%def name="render_form()">
   <div class="form">
     <${form.component}
       % if master.has_perm('execute'):
       @declare-failure-click="declareFailureClick"
       :declare-failure-submitting="declareFailureSubmitting"
       % if expose_websockets:
       % if instance_executable:
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 # :value="80" ## show-value ## format="percent" >
 click="declareFailureClick()"> Declare Failure
 key="line.key" v-html="line.text"> ## nb. we auto-scroll down to "see" this
 element
 % endif % if master.has_perm('execute'): ${h.form(master.get_action_url
 ('declare_failure', instance), ref='declareFailureForm')} ${h.csrf_token
 (request)} ${h.end_form()} % endif
-def> <%def name="render_buefy_form()">
+def> <%def name="render_form()">
 <${form.component} % if master.has_perm('execute'): @declare-failure-
 click="declareFailureClick" :declare-failure-
 submitting="declareFailureSubmitting" % if expose_websockets: % if
 instance_executable: @execute-upgrade-click="executeUpgrade" % endif :upgrade-
 executing="upgradeExecuting" % endif % endif >
 {form.component}>
 def> <%def name="render_form_buttons()"> % if instance_executable and
```

### Comparing `Tailbone-0.9.90/tailbone/templates/users/preferences.mako` & `tailbone-0.9.91/tailbone/templates/users/preferences.mako`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   <h3 class="block is-size-3">Display</h3>
   <div class="block" style="padding-left: 2rem;">
 
     <b-field label="Theme Style">
         <b-select name="tailbone.${user.uuid}.buefy_css"
                   v-model="simpleSettings['tailbone.${user.uuid}.buefy_css']"
                   @input="settingsNeedSaved = true">
-          <option v-for="option in buefyCSSOptions"
+          <option v-for="option in themeStyleOptions"
                   :key="option.value"
                   :value="option.value">
             {{ option.label }}
           </option>
         </b-select>
 
     </b-field>  
@@ -42,14 +42,14 @@
   </div>
 </%def>
 
 <%def name="modify_this_page_vars()">
   ${parent.modify_this_page_vars()}
   <script type="text/javascript">
 
-    ThisPageData.buefyCSSOptions = ${json.dumps(buefy_css_options)|n}
+    ThisPageData.themeStyleOptions = ${json.dumps(theme_style_options)|n}
 
   </script>
 </%def>
 
 
 ${parent.body()}
```

### Comparing `Tailbone-0.9.90/tailbone/templates/users/view.mako` & `tailbone-0.9.91/tailbone/templates/users/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/util.mako` & `tailbone-0.9.91/tailbone/templates/util.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/vendors/configure.mako` & `tailbone-0.9.91/tailbone/templates/vendors/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/views/model/create.mako` & `tailbone-0.9.91/tailbone/templates/views/model/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/templates/workorders/view.mako` & `tailbone-0.9.91/tailbone/templates/workorders/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/tweens.py` & `tailbone-0.9.91/tailbone/tweens.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/util.py` & `tailbone-0.9.91/tailbone/util.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/__init__.py` & `tailbone-0.9.91/tailbone/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/asgi/__init__.py` & `tailbone-0.9.91/tailbone/views/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/asgi/datasync.py` & `tailbone-0.9.91/tailbone/views/asgi/datasync.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/asgi/upgrades.py` & `tailbone-0.9.91/tailbone/views/asgi/upgrades.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/auth.py` & `tailbone-0.9.91/tailbone/views/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/__init__.py` & `tailbone-0.9.91/tailbone/views/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/core.py` & `tailbone-0.9.91/tailbone/views/batch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -28,31 +28,26 @@
 import sys
 import json
 import datetime
 import logging
 import socket
 import subprocess
 import tempfile
+import warnings
 
 import json
 import markdown
 import sqlalchemy as sa
 from sqlalchemy import orm
 
-from rattail.db import model, Session as RattailSession
-from rattail.db.util import short_session
 from rattail.threads import Thread
-from rattail.util import prettify, simple_error
-from rattail.progress import SocketProgress
+from rattail.util import simple_error
 
 import colander
-import deform
 from deform import widget as dfwidget
-from pyramid.renderers import render_to_response
-from pyramid.response import FileResponse
 from webhelpers2.html import HTML, tags
 
 from tailbone import forms, grids
 from tailbone.db import Session
 from tailbone.views import MasterView
 from tailbone.util import csrf_token
 
@@ -111,15 +106,15 @@
     row_labels = {
         'upc': "UPC",
         'item_id': "Item ID",
         'status_code': "Status",
     }
 
     def __init__(self, request):
-        super(BatchMasterView, self).__init__(request)
+        super().__init__(request)
         self.batch_handler = self.get_handler()
         # TODO: deprecate / remove this (?)
         self.handler = self.batch_handler
 
     @classmethod
     def get_handler_factory(cls, rattail_config):
         """
@@ -163,15 +158,15 @@
     def input_file_template_config_prefix(self):
         return '{}.input_file_template'.format(self.batch_handler.batch_key)
 
     def download_path(self, batch, filename):
         return self.rattail_config.batch_filepath(batch.batch_key, batch.uuid, filename)
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(BatchMasterView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
         batch = kwargs['instance']
         kwargs['batch'] = batch
         kwargs['handler'] = self.handler
 
         if self.has_worksheet_file and self.allow_worksheet(batch) and self.has_perm('worksheet'):
             kwargs['upload_worksheet_form'] = self.make_upload_worksheet_form(batch)
 
@@ -191,27 +186,27 @@
 
         factory = self.get_grid_factory()
         g = factory('batch_row_status_breakdown', [],
                     columns=['title', 'count'])
         g.set_click_handler('title', "autoFilterStatus(props.row)")
         kwargs['status_breakdown_data'] = breakdown
         kwargs['status_breakdown_grid'] = HTML.literal(
-            g.render_buefy_table_element(data_prop='statusBreakdownData',
-                                         empty_labels=True))
+            g.render_table_element(data_prop='statusBreakdownData',
+                                   empty_labels=True))
 
         return kwargs
 
     def make_upload_worksheet_form(self, batch):
         action_url = self.get_action_url('upload_worksheet', batch)
         form = forms.Form(schema=UploadWorksheet(),
                           request=self.request,
                           action_url=action_url,
                           component='upload-worksheet-form')
         form.set_type('worksheet_file', 'file')
-        # TODO: must set these to avoid some default Buefy code
+        # TODO: must set these to avoid some default code
         form.auto_disable = False
         form.auto_disable_save = False
         return form
 
     def download_worksheet(self):
         batch = self.get_instance()
         path = self.handler.write_worksheet(batch)
@@ -284,15 +279,16 @@
                 breakdown[row.status_code]['count'] += 1
         return list(breakdown.values())
 
     def allow_worksheet(self, batch):
         return not batch.executed and not batch.complete
 
     def configure_grid(self, g):
-        super(BatchMasterView, self).configure_grid(g)
+        super().configure_grid(g)
+        model = self.model
 
         # created_by
         CreatedBy = orm.aliased(model.User)
         g.set_joiner('created_by', lambda q: q.join(CreatedBy,
                                                     CreatedBy.uuid == self.model_class.created_by_uuid))
         g.set_sorter('created_by', CreatedBy.username)
         g.set_filter('created_by', CreatedBy.username)
@@ -333,15 +329,15 @@
 
     def get_instance_title(self, batch):
         if batch.description:
             return "{} {}".format(batch.id_str, batch.description)
         return batch.id_str
 
     def configure_form(self, f):
-        super(BatchMasterView, self).configure_form(f)
+        super().configure_form(f)
 
         # id
         f.set_readonly('id')
         f.set_renderer('id', self.render_id_str)
         f.set_label('id', "Batch ID")
 
         # params
@@ -432,17 +428,17 @@
 
         url = self.get_action_url('toggle_complete', batch)
         kwargs = {'@submit': 'togglingBatchComplete = true'}
         begin_form = tags.form(url, **kwargs)
 
         label = HTML.literal(
             '{{{{ togglingBatchComplete ? "Working, please wait..." : "{}" }}}}'.format(label))
-        submit = self.make_buefy_button(label, is_primary=True,
-                                        native_type='submit',
-                                        **{':disabled': 'togglingBatchComplete'})
+        submit = self.make_button(label, is_primary=True,
+                                  native_type='submit',
+                                  **{':disabled': 'togglingBatchComplete'})
 
         form = [
             begin_form,
             csrf_token(self.request),
             tags.hidden('complete', value=value),
             submit,
             tags.end_form(),
@@ -599,15 +595,15 @@
         if batch.executed:
             return False
         if batch.complete:
             return False
         return True
 
     def configure_row_grid(self, g):
-        super(BatchMasterView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
 
         g.set_sort_defaults('sequence')
         g.set_link('sequence')
         g.set_label('sequence', "Seq.")
         if 'sequence' in g.filters:
             g.filters['sequence'].label = "Sequence"
 
@@ -640,28 +636,28 @@
         """
         Only allow creating a new row if the batch hasn't yet been executed.
         """
         batch = self.get_instance()
         if batch.executed:
             self.request.session.flash("You cannot add new rows to a batch which has been executed")
             return self.redirect(self.get_action_url('view', batch))
-        return super(BatchMasterView, self).create_row()
+        return super().create_row()
 
     def save_create_row_form(self, form):
         batch = self.get_instance()
         row = self.objectify(form, self.form_deserialized)
         self.handler.add_row(batch, row)
         self.Session.flush()
         return row
 
     def after_create_row(self, row):
         self.handler.refresh_row(row)
 
     def configure_row_form(self, f):
-        super(BatchMasterView, self).configure_row_form(f)
+        super().configure_row_form(f)
 
         # sequence
         f.set_readonly('sequence')
 
         # upc (default rendering, just in case there is such a field
         # on our row model)
         f.set_renderer('upc', self.render_upc_pretty)
@@ -677,17 +673,17 @@
         f.set_readonly('status_text')
 
     def make_default_row_grid_tools(self, batch):
         if self.rows_creatable and not batch.executed and not batch.complete:
             permission_prefix = self.get_permission_prefix()
             if self.request.has_perm('{}.create_row'.format(permission_prefix)):
                 url = self.get_action_url('create_row', batch)
-                return self.make_buefy_button("New Row", url=url,
-                                              is_primary=True,
-                                              icon_left='plus')
+                return self.make_button("New Row", url=url,
+                                        is_primary=True,
+                                        icon_left='plus')
 
     def make_batch_row_grid_tools(self, batch):
         pass
 
     def make_row_grid_kwargs(self, **kwargs):
         """
         Whether or not rows may be edited or deleted will depend partially on
@@ -715,15 +711,15 @@
                 # delete action
                 if self.rows_deletable and self.has_perm('delete_row'):
                     actions.append(self.make_action('delete', icon='trash', url=self.row_delete_action_url))
                     kwargs.setdefault('delete_speedbump', self.rows_deletable_speedbump)
 
             kwargs['main_actions'] = actions
 
-        return super(BatchMasterView, self).make_row_grid_kwargs(**kwargs)
+        return super().make_row_grid_kwargs(**kwargs)
 
     def make_row_grid_tools(self, batch):
         return (self.make_default_row_grid_tools(batch) or '') + (self.make_batch_row_grid_tools(batch) or '')
 
     def redirect_after_edit(self, batch):
         """
         If refresh flag is set, do that; otherwise go (back) to view/edit page.
@@ -848,16 +844,19 @@
                             defaults[field.name] = self.request.session[key]
 
                     # make sure field label is preserved
                     if field.title:
                         labels = kwargs.setdefault('labels', {})
                         labels[field.name] = field.title
 
-                    # auto-convert select widgets for buefy theme
+                    # auto-convert select widgets for theme
                     if isinstance(field.widget, forms.widgets.PlainSelectWidget):
+                        warnings.warn("PlainSelectWidget is deprecated; "
+                                      "please use deform.widget.SelectWidget instead",
+                                      DeprecationWarning)
                         field.widget = dfwidget.SelectWidget(values=field.widget.values)
 
         if not schema:
             schema = colander.Schema()
 
         kwargs['component'] = 'execute-form'
         form = forms.Form(schema=schema, request=self.request, defaults=defaults, **kwargs)
@@ -1018,15 +1017,16 @@
         })
         data = data.encode('utf_8')
         cxn.send(data)
         cxn.send(suffix)
         cxn.close()
 
     def catchup_versions(self, port, batch_uuid, username, *models):
-        with short_session() as s:
+        app = self.get_rattail_app()
+        with app.short_session() as s:
             batch = s.get(self.model_class, batch_uuid)
             batch_id = batch.id_str
             description = str(batch)
 
         self.launch_subprocess(
             port=port, username=username,
             command='rattail',
@@ -1044,16 +1044,18 @@
         batch = self.get_instance()
         return self.handler_action(batch, 'populate')
 
     def populate_thread(self, batch_uuid, user_uuid, progress, **kwargs):
         """
         Thread target for populating batch data with progress indicator.
         """
+        app = self.get_rattail_app()
+        model = self.model
         # mustn't use tailbone web session here
-        session = RattailSession()
+        session = app.make_session()
         batch = session.get(self.model_class, batch_uuid)
         user = session.get(model.User, user_uuid)
         try:
             self.handler.do_populate(batch, user, progress=progress)
             session.flush()
         except Exception as error:
             session.rollback()
@@ -1103,15 +1105,17 @@
     def refresh_thread(self, batch_uuid, user_uuid, progress, **kwargs):
         """
         Thread target for refreshing batch data with progress indicator.
         """
         # Refresh data for the batch, with progress.  Note that we must use the
         # rattail session here; can't use tailbone because it has web request
         # transaction binding etc.
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         batch = session.get(self.model_class, batch_uuid)
         cognizer = session.get(model.User, user_uuid) if user_uuid else None
         try:
             self.refresh_data(session, batch, cognizer, progress=progress)
             session.flush()
         except Exception as error:
             session.rollback()
@@ -1156,15 +1160,17 @@
             'cancel_msg': "Batch execution was canceled",
         })
 
     def refresh_results_thread(self, batches, user_uuid, progress=None):
         """
         Thread target for refreshing multiple batches with progress indicator.
         """
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         batches = batches.with_session(session).all()
         user = session.get(model.User, user_uuid)
         try:
             self.handler.refresh_many(batches, user=user, progress=progress)
 
         except Exception as error:
             session.rollback()
@@ -1253,15 +1259,15 @@
     def delete_row_object(self, row):
         """
         Perform the actual deletion of given row object.
         """
         self.handler.do_remove_row(row)
 
     def delete_row_objects(self, rows):
-        deleted = super(BatchMasterView, self).delete_row_objects(rows)
+        deleted = super().delete_row_objects(rows)
         batch = self.get_instance()
 
         # decrement rowcount for batch
         if batch.rowcount is not None:
             batch.rowcount -= deleted
 
         # refresh batch status
@@ -1296,15 +1302,17 @@
     def execute_thread(self, key, user_uuid, progress, **kwargs):
         """
         Thread target for executing a batch with progress indicator.
         """
         # Execute the batch, with progress.  Note that we must use the rattail
         # session here; can't use tailbone because it has web request
         # transaction binding etc.
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         batch = self.get_instance_for_key(key, session)
         user = session.get(model.User, user_uuid)
         try:
             result = self.handler.do_execute(batch, user=user, progress=progress, **kwargs)
 
         # If anything goes wrong, rollback and log the error etc.
         except Exception as error:
@@ -1371,15 +1379,17 @@
         self.request.session.flash("Invalid request: {}".format(form.make_deform_form().error), 'error')
         return self.redirect(self.get_index_url())
 
     def execute_results_thread(self, batches, user_uuid, progress=None, **kwargs):
         """
         Thread target for executing multiple batches with progress indicator.
         """
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         batches = batches.with_session(session).all()
         user = session.get(model.User, user_uuid)
         try:
             result = self.handler.execute_many(batches, user=user, progress=progress, **kwargs)
 
         # If anything goes wrong, rollback and log the error etc.
         except Exception as error:
@@ -1411,15 +1421,15 @@
                 progress.session['success_url'] = success_url
                 progress.session.save()
 
     def get_execute_results_success_url(self, result, **kwargs):
         return self.get_index_url()
 
     def get_row_csv_fields(self):
-        fields = super(BatchMasterView, self).get_row_csv_fields()
+        fields = super().get_row_csv_fields()
         fields = [field for field in fields
                   if field not in ('uuid', 'batch_uuid', 'removed')]
         return fields
 
     def get_row_results_csv_filename(self, batch):
         return '{}.{}.csv'.format(self.get_route_prefix(), batch.id_str)
 
@@ -1534,15 +1544,15 @@
         uploads = self.rattail_config.get('tailbone', 'batch.uploads',
                                           default=uploads)
         if not os.path.exists(uploads):
             os.makedirs(uploads)
         return uploads
 
     def configure_form(self, f):
-        super(FileBatchMasterView, self).configure_form(f)
+        super().configure_form(f)
         batch = f.model_instance
 
         # filename
         if self.creating:
             # TODO: what's up with this re-insertion again..?
             # if 'filename' not in f.fields:
             #     f.fields.insert(0, 'filename')
```

### Comparing `Tailbone-0.9.90/tailbone/views/batch/delproduct.py` & `tailbone-0.9.91/tailbone/views/batch/delproduct.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/handheld.py` & `tailbone-0.9.91/tailbone/views/batch/handheld.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -22,50 +22,50 @@
 ################################################################################
 """
 Views for handheld batches
 """
 
 from collections import OrderedDict
 
-from rattail.db import model
+from rattail.db.model import HandheldBatch, HandheldBatchRow
 
 import colander
+from deform import widget as dfwidget
 from webhelpers2.html import tags
 
-from tailbone import forms
 from tailbone.views.batch import FileBatchMasterView
 
 
 ACTION_OPTIONS = OrderedDict([
     ('make_label_batch', "Make a new Label Batch"),
     ('make_inventory_batch', "Make a new Inventory Batch"),
 ])
 
 
 class ExecutionOptions(colander.Schema):
 
     action = colander.SchemaNode(
         colander.String(),
         validator=colander.OneOf(ACTION_OPTIONS),
-        widget=forms.widgets.PlainSelectWidget(values=ACTION_OPTIONS.items()))
+        widget=dfwidget.SelectWidget(values=ACTION_OPTIONS.items()))
 
 
 class HandheldBatchView(FileBatchMasterView):
     """
     Master view for handheld batches.
     """
-    model_class = model.HandheldBatch
+    model_class = HandheldBatch
     default_handler_spec = 'rattail.batch.handheld:HandheldBatchHandler'
     model_title_plural = "Handheld Batches"
     route_prefix = 'batch.handheld'
     url_prefix = '/batch/handheld'
     execution_options_schema = ExecutionOptions
     editable = False
 
-    model_row_class = model.HandheldBatchRow
+    model_row_class = HandheldBatchRow
     rows_creatable = False
     rows_editable = True
 
     grid_columns = [
         'id',
         'device_type',
         'device_name',
@@ -112,25 +112,25 @@
         'size',
         'status_code',
         'cases',
         'units',
     ]
 
     def configure_grid(self, g):
-        super(HandheldBatchView, self).configure_grid(g)
+        super().configure_grid(g)
         device_types = OrderedDict(sorted(self.enum.HANDHELD_DEVICE_TYPE.items(),
                                           key=lambda item: item[1]))
         g.set_enum('device_type', device_types)
 
     def grid_extra_class(self, batch, i):
         if batch.status_code is not None and batch.status_code != batch.STATUS_OK:
             return 'notice'
 
     def configure_form(self, f):
-        super(HandheldBatchView, self).configure_form(f)
+        super().configure_form(f)
         batch = f.model_instance
 
         # device_type
         device_types = OrderedDict(sorted(self.enum.HANDHELD_DEVICE_TYPE.items(),
                                           key=lambda item: item[1]))
         f.set_enum('device_type', device_types)
         f.widgets['device_type'].values.insert(0, ('', "(none)"))
@@ -152,31 +152,31 @@
         if not batch:
             return ""
         text = batch.id_str
         url = self.request.route_url('batch.inventory.view', uuid=batch.uuid)
         return tags.link_to(text, url)
 
     def get_batch_kwargs(self, batch):
-        kwargs = super(HandheldBatchView, self).get_batch_kwargs(batch)
+        kwargs = super().get_batch_kwargs(batch)
         kwargs['device_type'] = batch.device_type
         kwargs['device_name'] = batch.device_name
         return kwargs
 
     def configure_row_grid(self, g):
-        super(HandheldBatchView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
         g.set_type('cases', 'quantity')
         g.set_type('units', 'quantity')
         g.set_label('brand_name', "Brand")
 
     def row_grid_extra_class(self, row, i):
         if row.status_code == row.STATUS_PRODUCT_NOT_FOUND:
             return 'warning'
 
     def configure_row_form(self, f):
-        super(HandheldBatchView, self).configure_row_form(f)
+        super().configure_row_form(f)
 
         # readonly fields
         f.set_readonly('upc')
         f.set_readonly('brand_name')
         f.set_readonly('description')
         f.set_readonly('size')
 
@@ -184,15 +184,15 @@
         f.set_renderer('upc', self.render_upc)
 
     def get_execute_success_url(self, batch, result, **kwargs):
         if kwargs['action'] == 'make_inventory_batch':
             return self.request.route_url('batch.inventory.view', uuid=result.uuid)
         elif kwargs['action'] == 'make_label_batch':
             return self.request.route_url('labels.batch.view', uuid=result.uuid)
-        return super(HandheldBatchView, self).get_execute_success_url(batch)
+        return super().get_execute_success_url(batch)
 
     def get_execute_results_success_url(self, result, **kwargs):
         if result is True:
             # no batches were actually executed
             return self.get_index_url()
         batch = result
         return self.get_execute_success_url(batch, result, **kwargs)
```

### Comparing `Tailbone-0.9.90/tailbone/views/batch/importer.py` & `tailbone-0.9.91/tailbone/views/batch/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,15 @@
         def make_filter(field, **kwargs):
             column = getattr(self.current_row_table.c, field)
             g.set_filter(field, column, **kwargs)
 
         make_filter('object_key')
         make_filter('object_str')
 
-        # for some reason we have to do this differently for Buefy?
-        kwargs = {}
-        make_filter('status_code', label="Status", **kwargs)
+        make_filter('status_code', label="Status")
         g.filters['status_code'].set_choices(self.enum.IMPORTER_BATCH_ROW_STATUS)
 
         def make_sorter(field):
             column = getattr(self.current_row_table.c, field)
             g.sorters[field] = lambda q, d: q.order_by(getattr(column, d)())
 
         make_sorter('sequence')
```

### Comparing `Tailbone-0.9.90/tailbone/views/batch/inventory.py` & `tailbone-0.9.91/tailbone/views/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/labels.py` & `tailbone-0.9.91/tailbone/views/batch/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/newproduct.py` & `tailbone-0.9.91/tailbone/views/batch/newproduct.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/pos.py` & `tailbone-0.9.91/tailbone/views/batch/pos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -202,15 +202,15 @@
                 'description',
                 'rate',
                 'total',
             ],
         )
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='taxesData'))
+            g.render_table_element(data_prop='taxesData'))
 
     def template_kwargs_view(self, **kwargs):
         kwargs = super().template_kwargs_view(**kwargs)
         app = self.get_rattail_app()
         batch = kwargs['instance']
 
         taxes = []
```

### Comparing `Tailbone-0.9.90/tailbone/views/batch/pricing.py` & `tailbone-0.9.91/tailbone/views/batch/pricing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/product.py` & `tailbone-0.9.91/tailbone/views/batch/product.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -22,43 +22,43 @@
 ################################################################################
 """
 Views for generic product batches
 """
 
 from collections import OrderedDict
 
-from rattail.db import model
+from rattail.db.model import ProductBatch, ProductBatchRow
 
 import colander
+from deform import widget as dfwidget
 from webhelpers2.html import HTML
 
-from tailbone import forms
 from tailbone.views.batch import BatchMasterView
 
 
 ACTION_OPTIONS = OrderedDict([
     ('make_label_batch', "Make a new Label Batch"),
     ('make_pricing_batch', "Make a new Pricing Batch"),
 ])
 
 
 class ExecutionOptions(colander.Schema):
 
     action = colander.SchemaNode(
         colander.String(),
         validator=colander.OneOf(ACTION_OPTIONS),
-        widget=forms.widgets.PlainSelectWidget(values=ACTION_OPTIONS.items()))
+        widget=dfwidget.SelectWidget(values=ACTION_OPTIONS.items()))
 
 
 class ProductBatchView(BatchMasterView):
     """
     Master view for product batches.
     """
-    model_class = model.ProductBatch
-    model_row_class = model.ProductBatchRow
+    model_class = ProductBatch
+    model_row_class = ProductBatchRow
     default_handler_spec = 'rattail.batch.product:ProductBatchHandler'
     route_prefix = 'batch.product'
     url_prefix = '/batches/product'
     template_prefix = '/batch/product'
     downloadable = True
     cloneable = True
     bulk_deletable = True
@@ -125,25 +125,26 @@
         'current_price_ends',
         'suggested_price',
         'status_code',
         'status_text',
     ]
 
     def configure_form(self, f):
-        super(ProductBatchView, self).configure_form(f)
+        super().configure_form(f)
 
         # input_filename
         if self.creating:
             f.set_type('input_filename', 'file')
         else:
             f.set_readonly('input_filename')
             f.set_renderer('input_filename', self.render_downloadable_file)
 
     def configure_row_grid(self, g):
-        super(ProductBatchView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
+        model = self.model
 
         g.set_joiner('vendor', lambda q: q.outerjoin(model.Vendor))
         g.set_sorter('vendor', model.Vendor.name)
 
         g.set_joiner('department', lambda q: q.outerjoin(model.Department))
         g.set_sorter('department', model.Department.name)
 
@@ -161,15 +162,15 @@
 
     def row_grid_extra_class(self, row, i):
         if row.status_code in (row.STATUS_MISSING_KEY,
                                row.STATUS_PRODUCT_NOT_FOUND):
             return 'warning'
 
     def configure_row_form(self, f):
-        super(ProductBatchView, self).configure_row_form(f)
+        super().configure_row_form(f)
 
         f.set_type('upc', 'gpc')
 
         f.set_renderer('product', self.render_product)
         f.set_renderer('vendor', self.render_vendor)
         f.set_renderer('department', self.render_department)
         f.set_renderer('subdepartment', self.render_subdepartment)
@@ -200,18 +201,18 @@
         return text
 
     def get_execute_success_url(self, batch, result, **kwargs):
         if kwargs['action'] == 'make_label_batch':
             return self.request.route_url('labels.batch.view', uuid=result.uuid)
         elif kwargs['action'] == 'make_pricing_batch':
             return self.request.route_url('batch.pricing.view', uuid=result.uuid)
-        return super(ProductBatchView, self).get_execute_success_url(batch)
+        return super().get_execute_success_url(batch)
 
     def get_row_csv_fields(self):
-        fields = super(ProductBatchView, self).get_row_csv_fields()
+        fields = super().get_row_csv_fields()
 
         if 'vendor_uuid' in fields:
             i = fields.index('vendor_uuid')
             fields.insert(i + 1, 'vendor_id')
             fields.insert(i + 2, 'vendor_abbreviation')
             fields.insert(i + 3, 'vendor_name')
         else:
@@ -269,19 +270,19 @@
         report = row.reportcode
         if 'report_code' in fields:
             data['report_code'] = (report.code or '') if report else ''
         if 'report_name' in fields:
             data['report_name'] = (report.name or '') if report else ''
 
     def get_row_csv_row(self, row, fields):
-        csvrow = super(ProductBatchView, self).get_row_csv_row(row, fields)
+        csvrow = super().get_row_csv_row(row, fields)
         self.supplement_row_data(row, fields, csvrow)
         return csvrow
 
     def get_row_xlsx_row(self, row, fields):
-        xlrow = super(ProductBatchView, self).get_row_xlsx_row(row, fields)
+        xlrow = super().get_row_xlsx_row(row, fields)
         self.supplement_row_data(row, fields, xlrow)
         return xlrow
 
 
 def includeme(config):
     ProductBatchView.defaults(config)
```

### Comparing `Tailbone-0.9.90/tailbone/views/batch/vendorcatalog.py` & `tailbone-0.9.91/tailbone/views/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/batch/vendorinvoice.py` & `tailbone-0.9.91/tailbone/views/batch/vendorinvoice.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/bouncer.py` & `tailbone-0.9.91/tailbone/views/bouncer.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/brands.py` & `tailbone-0.9.91/tailbone/views/brands.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/categories.py` & `tailbone-0.9.91/tailbone/views/categories.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/common.py` & `tailbone-0.9.91/tailbone/views/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/core.py` & `tailbone-0.9.91/tailbone/views/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/customergroups.py` & `tailbone-0.9.91/tailbone/views/customergroups.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/customers.py` & `tailbone-0.9.91/tailbone/views/customers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -33,22 +33,22 @@
 from pyramid.httpexceptions import HTTPNotFound
 from webhelpers2.html import HTML, tags
 
 from tailbone import grids
 from tailbone.db import Session
 from tailbone.views import MasterView
 
-from rattail.db import model
+from rattail.db.model import Customer, CustomerShopper, PendingCustomer
 
 
 class CustomerView(MasterView):
     """
     Master view for the Customer class.
     """
-    model_class = model.Customer
+    model_class = Customer
     is_contact = True
     has_versions = True
     results_downloadable = True
     people_detachable = True
     touchable = True
     supports_autocomplete = True
     configurable = True
@@ -247,14 +247,15 @@
             instance = super().get_instance()
         except HTTPNotFound:
             pass
         else:
             if instance:
                 return instance
 
+        model = self.model
         key = self.request.matchdict['uuid']
 
         # search by Customer.id
         instance = self.Session.query(model.Customer)\
                                .filter(model.Customer.id == key)\
                                .first()
         if instance:
@@ -266,15 +267,15 @@
             return instance.customer
 
         # search by CustomerGroupAssignment.uuid
         instance = self.Session.get(model.CustomerGroupAssignment, key)
         if instance:
             return instance.customer
 
-        raise HTTPNotFound
+        raise self.notfound()
 
     def configure_form(self, f):
         super().configure_form(f)
         customer = f.model_instance
         permission_prefix = self.get_permission_prefix()
 
         # account_holder
@@ -337,15 +338,15 @@
                 f.remove('shoppers')
         else:
             f.remove('shoppers')
 
         # people
         if self.should_expose_people():
             if self.viewing:
-                f.set_renderer('people', self.render_people_buefy)
+                f.set_renderer('people', self.render_people)
             else:
                 f.remove('people')
         else:
             f.remove('people')
 
         # groups
         if self.creating:
@@ -432,14 +433,15 @@
                 people.setdefault(person.uuid, person)
 
             kwargs['show_profiles_people'] = list(people.values())
 
         return kwargs
 
     def unique_id(self, node, value):
+        model = self.model
         query = self.Session.query(model.Customer)\
                             .filter(model.Customer.id == value)
         if self.editing:
             customer = self.get_instance()
             query = query.filter(model.Customer.uuid != customer.uuid)
         if query.count():
             raise colander.Invalid(node, "Customer ID must be unique")
@@ -459,28 +461,14 @@
         if not person:
             return ""
 
         text = str(person)
         url = self.request.route_url('people.view', uuid=person.uuid)
         return tags.link_to(text, url)
 
-    # TODO: remove if no longer used
-    def render_people(self, customer, field):
-        people = customer.people
-        if not people:
-            return ""
-
-        items = []
-        for person in people:
-            text = str(person)
-            url = self.request.route_url('people.view', uuid=person.uuid)
-            link = tags.link_to(text, url)
-            items.append(HTML.tag('li', c=[link]))
-        return HTML.tag('ul', c=items)
-
     def render_shoppers(self, customer, field):
         route_prefix = self.get_route_prefix()
         permission_prefix = self.get_permission_prefix()
 
         factory = self.get_grid_factory()
         g = factory(
             key='{}.people'.format(route_prefix),
@@ -500,17 +488,17 @@
                      'phone': True,
                      'email': True,
                      'active': True},
             labels={'shopper_number': "Shopper #"},
         )
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='shoppers'))
+            g.render_table_element(data_prop='shoppers'))
 
-    def render_people_buefy(self, customer, field):
+    def render_people(self, customer, field):
         route_prefix = self.get_route_prefix()
         permission_prefix = self.get_permission_prefix()
 
         factory = self.get_grid_factory()
         g = factory(
             key='{}.people'.format(route_prefix),
             data=[],
@@ -529,15 +517,15 @@
             g.main_actions.append(self.make_action('edit', icon='edit'))
         if self.people_detachable and self.has_perm('detach_person'):
             g.main_actions.append(self.make_action('detach', icon='minus-circle',
                                                    link_class='has-text-warning',
                                                    click_handler="$emit('detach-person', props.row._action_url_detach)"))
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='peopleData'))
+            g.render_table_element(data_prop='peopleData'))
 
     def render_groups(self, customer, field):
         groups = customer.groups
         if not groups:
             return ""
         items = []
         for group in groups:
@@ -555,25 +543,27 @@
             text = str(member)
             url = self.request.route_url('members.view', uuid=member.uuid)
             items.append(HTML.tag('li', tags.link_to(text, url)))
         return HTML.tag('ul', HTML.literal('').join(items))
 
     def get_version_child_classes(self):
         classes = super().get_version_child_classes()
+        model = self.model
         classes.extend([
             (model.CustomerGroupAssignment, 'customer_uuid'),
             (model.CustomerPhoneNumber, 'parent_uuid'),
             (model.CustomerEmailAddress, 'parent_uuid'),
             (model.CustomerMailingAddress, 'parent_uuid'),
             (model.CustomerPerson, 'customer_uuid'),
             (model.CustomerNote, 'parent_uuid'),
         ])
         return classes
 
     def detach_person(self):
+        model = self.model
         customer = self.get_instance()
         person = self.Session.get(model.Person, self.request.matchdict['person_uuid'])
         if not person:
             return self.notfound()
 
         if person in customer.people:
             customer.people.remove(person)
@@ -661,31 +651,29 @@
         model_title = cls.get_model_title()
 
         # detach person
         if cls.people_detachable:
             config.add_tailbone_permission(permission_prefix,
                                            '{}.detach_person'.format(permission_prefix),
                                            "Detach a Person from a {}".format(model_title))
-            # TODO: this should require POST, but we'll add that once
-            # we can assume a Buefy theme is present, to avoid having
-            # to implement the logic in old jquery...
+            # TODO: this should require POST!
             config.add_route('{}.detach_person'.format(route_prefix),
                              '{}/detach-person/{{person_uuid}}'.format(instance_url_prefix),
                              # request_method='POST',
             )
             config.add_view(cls, attr='detach_person',
                             route_name='{}.detach_person'.format(route_prefix),
                             permission='{}.detach_person'.format(permission_prefix))
 
 
 class CustomerShopperView(MasterView):
     """
     Master view for the CustomerShopper class.
     """
-    model_class = model.CustomerShopper
+    model_class = CustomerShopper
     route_prefix = 'customer_shoppers'
     url_prefix = '/customer-shoppers'
 
     grid_columns = [
         'customer_key',
         'customer',
         'shopper_number',
@@ -758,15 +746,15 @@
         f.set_renderer('person', self.render_person)
 
 
 class PendingCustomerView(MasterView):
     """
     Master view for the Pending Customer class.
     """
-    model_class = model.PendingCustomer
+    model_class = PendingCustomer
     route_prefix = 'pending_customers'
     url_prefix = '/customers/pending'
 
     labels = {
         'id': "ID",
         'status_code': "Status",
     }
@@ -887,23 +875,25 @@
 #     if query.count():
 #         raise fa.ValidationError("Customer ID must be unique")
 
 
 # TODO: this only works when creating, need to add edit support?
 # TODO: can this just go away? since we have unique_id() view method above
 def unique_id(node, value):
-    customers = Session.query(model.Customer).filter(model.Customer.id == value)
+    customers = Session.query(Customer).filter(Customer.id == value)
     if customers.count():
         raise colander.Invalid(node, "Customer ID must be unique")
 
 
 def customer_info(request):
     """
     View which returns simple dictionary of info for a particular customer.
     """
+    app = request.rattail_config.get_app()
+    model = app.model
     uuid = request.params.get('uuid')
     customer = Session.get(model.Customer, uuid) if uuid else None
     if not customer:
         return {}
     return {
         'uuid':                 customer.uuid,
         'name':                 customer.name,
```

### Comparing `Tailbone-0.9.90/tailbone/views/custorders/__init__.py` & `tailbone-0.9.91/tailbone/views/custorders/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/custorders/batch.py` & `tailbone-0.9.91/tailbone/views/custorders/batch.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/custorders/creating.py` & `tailbone-0.9.91/tailbone/views/custorders/creating.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/custorders/items.py` & `tailbone-0.9.91/tailbone/views/custorders/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -397,15 +397,15 @@
                 'occurred': "When",
                 'type_code': "What",
                 'user': "Who",
             },
         )
 
         table = HTML.literal(
-            g.render_buefy_table_element(data_prop='eventsData'))
+            g.render_table_element(data_prop='eventsData'))
         elements = [table]
 
         if self.has_perm('add_note'):
             button = HTML.tag('b-button', type='is-primary', c="Add Note",
                               class_='is-pulled-right',
                               icon_pack='fas', icon_left='plus',
                               **{'@click': "$emit('add-note')"})
```

### Comparing `Tailbone-0.9.90/tailbone/views/custorders/orders.py` & `tailbone-0.9.91/tailbone/views/custorders/orders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/datasync.py` & `tailbone-0.9.91/tailbone/views/datasync.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/departments.py` & `tailbone-0.9.91/tailbone/views/departments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -107,17 +107,21 @@
         else:
             f.set_renderer('employees', self.render_employees)
 
         f.set_type('product', 'boolean')
         f.set_type('personnel', 'boolean')
 
         # tax
-        f.set_renderer('tax', self.render_tax)
-        # TODO: make this editable
-        f.set_readonly('tax')
+        if self.creating:
+            # TODO: make this editable instead
+            f.remove('tax')
+        else:
+            f.set_renderer('tax', self.render_tax)
+            # TODO: make this editable
+            f.set_readonly('tax')
 
         # default_custorder_discount
         f.set_type('default_custorder_discount', 'percent')
 
     def render_employees(self, department, field):
         route_prefix = self.get_route_prefix()
         permission_prefix = self.get_permission_prefix()
@@ -136,15 +140,15 @@
 
         if self.request.has_perm('employees.view'):
             g.main_actions.append(self.make_action('view', icon='eye'))
         if self.request.has_perm('employees.edit'):
             g.main_actions.append(self.make_action('edit', icon='edit'))
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='employeesData'))
+            g.render_table_element(data_prop='employeesData'))
 
     def template_kwargs_view(self, **kwargs):
         kwargs = super().template_kwargs_view(**kwargs)
         department = kwargs['instance']
         department_employees = sorted(department.employees, key=str)
 
         employees = []
```

### Comparing `Tailbone-0.9.90/tailbone/views/depositlinks.py` & `tailbone-0.9.91/tailbone/views/depositlinks.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/email.py` & `tailbone-0.9.91/tailbone/views/email.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/employees.py` & `tailbone-0.9.91/tailbone/views/employees.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/essentials.py` & `tailbone-0.9.91/tailbone/views/essentials.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/exports.py` & `tailbone-0.9.91/tailbone/views/exports.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/families.py` & `tailbone-0.9.91/tailbone/views/families.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/features.py` & `tailbone-0.9.91/tailbone/views/features.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/filemon.py` & `tailbone-0.9.91/tailbone/views/filemon.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/handheld.py` & `tailbone-0.9.91/tailbone/views/handheld.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/ifps.py` & `tailbone-0.9.91/tailbone/views/ifps.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/importing.py` & `tailbone-0.9.91/tailbone/views/importing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/inventory.py` & `tailbone-0.9.91/tailbone/views/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/labels/__init__.py` & `tailbone-0.9.91/tailbone/views/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/labels/batch.py` & `tailbone-0.9.91/tailbone/views/labels/batch.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/labels/profiles.py` & `tailbone-0.9.91/tailbone/views/labels/profiles.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/luigi.py` & `tailbone-0.9.91/tailbone/views/luigi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/master.py` & `tailbone-0.9.91/tailbone/views/master.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -26,40 +26,35 @@
 
 import io
 import os
 import csv
 import datetime
 import getpass
 import shutil
-import tempfile
 import logging
 from collections import OrderedDict
 
 import json
 import sqlalchemy as sa
 from sqlalchemy import orm
 import sqlalchemy_continuum as continuum
 from sqlalchemy_utils.functions import get_primary_keys, get_columns
 
-from rattail.db import model, Session as RattailSession
 from rattail.db.continuum import model_transaction_query
-from rattail.util import prettify, simple_error, get_class_hierarchy
-from rattail.time import localtime
+from rattail.util import simple_error, get_class_hierarchy
 from rattail.threads import Thread
 from rattail.csvutil import UnicodeDictWriter
-from rattail.files import temp_path
 from rattail.excel import ExcelWriter
 from rattail.gpc import GPC
 
 import colander
 import deform
 from deform import widget as dfwidget
 from pyramid import httpexceptions
 from pyramid.renderers import get_renderer, render_to_response, render
-from pyramid.response import FileResponse
 from webhelpers2.html import HTML, tags
 from webob.compat import cgi_FieldStorage
 
 from tailbone import forms, grids, diffs
 from tailbone.views import View
 from tailbone.db import Session
 from tailbone.config import global_help_url
@@ -217,15 +212,16 @@
         "isolated" from the rest of the web app in a sense.
 
         So whereas ``self.Session`` by default will return a reference to
         ``tailbone.db.Session``, which is a "scoped" session wrapper specific
         to the current thread (one per request), this method should instead
         return e.g. a new independent ``rattail.db.Session`` instance.
         """
-        return RattailSession()
+        app = self.get_rattail_app()
+        return app.make_session()
 
     @classmethod
     def get_grid_factory(cls):
         """
         Returns the grid factory or class which is to be used when creating new
         grid instances.
         """
@@ -320,14 +316,21 @@
         """
         View to list/filter/sort the model data.
 
         If this view receives a non-empty 'partial' parameter in the query
         string, then the view will return the rendered grid only.  Otherwise
         returns the full page.
         """
+        # nb. normally this "save defaults" flag is checked within make_grid()
+        # but it returns JSON data so we can't just do a redirect when there
+        # is no user; must return JSON error message instead
+        if (self.request.GET.get('save-current-filters-as-defaults') == 'true'
+            and not self.request.user):
+            return self.json_response({'error': "User is not currently logged in"})
+
         self.listing = True
         grid = self.make_grid()
 
         # If user just refreshed the page with a reset instruction, issue a
         # redirect in order to clear out the query string.
         if self.request.GET.get('reset-to-default-filters') == 'true':
             kw = {'_query': None}
@@ -338,15 +341,15 @@
 
         # Stash some grid stats, for possible use when generating URLs.
         if grid.pageable and hasattr(grid, 'pager'):
             self.first_visible_grid_index = grid.pager.first_item
 
         # return grid data only, if partial page was requested
         if self.request.params.get('partial'):
-            return self.json_response(grid.get_buefy_data())
+            return self.json_response(grid.get_table_data())
 
         context = {
             'grid': grid,
         }
 
         if self.results_downloadable and self.has_perm('download_results'):
             route_prefix = self.get_route_prefix()
@@ -709,18 +712,19 @@
             self.before_create_flush(obj, form)
         self.Session.add(obj)
         self.Session.flush()
         self.process_uploads(obj, form, uploads)
         return obj
 
     def normalize_uploads(self, form, skip=None):
+        app = self.get_rattail_app()
         uploads = {}
 
         def normalize(filedict):
-            tempdir = tempfile.mkdtemp()
+            tempdir = app.make_temp_dir()
             filepath = os.path.join(tempdir, filedict['filename'])
             tmpinfo = form.deform_form[node.name].widget.tmpstore.get(filedict['uid'])
             tmpdata = tmpinfo['fp'].read()
             with open(filepath, 'wb') as f:
                 f.write(tmpdata)
             return {'tempdir': tempdir,
                     'temp_path': filepath}
@@ -1104,15 +1108,16 @@
         return self.render_progress(progress, kwargs)
 
     def populate_thread(self, uuid, progress): # TODO: uuid?
         """
         Thread target for populating new object with progress indicator.
         """
         # mustn't use tailbone web session here
-        session = RattailSession()
+        app = self.get_rattail_app()
+        session = app.make_session()
         obj = session.get(self.model_class, uuid)
         try:
             self.populate_object(session, obj, progress=progress)
         except Exception as error:
             session.rollback()
             msg = "{} population failed".format(self.get_model_title())
             log.warning("{}: {}".format(msg, obj), exc_info=True)
@@ -1165,15 +1170,15 @@
                 if hash_:
                     kw['_anchor'] = hash_
                 return self.redirect(self.request.current_route_url(**kw))
 
             # return grid only, if partial page was requested
             if self.request.params.get('partial'):
                 # render grid data only, as JSON
-                return self.json_response(grid.get_buefy_data())
+                return self.json_response(grid.get_table_data())
 
         context = {
             'instance': instance,
             'instance_title': self.get_instance_title(instance),
             'instance_editable': self.editable_instance(instance),
             'instance_deletable': self.deletable_instance(instance),
             'form': form,
@@ -1298,15 +1303,15 @@
         instance = self.get_instance()
         instance_title = self.get_instance_title(instance)
         grid = self.make_version_grid(instance=instance)
 
         # return grid only, if partial page was requested
         if self.request.params.get('partial'):
             # render grid data only, as JSON
-            return self.json_response(grid.get_buefy_data())
+            return self.json_response(grid.get_table_data())
 
         return self.render_to_response('versions', {
             'instance': instance,
             'instance_title': instance_title,
             'instance_url': self.get_action_url('view', instance),
             'grid': grid,
         })
@@ -1350,14 +1355,15 @@
                 cls = (cls, 'uuid', 'uuid')
             elif len(cls) == 2:
                 cls = tuple([cls[0], cls[1], 'uuid'])
             classes.append(cls)
         return classes
 
     def make_revisions_grid(self, obj, empty_data=False):
+        model = self.model
         route_prefix = self.get_route_prefix()
         row_url = lambda txn, i: self.request.route_url(f'{route_prefix}.version',
                                                         uuid=obj.uuid,
                                                         txnid=txn.id)
 
         kwargs = {
             'component': 'versions-grid',
@@ -1386,16 +1392,16 @@
                                          .filter(txn_class.id == -1)
 
         else:
             kwargs['data'] = self.get_version_data(obj, order_by=False)
 
         grid = self.make_version_grid(**kwargs)
 
-        grid.set_joiner('user', lambda q: q.outerjoin(self.model.User))
-        grid.set_sorter('user', self.model.User.username)
+        grid.set_joiner('user', lambda q: q.outerjoin(model.User))
+        grid.set_sorter('user', model.User.username)
 
         grid.set_link('remote_addr')
 
         grid.append('id')
         grid.set_label('id', "TXN ID")
         grid.set_link('id')
 
@@ -1455,20 +1461,21 @@
                 'prev_txnid': older.id if older else None,
                 'next_txnid': newer.id if newer else None,
             }
 
         else: # no txnid, return grid data
             obj = self.get_instance()
             grid = self.make_revisions_grid(obj)
-            return grid.get_buefy_data()
+            return grid.get_table_data()
 
     def view_version(self):
         """
         View showing diff details of a particular object version.
         """
+        app = self.get_rattail_app()
         instance = self.get_instance()
         model_class = self.get_model_class()
         route_prefix = self.get_route_prefix()
         Transaction = continuum.transaction_class(model_class)
         transactions = model_transaction_query(self.Session(), instance, model_class,
                                                child_classes=self.normalize_version_child_classes())
         transaction_id = self.request.matchdict['txnid']
@@ -1508,15 +1515,15 @@
 
         return self.render_to_response('view_version', {
             'instance': instance,
             'instance_title': "{} (history)".format(instance_title),
             'instance_title_normal': instance_title,
             'instance_url': self.get_action_url('versions', instance),
             'transaction': transaction,
-            'changed': localtime(self.rattail_config, transaction.issued_at, from_utc=True),
+            'changed': app.localtime(transaction.issued_at, from_utc=True),
             'version_diffs': version_diffs,
             'show_prev_next': True,
             'prev_url': prev_url,
             'next_url': next_url,
             'previous_transaction': older,
             'next_transaction': newer,
             'title_for_version': self.title_for_version,
@@ -1759,24 +1766,18 @@
         View for downloading a data file.
         """
         obj = self.get_instance()
         filename = self.request.GET.get('filename', None)
         path = self.download_path(obj, filename)
         if not path or not os.path.exists(path):
             raise self.notfound()
-        response = FileResponse(path, request=self.request)
-        response.content_length = os.path.getsize(path)
+        response = self.file_response(path)
         content_type = self.download_content_type(path, filename)
         if content_type:
             response.content_type = content_type
-
-        # content-disposition
-        filename = os.path.basename(path)
-        response.content_disposition = str('attachment; filename="{}"'.format(filename))
-
         return response
 
     def download_content_type(self, path, filename):
         """
         Return a content type for a file download, if known.
         """
 
@@ -1845,15 +1846,15 @@
         return self.redirect(self.get_action_url('view', instance))
 
     def delete(self):
         """
         View for deleting an existing model record.
         """
         if not self.deletable:
-            raise httpexceptions.HTTPForbidden()
+            raise self.forbidden()
 
         self.deleting = True
         instance = self.get_instance()
         instance_title = self.get_instance_title(instance)
 
         if not self.deletable_instance(instance):
             self.request.session.flash("Deletion is not permitted for {}: {}".format(
@@ -2100,15 +2101,17 @@
             return session.get(self.model_class, uuid)
         raise NotImplementedError
 
     def execute_thread(self, key, user_uuid, progress=None, **kwargs):
         """
         Thread target for executing an object.
         """
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         obj = self.get_instance_for_key(key, session)
         user = session.get(model.User, user_uuid)
         try:
             success_msg = self.execute_instance(obj, user,
                                                 progress=progress,
                                                 **kwargs)
 
@@ -2915,19 +2918,19 @@
             # build a button if only given the data
             if isinstance(button, dict):
                 button = self.make_xref_button(**button)
 
             normal.append(button)
         return normal
 
-    def make_buefy_button(self, label,
-                          type=None, is_primary=False,
-                          url=None, target=None, is_external=False,
-                          icon_left=None,
-                          **kwargs):
+    def make_button(self, label,
+                    type=None, is_primary=False,
+                    url=None, target=None, is_external=False,
+                    icon_left=None,
+                    **kwargs):
         """
         Make and return a HTML ``<b-button>`` literal.
         """
         btn_kw = kwargs
         btn_kw.setdefault('c', label)
         btn_kw.setdefault('icon_pack', 'fas')
 
@@ -2972,15 +2975,15 @@
         :param url: URL for the link.
         :param text: Label for the button.
         :param internal: Boolean indicating if the link is internal to
            the site.  This is false by default, meaning the link is
            assumed to be external, which affects the icon and causes
            button click to open link in a new tab.
         """
-        # TODO: this should call make_buefy_button()
+        # TODO: this should call make_button()
 
         # nb. unfortunately HTML.tag() calls its first arg 'tag' and
         # so we can't pass a kwarg with that name...so instead we
         # patch that into place manually
         btn_kw = dict(type='is-primary',
                       href=kwargs['url'],
                       icon_pack='fas',
@@ -3498,22 +3501,22 @@
         return fields
 
     def download_results_normalize(self, obj, fields, **kwargs):
         """
         Normalize the given object into a data dict, for use when writing to
         the results file for download.
         """
+        app = self.get_rattail_app()
         data = {}
         for field in fields:
             value = getattr(obj, field, None)
 
             # make timestamps zone-aware
             if isinstance(value, datetime.datetime):
-                value = localtime(self.rattail_config, value,
-                                  from_utc=not self.has_local_times)
+                value = app.localtime(value, from_utc=not self.has_local_times)
 
             data[field] = value
 
         return data
 
     def download_results_coerce_csv(self, data, fields, **kwargs):
         """
@@ -3535,21 +3538,22 @@
         return csvrow
 
     def download_results_coerce_xlsx(self, data, fields, **kwargs):
         """
         Coerce the given data dict record, to a "row" dict suitable for use
         when writing directly to XLSX file.
         """
+        app = self.get_rattail_app()
         data = dict(data)
         for key in data:
             value = data[key]
 
             # make timestamps local, "zone-naive"
             if isinstance(value, datetime.datetime):
-                value = localtime(self.rattail_config, value, tzinfo=False)
+                value = app.localtime(value, tzinfo=False)
 
             data[key] = value
 
         return data
 
     def results_csv(self):
         """
@@ -3997,22 +4001,22 @@
                                message="Writing Excel file to disk")
 
     def download_results_rows_normalize(self, row, fields, **kwargs):
         """
         Normalize the given row object into a data dict, for use when writing
         to the results file for download.
         """
+        app = self.get_rattail_app()
         data = {}
         for field in fields:
             value = getattr(row, field, None)
 
             # make timestamps zone-aware
             if isinstance(value, datetime.datetime):
-                value = localtime(self.rattail_config, value,
-                                  from_utc=not self.has_local_times)
+                value = app.localtime(value, from_utc=not self.has_local_times)
 
             data[field] = value
 
         return data
 
     def download_results_rows_coerce_csv(self, data, fields, **kwargs):
         """
@@ -4034,38 +4038,40 @@
         return csvrow
 
     def download_results_rows_coerce_xlsx(self, data, fields, **kwargs):
         """
         Coerce the given data dict record, to a "row" dict suitable for use
         when writing directly to XLSX file.
         """
+        app = self.get_rattail_app()
         data = dict(data)
         for key in data:
             value = data[key]
 
             # convert GPC to pretty string
             if isinstance(value, GPC):
                 value = value.pretty()
 
             # make timestamps local, "zone-naive"
             elif isinstance(value, datetime.datetime):
-                value = localtime(self.rattail_config, value, tzinfo=False)
+                value = app.localtime(value, tzinfo=False)
 
             data[key] = value
 
         return data
 
     def row_results_xlsx(self):
         """
         Download current *row* results as XLSX.
         """
+        app = self.get_rattail_app()
         obj = self.get_instance()
         results = self.get_effective_row_data(sort=True)
         fields = self.get_row_xlsx_fields()
-        path = temp_path(suffix='.xlsx')
+        path = app.make_temp_file(suffix='.xlsx')
         writer = ExcelWriter(path, fields, sheet_title=self.get_row_model_title_plural())
         writer.write_header()
 
         rows = []
         for row_obj in results:
             data = self.get_row_xlsx_row(row_obj, fields)
             row = [data[field] for field in fields]
@@ -4095,29 +4101,30 @@
         # TODO: should this be shared at all? in a better way?
         return self.get_row_csv_fields()
 
     def get_row_xlsx_row(self, row, fields):
         """
         Return a dict for use when writing the row's data to XLSX download.
         """
+        app = self.get_rattail_app()
         xlrow = {}
         for field in fields:
             value = getattr(row, field, None)
 
             if isinstance(value, GPC):
                 value = str(value)
 
             elif isinstance(value, datetime.datetime):
                 # datetime values we provide to Excel must *not* have time zone info,
                 # but we should make sure they're in "local" time zone effectively.
                 # note however, this assumes a "naive" time value is in UTC zone!
                 if value.tzinfo:
-                    value = localtime(self.rattail_config, value, tzinfo=False)
+                    value = app.localtime(value, tzinfo=False)
                 else:
-                    value = localtime(self.rattail_config, value, from_utc=True, tzinfo=False)
+                    value = app.localtime(value, from_utc=True, tzinfo=False)
 
             xlrow[field] = value
         return xlrow
 
     def get_row_results_xlsx_filename(self, obj):
         return '{}.xlsx'.format(self.get_row_grid_key())
 
@@ -4173,33 +4180,35 @@
                     fields.append(prop.key)
         return fields
 
     def get_csv_row(self, obj, fields):
         """
         Return a dict for use when writing the row's data to CSV download.
         """
+        app = self.get_rattail_app()
         csvrow = {}
         for field in fields:
             value = getattr(obj, field, None)
             if isinstance(value, datetime.datetime):
                 # TODO: this assumes value is *always* naive UTC
-                value = localtime(self.rattail_config, value, from_utc=True)
+                value = app.localtime(value, from_utc=True)
             csvrow[field] = '' if value is None else str(value)
         return csvrow
 
     def get_row_csv_row(self, row, fields):
         """
         Return a dict for use when writing the row's data to CSV download.
         """
+        app = self.get_rattail_app()
         csvrow = {}
         for field in fields:
             value = getattr(row, field, None)
             if isinstance(value, datetime.datetime):
                 # TODO: this assumes value is *always* naive UTC
-                value = localtime(self.rattail_config, value, from_utc=True)
+                value = app.localtime(value, from_utc=True)
             csvrow[field] = '' if value is None else str(value)
         return csvrow
 
     ##############################
     # CRUD Stuff
     ##############################
 
@@ -5023,29 +5032,30 @@
     # Configuration Views
     ##############################
 
     def configure(self):
         """
         Generic view for configuring some aspect of the software.
         """
+        app = self.get_rattail_app()
         if self.request.method == 'POST':
             if self.request.POST.get('remove_settings'):
                 self.configure_remove_settings()
                 self.request.session.flash("All settings for {} have been "
                                            "removed.".format(self.get_config_title()),
                                            'warning')
                 return self.redirect(self.request.current_route_url())
             else:
                 data = self.request.POST
 
                 # collect any uploaded files
                 uploads = {}
                 for key, value in data.items():
                     if isinstance(value, cgi_FieldStorage):
-                        tempdir = tempfile.mkdtemp()
+                        tempdir = app.make_temp_dir()
                         filename = os.path.basename(value.filename)
                         filepath = os.path.join(tempdir, filename)
                         with open(filepath, 'wb') as f:
                             f.write(value.file.read())
                         uploads[key] = {
                             'filedir': tempdir,
                             'filename': filename,
```

### Comparing `Tailbone-0.9.90/tailbone/views/members.py` & `tailbone-0.9.91/tailbone/views/members.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/menus.py` & `tailbone-0.9.91/tailbone/views/menus.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/messages.py` & `tailbone-0.9.91/tailbone/views/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -25,18 +25,16 @@
 """
 
 from rattail.db import model
 from rattail.time import localtime
 
 import colander
 from deform import widget as dfwidget
-from pyramid import httpexceptions
 from webhelpers2.html import tags, HTML
 
-# from tailbone import forms
 from tailbone.db import Session
 from tailbone.views import MasterView
 from tailbone.util import raw_datetime
 
 
 class MessageView(MasterView):
     """
@@ -79,23 +77,23 @@
 
     def get_index_url(self, **kwargs):
         # not really used, but necessary to make certain other code happy
         return self.request.route_url('messages.inbox')
 
     def index(self):
         if not self.request.user:
-            raise httpexceptions.HTTPForbidden
+            raise self.forbidden()
         return super().index()
 
     def get_instance(self):
         if not self.request.user:
-            raise httpexceptions.HTTPForbidden
+            raise self.forbidden()
         message = super().get_instance()
         if not self.associated_with(message):
-            raise httpexceptions.HTTPForbidden
+            raise self.forbidden()
         return message
 
     def associated_with(self, message):
         if message.sender is self.request.user:
             return True
         for recip in message.recipients:
             if recip.recipient is self.request.user:
@@ -391,15 +389,15 @@
     def move(self):
         """
         Move a message, either to the archive or back to the inbox.
         """
         message = self.get_instance()
         recipient = self.get_recipient(message)
         if not recipient:
-            raise httpexceptions.HTTPForbidden
+            raise self.forbidden()
 
         dest = self.request.GET.get('dest')
         if dest not in ('inbox', 'archive'):
             self.request.session.flash("Sorry, I couldn't make sense out of that request.")
             return self.redirect(self.request.get_referrer(
                 default=self.request.route_url('messages_inbox')))
 
@@ -514,17 +512,17 @@
                                              .join(model.Person)
         g.filters['recipients'] = g.make_filter('recipients', model.Person.display_name,
                                                 default_active=True, default_verb='contains')
 
 
 class RecipientsWidgetBuefy(dfwidget.Widget):
     """
-    Custom "message recipients" widget, for use with Buefy / Vue.js themes.
+    Custom "message recipients" widget, for use with Vue.js themes.
     """
-    template = 'message_recipients_buefy'
+    template = 'message_recipients'
 
     def deserialize(self, field, pstruct):
         if pstruct is colander.null:
             return colander.null
         if not isinstance(pstruct, str):
             raise colander.Invalid(field.schema, "Pstruct is not a string")
         if not pstruct:
```

### Comparing `Tailbone-0.9.90/tailbone/views/people.py` & `tailbone-0.9.91/tailbone/views/people.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,17 @@
 
 import sqlalchemy as sa
 from sqlalchemy import orm
 import sqlalchemy_continuum as continuum
 
 from rattail.db import api
 from rattail.db.model import Person, PersonNote, MergePeopleRequest
-from rattail.db.util import maxlen
-from rattail.time import localtime
 from rattail.util import simple_error
 
 import colander
-from pyramid.httpexceptions import HTTPFound, HTTPNotFound
 from webhelpers2.html import HTML, tags
 
 from tailbone import forms, grids
 from tailbone.views import MasterView
 from tailbone.util import raw_datetime
 
 
@@ -217,15 +214,15 @@
         key = self.request.matchdict['uuid']
         instance = self.Session.get(model.Person, key)
         if instance:
             return instance
         instance = self.Session.get(model.VendorContact, key)
         if instance:
             return instance.person
-        raise HTTPNotFound
+        raise self.notfound()
 
     def is_person_protected(self, person):
         for user in person.users:
             if self.user_is_protected(user):
                 return True
         return False
 
@@ -491,15 +488,15 @@
             'max_one_member': app.get_membership_handler().max_one_per_person(),
             'use_preferred_first_name': self.people_handler.should_use_preferred_first_name(),
         }
 
         if self.request.has_perm('people_profile.view_versions'):
             context['revisions_grid'] = self.profile_revisions_grid(person)
 
-        return self.render_to_response('view_profile_buefy', context)
+        return self.render_to_response('view_profile', context)
 
     def get_context_tabchecks(self, person):
         app = self.get_rattail_app()
         membership = app.get_membership_handler()
         clientele = app.get_clientele_handler()
         tabchecks = {}
 
@@ -554,36 +551,29 @@
 
     def template_kwargs_view_profile(self, **kwargs):
         """
         Stub method so subclass can call `super()` for it.
         """
         return kwargs
 
-    def template_kwargs_view_profile_buefy(self, **kwargs):
-        """
-        Note that any subclass should not need to define this method.
-        It by default invokes :meth:`template_kwargs_view_profile()`
-        and returns that result.
-        """
-        return self.template_kwargs_view_profile(**kwargs)
-
     def get_max_lengths(self):
+        app = self.get_rattail_app()
         model = self.model
         lengths = {
-            'person_first_name': maxlen(model.Person.first_name),
-            'person_middle_name': maxlen(model.Person.middle_name),
-            'person_last_name': maxlen(model.Person.last_name),
-            'address_street': maxlen(model.PersonMailingAddress.street),
-            'address_street2': maxlen(model.PersonMailingAddress.street2),
-            'address_city': maxlen(model.PersonMailingAddress.city),
-            'address_state': maxlen(model.PersonMailingAddress.state),
-            'address_zipcode': maxlen(model.PersonMailingAddress.zipcode),
+            'person_first_name': app.maxlen(model.Person.first_name),
+            'person_middle_name': app.maxlen(model.Person.middle_name),
+            'person_last_name': app.maxlen(model.Person.last_name),
+            'address_street': app.maxlen(model.PersonMailingAddress.street),
+            'address_street2': app.maxlen(model.PersonMailingAddress.street2),
+            'address_city': app.maxlen(model.PersonMailingAddress.city),
+            'address_state': app.maxlen(model.PersonMailingAddress.state),
+            'address_zipcode': app.maxlen(model.PersonMailingAddress.zipcode),
         }
         if self.people_handler.should_use_preferred_first_name():
-            lengths['person_preferred_first_name'] = maxlen(model.Person.preferred_first_name)
+            lengths['person_preferred_first_name'] = app.maxlen(model.Person.preferred_first_name)
         return lengths
 
     def get_phone_type_options(self):
         """
         Returns a list of "phone type" options, for use in dropdown.
         """
         # TODO: should probably define this list somewhere else
@@ -1410,15 +1400,15 @@
 
         return versions
 
     def profile_revisions_data(self):
         """
         View which locates and organizes all relevant "transaction"
         (version) history data for a given Person.  Returns JSON, for
-        use with the Buefy table element on the full profile view.
+        use with the table element on the full profile view.
         """
         person = self.get_instance()
         versions = self.profile_revisions_collect(person)
 
         # organize final table data
         data = []
         all_txns = set([v.transaction for v in versions])
```

### Comparing `Tailbone-0.9.90/tailbone/views/permissions.py` & `tailbone-0.9.91/tailbone/views/permissions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/poser/__init__.py` & `tailbone-0.9.91/tailbone/views/poser/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/poser/master.py` & `tailbone-0.9.91/tailbone/views/poser/master.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/poser/reports.py` & `tailbone-0.9.91/tailbone/views/poser/reports.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/poser/views.py` & `tailbone-0.9.91/tailbone/views/poser/views.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/principal.py` & `tailbone-0.9.91/tailbone/views/principal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -39,15 +39,15 @@
     """
     Master view base class for security principal models, i.e. User and Role.
     """
 
     def get_fallback_templates(self, template, **kwargs):
         return [
             '/principal/{}.mako'.format(template),
-        ] + super(PrincipalMasterView, self).get_fallback_templates(template, **kwargs)
+        ] + super().get_fallback_templates(template, **kwargs)
 
     def perm_sortkey(self, item):
         key, value = item
         return value['label'].lower()
 
     def find_by_perm(self):
         """
@@ -70,17 +70,17 @@
                                                               permission)
         else: # otherwise clear both values
             permission_group = None
             permission = None
 
         context = {'permissions': sorted_perms, 'principals': principals}
 
-        perms = self.get_buefy_perms_data(sorted_perms)
-        context['buefy_perms'] = perms
-        context['buefy_sorted_groups'] = list(perms)
+        perms = self.get_perms_data(sorted_perms)
+        context['perms_data'] = perms
+        context['sorted_groups_data'] = list(perms)
 
         if permission_group and permission_group not in perms:
             permission_group = None
         if permission:
             if permission_group:
                 group = dict([(p['permkey'], p) for p in perms[permission_group]['permissions']])
                 if permission in group:
@@ -91,15 +91,15 @@
                 permission = None
 
         context['selected_group'] = permission_group
         context['selected_permission'] = permission
 
         return self.render_to_response('find_by_perm', context)
 
-    def get_buefy_perms_data(self, sorted_perms):
+    def get_perms_data(self, sorted_perms):
         data = OrderedDict()
         for gkey, group in sorted_perms:
 
             gperms = []
             for pkey, perm in group['perms']:
                 gperms.append({
                     'permkey': pkey,
```

### Comparing `Tailbone-0.9.90/tailbone/views/products.py` & `tailbone-0.9.91/tailbone/views/products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -33,16 +33,15 @@
 import sqlalchemy_continuum as continuum
 
 from rattail import enum, pod, sil
 from rattail.db import model, api, auth, Session as RattailSession
 from rattail.gpc import GPC
 from rattail.threads import Thread
 from rattail.exceptions import LabelPrintingError
-from rattail.util import load_object, pretty_quantity, simple_error
-from rattail.time import localtime, make_utc
+from rattail.util import simple_error
 
 import colander
 from deform import widget as dfwidget
 from webhelpers2.html import tags, HTML
 
 from tailbone import forms, grids
 from tailbone.views import MasterView
@@ -413,21 +412,21 @@
         text = self.render_price(product, field) or ""
 
         price = product.current_price
         if price:
             app = self.get_rattail_app()
 
             if price.starts:
-                starts = localtime(self.rattail_config, price.starts, from_utc=True)
+                starts = app.localtime(price.starts, from_utc=True)
                 starts = app.render_date(starts.date())
             else:
                 starts = "??"
 
             if price.ends:
-                ends = localtime(self.rattail_config, price.ends, from_utc=True)
+                ends = app.localtime(price.ends, from_utc=True)
                 ends = app.render_date(ends.date())
             else:
                 ends = "??"
 
             return HTML.tag('span', c=text,
                             title="{} thru {}".format(starts, ends))
 
@@ -452,31 +451,33 @@
         if not self.rattail_config.versioning_enabled():
             return False
         return self.rattail_config.getbool(
             'tailbone', 'products.show_effective_price_dates',
             default=True)
 
     def render_regular_price(self, product, field):
+        app = self.get_rattail_app()
         text = self.render_price(product, field)
 
         if text and self.show_price_effective_dates():
             history = self.get_regular_price_history(product)
             if history:
-                date = localtime(self.rattail_config, history[0]['changed'], from_utc=True).date()
+                date = app.localtime(history[0]['changed'], from_utc=True).date()
                 text = "{} (as of {})".format(text, date)
 
         return self.add_price_history_link(text, 'regular')
 
     def render_current_price(self, product, field):
+        app = self.get_rattail_app()
         text = self.render_price(product, field)
 
         if text and self.show_price_effective_dates():
             history = self.get_current_price_history(product)
             if history:
-                date = localtime(self.rattail_config, history[0]['changed'], from_utc=True).date()
+                date = app.localtime(history[0]['changed'], from_utc=True).date()
                 text = "{} (as of {})".format(text, date)
 
         return self.add_price_history_link(text, 'current')
 
     def warn_if_regprice_more_than_srp(self, product, text):
         sugprice = product.suggested_price.price if product.suggested_price else None
         regprice = product.regular_price.price if product.regular_price else None
@@ -485,18 +486,19 @@
         return text
 
     def render_suggested_price(self, product, column):
         text = self.render_price(product, column)
         if not text:
             return
 
+        app = self.get_rattail_app()
         if self.show_price_effective_dates():
             history = self.get_suggested_price_history(product)
             if history:
-                date = localtime(self.rattail_config, history[0]['changed'], from_utc=True).date()
+                date = app.localtime(history[0]['changed'], from_utc=True).date()
                 text = "{} (as of {})".format(text, date)
 
         text = self.warn_if_regprice_more_than_srp(product, text)
         return self.add_price_history_link(text, 'suggested')
 
     def render_grid_suggested_price(self, product, field):
         text = self.render_price(product, field)
@@ -522,21 +524,23 @@
         return app.render_percent(product.volatile.true_margin,
                                   places=3)
 
     def render_on_hand(self, product, column):
         inventory = product.inventory
         if not inventory:
             return ""
-        return pretty_quantity(inventory.on_hand)
+        app = self.get_rattail_app()
+        return app.render_quantity(inventory.on_hand)
 
     def render_on_order(self, product, column):
         inventory = product.inventory
         if not inventory:
             return ""
-        return pretty_quantity(inventory.on_order)
+        app = self.get_rattail_app()
+        return app.render_quantity(inventory.on_order)
 
     def template_kwargs_index(self, **kwargs):
         kwargs = super().template_kwargs_index(**kwargs)
         app = self.get_rattail_app()
         label_handler = app.get_label_handler()
         model = self.model
 
@@ -1101,23 +1105,25 @@
 
     def render_inventory_on_hand(self, product, field):
         if not product.inventory:
             return ""
         value = product.inventory.on_hand
         if not value:
             return ""
-        return pretty_quantity(value)
+        app = self.get_rattail_app()
+        return app.render_quantity(value)
 
     def render_inventory_on_order(self, product, field):
         if not product.inventory:
             return ""
         value = product.inventory.on_order
         if not value:
             return ""
-        return pretty_quantity(value)
+        app = self.get_rattail_app()
+        return app.render_quantity(value)
 
     def price_history(self):
         """
         AJAX view for fetching various types of price history for a product.
         """
         app = self.get_rattail_app()
         product = self.get_instance()
@@ -1132,41 +1138,42 @@
         jsdata = []
         for history in data:
             history = dict(history)
             price = history['price']
             if price is not None:
                 history['price'] = float(price)
                 history['price_display'] = app.render_currency(price)
-            changed = localtime(self.rattail_config, history['changed'], from_utc=True)
+            changed = app.localtime(history['changed'], from_utc=True)
             history['changed'] = str(changed)
             history['changed_display_html'] = raw_datetime(self.rattail_config, changed)
             user = history.pop('changed_by')
             history['changed_by_uuid'] = user.uuid if user else None
             history['changed_by_display'] = str(user or "??")
             jsdata.append(history)
         return jsdata
 
     def cost_history(self):
         """
         AJAX view for fetching cost history for a product.
         """
+        app = self.get_rattail_app()
         product = self.get_instance()
         data = self.get_cost_history(product)
 
         # make some data JSON-friendly
         jsdata = []
         for history in data:
             history = dict(history)
             cost = history['cost']
             if cost is not None:
                 history['cost'] = float(cost)
                 history['cost_display'] = "${:0.2f}".format(cost)
             else:
                 history['cost_display'] = None
-            changed = localtime(self.rattail_config, history['changed'], from_utc=True)
+            changed = app.localtime(history['changed'], from_utc=True)
             history['changed'] = str(changed)
             history['changed_display_html'] = raw_datetime(self.rattail_config, changed)
             user = history.pop('changed_by')
             history['changed_by_uuid'] = user.uuid
             history['changed_by_display'] = str(user)
             jsdata.append(history)
         return jsdata
@@ -1384,18 +1391,19 @@
         return {'grid': g, 'data': lookup_codes}
 
     def get_regular_price_history(self, product):
         """
         Returns a sequence of "records" which corresponds to the given
         product's regular price history.
         """
+        app = self.get_rattail_app()
         Transaction = continuum.transaction_class(model.Product)
         ProductVersion = continuum.version_class(model.Product)
         ProductPriceVersion = continuum.version_class(model.ProductPrice)
-        now = make_utc()
+        now = app.make_utc()
         history = []
 
         # first we find all relevant ProductVersion records
         versions = self.Session.query(ProductVersion)\
                                .join(Transaction,
                                      Transaction.id == ProductVersion.transaction_id)\
                                .filter(ProductVersion.uuid == product.uuid)\
@@ -1453,18 +1461,19 @@
         return list(final_history.values())
 
     def get_current_price_history(self, product):
         """
         Returns a sequence of "records" which corresponds to the given
         product's current price history.
         """
+        app = self.get_rattail_app()
         Transaction = continuum.transaction_class(model.Product)
         ProductVersion = continuum.version_class(model.Product)
         ProductPriceVersion = continuum.version_class(model.ProductPrice)
-        now = make_utc()
+        now = app.make_utc()
         history = []
 
         # first we find all relevant ProductVersion records
         versions = self.Session.query(ProductVersion)\
                                .join(Transaction,
                                      Transaction.id == ProductVersion.transaction_id)\
                                .filter(ProductVersion.uuid == product.uuid)\
@@ -1595,18 +1604,19 @@
         return list(final_history.values())
 
     def get_suggested_price_history(self, product):
         """
         Returns a sequence of "records" which corresponds to the given
         product's SRP history.
         """
+        app = self.get_rattail_app()
         Transaction = continuum.transaction_class(model.Product)
         ProductVersion = continuum.version_class(model.Product)
         ProductPriceVersion = continuum.version_class(model.ProductPrice)
-        now = make_utc()
+        now = app.make_utc()
         history = []
 
         # first we find all relevant ProductVersion records
         versions = self.Session.query(ProductVersion)\
                                .join(Transaction,
                                      Transaction.id == ProductVersion.transaction_id)\
                                .filter(ProductVersion.uuid == product.uuid)\
@@ -1664,18 +1674,19 @@
         return list(final_history.values())
 
     def get_cost_history(self, product):
         """
         Returns a sequence of "records" which corresponds to the given
         product's cost history.
         """
+        app = self.get_rattail_app()
         Transaction = continuum.transaction_class(model.Product)
         ProductVersion = continuum.version_class(model.Product)
         ProductCostVersion = continuum.version_class(model.ProductCost)
-        now = make_utc()
+        now = app.make_utc()
         history = []
 
         # we just find all relevant (preferred!) ProductCostVersion records
         versions = self.Session.query(ProductCostVersion)\
                                .join(Transaction,
                                      Transaction.id == ProductCostVersion.transaction_id)\
                                .filter(ProductCostVersion.product_uuid == product.uuid)\
@@ -1785,16 +1796,16 @@
             log.warning("error occurred while printing labels", exc_info=True)
             return {'error': str(error)}
         return {'ok': True}
 
     def search(self):
         """
         Perform a product search across multiple fields, and return
-        the results as JSON suitable for row data for a Buefy
-        ``<b-table>`` component.
+        the results as JSON suitable for row data for a table
+        component.
         """
         if 'term' not in self.request.GET:
             # TODO: deprecate / remove this?  not sure if/where it is used
             return self.search_v1()
 
         term = self.request.GET.get('term')
         if not term:
@@ -1944,18 +1955,19 @@
             }),
         ])
 
     def make_batch(self):
         """
         View for making a new batch from current product grid query.
         """
+        app = self.get_rattail_app()
         supported = self.get_supported_batches()
         batch_options = []
         for key, info in list(supported.items()):
-            handler = load_object(info['spec'])(self.rattail_config)
+            handler = app.load_object(info['spec'])(self.rattail_config)
             handler.spec = info['spec']
             handler.option_key = key
             handler.option_title = info.get('title', handler.get_model_title())
             supported[key] = handler
             batch_options.append((key, handler.option_title))
 
         schema = colander.SchemaNode(
@@ -2444,27 +2456,27 @@
 
         # but maybe also show buttons to change status
         buttons = []
 
         if (self.has_perm('ignore_product')
             and status in (self.enum.PENDING_PRODUCT_STATUS_PENDING,
                            self.enum.PENDING_PRODUCT_STATUS_READY)):
-            buttons.append(self.make_buefy_button("Ignore Product",
-                                                  type='is-warning',
-                                                  icon_left='ban',
-                                                  **{'@click': "$emit('ignore-product')"}))
+            buttons.append(self.make_button("Ignore Product",
+                                            type='is-warning',
+                                            icon_left='ban',
+                                            **{'@click': "$emit('ignore-product')"}))
 
         if (self.has_perm('resolve_product')
             and status in (self.enum.PENDING_PRODUCT_STATUS_PENDING,
                            self.enum.PENDING_PRODUCT_STATUS_READY,
                            self.enum.PENDING_PRODUCT_STATUS_IGNORED)):
-            buttons.append(self.make_buefy_button("Resolve Product",
-                                                  is_primary=True,
-                                                  icon_left='object-ungroup',
-                                                  **{'@click': "$emit('resolve-product')"}))
+            buttons.append(self.make_button("Resolve Product",
+                                            is_primary=True,
+                                            icon_left='object-ungroup',
+                                            **{'@click': "$emit('resolve-product')"}))
 
         if buttons:
             text = HTML.tag('span', class_='control', c=[text])
             buttons = HTML.tag('div', class_='buttons', c=buttons)
             html = HTML.tag('b-field', grouped='grouped', c=[text, buttons])
 
         return html
```

### Comparing `Tailbone-0.9.90/tailbone/views/progress.py` & `tailbone-0.9.91/tailbone/views/progress.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/projects.py` & `tailbone-0.9.91/tailbone/views/projects.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchases/__init__.py` & `tailbone-0.9.91/tailbone/views/purchases/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchases/core.py` & `tailbone-0.9.91/tailbone/views/purchases/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchases/credits.py` & `tailbone-0.9.91/tailbone/views/purchases/credits.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchasing/__init__.py` & `tailbone-0.9.91/tailbone/views/purchasing/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchasing/batch.py` & `tailbone-0.9.91/tailbone/views/purchasing/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -24,18 +24,17 @@
 Base class for purchasing batch views
 """
 
 from rattail.db.model import PurchaseBatch, PurchaseBatchRow
 
 import colander
 from deform import widget as dfwidget
-from pyramid import httpexceptions
 from webhelpers2.html import tags, HTML
 
-from tailbone import forms, grids
+from tailbone import forms
 from tailbone.views.batch import BatchMasterView
 
 
 class PurchasingBatchView(BatchMasterView):
     """
     Master view base class, for purchase batches.  The views for both
     "ordering" and "receiving" batches will inherit from this.
@@ -822,15 +821,15 @@
             g.remove('expiration_date')
 
         return g
 
     def render_row_credits(self, row, field):
         g = self.make_row_credits_grid(row)
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='rowData.credits'))
+            g.render_table_element(data_prop='rowData.credits'))
 
 #     def before_create_row(self, form):
 #         row = form.fieldset.model
 #         batch = self.get_instance()
 #         batch.add_row(row)
 #         # TODO: this seems heavy-handed but works..
 #         row.product_uuid = self.item_lookup(form.fieldset.item_lookup.value)
```

### Comparing `Tailbone-0.9.90/tailbone/views/purchasing/costing.py` & `tailbone-0.9.91/tailbone/views/purchasing/costing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/purchasing/ordering.py` & `tailbone-0.9.91/tailbone/views/purchasing/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,32 +306,30 @@
         history = list(reversed(history))
 
         title = self.get_instance_title(batch)
         order_date = batch.date_ordered
         if not order_date:
             order_date = localtime(self.rattail_config).date()
 
-        buefy_data = self.get_worksheet_buefy_data(departments)
-
         return self.render_to_response('worksheet', {
             'batch': batch,
             'order_date': order_date,
             'instance': batch,
             'instance_title': title,
             'instance_url': self.get_action_url('view', batch),
             'vendor': batch.vendor,
             'departments': departments,
             'history': history,
             'get_upc': lambda p: p.upc.pretty() if p.upc else '',
             'header_columns': self.order_form_header_columns,
             'ignore_cases': not self.handler.allow_cases(),
-            'worksheet_data': buefy_data,
+            'worksheet_data': self.get_worksheet_data(departments),
         })
 
-    def get_worksheet_buefy_data(self, departments):
+    def get_worksheet_data(self, departments):
         data = {}
         for department in departments.values():
             for subdepartment in department._order_subdepartments.values():
                 for i, cost in enumerate(subdepartment._order_costs, 1):
                     cases = int(cost._batchrow.cases_ordered or 0) if cost._batchrow else None
                     units = int(cost._batchrow.units_ordered or 0) if cost._batchrow else None
                     key = 'cost_{}'.format(cost.uuid)
```

### Comparing `Tailbone-0.9.90/tailbone/views/purchasing/receiving.py` & `tailbone-0.9.91/tailbone/views/purchasing/receiving.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -29,20 +29,18 @@
 import decimal
 import logging
 from collections import OrderedDict
 
 import humanize
 
 from rattail import pod
-from rattail.time import localtime, make_utc
-from rattail.util import pretty_quantity, prettify, simple_error
+from rattail.util import prettify, simple_error
 
 import colander
 from deform import widget as dfwidget
-from pyramid import httpexceptions
 from webhelpers2.html import tags, HTML
 
 from tailbone import forms, grids
 from tailbone.util import get_form_data
 from tailbone.views.purchasing import PurchasingBatchView
 
 
@@ -777,16 +775,16 @@
             factory = self.get_grid_factory()
 
             g = factory('batch_po_vs_invoice_breakdown', [],
                 columns=['title', 'count'])
             g.set_click_handler('title', "autoFilterPoVsInvoice(props.row)")
             kwargs['po_vs_invoice_breakdown_data'] = breakdown
             kwargs['po_vs_invoice_breakdown_grid'] = HTML.literal(
-                g.render_buefy_table_element(data_prop='poVsInvoiceBreakdownData',
-                                             empty_labels=True))
+                g.render_table_element(data_prop='poVsInvoiceBreakdownData',
+                                       empty_labels=True))
 
         kwargs['allow_edit_catalog_unit_cost'] = self.allow_edit_catalog_unit_cost(batch)
         kwargs['allow_edit_invoice_unit_cost'] = self.allow_edit_invoice_unit_cost(batch)
 
         if (kwargs['allow_edit_catalog_unit_cost']
             and kwargs['allow_edit_invoice_unit_cost']
             and not batch.get_param('confirmed_all_costs')):
@@ -1133,14 +1131,15 @@
             result['units'] = float(result['units'])
         return result
 
     def receive_row(self, **kwargs):
         """
         Primary desktop view for row-level receiving.
         """
+        app = self.get_rattail_app()
         # TODO: this code was largely copied from mobile_receive_row() but it
         # tries to pave the way for shared logic, i.e. where the latter would
         # simply invoke this method and return the result.  however we're not
         # there yet...for now it's only tested for desktop
         self.viewing = True
         row = self.get_row_instance()
 
@@ -1266,25 +1265,25 @@
                 context['quick_receive_uom'] = context['unit_uom']
                 accounted_for = self.handler.get_units_accounted_for(row)
                 remainder = self.handler.get_units_ordered(row) - accounted_for
 
                 if accounted_for:
                     # some product accounted for; button should receive "remainder" only
                     if remainder:
-                        remainder = pretty_quantity(remainder)
+                        remainder = app.render_quantity(remainder)
                         context['quick_receive_quantity'] = remainder
                         context['quick_receive_text'] = "Receive Remainder ({} {})".format(remainder, context['unit_uom'])
                     else:
                         # unless there is no remainder, in which case disable it
                         context['quick_receive'] = False
 
                 else: # nothing yet accounted for, button should receive "all"
                     if not remainder:
                         raise ValueError("why is remainder empty?")
-                    remainder = pretty_quantity(remainder)
+                    remainder = app.render_quantity(remainder)
                     context['quick_receive_quantity'] = remainder
                     context['quick_receive_text'] = "Receive ALL ({} {})".format(remainder, context['unit_uom'])
 
         # effective uom can vary in a few ways...the basic default is 'CS' if
         # self.default_uom_is_case is true, otherwise whatever unit_uom is.
         sticky_case = None
         # if mobile:
```

### Comparing `Tailbone-0.9.90/tailbone/views/reportcodes.py` & `tailbone-0.9.91/tailbone/views/reportcodes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/reports.py` & `tailbone-0.9.91/tailbone/views/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -28,17 +28,16 @@
 import json
 import re
 import datetime
 import logging
 from collections import OrderedDict
 
 import rattail
-from rattail.db import model, Session as RattailSession
+from rattail.db.model import ReportOutput
 from rattail.files import resource_path
-from rattail.time import localtime
 from rattail.threads import Thread
 from rattail.util import simple_error
 
 import colander
 from deform import widget as dfwidget
 from mako.template import Template
 from pyramid.response import Response
@@ -77,14 +76,15 @@
     """
 
     report_template_path = 'tailbone:reports/ordering_worksheet.mako'
 
     upc_getter = staticmethod(get_upc)
 
     def __call__(self):
+        model = self.model
         if self.request.params.get('vendor'):
             vendor = Session.get(model.Vendor, self.request.params['vendor'])
             if vendor:
                 departments = []
                 uuids = self.request.params.get('departments')
                 if uuids:
                     for uuid in uuids.split(','):
@@ -100,15 +100,16 @@
                 return response
         return {}
 
     def write_report(self, vendor, departments, preferred_only):
         """
         Rendering engine for the ordering worksheet report.
         """
-
+        app = self.get_rattail_app()
+        model = self.model
         q = Session.query(model.ProductCost)
         q = q.join(model.Product)
         q = q.filter(model.Product.deleted == False)
         q = q.filter(model.ProductCost.vendor == vendor)
         q = q.filter(model.Product.department_uuid.in_([x.uuid for x in departments]))
         if preferred_only:
             q = q.filter(model.ProductCost.preference == 1)
@@ -123,15 +124,15 @@
 
         def cost_sort_key(cost):
             product = cost.product
             brand = product.brand.name if product.brand else ''
             key = '{0} {1}'.format(brand, product.description)
             return key
 
-        now = localtime(self.request.rattail_config)
+        now = app.localtime()
         data = dict(
             vendor=vendor,
             costs=costs,
             cost_sort_key=cost_sort_key,
             date=now.strftime('%a %d %b %Y'),
             time=now.strftime('%I:%M %p'),
             get_upc=self.upc_getter,
@@ -153,15 +154,15 @@
 
     upc_getter = staticmethod(get_upc)
 
     def __call__(self):
         """
         This is the "Inventory Worksheet" report.
         """
-
+        model = self.model
         departments = Session.query(model.Department)
 
         if self.request.params.get('department'):
             department = departments.get(self.request.params['department'])
             if department:
                 body = self.write_report(department)
                 response = Response(content_type=str('text/html'))
@@ -174,28 +175,30 @@
         departments = departments.all()
         return{'departments': departments}
 
     def write_report(self, department):
         """
         Generates the Inventory Worksheet report.
         """
+        app = self.get_rattail_app()
+        model = self.model
 
         def get_products(subdepartment):
             q = Session.query(model.Product)
             q = q.outerjoin(model.Brand)
             q = q.filter(model.Product.deleted == False)
             q = q.filter(model.Product.subdepartment == subdepartment)
             if self.request.params.get('weighted-only'):
                 q = q.filter(model.Product.weighed == True)
             if self.request.params.get('exclude-not-for-sale'):
                 q = q.filter(model.Product.not_for_sale == False)
             q = q.order_by(model.Brand.name, model.Product.description)
             return q.all()
 
-        now = localtime(self.request.rattail_config)
+        now = app.localtime()
         data = dict(
             date=now.strftime('%a %d %b %Y'),
             time=now.strftime('%I:%M %p'),
             department=department,
             get_products=get_products,
             get_upc=self.upc_getter,
             )
@@ -205,15 +208,15 @@
         return template.render(**data)
 
 
 class ReportOutputView(ExportMasterView):
     """
     Master view for report output
     """
-    model_class = model.ReportOutput
+    model_class = ReportOutput
     route_prefix = 'report_output'
     url_prefix = '/reports/generated'
     creatable = True
     downloadable = True
     bulk_deletable = True
     configurable = True
     config_title = "Reporting"
@@ -234,31 +237,31 @@
         'params',
         'filename',
         'created',
         'created_by',
     ]
 
     def __init__(self, request):
-        super(ReportOutputView, self).__init__(request)
+        super().__init__(request)
         self.report_handler = self.get_report_handler()
 
     def get_report_handler(self):
         app = self.get_rattail_app()
         return app.get_report_handler()
 
     def configure_grid(self, g):
-        super(ReportOutputView, self).configure_grid(g)
+        super().configure_grid(g)
 
         g.filters['report_name'].default_active = True
         g.filters['report_name'].default_verb = 'contains'
 
         g.set_link('filename')
 
     def configure_form(self, f):
-        super(ReportOutputView, self).configure_form(f)
+        super().configure_form(f)
 
         # report_type
         f.set_renderer('report_type', self.render_report_type)
 
         # params
         f.set_renderer('params', self.render_params)
 
@@ -278,18 +281,18 @@
                 url = self.request.route_url('poser_reports.view',
                                              report_key=poser_key)
                 rendered = tags.link_to(type_key, url)
 
         # add help button if report has a link
         report = self.report_handler.get_report(type_key)
         if report and report.help_url:
-            button = self.make_buefy_button("Help for this report",
-                                            url=report.help_url,
-                                            is_external=True,
-                                            icon_left='question-circle')
+            button = self.make_button("Help for this report",
+                                      url=report.help_url,
+                                      is_external=True,
+                                      icon_left='question-circle')
             button = HTML.tag('div', class_='level-item', c=[button])
             rendered = HTML.tag('div', class_='level-item', c=[rendered])
             rendered = HTML.tag('div', class_='level-left', c=[rendered, button])
 
         return rendered
 
     def render_params(self, report, field):
@@ -307,27 +310,27 @@
         g = factory(
             key='{}.params'.format(route_prefix),
             data=params,
             columns=['key', 'value'],
             labels={'key': "Name"},
         )
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='paramsData'))
+            g.render_table_element(data_prop='paramsData'))
 
     def get_params_context(self, report):
         params_data = []
         for name, value in (report.params or {}).items():
             params_data.append({
                 'key': name,
                 'value': value,
             })
         return params_data
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(ReportOutputView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
         output = kwargs['instance']
 
         kwargs['params_data'] = self.get_params_context(output)
 
         # build custom URL to re-build this report
         url = None
         if output.report_type:
@@ -335,15 +338,15 @@
                                          type_key=output.report_type,
                                          _query=output.params)
         kwargs['rerun_report_url'] = url
 
         return kwargs
 
     def template_kwargs_delete(self, **kwargs):
-        kwargs = super(ReportOutputView, self).template_kwargs_delete(**kwargs)
+        kwargs = super().template_kwargs_delete(**kwargs)
 
         report = kwargs['instance']
         kwargs['params_data'] = self.get_params_context(report)
 
         return kwargs
 
     def create(self):
@@ -492,15 +495,17 @@
 
     def generate_thread(self, report, params, user_uuid, progress=None):
         """
         Generate output for the given report and params, and return the
         resulting :class:`rattail:~rattail.db.model.reports.ReportOutput`
         object.
         """
-        session = RattailSession()
+        app = self.get_rattail_app()
+        model = self.model
+        session = app.make_session()
         user = session.get(model.User, user_uuid)
         try:
             output = self.report_handler.generate_output(session, report, params, user, progress=progress)
 
         # if anything goes wrong, rollback and log the error etc.
         except Exception as error:
             session.rollback()
@@ -599,15 +604,15 @@
         'system_key',
         # 'problem_key',
         'problem_title',
         'email_recipients',
     ]
 
     def __init__(self, request):
-        super(ProblemReportView, self).__init__(request)
+        super().__init__(request)
 
         app = self.get_rattail_app()
         self.problem_handler = app.get_problem_report_handler()
         # TODO: deprecate / remove this
         self.handler = self.problem_handler
 
     def normalize(self, report, keep_report=True):
@@ -656,15 +661,15 @@
     def get_instance_title(self, report_info):
         return report_info['problem_title']
 
     def make_form_schema(self):
         return ProblemReportSchema()
 
     def configure_form(self, f):
-        super(ProblemReportView, self).configure_form(f)
+        super().configure_form(f)
 
         # email_*
         if self.editing:
             f.remove('email_key',
                      'email_recipients')
         else:
             f.set_renderer('email_key', self.render_email_key)
@@ -699,18 +704,18 @@
         recips = report_info['email_recipients']
         return ', '.join(recips)
 
     def render_days(self, report_info, field):
         g = self.get_grid_factory()('days', [],
                                     columns=['weekday_name', 'enabled'],
                                     labels={'weekday_name': "Weekday"})
-        return HTML.literal(g.render_buefy_table_element(data_prop='weekdaysData'))
+        return HTML.literal(g.render_table_element(data_prop='weekdaysData'))
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(ProblemReportView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
         report_info = kwargs['instance']
 
         data = []
         for i in range(7):
             data.append({
                 'weekday': i,
                 'weekday_name': calendar.day_name[i],
```

### Comparing `Tailbone-0.9.90/tailbone/views/roles.py` & `tailbone-0.9.91/tailbone/views/roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -25,15 +25,15 @@
 """
 
 import os
 
 from sqlalchemy import orm
 from openpyxl.styles import Font, PatternFill
 
-from rattail.db import model
+from rattail.db.model import Role
 from rattail.db.auth import administrator_role, guest_role, authenticated_role
 from rattail.excel import ExcelWriter
 
 import colander
 from deform import widget as dfwidget
 from webhelpers2.html import HTML
 
@@ -42,15 +42,15 @@
 from tailbone.views.principal import PrincipalMasterView, PermissionsRenderer
 
 
 class RoleView(PrincipalMasterView):
     """
     Master view for the Role model.
     """
-    model_class = model.Role
+    model_class = Role
     has_versions = True
     touchable = True
 
     labels = {
         'adminish': "Admin-ish",
         'sync_me': "Sync Attrs & Perms",
     }
@@ -73,15 +73,15 @@
         'sync_users',
         'node_type',
         'users',
         'permissions',
     ]
 
     def configure_grid(self, g):
-        super(RoleView, self).configure_grid(g)
+        super().configure_grid(g)
 
         # name
         g.filters['name'].default_active = True
         g.filters['name'].default_verb = 'contains'
         g.set_sort_defaults('name')
         g.set_link('name')
 
@@ -154,24 +154,25 @@
         user = self.request.user
         if user and role in user.roles:
             return self.has_perm('edit_my')
 
         return True
 
     def unique_name(self, node, value):
+        model = self.model
         query = self.Session.query(model.Role)\
                             .filter(model.Role.name == value)
         if self.editing:
             role = self.get_instance()
             query = query.filter(model.Role.uuid != role.uuid)
         if query.count():
             raise colander.Invalid(node, "Name must be unique")
 
     def configure_form(self, f):
-        super(RoleView, self).configure_form(f)
+        super().configure_form(f)
         role = f.model_instance
         app = self.get_rattail_app()
         auth = app.get_auth_handler()
 
         # name
         f.set_validator('name', self.unique_name)
 
@@ -261,15 +262,15 @@
 
         if self.request.has_perm('users.view'):
             g.main_actions.append(self.make_action('view', icon='eye'))
         if self.request.has_perm('users.edit'):
             g.main_actions.append(self.make_action('edit', icon='edit'))
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='usersData'))
+            g.render_table_element(data_prop='usersData'))
 
     def get_available_permissions(self):
         """
         Should return a dictionary with all "available" permissions.  The
         result of this will vary depending on the current user, because a user
         is only allowed to "manage" permissions which they themselves have been
         granted.
@@ -318,15 +319,15 @@
 
         The role is updated as per usual, and then we also invoke
         :meth:`update_permissions()` in order to correctly handle that part,
         i.e. ensure the user can't modify permissions which they do not have.
         """
         if data is None:
             data = form.validated
-        role = super(RoleView, self).objectify(form, data)
+        role = super().objectify(form, data)
         self.update_permissions(role, data['permissions'])
         return role
 
     def update_permissions(self, role, permissions):
         """
         Update the given role's permissions, according to those specified.
         Note that this will not simply "clobber" the role's existing
@@ -341,14 +342,15 @@
             for pkey, perm in group['perms'].items():
                 if pkey in permissions:
                     auth.grant_permission(role, pkey)
                 else:
                     auth.revoke_permission(role, pkey)
 
     def template_kwargs_view(self, **kwargs):
+        model = self.model
         role = kwargs['instance']
         if role.users:
             users = sorted(role.users, key=lambda u: u.username)
             actions = [
                 grids.GridAction('view', icon='zoomin',
                                  url=lambda r, i: self.request.route_url('users.view', uuid=r.uuid))
             ]
@@ -386,14 +388,15 @@
         authenticated = authenticated_role(self.Session())
         if role in (admin, guest, authenticated):
             self.request.session.flash("You may not delete the {} role.".format(role.name), 'error')
             return self.redirect(self.request.get_referrer(default=self.request.route_url('roles')))
 
     def find_principals_with_permission(self, session, permission):
         app = self.get_rattail_app()
+        model = self.model
         auth = app.get_auth_handler()
 
         # TODO: this should search Permission table instead, and work backward to Role?
         all_roles = session.query(model.Role)\
                            .order_by(model.Role.name)\
                            .options(orm.joinedload(model.Role._permissions))
         roles = []
@@ -404,14 +407,15 @@
 
     def download_permissions_matrix(self):
         """
         View which renders the complete role / permissions matrix data into an
         Excel spreadsheet, and returns that file.
         """
         app = self.get_rattail_app()
+        model = self.model
         auth = app.get_auth_handler()
 
         roles = self.Session.query(model.Role)\
                             .order_by(model.Role.name)\
                             .all()
 
         permissions = self.get_available_permissions()
```

### Comparing `Tailbone-0.9.90/tailbone/views/settings.py` & `tailbone-0.9.91/tailbone/views/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -28,16 +28,16 @@
 import re
 import subprocess
 import sys
 from collections import OrderedDict
 
 import json
 
-from rattail.db import model
-from rattail.settings import Setting
+from rattail.db.model import Setting
+from rattail.settings import Setting as AppSetting
 from rattail.util import import_module_path
 
 import colander
 
 from tailbone import forms
 from tailbone.db import Session
 from tailbone.views import MasterView, View
@@ -77,33 +77,33 @@
 
         for pkg in data:
             pkg.setdefault('editable_project_location', '')
 
         return data
 
     def configure_grid(self, g):
-        super(AppInfoView, self).configure_grid(g)
+        super().configure_grid(g)
 
         g.sorters['name'] = g.make_simple_sorter('name', foldcase=True)
         g.set_sort_defaults('name')
         g.set_searchable('name')
 
         g.sorters['version'] = g.make_simple_sorter('version', foldcase=True)
 
         g.sorters['editable_project_location'] = g.make_simple_sorter(
             'editable_project_location', foldcase=True)
         g.set_searchable('editable_project_location')
 
     def template_kwargs_index(self, **kwargs):
-        kwargs = super(AppInfoView, self).template_kwargs_index(**kwargs)
+        kwargs = super().template_kwargs_index(**kwargs)
         kwargs['configure_button_title'] = "Configure App"
         return kwargs
 
     def configure_get_context(self, **kwargs):
-        context = super(AppInfoView, self).configure_get_context(**kwargs)
+        context = super().configure_get_context(**kwargs)
 
         weblibs = OrderedDict([
             ('vue', "Vue"),
             ('vue_resource', "vue-resource"),
             ('buefy', "Buefy"),
             ('buefy.css', "Buefy CSS"),
             ('fontawesome', "FontAwesome"),
@@ -191,38 +191,39 @@
         ]
 
 
 class SettingView(MasterView):
     """
     Master view for the settings model.
     """
-    model_class = model.Setting
+    model_class = Setting
     model_title = "Raw Setting"
     model_title_plural = "Raw Settings"
     bulk_deletable = True
     feedback = re.compile(r'^rattail\.mail\.user_feedback\..*')
 
     grid_columns = [
         'name',
         'value',
     ]
 
     def configure_grid(self, g):
-        super(SettingView, self).configure_grid(g)
+        super().configure_grid(g)
         g.filters['name'].default_active = True
         g.filters['name'].default_verb = 'contains'
         g.set_sort_defaults('name')
         g.set_link('name')
 
     def configure_form(self, f):
-        super(SettingView, self).configure_form(f)
+        super().configure_form(f)
         if self.creating:
             f.set_validator('name', self.unique_name)
 
     def unique_name(self, node, value):
+        model = self.model
         setting = self.Session.get(model.Setting, value)
         if setting:
             raise colander.Invalid(node, "Setting name must be unique")
 
     def editable_instance(self, setting):
         if self.rattail_config.demo():
             return not bool(self.feedback.match(setting.name))
@@ -241,15 +242,15 @@
 
     def delete_instance(self, setting):
 
         # nb. force cache invalidation
         self.rattail_config.beaker_invalidate_setting(setting.name)
 
         # otherwise delete like normal
-        super(SettingView, self).delete_instance(setting)
+        super().delete_instance(setting)
 
 
 # TODO: deprecate / remove this
 SettingsView = SettingView
 
 
 class AppSettingsForm(forms.Form):
@@ -303,22 +304,22 @@
             'index_title': "App Settings",
             'form': form,
             'dform': form.make_deform_form(),
             'groups': groups,
             'settings': settings,
             'config_options': config_options,
         }
-        context['buefy_data'] = self.get_buefy_data(form, groups, settings)
+        context['settings_data'] = self.get_settings_data(form, groups, settings)
         # TODO: this seems hacky, and probably only needed if theme changes?
         if current_group == '(All)':
             current_group = ''
         context['current_group'] = current_group
         return context
 
-    def get_buefy_data(self, form, groups, settings):
+    def get_settings_data(self, form, groups, settings):
         dform = form.make_deform_form()
         grouped = dict([(label, [])
                         for label in groups])
 
         for setting in settings:
             field = dform[setting.node_name]
             s = {
@@ -336,16 +337,15 @@
             # as Python value here, and it will be JSON-encoded later.
             value = form.get_vuejs_model_value(field)
             value = json.loads(value)
             s['value'] = value
 
             # specify error / message if applicable
             # TODO: not entirely clear to me why some field errors are
-            # represented differently?  presumably it depends on
-            # whether Buefy is used by the theme.
+            # represented differently?
             if field.error:
                 s['error'] = True
                 if isinstance(field.error, colander.Invalid):
                     s['error_messages'] = [field.errormsg]
                 else:
                     s['error_messages'] = field.error_messages()
 
@@ -403,15 +403,15 @@
             modules = ['rattail.settings']
             core_only = True
 
         for module in modules:
             module = import_module_path(module)
             for name in dir(module):
                 obj = getattr(module, name)
-                if isinstance(obj, type) and issubclass(obj, Setting) and obj is not Setting:
+                if isinstance(obj, type) and issubclass(obj, AppSetting) and obj is not AppSetting:
                     if core_only and not obj.core:
                         continue
                     # NOTE: we set this here, and reference it elsewhere
                     obj.node_name = self.get_node_name(obj)
                     yield obj
 
     def get_node_name(self, setting):
```

### Comparing `Tailbone-0.9.90/tailbone/views/shifts/__init__.py` & `tailbone-0.9.91/tailbone/views/shifts/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/shifts/core.py` & `tailbone-0.9.91/tailbone/views/shifts/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/shifts/lib.py` & `tailbone-0.9.91/tailbone/views/shifts/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -24,17 +24,16 @@
 Base views for time sheets
 """
 
 import datetime
 
 import sqlalchemy as sa
 
-from rattail import enum
-from rattail.db import model, api
-from rattail.time import localtime, make_utc, get_sunday
+from rattail.db import api
+from rattail.time import get_sunday
 from rattail.util import hours_as_decimal
 
 import colander
 from deform import widget as dfwidget
 from webhelpers2.html import tags, HTML
 
 from tailbone import forms
@@ -79,25 +78,27 @@
     def get_url_prefix(cls):
         return getattr(cls, 'url_prefix', cls.key).rstrip('/')
 
     def get_timesheet_context(self):
         """
         Determine date/store/dept context from user's session and/or defaults.
         """
+        app = self.get_rattail_app()
+        model = self.model
         date = None
         date_key = 'timesheet.{}.date'.format(self.key)
         if date_key in self.request.session:
             date_value = self.request.session.get(date_key)
             if date_value:
                 try:
                     date = datetime.datetime.strptime(date_value, '%m/%d/%Y').date()
                 except ValueError:
                     pass
         if not date:
-            date = localtime(self.rattail_config).date()
+            date = app.today()
 
         store = None
         department = None
         store_key = 'timesheet.{}.store'.format(self.key)
         department_key = 'timesheet.{}.department'.format(self.key)
         if store_key in self.request.session or department_key in self.request.session:
             store_uuid = self.request.session.get(store_key)
@@ -109,15 +110,15 @@
         else: # no store/department in session
             if self.default_filter_store:
                 store = self.rattail_config.get('rattail', 'store')
                 if store:
                     store = api.get_store(Session(), store)
 
         employees = Session.query(model.Employee)\
-                           .filter(model.Employee.status == enum.EMPLOYEE_STATUS_CURRENT)
+                           .filter(model.Employee.status == self.enum.EMPLOYEE_STATUS_CURRENT)
         if store:
             employees = employees.join(model.EmployeeStore)\
                                  .filter(model.EmployeeStore.store == store)
         if department:
             employees = employees.join(model.EmployeeDepartment)\
                                  .filter(model.EmployeeDepartment.department == department)
 
@@ -128,25 +129,27 @@
             'employees': employees.all(),
         }
 
     def get_employee_context(self):
         """
         Determine employee/date context from user's session and/or defaults
         """
+        app = self.get_rattail_app()
+        model = self.model
         date = None
         date_key = 'timesheet.{}.employee.date'.format(self.key)
         if date_key in self.request.session:
             date_value = self.request.session.get(date_key)
             if date_value:
                 try:
                     date = datetime.datetime.strptime(date_value, '%m/%d/%Y').date()
                 except ValueError:
                     pass
         if not date:
-            date = localtime(self.rattail_config).date()
+            date = app.today()
 
         employee = None
         employee_key = 'timesheet.{}.employee'.format(self.key)
         if employee_key in self.request.session:
             employee_uuid = self.request.session[employee_key]
             employee = Session.get(model.Employee, employee_uuid) if employee_uuid else None
         if not employee:
@@ -187,27 +190,27 @@
 
     def make_full_filter_form(self, context):
         form = forms.Form(schema=ShiftFilter(), request=self.request)
 
         stores = self.get_stores()
         store_values = [(s.uuid, "{} - {}".format(s.id, s.name)) for s in stores]
         store_values.insert(0, ('', "(all)"))
-        form.set_widget('store', forms.widgets.PlainSelectWidget(values=store_values))
+        form.set_widget('store', dfwidget.SelectWidget(values=store_values))
         if context['store']:
             form.set_default('store', context['store'].uuid)
         else:
             # TODO: why is this necessary? somehow the previous store is being
             # preserved as the "default" when switching from single store view
             # to "all stores" view
             form.set_default('store', '')
 
         departments = self.get_departments()
         department_values = [(d.uuid, d.name) for d in departments]
         department_values.insert(0, ('', "(all)"))
-        form.set_widget('department', forms.widgets.PlainSelectWidget(values=department_values))
+        form.set_widget('department', dfwidget.SelectWidget(values=department_values))
         if context['department']:
             form.set_default('department', context['department'].uuid)
         else:
             # TODO: why is this necessary? somehow the previous dept is being
             # preserved as the "default" when switching from single dept view
             # to "all depts" view
             form.set_default('department', '')
@@ -288,21 +291,23 @@
 
     def session_put(self, key, value, mainkey=None):
         if mainkey is None:
             mainkey = self.key
         self.request.session['timesheet.{}.{}'.format(mainkey, key)] = value
 
     def get_stores(self):
+        model = self.model
         return Session.query(model.Store).order_by(model.Store.id).all()
 
     def get_store_options(self, stores):
         options = [tags.Option("{} - {}".format(s.id, s.name), s.uuid) for s in stores]
         return tags.Options(options, prompt="(all)")
 
     def get_departments(self):
+        model = self.model
         return Session.query(model.Department).order_by(model.Department.name).all()
 
     def get_department_options(self, departments):
         options = [tags.Option(d.name, d.uuid) for d in departments]
         return tags.Options(options, prompt="(all)")
 
     def render_full(self, date=None, employees=None, store=None, department=None, form=None, **kwargs):
@@ -398,38 +403,39 @@
 
     def fetch_shift_data(self, cls, employees, weekdays):
         """
         Fetch all shift data of the given model class (``cls``), according to
         the given params.  The cached shift data is attached to each employee.
         """
         app = self.get_rattail_app()
+        model = self.model
 
         # TODO: a bit hacky, this?  display hours as HH:MM by default, but
         # check config in order to display as HH.HH for certain users
         hours_style = 'pretty'
         if self.request.user:
             hours_style = self.rattail_config.get('tailbone', 'hours_style.{}'.format(self.request.user.username),
                                                   default='pretty')
         if hours_style != 'decimal':
             hours_style = 'pretty'
 
         shift_type = 'scheduled' if cls is model.ScheduledShift else 'worked'
-        min_time = localtime(self.rattail_config, datetime.datetime.combine(weekdays[0], datetime.time(0)))
-        max_time = localtime(self.rattail_config, datetime.datetime.combine(weekdays[-1] + datetime.timedelta(days=1), datetime.time(0)))
+        min_time = app.localtime(datetime.datetime.combine(weekdays[0], datetime.time(0)))
+        max_time = app.localtime(datetime.datetime.combine(weekdays[-1] + datetime.timedelta(days=1), datetime.time(0)))
         shifts = Session.query(cls)\
                         .filter(cls.employee_uuid.in_([e.uuid for e in employees]))\
                         .filter(sa.or_(
                             sa.and_(
-                                cls.start_time >= make_utc(min_time),
-                                cls.start_time < make_utc(max_time),
+                                cls.start_time >= app.make_utc(min_time),
+                                cls.start_time < app.make_utc(max_time),
                             ),
                             sa.and_(
                                 cls.start_time == None,
-                                cls.end_time >= make_utc(min_time),
-                                cls.end_time < make_utc(max_time),
+                                cls.end_time >= app.make_utc(min_time),
+                                cls.end_time < app.make_utc(max_time),
                             )))\
                         .all()
 
         for employee in employees:
             employee_shifts = sorted([s for s in shifts if s.employee_uuid == employee.uuid],
                                      key=lambda s: s.start_time or s.end_time)
             if not hasattr(employee, 'weekdays'):
```

### Comparing `Tailbone-0.9.90/tailbone/views/shifts/schedule.py` & `tailbone-0.9.91/tailbone/views/shifts/schedule.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/shifts/timesheet.py` & `tailbone-0.9.91/tailbone/views/shifts/timesheet.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/stores.py` & `tailbone-0.9.91/tailbone/views/stores.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/subdepartments.py` & `tailbone-0.9.91/tailbone/views/subdepartments.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tables.py` & `tailbone-0.9.91/tailbone/views/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -76,15 +76,15 @@
         'column_name',
         'data_type',
         'nullable',
         'description',
     ]
 
     def __init__(self, request):
-        super(TableView, self).__init__(request)
+        super().__init__(request)
         app = self.get_rattail_app()
         self.db_handler = app.get_db_handler()
 
     def get_data(self, **kwargs):
         """
         Fetch existing table names and estimate row counts via PG SQL
         """
@@ -98,27 +98,27 @@
         order by n_live_tup desc;
         """
         result = self.Session.execute(sa.text(sql))
         return [dict(table_name=row.relname, row_count=row.n_live_tup)
                 for row in result]
 
     def configure_grid(self, g):
-        super(TableView, self).configure_grid(g)
+        super().configure_grid(g)
 
         # table_name
         g.sorters['table_name'] = g.make_simple_sorter('table_name', foldcase=True)
         g.set_sort_defaults('table_name')
         g.set_searchable('table_name')
         g.set_link('table_name')
 
         # row_count
         g.sorters['row_count'] = g.make_simple_sorter('row_count')
 
     def configure_form(self, f):
-        super(TableView, self).configure_form(f)
+        super().configure_form(f)
 
         # TODO: should render this instead, by inspecting table
         if not self.creating:
             f.remove('versioned')
 
     def get_instance(self):
         model = self.model
@@ -165,36 +165,36 @@
     def get_instance_title(self, table):
         return table['table_name']
 
     def make_form_schema(self):
         return TableSchema()
 
     def get_xref_buttons(self, table):
-        buttons = super(TableView, self).get_xref_buttons(table)
+        buttons = super().get_xref_buttons(table)
 
         if table.get('model_name'):
             all_views = self.request.registry.settings['tailbone_model_views']
             model_views = all_views.get(table['model_name'], [])
             for view in model_views:
                 url = self.request.route_url(view['route_prefix'])
                 buttons.append(self.make_xref_button(url=url, text=view['label'],
                                                      internal=True))
 
             if self.request.has_perm('model_views.create'):
                 url = self.request.route_url('model_views.create',
                                              _query={'model_name': table['model_name']})
-                buttons.append(self.make_buefy_button("New View",
-                                                      is_primary=True,
-                                                      url=url,
-                                                      icon_left='plus'))
+                buttons.append(self.make_button("New View",
+                                                is_primary=True,
+                                                url=url,
+                                                icon_left='plus'))
 
         return buttons
 
     def template_kwargs_create(self, **kwargs):
-        kwargs = super(TableView, self).template_kwargs_create(**kwargs)
+        kwargs = super().template_kwargs_create(**kwargs)
         app = self.get_rattail_app()
         model = self.model
 
         kwargs['alembic_current_head'] = self.db_handler.check_alembic_current_head()
 
         kwargs['branch_name_options'] = self.db_handler.get_alembic_branch_names()
 
@@ -297,15 +297,15 @@
                 'data_type': str(repr(column.type)),
                 'nullable': column.nullable,
                 'description': column.doc,
             })
         return data
 
     def configure_row_grid(self, g):
-        super(TableView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
 
         g.sorters['sequence'] = g.make_simple_sorter('sequence')
         g.set_sort_defaults('sequence')
         g.set_label('sequence', "Seq.")
 
         g.sorters['column_name'] = g.make_simple_sorter('column_name',
                                                         foldcase=True)
@@ -415,15 +415,15 @@
 
 
 class TablesView(TableView):
 
     def __init__(self, request):
         warnings.warn("TablesView is deprecated; please use TableView instead",
                       DeprecationWarning, stacklevel=2)
-        super(TablesView, self).__init__(request)
+        super().__init__(request)
 
 
 class TableSchema(colander.Schema):
 
     table_name = colander.SchemaNode(colander.String())
 
     row_count = colander.SchemaNode(colander.Integer(),
```

### Comparing `Tailbone-0.9.90/tailbone/views/taxes.py` & `tailbone-0.9.91/tailbone/views/taxes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/__init__.py` & `tailbone-0.9.91/tailbone/views/tempmon/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/appliances.py` & `tailbone-0.9.91/tailbone/views/tempmon/appliances.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/clients.py` & `tailbone-0.9.91/tailbone/views/tempmon/clients.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/core.py` & `tailbone-0.9.91/tailbone/views/tempmon/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -94,8 +94,8 @@
                 'good_temp_max': "Good Max",
                 'critical_temp_max': "Crit. Max",
             },
             linked_columns=['description'],
             main_actions=actions,
         )
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='probesData'))
+            g.render_table_element(data_prop='probesData'))
```

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/dashboard.py` & `tailbone-0.9.91/tailbone/views/tempmon/dashboard.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/probes.py` & `tailbone-0.9.91/tailbone/views/tempmon/probes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tempmon/readings.py` & `tailbone-0.9.91/tailbone/views/tempmon/readings.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/tenders.py` & `tailbone-0.9.91/tailbone/views/tenders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/trainwreck/__init__.py` & `tailbone-0.9.91/tailbone/views/trainwreck/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/trainwreck/base.py` & `tailbone-0.9.91/tailbone/views/trainwreck/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -198,15 +198,15 @@
         g.set_link('total')
 
     def grid_extra_class(self, transaction, i):
         if transaction.void:
             return 'warning'
 
     def configure_form(self, f):
-        super(TransactionView, self).configure_form(f)
+        super().configure_form(f)
 
         # system
         f.set_enum('system', self.enum.TRAINWRECK_SYSTEM)
 
         # currency fields
         f.set_type('subtotal', 'currency')
         f.set_type('discounted_subtotal', 'currency')
@@ -236,18 +236,18 @@
         g = factory(
             key='{}.custorder_xref_markers'.format(route_prefix),
             data=[],
             columns=['custorder_xref', 'custorder_item_xref'],
             request=self.request)
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='custorderXrefMarkersData'))
+            g.render_table_element(data_prop='custorderXrefMarkersData'))
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(TransactionView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
 
         form = kwargs['form']
         if 'custorder_xref_markers' in form:
             txn = kwargs['instance']
             markers = []
             for marker in txn.custorder_xref_markers:
                 markers.append({
@@ -262,15 +262,15 @@
         return self.Session.query(self.model_row_class)\
                            .filter(self.model_row_class.transaction == transaction)
 
     def get_parent(self, item):
         return item.transaction
 
     def configure_row_grid(self, g):
-        super(TransactionView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
         g.set_sort_defaults('sequence')
 
         g.set_type('unit_quantity', 'quantity')
         g.set_type('subtotal', 'currency')
         g.set_type('discounted_subtotal', 'currency')
         g.set_type('tax', 'currency')
         g.set_type('total', 'currency')
@@ -282,15 +282,15 @@
         if row.void:
             return 'warning'
 
     def get_row_instance_title(self, instance):
         return "Trainwreck Line Item"
 
     def configure_row_form(self, f):
-        super(TransactionView, self).configure_row_form(f)
+        super().configure_row_form(f)
 
         # transaction
         f.set_renderer('transaction', self.render_transaction)
 
         # quantity fields
         f.set_type('unit_quantity', 'quantity')
 
@@ -321,15 +321,15 @@
             key='{}.discounts'.format(route_prefix),
             data=[],
             columns=['discount_type', 'description', 'amount'],
             labels={'discount_type': "Type"},
             request=self.request)
 
         return HTML.literal(
-            g.render_buefy_table_element(data_prop='discountsData'))
+            g.render_table_element(data_prop='discountsData'))
 
     def template_kwargs_view_row(self, **kwargs):
         form = kwargs['form']
         if 'discounts' in form:
 
             app = self.get_rattail_app()
             item = kwargs['instance']
@@ -397,29 +397,29 @@
             {'section': 'trainwreck',
              'option': 'current_years',
              'type': int},
 
         ]
 
     def configure_get_context(self):
-        context = super(TransactionView, self).configure_get_context()
+        context = super().configure_get_context()
 
         app = self.get_rattail_app()
         trainwreck_handler = app.get_trainwreck_handler()
         trainwreck_engines = trainwreck_handler.get_trainwreck_engines()
 
         context['trainwreck_engines'] = trainwreck_engines
         context['hidden_databases'] = dict([
             (key, trainwreck_handler.engine_is_hidden(key))
             for key in trainwreck_engines])
 
         return context
 
     def configure_gather_settings(self, data):
-        settings = super(TransactionView, self).configure_gather_settings(data)
+        settings = super().configure_gather_settings(data)
 
         app = self.get_rattail_app()
         trainwreck_handler = app.get_trainwreck_handler()
         trainwreck_engines = trainwreck_handler.get_trainwreck_engines()
 
         hidden = []
         for key in trainwreck_engines:
@@ -428,15 +428,15 @@
                 hidden.append(key)
         settings.append({'name': 'trainwreck.db.hide',
                          'value': ', '.join(hidden)})
 
         return settings
 
     def configure_remove_settings(self):
-        super(TransactionView, self).configure_remove_settings()
+        super().configure_remove_settings()
         app = self.get_rattail_app()
 
         names = [
             'trainwreck.db.hide',
             'tailbone.engines.trainwreck.hidden', # deprecated
         ]
```

### Comparing `Tailbone-0.9.90/tailbone/views/trainwreck/defaults.py` & `tailbone-0.9.91/tailbone/views/trainwreck/defaults.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/typical.py` & `tailbone-0.9.91/tailbone/views/typical.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/uoms.py` & `tailbone-0.9.91/tailbone/views/uoms.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/upgrades.py` & `tailbone-0.9.91/tailbone/views/upgrades.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -29,17 +29,15 @@
 import re
 import logging
 import warnings
 from collections import OrderedDict
 
 import sqlalchemy as sa
 
-from rattail.core import Object
-from rattail.db import model, Session as RattailSession
-from rattail.time import make_utc
+from rattail.db.model import Upgrade
 from rattail.threads import Thread
 
 from deform import widget as dfwidget
 from webhelpers2.html import tags, HTML
 
 from tailbone.views import MasterView
 from tailbone.progress import get_progress_session #, SessionProgress
@@ -49,15 +47,15 @@
 log = logging.getLogger(__name__)
 
 
 class UpgradeView(MasterView):
     """
     Master view for all user events
     """
-    model_class = model.Upgrade
+    model_class = Upgrade
     downloadable = True
     cloneable = True
     configurable = True
     executable = True
     execute_progress_template = '/upgrade.mako'
     execute_progress_initial_msg = "Upgrading"
     execute_can_cancel = False
@@ -96,15 +94,15 @@
         'stdout_file',
         'stderr_file',
         'exit_code',
         'package_diff',
     ]
 
     def __init__(self, request):
-        super(UpgradeView, self).__init__(request)
+        super().__init__(request)
 
         if hasattr(self, 'get_handler'):
             warnings.warn("defining get_handler() is deprecated.  please "
                           "override AppHandler.get_upgrade_handler() instead",
                           DeprecationWarning, stacklevel=2)
             self.upgrade_handler = self.get_handler()
 
@@ -116,15 +114,16 @@
     def handler(self):
         warnings.warn("handler attribute is deprecated; "
                       "please use upgrade_handler instead",
                       DeprecationWarning, stacklevel=2)
         return self.upgrade_handler
 
     def configure_grid(self, g):
-        super(UpgradeView, self).configure_grid(g)
+        super().configure_grid(g)
+        model = self.model
 
         # system
         systems = self.upgrade_handler.get_all_systems()
         systems_enum = dict([(s['key'], s['label']) for s in systems])
         g.set_enum('system', systems_enum)
 
         g.set_joiner('executed_by', lambda q: q.join(model.User, model.User.uuid == model.Upgrade.executed_by_uuid).outerjoin(model.Person))
@@ -143,15 +142,16 @@
     def grid_extra_class(self, upgrade, i):
         if upgrade.status_code == self.enum.UPGRADE_STATUS_FAILED:
             return 'warning'
         if upgrade.status_code == self.enum.UPGRADE_STATUS_EXECUTING:
             return 'notice'
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(UpgradeView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
+        model = self.model
         upgrade = kwargs['instance']
 
         kwargs['system_title'] = self.rattail_config.app_title()
         if upgrade.system:
             system = self.upgrade_handler.get_system(upgrade.system)
             if system:
                 kwargs['system_title'] = system['label']
@@ -173,15 +173,15 @@
             kwargs['prev_url'] = self.get_action_url('view', older)
         if newer:
             kwargs['next_url'] = self.get_action_url('view', newer)
 
         return kwargs
 
     def configure_form(self, f):
-        super(UpgradeView, self).configure_form(f)
+        super().configure_form(f)
         upgrade = f.model_instance
 
         # system
         systems = self.upgrade_handler.get_all_systems()
         systems_enum = OrderedDict([(s['key'], s['label'])
                                     for s in systems])
         f.set_enum('system', systems_enum)
@@ -271,17 +271,18 @@
         # just show status per normal
         return text
 
     def configure_clone_form(self, f):
         f.fields = ['system', 'description', 'notes', 'enabled']
 
     def clone_instance(self, original):
+        app = self.get_rattail_app()
         cloned = self.model_class()
         cloned.system = original.system
-        cloned.created = make_utc()
+        cloned.created = app.make_utc()
         cloned.created_by = self.request.user
         cloned.description = original.description
         cloned.notes = original.notes
         cloned.status_code = self.enum.UPGRADE_STATUS_PENDING
         cloned.enabled = original.enabled
         self.Session.add(cloned)
         self.Session.flush()
@@ -331,15 +332,14 @@
             return HTML.tag('div', c=[showing + diff.render_html()])
 
         except:
             log.debug("failed to render package diff for upgrade: {}".format(upgrade), exc_info=True)
             return HTML.tag('div', c="(not available for this upgrade)")
 
     def get_extra_diff_row_attrs(self, field, attrs):
-        # note, this is only needed/used with Buefy
         extra = {}
         if attrs.get('class') != 'diff':
             extra['v-show'] = "showingPackages == 'all'"
         return extra
 
     def changelog_link(self, project, url):
         return tags.link_to(project, url, target='_blank')
@@ -445,21 +445,22 @@
                     if req:
                         packages[req.name] = req.version
                     else:
                         log.warning("could not parse req from line: %s", line)
         return packages
 
     def parse_requirement(self, line):
+        app = self.get_rattail_app()
         match = re.match(r'^.*@(.*)#egg=(.*)$', line)
         if match:
-            return Object(name=match.group(2), version=match.group(1))
+            return app.make_object(name=match.group(2), version=match.group(1))
 
         match = re.match(r'^(.*)==(.*)$', line)
         if match:
-            return Object(name=match.group(1), version=match.group(2))
+            return app.make_object(name=match.group(1), version=match.group(2))
 
     def download_path(self, upgrade, filename):
         return self.rattail_config.upgrade_filepath(upgrade.uuid, filename=filename)
 
     def download_content_type(self, path, filename):
         return 'text/plain'
 
@@ -533,25 +534,25 @@
             self.request.session.flash("Upgrade was not currently executing!  "
                                        "So it was not declared a failure.",
                                        'error')
         return self.redirect(self.get_action_url('view', upgrade))
 
     def delete_instance(self, upgrade):
         self.handler.delete_files(upgrade)
-        super(UpgradeView, self).delete_instance(upgrade)
+        super().delete_instance(upgrade)
 
     def configure_get_context(self, **kwargs):
-        context = super(UpgradeView, self).configure_get_context(**kwargs)
+        context = super().configure_get_context(**kwargs)
 
         context['upgrade_systems'] = self.upgrade_handler.get_all_systems()
 
         return context
 
     def configure_gather_settings(self, data):
-        settings = super(UpgradeView, self).configure_gather_settings(data)
+        settings = super().configure_gather_settings(data)
 
         keys = []
         for system in json.loads(data['upgrade_systems']):
             key = system['key']
             if key == 'rattail':
                 settings.append({'name': 'rattail.upgrades.command',
                                  'value': system['command']})
@@ -564,15 +565,15 @@
         if keys:
             settings.append({'name': 'rattail.upgrades.systems',
                              'value': ', '.join(keys)})
 
         return settings
 
     def configure_remove_settings(self):
-        super(UpgradeView, self).configure_remove_settings()
+        super().configure_remove_settings()
         app = self.get_rattail_app()
         model = self.model
 
         to_delete = self.Session.query(model.Setting)\
                            .filter(sa.or_(
                                model.Setting.name == 'rattail.upgrades.command',
                                model.Setting.name == 'rattail.upgrades.systems',
```

### Comparing `Tailbone-0.9.90/tailbone/views/users.py` & `tailbone-0.9.91/tailbone/views/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -80,33 +80,33 @@
 
     row_grid_columns = [
         'type_code',
         'occurred',
     ]
 
     def __init__(self, request):
-        super(UserView, self).__init__(request)
+        super().__init__(request)
         app = self.get_rattail_app()
 
         # always get a reference to the auth/merge handler
         self.auth_handler = app.get_auth_handler()
         self.merge_handler = self.auth_handler
 
     def query(self, session):
-        query = super(UserView, self).query(session)
+        query = super().query(session)
         model = self.model
 
         # bring in the related Person(s)
         query = query.outerjoin(model.Person)\
                      .options(orm.joinedload(model.User.person))
 
         return query
 
     def configure_grid(self, g):
-        super(UserView, self).configure_grid(g)
+        super().configure_grid(g)
         model = self.model
 
         del g.filters['salt']
         g.filters['username'].default_active = True
         g.filters['username'].default_verb = 'contains'
         g.filters['active'].default_active = True
         g.filters['active'].default_verb = 'is_true'
@@ -173,15 +173,15 @@
         if value:
             model = self.model
             person = self.Session.get(model.Person, value)
             if not person:
                 raise colander.Invalid(node, "Person not found (you must *select* a record)")
 
     def configure_form(self, f):
-        super(UserView, self).configure_form(f)
+        super().configure_form(f)
         model = self.model
         user = f.model_instance
 
         # username
         f.set_validator('username', self.unique_username)
 
         # person
@@ -286,20 +286,20 @@
             key='{}.api_tokens'.format(route_prefix),
             data=[],
             columns=['description', 'created'],
             main_actions=[
                 self.make_action('delete', icon='trash',
                                  click_handler="$emit('api-token-delete', props.row)")])
 
-        button = self.make_buefy_button("New", is_primary=True,
-                                        icon_left='plus',
-                                        **{'@click': "$emit('api-new-token')"})
+        button = self.make_button("New", is_primary=True,
+                                  icon_left='plus',
+                                  **{'@click': "$emit('api-new-token')"})
 
         table = HTML.literal(
-            g.render_buefy_table_element(data_prop='apiTokens'))
+            g.render_table_element(data_prop='apiTokens'))
 
         return HTML.tag('div', c=[button, table])
 
     def add_api_token(self):
         user = self.get_instance()
         data = self.request.json_body
 
@@ -325,15 +325,15 @@
         self.auth_handler.delete_api_token(token)
         self.Session.flush()
 
         return {'ok': True,
                 'tokens': self.get_api_tokens(user)}
 
     def template_kwargs_view(self, **kwargs):
-        kwargs = super(UserView, self).template_kwargs_view(**kwargs)
+        kwargs = super().template_kwargs_view(**kwargs)
         user = kwargs['instance']
 
         kwargs['api_tokens_data'] = self.get_api_tokens(user)
 
         return kwargs
 
     def get_api_tokens(self, user):
@@ -373,15 +373,15 @@
 
     def objectify(self, form, data=None):
         model = self.model
 
         # create/update user as per normal
         if data is None:
             data = form.validated
-        user = super(UserView, self).objectify(form, data)
+        user = super().objectify(form, data)
 
         # create/update person as needed
         names = {}
         if 'first_name_' in form and data['first_name_']:
             names['first'] = data['first_name_']
         if 'last_name_' in form and data['last_name_']:
             names['last'] = data['last_name_']
@@ -483,15 +483,15 @@
 
     def get_row_data(self, user):
         model = self.model
         return self.Session.query(model.UserEvent)\
                            .filter(model.UserEvent.user == user)
 
     def configure_row_grid(self, g):
-        super(UserView, self).configure_row_grid(g)
+        super().configure_row_grid(g)
         g.width = 'half'
         g.filterable = False
         g.set_sort_defaults('occurred', 'desc')
         g.set_enum('type_code', self.enum.USER_EVENT)
         g.set_label('type_code', "Event Type")
         g.main_actions = []
 
@@ -584,15 +584,15 @@
         styles = self.rattail_config.getlist('tailbone', 'themes.styles',
                                              default=[])
         for name in styles:
             css = self.rattail_config.get('tailbone',
                                           'themes.style.{}'.format(name))
             if css:
                 options.append({'value': css, 'label': name})
-        context['buefy_css_options'] = options
+        context['theme_style_options'] = options
 
         return context
 
     def preferences_get_simple_settings(self, user):
         """
         This method is conceptually the same as for
         :meth:`~tailbone.views.master.MasterView.configure_get_simple_settings()`.
@@ -695,20 +695,20 @@
         'user',
         'person',
         'type_code',
         'occurred',
     ]
 
     def get_data(self, session=None):
-        query = super(UserEventView, self).get_data(session=session)
+        query = super().get_data(session=session)
         model = self.model
         return query.join(model.User)
 
     def configure_grid(self, g):
-        super(UserEventView, self).configure_grid(g)
+        super().configure_grid(g)
         model = self.model
         g.set_joiner('person', lambda q: q.outerjoin(model.Person))
         g.set_sorter('user', model.User.username)
         g.set_sorter('person', model.Person.display_name)
         g.filters['user'] = g.make_filter('user', model.User.username)
         g.filters['person'] = g.make_filter('person', model.Person.display_name)
         g.set_enum('type_code', self.enum.USER_EVENT)
```

### Comparing `Tailbone-0.9.90/tailbone/views/vendors/__init__.py` & `tailbone-0.9.91/tailbone/views/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/vendors/catalogs.py` & `tailbone-0.9.91/tailbone/views/vendors/catalogs.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/vendors/core.py` & `tailbone-0.9.91/tailbone/views/vendors/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/vendors/invoices.py` & `tailbone-0.9.91/tailbone/views/vendors/invoices.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/vendors/samplefiles.py` & `tailbone-0.9.91/tailbone/views/vendors/samplefiles.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/versions.py` & `tailbone-0.9.91/tailbone/views/versions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/views.py` & `tailbone-0.9.91/tailbone/views/views.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/views/workorders.py` & `tailbone-0.9.91/tailbone/views/workorders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tailbone/webapi.py` & `tailbone-0.9.91/tailbone/webapi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.90/tasks.py` & `tailbone-0.9.91/tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2022 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,16 +20,14 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 Tasks for Tailbone
 """
 
-from __future__ import unicode_literals, absolute_import
-
 import os
 import shutil
 
 from invoke import task
 
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -43,8 +41,8 @@
     """
     if tests:
         c.run('tox')
 
     if os.path.exists('Tailbone.egg-info'):
         shutil.rmtree('Tailbone.egg-info')
     c.run('python -m build --sdist')
-    c.run('twine upload dist/Tailbone-{}.tar.gz'.format(__version__))
+    c.run(f'twine upload dist/tailbone-{__version__}.tar.gz')
```

### Comparing `Tailbone-0.9.90/tests/test_app.py` & `tailbone-0.9.91/tests/test_app.py`

 * *Files identical despite different names*

