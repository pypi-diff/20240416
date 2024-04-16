# Comparing `tmp/bw2ui-0.8.tar.gz` & `tmp/bw2ui-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bw2ui-0.8.tar", last modified: Thu Oct 17 15:49:17 2013, max compression
+gzip compressed data, was "dist/bw2ui-0.8.1.tar", last modified: Thu Oct 31 07:57:09 2013, max compression
```

## Comparing `bw2ui-0.8.tar` & `bw2ui-0.8.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/
--rw-r--r--   0 cmutel     (501) staff       (20)       90 2013-10-17 15:48:21.000000 bw2ui-0.8/bw2ui/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)      883 2013-10-15 12:20:03.000000 bw2ui-0.8/bw2ui/bin/bw2-controller.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2063 2013-05-08 14:39:18.000000 bw2ui-0.8/bw2ui/bin/bw2-web.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4420 2013-10-15 13:02:20.000000 bw2ui-0.8/bw2ui/controller.py
--rw-r--r--   0 cmutel     (501) staff       (20)       94 2013-02-08 17:22:04.000000 bw2ui-0.8/bw2ui/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)      168 2013-02-08 15:40:58.000000 bw2ui-0.8/bw2ui/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/
--rw-r--r--   0 cmutel     (501) staff       (20)       33 2012-11-12 08:36:35.000000 bw2ui-0.8/bw2ui/web/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13848 2013-10-16 12:42:26.000000 bw2ui-0.8/bw2ui/web/app.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1095 2012-12-17 18:08:27.000000 bw2ui-0.8/bw2ui/web/gzip_response.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2401 2012-11-22 10:35:41.000000 bw2ui-0.8/bw2ui/web/jobs.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/backgrid/
--rw-r--r--   0 cmutel     (501) staff       (20)     1281 2013-10-16 10:00:59.000000 bw2ui-0.8/bw2ui/web/static/backgrid/backgrid-table.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5519 2013-10-15 22:03:34.000000 bw2ui-0.8/bw2ui/web/static/backgrid/backgrid.css
--rw-r--r--   0 cmutel     (501) staff       (20)    85087 2013-10-16 09:34:42.000000 bw2ui-0.8/bw2ui/web/static/backgrid/backgrid.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/
--rw-r--r--   0 cmutel     (501) staff       (20)     1938 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/ie.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/
--rwxr-xr-x   0 cmutel     (501) staff       (20)      655 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/cross.png
--rwxr-xr-x   0 cmutel     (501) staff       (20)      455 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/key.png
--rwxr-xr-x   0 cmutel     (501) staff       (20)      537 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/tick.png
--rw-r--r--   0 cmutel     (501) staff       (20)     2004 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/screen.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/fancy-type/
--rw-r--r--   0 cmutel     (501) staff       (20)     2244 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/fancy-type/screen.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/
--rw-r--r--   0 cmutel     (501) staff       (20)      777 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/doc.png
--rw-r--r--   0 cmutel     (501) staff       (20)      641 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/email.png
--rw-r--r--   0 cmutel     (501) staff       (20)    46848 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/external.png
--rw-r--r--   0 cmutel     (501) staff       (20)      691 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/feed.png
--rw-r--r--   0 cmutel     (501) staff       (20)      741 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/im.png
--rw-r--r--   0 cmutel     (501) staff       (20)      749 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/lock.png
--rw-r--r--   0 cmutel     (501) staff       (20)      591 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/pdf.png
--rw-r--r--   0 cmutel     (501) staff       (20)    46990 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/visited.png
--rw-r--r--   0 cmutel     (501) staff       (20)      663 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/xls.png
--rw-r--r--   0 cmutel     (501) staff       (20)     1458 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/screen.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/rtl/
--rw-r--r--   0 cmutel     (501) staff       (20)     4839 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/plugins/rtl/screen.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1286 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/print.css
--rw-r--r--   0 cmutel     (501) staff       (20)    12336 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/screen.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/
--rw-r--r--   0 cmutel     (501) staff       (20)     2686 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/forms.css
--rwxr-xr-x   0 cmutel     (501) staff       (20)     9518 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/grid.css
--rw-r--r--   0 cmutel     (501) staff       (20)      104 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/grid.png
--rw-r--r--   0 cmutel     (501) staff       (20)     2669 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/ie.css
--rwxr-xr-x   0 cmutel     (501) staff       (20)     2157 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/print.css
--rwxr-xr-x   0 cmutel     (501) staff       (20)     1577 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/reset.css
--rw-r--r--   0 cmutel     (501) staff       (20)     3638 2011-06-06 16:04:52.000000 bw2ui-0.8/bw2ui/web/static/blueprint/src/typography.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/css/
--rw-r--r--   0 cmutel     (501) staff       (20)     1338 2013-01-29 07:39:53.000000 bw2ui-0.8/bw2ui/web/static/css/base.css
--rw-r--r--   0 cmutel     (501) staff       (20)       62 2012-12-19 21:42:11.000000 bw2ui-0.8/bw2ui/web/static/css/index.css
--rw-r--r--   0 cmutel     (501) staff       (20)      454 2013-10-13 14:36:38.000000 bw2ui-0.8/bw2ui/web/static/css/treemap.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/d3-tip/
--rw-r--r--   0 cmutel     (501) staff       (20)      180 2013-10-13 14:34:06.000000 bw2ui-0.8/bw2ui/web/static/d3-tip/d3-tip.css
--rw-r--r--   0 cmutel     (501) staff       (20)     6747 2013-10-13 14:34:22.000000 bw2ui-0.8/bw2ui/web/static/d3-tip/d3-tip.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/img/
--rw-r--r--   0 cmutel     (501) staff       (20)     1406 2012-12-18 10:45:15.000000 bw2ui-0.8/bw2ui/web/static/img/favicon.ico
--rw-r--r--   0 cmutel     (501) staff       (20)    77595 2012-11-20 19:07:57.000000 bw2ui-0.8/bw2ui/web/static/img/linedpaper.png
--rw-r--r--   0 cmutel     (501) staff       (20)    10381 2012-11-16 11:42:35.000000 bw2ui-0.8/bw2ui/web/static/img/llama.jpg
--rw-r--r--   0 cmutel     (501) staff       (20)    19939 2012-11-16 11:18:32.000000 bw2ui-0.8/bw2ui/web/static/img/monster.jpg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/
--rw-r--r--   0 cmutel     (501) staff       (20)      464 2006-03-12 22:48:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/application.png
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/code.png
--rw-r--r--   0 cmutel     (501) staff       (20)      618 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/css.png
--rw-r--r--   0 cmutel     (501) staff       (20)      579 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/db.png
--rw-r--r--   0 cmutel     (501) staff       (20)      537 2006-03-12 21:53:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/directory.png
--rw-r--r--   0 cmutel     (501) staff       (20)      651 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/doc.png
--rw-r--r--   0 cmutel     (501) staff       (20)      294 2006-03-12 21:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/file.png
--rw-r--r--   0 cmutel     (501) staff       (20)      653 2006-03-12 22:52:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/film.png
--rw-r--r--   0 cmutel     (501) staff       (20)      582 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/flash.png
--rw-r--r--   0 cmutel     (501) staff       (20)      583 2008-03-17 22:29:50.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/folder_open.png
--rw-r--r--   0 cmutel     (501) staff       (20)      734 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/html.png
--rw-r--r--   0 cmutel     (501) staff       (20)      633 2006-03-12 22:51:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/java.png
--rw-r--r--   0 cmutel     (501) staff       (20)      668 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/linux.png
--rw-r--r--   0 cmutel     (501) staff       (20)      385 2006-03-12 22:54:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/music.png
--rw-r--r--   0 cmutel     (501) staff       (20)      591 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/pdf.png
--rw-r--r--   0 cmutel     (501) staff       (20)      538 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/php.png
--rw-r--r--   0 cmutel     (501) staff       (20)      606 2006-03-12 22:56:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/picture.png
--rw-r--r--   0 cmutel     (501) staff       (20)      588 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/ppt.png
--rw-r--r--   0 cmutel     (501) staff       (20)      856 2006-03-12 22:56:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/psd.png
--rw-r--r--   0 cmutel     (501) staff       (20)      626 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/ruby.png
--rw-r--r--   0 cmutel     (501) staff       (20)      859 2006-03-12 22:56:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/script.png
--rw-r--r--   0 cmutel     (501) staff       (20)     2530 2008-03-24 16:58:44.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/spinner.gif
--rw-r--r--   0 cmutel     (501) staff       (20)      342 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/txt.png
--rw-r--r--   0 cmutel     (501) staff       (20)      663 2006-03-12 22:55:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/xls.png
--rw-r--r--   0 cmutel     (501) staff       (20)      386 2006-03-12 22:56:00.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/zip.png
--rw-r--r--   0 cmutel     (501) staff       (20)     5787 2008-03-24 16:58:52.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4003 2013-01-10 10:33:37.000000 bw2ui-0.8/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/js/
--rw-r--r--   0 cmutel     (501) staff       (20)     2352 2013-02-13 20:30:00.000000 bw2ui-0.8/bw2ui/web/static/js/force-directed.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3178 2012-12-02 10:32:00.000000 bw2ui-0.8/bw2ui/web/static/js/hinton.js
--rw-r--r--   0 cmutel     (501) staff       (20)     2643 2012-12-02 11:51:22.000000 bw2ui-0.8/bw2ui/web/static/js/interp-histogram.js
--rw-r--r--   0 cmutel     (501) staff       (20)     2912 2013-02-14 14:13:50.000000 bw2ui-0.8/bw2ui/web/static/js/stepped-histogram.js
--rw-r--r--   0 cmutel     (501) staff       (20)     9005 2013-10-13 14:37:14.000000 bw2ui-0.8/bw2ui/web/static/js/treemap.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/
--rw-r--r--   0 cmutel     (501) staff       (20)   282978 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/ace.js
--rw-r--r--   0 cmutel     (501) staff       (20)    14438 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor-icons.png
--rw-r--r--   0 cmutel     (501) staff       (20)    66014 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor-min.js
--rw-r--r--   0 cmutel     (501) staff       (20)    13199 2013-09-14 08:26:07.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor.css
--rw-r--r--   0 cmutel     (501) staff       (20)    16189 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/jsonlint.js
--rw-r--r--   0 cmutel     (501) staff       (20)     9125 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/mode-json.js
--rw-r--r--   0 cmutel     (501) staff       (20)     4621 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/theme-jsoneditor.js
--rw-r--r--   0 cmutel     (501) staff       (20)     4735 2013-09-13 19:47:14.000000 bw2ui-0.8/bw2ui/web/static/jsoneditor/theme-textmate.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui/web/templates/
--rw-r--r--   0 cmutel     (501) staff       (20)      469 2012-11-20 17:10:06.000000 bw2ui-0.8/bw2ui/web/templates/404.html
--rw-r--r--   0 cmutel     (501) staff       (20)      444 2012-11-20 17:22:13.000000 bw2ui-0.8/bw2ui/web/templates/500.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2464 2013-10-16 09:23:29.000000 bw2ui-0.8/bw2ui/web/templates/base.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1019 2013-10-16 10:40:36.000000 bw2ui-0.8/bw2ui/web/templates/database.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1460 2012-11-26 18:05:43.000000 bw2ui-0.8/bw2ui/web/templates/database_tree.html
--rw-r--r--   0 cmutel     (501) staff       (20)      756 2013-02-19 11:44:22.000000 bw2ui-0.8/bw2ui/web/templates/edit-raw.html
--rw-r--r--   0 cmutel     (501) staff       (20)      237 2013-01-10 10:38:15.000000 bw2ui-0.8/bw2ui/web/templates/fp-select.html
--rw-r--r--   0 cmutel     (501) staff       (20)      914 2013-01-10 10:39:47.000000 bw2ui-0.8/bw2ui/web/templates/fp.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3645 2012-11-22 10:51:00.000000 bw2ui-0.8/bw2ui/web/templates/hist.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2390 2013-01-29 08:23:26.000000 bw2ui-0.8/bw2ui/web/templates/import-database.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2199 2013-01-11 10:50:18.000000 bw2ui-0.8/bw2ui/web/templates/import-method.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2032 2013-10-16 10:13:39.000000 bw2ui-0.8/bw2ui/web/templates/index.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1900 2013-10-16 12:54:46.000000 bw2ui-0.8/bw2ui/web/templates/jsoneditor.html
--rw-r--r--   0 cmutel     (501) staff       (20)      899 2013-10-16 12:40:00.000000 bw2ui-0.8/bw2ui/web/templates/method.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1500 2012-11-21 10:32:54.000000 bw2ui-0.8/bw2ui/web/templates/progress.html
--rw-r--r--   0 cmutel     (501) staff       (20)     6003 2013-02-14 22:08:15.000000 bw2ui-0.8/bw2ui/web/templates/report.html
--rw-r--r--   0 cmutel     (501) staff       (20)     5324 2013-01-29 10:19:39.000000 bw2ui-0.8/bw2ui/web/templates/select.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2371 2013-03-20 08:59:38.000000 bw2ui-0.8/bw2ui/web/templates/settings.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3422 2013-10-17 15:42:49.000000 bw2ui-0.8/bw2ui/web/templates/start.html
--rw-r--r--   0 cmutel     (501) staff       (20)      474 2012-11-22 15:51:02.000000 bw2ui-0.8/bw2ui/web/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-17 15:49:17.000000 bw2ui-0.8/bw2ui.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2013-10-17 15:49:15.000000 bw2ui-0.8/bw2ui.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     2681 2013-10-17 15:49:15.000000 bw2ui-0.8/bw2ui.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2013-10-17 15:49:15.000000 bw2ui-0.8/bw2ui.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     4652 2013-10-17 15:49:15.000000 bw2ui-0.8/bw2ui.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2013-10-17 15:49:15.000000 bw2ui-0.8/bw2ui.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     1492 2013-01-17 20:27:15.000000 bw2ui-0.8/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      300 2013-01-28 17:35:57.000000 bw2ui-0.8/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     2681 2013-10-17 15:49:17.000000 bw2ui-0.8/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      230 2013-02-14 22:25:36.000000 bw2ui-0.8/README.rst
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2013-10-17 15:49:17.000000 bw2ui-0.8/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1839 2013-10-17 15:48:07.000000 bw2ui-0.8/setup.py
--rw-r--r--   0 cmutel     (501) staff       (20)      343 2012-11-10 18:35:22.000000 bw2ui-0.8/TODO.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/
+-rw-r--r--   0 cmutel     (501) staff       (20)       93 2013-10-31 07:55:17.000000 bw2ui-0.8.1/bw2ui/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)      918 2013-10-31 07:45:43.000000 bw2ui-0.8.1/bw2ui/bin/bw2-controller.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2063 2013-05-08 14:39:18.000000 bw2ui-0.8.1/bw2ui/bin/bw2-web.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5059 2013-10-31 07:52:35.000000 bw2ui-0.8.1/bw2ui/controller.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       94 2013-02-08 17:22:04.000000 bw2ui-0.8.1/bw2ui/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      168 2013-02-08 15:40:58.000000 bw2ui-0.8.1/bw2ui/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/
+-rw-r--r--   0 cmutel     (501) staff       (20)       33 2012-11-12 08:36:35.000000 bw2ui-0.8.1/bw2ui/web/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    14003 2013-10-31 07:20:22.000000 bw2ui-0.8.1/bw2ui/web/app.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1095 2012-12-17 18:08:27.000000 bw2ui-0.8.1/bw2ui/web/gzip_response.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2401 2012-11-22 10:35:41.000000 bw2ui-0.8.1/bw2ui/web/jobs.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/backgrid/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1281 2013-10-16 10:00:59.000000 bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid-table.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5519 2013-10-17 16:27:08.000000 bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    85087 2013-10-16 09:34:42.000000 bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1938 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/ie.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/
+-rwxr-xr-x   0 cmutel     (501) staff       (20)      655 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/cross.png
+-rwxr-xr-x   0 cmutel     (501) staff       (20)      455 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/key.png
+-rwxr-xr-x   0 cmutel     (501) staff       (20)      537 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/tick.png
+-rw-r--r--   0 cmutel     (501) staff       (20)     2004 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/screen.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/fancy-type/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2244 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/fancy-type/screen.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/
+-rw-r--r--   0 cmutel     (501) staff       (20)      777 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/doc.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      641 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/email.png
+-rw-r--r--   0 cmutel     (501) staff       (20)    46848 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/external.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      691 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/feed.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      741 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/im.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      749 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/lock.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      591 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/pdf.png
+-rw-r--r--   0 cmutel     (501) staff       (20)    46990 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/visited.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      663 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/xls.png
+-rw-r--r--   0 cmutel     (501) staff       (20)     1458 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/screen.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/rtl/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4839 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/rtl/screen.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1286 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/print.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    12336 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/screen.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2686 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/forms.css
+-rwxr-xr-x   0 cmutel     (501) staff       (20)     9518 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/grid.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      104 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/grid.png
+-rw-r--r--   0 cmutel     (501) staff       (20)     2669 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/ie.css
+-rwxr-xr-x   0 cmutel     (501) staff       (20)     2157 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/print.css
+-rwxr-xr-x   0 cmutel     (501) staff       (20)     1577 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/reset.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     3638 2011-06-06 16:04:52.000000 bw2ui-0.8.1/bw2ui/web/static/blueprint/src/typography.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/css/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1338 2013-01-29 07:39:53.000000 bw2ui-0.8.1/bw2ui/web/static/css/base.css
+-rw-r--r--   0 cmutel     (501) staff       (20)       62 2012-12-19 21:42:11.000000 bw2ui-0.8.1/bw2ui/web/static/css/index.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      454 2013-10-13 14:36:38.000000 bw2ui-0.8.1/bw2ui/web/static/css/treemap.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/d3-tip/
+-rw-r--r--   0 cmutel     (501) staff       (20)      180 2013-10-13 14:34:06.000000 bw2ui-0.8.1/bw2ui/web/static/d3-tip/d3-tip.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     6747 2013-10-13 14:34:22.000000 bw2ui-0.8.1/bw2ui/web/static/d3-tip/d3-tip.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/img/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1406 2012-12-18 10:45:15.000000 bw2ui-0.8.1/bw2ui/web/static/img/favicon.ico
+-rw-r--r--   0 cmutel     (501) staff       (20)    77595 2012-11-20 19:07:57.000000 bw2ui-0.8.1/bw2ui/web/static/img/linedpaper.png
+-rw-r--r--   0 cmutel     (501) staff       (20)    10381 2012-11-16 11:42:35.000000 bw2ui-0.8.1/bw2ui/web/static/img/llama.jpg
+-rw-r--r--   0 cmutel     (501) staff       (20)    19939 2012-11-16 11:18:32.000000 bw2ui-0.8.1/bw2ui/web/static/img/monster.jpg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/
+-rw-r--r--   0 cmutel     (501) staff       (20)      464 2006-03-12 22:48:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/application.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/code.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      618 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/css.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      579 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/db.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      537 2006-03-12 21:53:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/directory.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      651 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/doc.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      294 2006-03-12 21:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/file.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      653 2006-03-12 22:52:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/film.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      582 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/flash.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      583 2008-03-17 22:29:50.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/folder_open.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      734 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/html.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      633 2006-03-12 22:51:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/java.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      668 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/linux.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      385 2006-03-12 22:54:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/music.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      591 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/pdf.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      538 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/php.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      606 2006-03-12 22:56:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/picture.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      588 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/ppt.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      856 2006-03-12 22:56:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/psd.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      626 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/ruby.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      859 2006-03-12 22:56:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/script.png
+-rw-r--r--   0 cmutel     (501) staff       (20)     2530 2008-03-24 16:58:44.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/spinner.gif
+-rw-r--r--   0 cmutel     (501) staff       (20)      342 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/txt.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      663 2006-03-12 22:55:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/xls.png
+-rw-r--r--   0 cmutel     (501) staff       (20)      386 2006-03-12 22:56:00.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/zip.png
+-rw-r--r--   0 cmutel     (501) staff       (20)     5787 2008-03-24 16:58:52.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4003 2013-01-10 10:33:37.000000 bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/js/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2352 2013-02-13 20:30:00.000000 bw2ui-0.8.1/bw2ui/web/static/js/force-directed.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3178 2012-12-02 10:32:00.000000 bw2ui-0.8.1/bw2ui/web/static/js/hinton.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     2643 2012-12-02 11:51:22.000000 bw2ui-0.8.1/bw2ui/web/static/js/interp-histogram.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     2912 2013-02-14 14:13:50.000000 bw2ui-0.8.1/bw2ui/web/static/js/stepped-histogram.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9005 2013-10-13 14:37:14.000000 bw2ui-0.8.1/bw2ui/web/static/js/treemap.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/
+-rw-r--r--   0 cmutel     (501) staff       (20)   282978 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/ace.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    14438 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor-icons.png
+-rw-r--r--   0 cmutel     (501) staff       (20)    66014 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor-min.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    13199 2013-09-14 08:26:07.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    16189 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsonlint.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9125 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/mode-json.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4621 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/theme-jsoneditor.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4735 2013-09-13 19:47:14.000000 bw2ui-0.8.1/bw2ui/web/static/jsoneditor/theme-textmate.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui/web/templates/
+-rw-r--r--   0 cmutel     (501) staff       (20)      469 2012-11-20 17:10:06.000000 bw2ui-0.8.1/bw2ui/web/templates/404.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      444 2012-11-20 17:22:13.000000 bw2ui-0.8.1/bw2ui/web/templates/500.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2464 2013-10-16 09:23:29.000000 bw2ui-0.8.1/bw2ui/web/templates/base.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1019 2013-10-16 10:40:36.000000 bw2ui-0.8.1/bw2ui/web/templates/database.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1460 2012-11-26 18:05:43.000000 bw2ui-0.8.1/bw2ui/web/templates/database_tree.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      756 2013-02-19 11:44:22.000000 bw2ui-0.8.1/bw2ui/web/templates/edit-raw.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      237 2013-01-10 10:38:15.000000 bw2ui-0.8.1/bw2ui/web/templates/fp-select.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      914 2013-01-10 10:39:47.000000 bw2ui-0.8.1/bw2ui/web/templates/fp.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3645 2012-11-22 10:51:00.000000 bw2ui-0.8.1/bw2ui/web/templates/hist.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2999 2013-10-22 15:03:55.000000 bw2ui-0.8.1/bw2ui/web/templates/import-database.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2808 2013-10-22 15:04:03.000000 bw2ui-0.8.1/bw2ui/web/templates/import-method.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2032 2013-10-17 16:26:58.000000 bw2ui-0.8.1/bw2ui/web/templates/index.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1900 2013-10-16 12:54:46.000000 bw2ui-0.8.1/bw2ui/web/templates/jsoneditor.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      899 2013-10-16 12:40:00.000000 bw2ui-0.8.1/bw2ui/web/templates/method.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1500 2012-11-21 10:32:54.000000 bw2ui-0.8.1/bw2ui/web/templates/progress.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     6003 2013-02-14 22:08:15.000000 bw2ui-0.8.1/bw2ui/web/templates/report.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     5324 2013-01-29 10:19:39.000000 bw2ui-0.8.1/bw2ui/web/templates/select.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2371 2013-03-20 08:59:38.000000 bw2ui-0.8.1/bw2ui/web/templates/settings.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3478 2013-10-22 14:48:21.000000 bw2ui-0.8.1/bw2ui/web/templates/start.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      474 2012-11-22 15:51:02.000000 bw2ui-0.8.1/bw2ui/web/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2013-10-31 07:57:09.000000 bw2ui-0.8.1/bw2ui.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2013-10-31 07:57:08.000000 bw2ui-0.8.1/bw2ui.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2683 2013-10-31 07:57:08.000000 bw2ui-0.8.1/bw2ui.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)       16 2013-10-31 07:57:08.000000 bw2ui-0.8.1/bw2ui.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     4652 2013-10-31 07:57:08.000000 bw2ui-0.8.1/bw2ui.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2013-10-31 07:57:08.000000 bw2ui-0.8.1/bw2ui.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     1492 2013-01-17 20:27:15.000000 bw2ui-0.8.1/LICENSE.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      300 2013-01-28 17:35:57.000000 bw2ui-0.8.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     2683 2013-10-31 07:57:09.000000 bw2ui-0.8.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      230 2013-02-14 22:25:36.000000 bw2ui-0.8.1/README.rst
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2013-10-31 07:57:09.000000 bw2ui-0.8.1/setup.cfg
+-rw-r--r--   0 cmutel     (501) staff       (20)     1841 2013-10-31 07:55:27.000000 bw2ui-0.8.1/setup.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      343 2012-11-10 18:35:22.000000 bw2ui-0.8.1/TODO.txt
```

### Comparing `bw2ui-0.8/bw2ui/bin/bw2-controller.py` & `bw2ui-0.8.1/bw2ui/bin/bw2-controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """Brightway2 command line controller.
 
 Usage:
-  bw2-controller.py list [databases|methods]
+  bw2-controller.py list (databases|methods)
   bw2-controller.py details <name>
   bw2-controller.py copy <name> <newname>
   bw2-controller.py backup <name>
   bw2-controller.py validate <name>
   bw2-controller.py versions <name>
   bw2-controller.py revert <name> <revision>
   bw2-controller.py remove <name>
   bw2-controller.py import <path> <name>
   bw2-controller.py export <name> [--include-dependencies]
   bw2-controller.py setup [--data-dir=<datadir>]
   bw2-controller.py upload_logs [COMMENT]
+  bw2-controller.py color (on|off)
 
 Options:
   -h --help     Show this screen.
   --version     Show version.
 
 """
 from docopt import docopt
```

### Comparing `bw2ui-0.8/bw2ui/bin/bw2-web.py` & `bw2ui-0.8.1/bw2ui/bin/bw2-web.py`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/controller.py` & `bw2ui-0.8.1/bw2ui/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,71 @@
 # -*- coding: utf-8 -*-
+from __future__ import print_function
 from brightway2 import databases, methods, Database, config, reset_meta
 from bw2data.io import Ecospold1Importer, download_biosphere, \
-    BW2PackageImporter, BW2PackageExporter
+    BW2PackageImporter, BW2PackageExporter, download_methods
 from bw2data.logs import upload_logs_to_server
-from bw2data.utils import Fore
+from bw2data.colors import Fore, safe_colorama
 from errors import UnknownAction, UnknownDatabase
 import datetime
 import os
 import sys
 
+
+def exit(text):
+    print(safe_colorama(text))
+    sys.exit(1)
+
+
 def strfdelta(tdelta):
     """From http://stackoverflow.com/questions/8906926/formatting-python-timedelta-objects"""
     d = {"days": tdelta.days}
     d["hours"], rem = divmod(tdelta.seconds, 3600)
     d["minutes"], d["seconds"] = divmod(rem, 60)
     fmt = "{days} days {hours}h:{minutes}m:{seconds}s old"
     return fmt.format(**d)
 
 
 class Controller(object):
     def dispatch(self, **kwargs):
         options = ("list", "details", "copy", "backup", "validate", "versions",
-            "revert", "remove", "export", "setup", "upload_logs")
+            "revert", "remove", "export", "setup", "upload_logs", "color")
         for option in options:
             if kwargs[option]:
                 return getattr(self, option)(kwargs)
         if kwargs["import"]:
             return self.importer(kwargs)
         raise UnknownAction("No suitable action found")
 
     def get_name(self, kwargs):
         name = kwargs['<name>']
         if name not in databases:
             raise UnknownDatabase("Can't find the database %s" % name)
         return name
 
+    def color(self, kwargs):
+        if kwargs['on']:
+            if 'no_color' in config.p:
+                del config.p['no_color']
+                config.save_preferences()
+            return u"Color turned on"
+        elif kwargs['off']:
+            config.p['no_color'] = True
+            config.save_preferences()
+            return u"Color turned off"
+        else:
+            return
+
     def list(self, kwargs):
         if kwargs['databases']:
             return databases.list
-        else:
+        elif kwargs['methods']:
             return methods.list
+        else:
+            return
 
     def details(self, kwargs):
         return databases[self.get_name(kwargs)]
 
     def copy(self, kwargs):
         name = self.get_name(kwargs)
         new_name = kwargs['<newname>']
@@ -88,29 +110,30 @@
         path = BW2PackageExporter().export(name, dependencies)
         return u"%s exported to Brightway package: %s" % (name, path)
 
     def setup(self, kwargs):
         if kwargs['--data-dir']:
             data_dir = unicode(kwargs['--data-dir'])
             if os.path.exists(data_dir):
-                sys.exit(Fore.RED + "Error" + Fore.RESET + ": This directory already exists")
+                exit(Fore.RED + "Error" + Fore.RESET + ": This directory already exists")
             elif not os.access(os.path.abspath(os.path.join(data_dir, "..")), os.W_OK):
-                sys.exit(Fore.RED + "Error" + Fore.RESET + ": Given directory is not writable")
+                exit(Fore.RED + "Error" + Fore.RESET + ": Given directory is not writable")
                 return
-            print "\nPlease confirm that you want to create the following data directory:\n\t" + Fore.BLUE + data_dir + Fore.RESET + "\n" + Fore.GREEN + "y" + Fore.RESET + "/" + Fore.RED + "n" + Fore.RESET + " (or any other input):",
-            response = raw_input()
+            question_text = safe_colorama("\nPlease confirm that you want to create the following data directory:\n\t" + Fore.BLUE + data_dir + Fore.RESET + "\n" + Fore.GREEN + "y" + Fore.RESET + "/" + Fore.RED + "n" + Fore.RESET + " (or any other input):")
+            response = raw_input(question_text)
             if response != "y":
-                sys.exit(Fore.RED + "\nSetup cancelled" + Fore.RESET)
+                exit(Fore.RED + "\nSetup cancelled" + Fore.RESET)
                 return
             os.mkdir(data_dir)
             config.dir = data_dir
             reset_meta()
         config.create_basic_directories()
         download_biosphere()
-        sys.exit(Fore.GREEN + u"Brightway2 setup successful" + Fore.RESET)
+        download_methods()
+        exit(Fore.GREEN + u"Brightway2 setup successful" + Fore.RESET)
 
     def upload_logs(self, kwargs):
         response = upload_logs_to_server({'comment': kwargs.get('COMMENT', "")})
         if response.text == "OK":
             return "Logs uploaded successfully"
         else:
             return "There was a problem uploading the log files"
```

### Comparing `bw2ui-0.8/bw2ui/web/app.py` & `bw2ui-0.8.1/bw2ui/web/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,23 @@
         })
     return render_template("fp-select.html", dirtree=data)
 
 #######################
 ### Getting started ###
 #######################
 
+def get_windows_drives():
+    if not config._windows:
+        return {'windows': False}
+    else:
+        return {
+            'windows': True,
+            'drive_letters': get_windows_drive_letters(),
+            'current_drive': os.path.splitdrive(os.getcwd())[0]
+        }
 
 @app.route('/start/path', methods=["POST"])
 def set_path():
     path = urllib2.unquote(request.form["path"])
     dirname = urllib2.unquote(request.form["dirname"])
     set_data_dir(os.path.join(path, dirname))
     return "1"
@@ -135,45 +144,40 @@
 def install_biosphere():
     bw2setup()
     return "1"
 
 
 @app.route('/start')
 def start():
-    if config._windows:
-        windows, drive_letters = True, get_windows_drive_letters()
-    else:
-        windows, drive_letters = False, []
     return render_template(
         "start.html",
         root_path=json.dumps(os.path.abspath("/")),
-        windows=windows,
-        drive_letters=drive_letters
+        **get_windows_drives()
     )
 
 #################
 ### Importing ###
 #################
 
 
 @app.route("/import/database", methods=["GET", "POST"])
 def import_database():
     if request.method == "GET":
-        return render_template("import-database.html")
+        return render_template("import-database.html", **get_windows_drives())
     else:
         path = urllib2.unquote(request.form["path"])
         name = urllib2.unquote(request.form["name"])
         Ecospold1Importer().importer(path, name)
         return "1"
 
 
 @app.route("/import/method", methods=["GET", "POST"])
 def import_method():
     if request.method == "GET":
-        return render_template("import-method.html")
+        return render_template("import-method.html", **get_windows_drives())
     else:
         path = urllib2.unquote(request.form["path"])
         EcospoldImpactAssessmentImporter().importer(path)
         return "1"
 
 ###################
 ### Basic views ###
@@ -284,15 +288,15 @@
         return "---"
 
 
 @app.route('/lca', methods=["GET", "POST"])
 def lca():
     if request.method == "GET":
         return render_template("select.html",
-            db_names=[x for x in databases.list if x != "biosphere"],
+            db_names=[x for x in databases.list if x != config.biosphere],
             lcia_methods=[{
                 "l1": get_tuple_index(key, 0),
                 "l2": get_tuple_index(key, 1),
                 "l3": get_tuple_index(key, 2),
                 "u": value["unit"],
                 "n": value["num_cfs"],
             } for key, value in methods.data.iteritems() if value.get(
```

### Comparing `bw2ui-0.8/bw2ui/web/gzip_response.py` & `bw2ui-0.8.1/bw2ui/web/gzip_response.py`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/jobs.py` & `bw2ui-0.8.1/bw2ui/web/jobs.py`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/backgrid/backgrid-table.js` & `bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid-table.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/backgrid/backgrid.css` & `bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/backgrid/backgrid.js` & `bw2ui-0.8.1/bw2ui/web/static/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/ie.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/ie.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/cross.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/cross.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/icons/tick.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/icons/tick.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/buttons/screen.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/buttons/screen.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/fancy-type/screen.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/fancy-type/screen.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/doc.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/doc.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/email.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/email.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/external.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/external.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/feed.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/feed.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/im.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/im.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/lock.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/lock.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/pdf.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/pdf.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/visited.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/visited.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/icons/xls.png` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/icons/xls.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/link-icons/screen.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/link-icons/screen.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/plugins/rtl/screen.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/plugins/rtl/screen.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/print.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/print.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/screen.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/screen.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/forms.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/forms.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/grid.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/grid.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/ie.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/ie.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/print.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/print.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/reset.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/reset.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/blueprint/src/typography.css` & `bw2ui-0.8.1/bw2ui/web/static/blueprint/src/typography.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/css/base.css` & `bw2ui-0.8.1/bw2ui/web/static/css/base.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/d3-tip/d3-tip.js` & `bw2ui-0.8.1/bw2ui/web/static/d3-tip/d3-tip.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/img/favicon.ico` & `bw2ui-0.8.1/bw2ui/web/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/img/linedpaper.png` & `bw2ui-0.8.1/bw2ui/web/static/img/linedpaper.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/img/llama.jpg` & `bw2ui-0.8.1/bw2ui/web/static/img/llama.jpg`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/img/monster.jpg` & `bw2ui-0.8.1/bw2ui/web/static/img/monster.jpg`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/code.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/code.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/css.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/css.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/db.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/db.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/directory.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/directory.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/doc.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/doc.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/film.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/film.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/flash.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/flash.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/folder_open.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/folder_open.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/html.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/html.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/java.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/java.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/linux.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/linux.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/pdf.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/pdf.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/php.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/php.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/picture.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/picture.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/ppt.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/ppt.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/psd.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/psd.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/ruby.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/ruby.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/script.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/script.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/spinner.gif` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/images/xls.png` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/images/xls.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js` & `bw2ui-0.8.1/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/js/force-directed.js` & `bw2ui-0.8.1/bw2ui/web/static/js/force-directed.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/js/hinton.js` & `bw2ui-0.8.1/bw2ui/web/static/js/hinton.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/js/interp-histogram.js` & `bw2ui-0.8.1/bw2ui/web/static/js/interp-histogram.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/js/stepped-histogram.js` & `bw2ui-0.8.1/bw2ui/web/static/js/stepped-histogram.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/js/treemap.js` & `bw2ui-0.8.1/bw2ui/web/static/js/treemap.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/ace.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/ace.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor-icons.png` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor-icons.png`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor-min.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor-min.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/jsoneditor.css` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsoneditor.css`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/jsonlint.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/jsonlint.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/mode-json.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/mode-json.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/theme-jsoneditor.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/theme-jsoneditor.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/static/jsoneditor/theme-textmate.js` & `bw2ui-0.8.1/bw2ui/web/static/jsoneditor/theme-textmate.js`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/base.html` & `bw2ui-0.8.1/bw2ui/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/database.html` & `bw2ui-0.8.1/bw2ui/web/templates/database.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/database_tree.html` & `bw2ui-0.8.1/bw2ui/web/templates/database_tree.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/edit-raw.html` & `bw2ui-0.8.1/bw2ui/web/templates/edit-raw.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/fp.html` & `bw2ui-0.8.1/bw2ui/web/templates/fp.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/hist.html` & `bw2ui-0.8.1/bw2ui/web/templates/hist.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/import-database.html` & `bw2ui-0.8.1/bw2ui/web/templates/import-database.html`

 * *Files 9% similar despite different names*

```diff
@@ -23,128 +23,166 @@
 00000160: 7365 6c65 6374 2074 6865 2064 6972 6563  select the direc
 00000170: 746f 7279 2074 6861 7420 7468 6520 584d  tory that the XM
 00000180: 4c20 6669 6c65 7320 6172 6520 696e 2c20  L files are in, 
 00000190: 6f72 2061 2073 696e 676c 6520 584d 4c20  or a single XML 
 000001a0: 6669 6c65 2e3c 2f68 333e 0a20 2020 203c  file.</h3>.    <
 000001b0: 703e 4e6f 7465 3a20 4e6f 7420 616c 6c20  p>Note: Not all 
 000001c0: 6669 6c65 7320 6172 6520 7368 6f77 6e2e  files are shown.
-000001d0: 2e2e 3c2f 703e 0a20 2020 203c 6469 7620  ..</p>.    <div 
-000001e0: 6964 3d22 6670 223e 3c2f 6469 763e 0a20  id="fp"></div>. 
-000001f0: 203c 2f64 6976 3e0a 2020 3c64 6976 2063   </div>.  <div c
-00000200: 6c61 7373 3d22 7370 616e 2d38 206c 6173  lass="span-8 las
-00000210: 7422 3e0a 2020 2020 3c66 6f72 6d20 6e61  t">.    <form na
-00000220: 6d65 3d22 7061 7468 2d66 6f72 6d22 3e0a  me="path-form">.
-00000230: 2020 2020 2020 3c68 333e 322e 2054 6865        <h3>2. The
-00000240: 6e20 6e61 6d65 2074 6865 2064 6174 6162  n name the datab
-00000250: 6173 653a 3c2f 6833 3e0a 2020 2020 2020  ase:</h3>.      
-00000260: 3c69 6e70 7574 2069 643d 2264 6972 2d66  <input id="dir-f
-00000270: 696c 6522 206e 616d 653d 226e 616d 6522  ile" name="name"
-00000280: 2074 7970 653d 2274 6578 7422 2076 616c   type="text" val
-00000290: 7565 3d22 223e 3c62 723e 0a20 2020 2020  ue=""><br>.     
-000002a0: 203c 696e 7075 7420 6964 3d22 6869 6464   <input id="hidd
-000002b0: 656e 2d70 6174 6822 206e 616d 653d 2270  en-path" name="p
-000002c0: 6174 6822 2074 7970 653d 2268 6964 6465  ath" type="hidde
-000002d0: 6e22 2076 616c 7565 3d22 223e 0a20 2020  n" value="">.   
-000002e0: 2020 203c 6469 7620 6964 3d22 6d69 7373     <div id="miss
-000002f0: 696e 672d 6e61 6d65 223e 3c2f 6469 763e  ing-name"></div>
-00000300: 0a20 2020 2020 203c 6275 7474 6f6e 2069  .      <button i
-00000310: 643d 2273 7562 6d69 742d 7061 7468 2220  d="submit-path" 
-00000320: 7479 7065 3d22 7375 626d 6974 2220 7374  type="submit" st
-00000330: 796c 653d 2222 3e49 6d70 6f72 7420 7468  yle="">Import th
-00000340: 6573 6520 6669 6c65 2873 293c 2f62 7574  ese file(s)</but
-00000350: 746f 6e3e 0a20 2020 203c 2f66 6f72 6d3e  ton>.    </form>
-00000360: 0a20 203c 2f64 6976 3e0a 3c2f 6469 763e  .  </div>.</div>
-00000370: 0a0a 3c64 6976 2069 643d 2269 6e2d 7375  ..<div id="in-su
-00000380: 626d 6973 7369 6f6e 2220 636c 6173 733d  bmission" class=
-00000390: 2273 7061 6e2d 3234 2063 6c65 6172 223e  "span-24 clear">
-000003a0: 0a20 203c 6833 3e59 6f75 7220 636f 6d70  .  <h3>Your comp
-000003b0: 7574 6572 2069 7320 6e6f 7720 776f 726b  uter is now work
-000003c0: 696e 6720 6173 2066 6173 7420 6173 2069  ing as fast as i
-000003d0: 7420 6361 6e20 696d 706f 7274 696e 6720  t can importing 
-000003e0: 796f 7572 206e 6577 2064 6174 6162 6173  your new databas
-000003f0: 652e 3c2f 6833 3e0a 2020 3c70 3e50 6c65  e.</h3>.  <p>Ple
-00000400: 6173 6520 6265 2070 6174 6965 6e74 2e2e  ase be patient..
-00000410: 2e20 796f 7520 7769 6c6c 2062 6520 7265  . you will be re
-00000420: 6469 7265 6374 6564 2074 6f20 7468 6520  directed to the 
-00000430: 686f 6d65 2070 6167 6520 6173 2073 6f6f  home page as soo
-00000440: 6e20 6173 2074 6865 2069 6d70 6f72 7420  n as the import 
-00000450: 6973 2066 696e 6973 6865 642e 3c2f 703e  is finished.</p>
-00000460: 0a3c 2f64 6976 3e0a 0a3c 7363 7269 7074  .</div>..<script
-00000470: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
-00000480: 7363 7269 7074 223e 0a66 756e 6374 696f  script">.functio
-00000490: 6e20 6670 7365 6c65 6374 6f72 2028 6129  n fpselector (a)
-000004a0: 207b 0a20 2024 2822 2366 702d 7365 6c65   {.  $("#fp-sele
-000004b0: 6374 6564 2229 2e74 6578 7428 2243 7572  cted").text("Cur
-000004c0: 7265 6e74 6c79 2073 656c 6563 7465 643a  rently selected:
-000004d0: 2022 202b 2061 2e61 7474 7228 2772 656c   " + a.attr('rel
-000004e0: 2729 293b 0a20 2024 2822 2368 6964 6465  '));.  $("#hidde
-000004f0: 6e2d 7061 7468 2229 2e76 616c 2861 2e61  n-path").val(a.a
-00000500: 7474 7228 2772 656c 2729 293b 0a7d 3b0a  ttr('rel'));.};.
-00000510: 3c2f 7363 7269 7074 3e0a 3c73 6372 6970  </script>.<scrip
-00000520: 7420 7372 633d 227b 7b20 7572 6c5f 666f  t src="{{ url_fo
-00000530: 7228 2773 7461 7469 6327 2c20 6669 6c65  r('static', file
-00000540: 6e61 6d65 3d22 6a71 7565 7279 4669 6c65  name="jqueryFile
-00000550: 5472 6565 2f6a 7175 6572 7946 696c 6554  Tree/jqueryFileT
-00000560: 7265 652e 6a73 2229 207d 7d22 3e3c 2f73  ree.js") }}"></s
-00000570: 6372 6970 743e 0a3c 7363 7269 7074 2074  cript>.<script t
-00000580: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
-00000590: 7269 7074 223e 2020 2020 2020 0a24 2864  ript">      .$(d
-000005a0: 6f63 756d 656e 7429 2e72 6561 6479 2820  ocument).ready( 
-000005b0: 6675 6e63 7469 6f6e 2829 207b 2020 2020  function() {    
-000005c0: 2020 2020 0a20 2024 2822 2373 7563 6365      .  $("#succe
-000005d0: 7373 2229 2e68 6964 6528 293b 0a0a 2020  ss").hide();..  
-000005e0: 2428 2723 6670 2729 2e66 696c 6554 7265  $('#fp').fileTre
-000005f0: 6528 7b0a 2020 2020 726f 6f74 3a20 272f  e({.    root: '/
-00000600: 272c 200a 2020 2020 7363 7269 7074 3a20  ', .    script: 
-00000610: 277b 7b20 7572 6c5f 666f 7228 2766 705f  '{{ url_for('fp_
-00000620: 6170 6927 2920 7d7d 272c 200a 2020 2020  api') }}', .    
-00000630: 666f 6c64 6572 4576 656e 743a 2027 636c  folderEvent: 'cl
-00000640: 6963 6b27 2c20 0a20 2020 206d 756c 7469  ick', .    multi
-00000650: 466f 6c64 6572 3a20 6661 6c73 6520 0a20  Folder: false . 
-00000660: 2020 207d 2c20 0a20 2020 2066 756e 6374     }, .    funct
-00000670: 696f 6e28 6669 6c65 2920 7b20 0a20 2020  ion(file) { .   
-00000680: 2020 2024 2822 2366 702d 7365 6c65 6374     $("#fp-select
-00000690: 6564 2229 2e74 6578 7428 2243 7572 7265  ed").text("Curre
-000006a0: 6e74 6c79 2073 656c 6563 7465 643a 2022  ntly selected: "
-000006b0: 202b 2066 696c 6529 3b0a 2020 2020 2020   + file);.      
-000006c0: 2428 2223 6869 6464 656e 2d70 6174 6822  $("#hidden-path"
-000006d0: 292e 7661 6c28 6669 6c65 293b 0a20 2020  ).val(file);.   
-000006e0: 207d 0a20 2029 3b0a 0a20 2024 2827 666f   }.  );..  $('fo
-000006f0: 726d 5b6e 616d 653d 7061 7468 2d66 6f72  rm[name=path-for
-00000700: 6d5d 2729 2e73 7562 6d69 7428 2066 756e  m]').submit( fun
-00000710: 6374 696f 6e20 2865 2920 7b0a 2020 2020  ction (e) {.    
-00000720: 652e 7072 6576 656e 7444 6566 6175 6c74  e.preventDefault
-00000730: 2829 3b0a 2020 2020 6966 2028 2824 2822  ();.    if (($("
-00000740: 2364 6972 2d66 696c 6522 292e 7661 6c28  #dir-file").val(
-00000750: 2920 213d 2027 2729 2026 2620 2824 2822  ) != '') && ($("
-00000760: 2368 6964 6465 6e2d 7061 7468 2229 2e76  #hidden-path").v
-00000770: 616c 2829 2021 3d20 2727 2929 207b 0a20  al() != '')) {. 
-00000780: 2020 2020 2024 2822 2369 6e2d 7375 626d       $("#in-subm
-00000790: 6973 7369 6f6e 2229 2e73 686f 7728 293b  ission").show();
-000007a0: 0a20 2020 2020 2024 2822 2373 656c 6563  .      $("#selec
-000007b0: 742d 7061 7468 2229 2e68 6964 6528 293b  t-path").hide();
-000007c0: 0a20 2020 2020 2024 2e61 6a61 7828 7b0a  .      $.ajax({.
-000007d0: 2020 2020 2020 2020 7479 7065 3a20 2250          type: "P
-000007e0: 4f53 5422 2c0a 2020 2020 2020 2020 7572  OST",.        ur
-000007f0: 6c3a 2027 7b7b 2075 726c 5f66 6f72 2827  l: '{{ url_for('
-00000800: 696d 706f 7274 5f64 6174 6162 6173 6527  import_database'
-00000810: 2920 7d7d 272c 0a20 2020 2020 2020 2064  ) }}',.        d
-00000820: 6174 613a 2024 2874 6869 7329 2e73 6572  ata: $(this).ser
-00000830: 6961 6c69 7a65 2829 2c0a 2020 2020 2020  ialize(),.      
-00000840: 2020 7375 6363 6573 733a 2066 756e 6374    success: funct
-00000850: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
-00000860: 2020 2064 6f63 756d 656e 742e 6c6f 6361     document.loca
-00000870: 7469 6f6e 2e68 7265 663d 277b 7b20 7572  tion.href='{{ ur
-00000880: 6c5f 666f 7228 2769 6e64 6578 2729 207d  l_for('index') }
-00000890: 7d27 3b0a 2020 2020 2020 2020 7d0a 2020  }';.        }.  
-000008a0: 2020 2020 7d29 3b0a 2020 2020 7d20 656c      });.    } el
-000008b0: 7365 207b 0a20 2020 2020 2024 2822 236d  se {.      $("#m
-000008c0: 6973 7369 6e67 2d6e 616d 6522 292e 6874  issing-name").ht
-000008d0: 6d6c 2827 3c70 2073 7479 6c65 3d22 636f  ml('<p style="co
-000008e0: 6c6f 723a 2072 6564 223e 596f 7520 6d75  lor: red">You mu
-000008f0: 7374 2066 6972 7374 2073 656c 6563 7420  st first select 
-00000900: 626f 7468 2061 2066 696c 652f 6469 7265  both a file/dire
-00000910: 6374 6f72 7920 616e 6420 656e 7465 7220  ctory and enter 
-00000920: 6120 6e61 6d65 3c2f 703e 2729 3b0a 2020  a name</p>');.  
-00000930: 2020 7d0a 2020 7d29 3b0a 7d29 3b0a 3c2f    }.  });.});.</
-00000940: 7363 7269 7074 3e0a 7b25 2065 6e64 626c  script>.{% endbl
-00000950: 6f63 6b20 257d                           ock %}
+000001d0: 2e2e 3c2f 703e 0a20 2020 207b 2520 6966  ..</p>.    {% if
+000001e0: 2077 696e 646f 7773 2025 7d0a 2020 2020   windows %}.    
+000001f0: 2020 3c68 333e 4368 616e 6765 2074 6865    <h3>Change the
+00000200: 2064 7269 7665 2028 5769 6e64 6f77 7320   drive (Windows 
+00000210: 6f6e 6c79 293c 2f68 333e 0a20 2020 2020  only)</h3>.     
+00000220: 203c 7365 6c65 6374 2069 643d 2264 7269   <select id="dri
+00000230: 7665 6c65 7474 6572 223e 0a20 2020 2020  veletter">.     
+00000240: 207b 2520 666f 7220 6c65 7474 6572 2069   {% for letter i
+00000250: 6e20 6472 6976 655f 6c65 7474 6572 7320  n drive_letters 
+00000260: 257d 0a20 2020 2020 2020 203c 6f70 7469  %}.        <opti
+00000270: 6f6e 2076 616c 7565 3d22 7b7b 206c 6574  on value="{{ let
+00000280: 7465 7220 7d7d 2220 7b25 2069 6620 6c65  ter }}" {% if le
+00000290: 7474 6572 5b3a 325d 203d 3d20 6375 7272  tter[:2] == curr
+000002a0: 656e 745f 6472 6976 6520 257d 7365 6c65  ent_drive %}sele
+000002b0: 6374 6564 7b25 2065 6e64 6966 2025 7d3e  cted{% endif %}>
+000002c0: 7b7b 206c 6574 7465 7220 7d7d 3c2f 6f70  {{ letter }}</op
+000002d0: 7469 6f6e 3e0a 2020 2020 2020 7b25 2065  tion>.      {% e
+000002e0: 6e64 666f 7220 257d 0a20 2020 2020 203c  ndfor %}.      <
+000002f0: 2f73 656c 6563 743e 0a20 2020 207b 2520  /select>.    {% 
+00000300: 656e 6469 6620 257d 0a20 2020 203c 6469  endif %}.    <di
+00000310: 7620 6964 3d22 6670 223e 3c2f 6469 763e  v id="fp"></div>
+00000320: 0a20 203c 2f64 6976 3e0a 2020 3c64 6976  .  </div>.  <div
+00000330: 2063 6c61 7373 3d22 7370 616e 2d38 206c   class="span-8 l
+00000340: 6173 7422 3e0a 2020 2020 3c66 6f72 6d20  ast">.    <form 
+00000350: 6e61 6d65 3d22 7061 7468 2d66 6f72 6d22  name="path-form"
+00000360: 3e0a 2020 2020 2020 3c68 333e 322e 2054  >.      <h3>2. T
+00000370: 6865 6e20 6e61 6d65 2074 6865 2064 6174  hen name the dat
+00000380: 6162 6173 653a 3c2f 6833 3e0a 2020 2020  abase:</h3>.    
+00000390: 2020 3c69 6e70 7574 2069 643d 2264 6972    <input id="dir
+000003a0: 2d66 696c 6522 206e 616d 653d 226e 616d  -file" name="nam
+000003b0: 6522 2074 7970 653d 2274 6578 7422 2076  e" type="text" v
+000003c0: 616c 7565 3d22 223e 3c62 723e 0a20 2020  alue=""><br>.   
+000003d0: 2020 203c 696e 7075 7420 6964 3d22 6869     <input id="hi
+000003e0: 6464 656e 2d70 6174 6822 206e 616d 653d  dden-path" name=
+000003f0: 2270 6174 6822 2074 7970 653d 2268 6964  "path" type="hid
+00000400: 6465 6e22 2076 616c 7565 3d22 223e 0a20  den" value="">. 
+00000410: 2020 2020 203c 6469 7620 6964 3d22 6d69       <div id="mi
+00000420: 7373 696e 672d 6e61 6d65 223e 3c2f 6469  ssing-name"></di
+00000430: 763e 0a20 2020 2020 203c 6275 7474 6f6e  v>.      <button
+00000440: 2069 643d 2273 7562 6d69 742d 7061 7468   id="submit-path
+00000450: 2220 7479 7065 3d22 7375 626d 6974 2220  " type="submit" 
+00000460: 7374 796c 653d 2222 3e49 6d70 6f72 7420  style="">Import 
+00000470: 7468 6573 6520 6669 6c65 2873 293c 2f62  these file(s)</b
+00000480: 7574 746f 6e3e 0a20 2020 203c 2f66 6f72  utton>.    </for
+00000490: 6d3e 0a20 203c 2f64 6976 3e0a 3c2f 6469  m>.  </div>.</di
+000004a0: 763e 0a0a 3c64 6976 2069 643d 2269 6e2d  v>..<div id="in-
+000004b0: 7375 626d 6973 7369 6f6e 2220 636c 6173  submission" clas
+000004c0: 733d 2273 7061 6e2d 3234 2063 6c65 6172  s="span-24 clear
+000004d0: 223e 0a20 203c 6833 3e59 6f75 7220 636f  ">.  <h3>Your co
+000004e0: 6d70 7574 6572 2069 7320 6e6f 7720 776f  mputer is now wo
+000004f0: 726b 696e 6720 6173 2066 6173 7420 6173  rking as fast as
+00000500: 2069 7420 6361 6e20 696d 706f 7274 696e   it can importin
+00000510: 6720 796f 7572 206e 6577 2064 6174 6162  g your new datab
+00000520: 6173 652e 3c2f 6833 3e0a 2020 3c70 3e50  ase.</h3>.  <p>P
+00000530: 6c65 6173 6520 6265 2070 6174 6965 6e74  lease be patient
+00000540: 2e2e 2e20 796f 7520 7769 6c6c 2062 6520  ... you will be 
+00000550: 7265 6469 7265 6374 6564 2074 6f20 7468  redirected to th
+00000560: 6520 686f 6d65 2070 6167 6520 6173 2073  e home page as s
+00000570: 6f6f 6e20 6173 2074 6865 2069 6d70 6f72  oon as the impor
+00000580: 7420 6973 2066 696e 6973 6865 642e 3c2f  t is finished.</
+00000590: 703e 0a3c 2f64 6976 3e0a 0a3c 7363 7269  p>.</div>..<scri
+000005a0: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
+000005b0: 7661 7363 7269 7074 223e 0a66 756e 6374  vascript">.funct
+000005c0: 696f 6e20 6670 7365 6c65 6374 6f72 2028  ion fpselector (
+000005d0: 6129 207b 0a20 2024 2822 2366 702d 7365  a) {.  $("#fp-se
+000005e0: 6c65 6374 6564 2229 2e74 6578 7428 2243  lected").text("C
+000005f0: 7572 7265 6e74 6c79 2073 656c 6563 7465  urrently selecte
+00000600: 643a 2022 202b 2061 2e61 7474 7228 2772  d: " + a.attr('r
+00000610: 656c 2729 293b 0a20 2024 2822 2368 6964  el'));.  $("#hid
+00000620: 6465 6e2d 7061 7468 2229 2e76 616c 2861  den-path").val(a
+00000630: 2e61 7474 7228 2772 656c 2729 293b 0a7d  .attr('rel'));.}
+00000640: 3b0a 3c2f 7363 7269 7074 3e0a 3c73 6372  ;.</script>.<scr
+00000650: 6970 7420 7372 633d 227b 7b20 7572 6c5f  ipt src="{{ url_
+00000660: 666f 7228 2773 7461 7469 6327 2c20 6669  for('static', fi
+00000670: 6c65 6e61 6d65 3d22 6a71 7565 7279 4669  lename="jqueryFi
+00000680: 6c65 5472 6565 2f6a 7175 6572 7946 696c  leTree/jqueryFil
+00000690: 6554 7265 652e 6a73 2229 207d 7d22 3e3c  eTree.js") }}"><
+000006a0: 2f73 6372 6970 743e 0a3c 7363 7269 7074  /script>.<script
+000006b0: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
+000006c0: 7363 7269 7074 223e 0a24 2864 6f63 756d  script">.$(docum
+000006d0: 656e 7429 2e72 6561 6479 2820 6675 6e63  ent).ready( func
+000006e0: 7469 6f6e 2829 207b 0a20 2024 2822 2373  tion() {.  $("#s
+000006f0: 7563 6365 7373 2229 2e68 6964 6528 293b  uccess").hide();
+00000700: 0a0a 2020 2428 2723 6670 2729 2e66 696c  ..  $('#fp').fil
+00000710: 6554 7265 6528 7b0a 2020 2020 726f 6f74  eTree({.    root
+00000720: 3a20 272f 272c 0a20 2020 2073 6372 6970  : '/',.    scrip
+00000730: 743a 2027 7b7b 2075 726c 5f66 6f72 2827  t: '{{ url_for('
+00000740: 6670 5f61 7069 2729 207d 7d27 2c0a 2020  fp_api') }}',.  
+00000750: 2020 666f 6c64 6572 4576 656e 743a 2027    folderEvent: '
+00000760: 636c 6963 6b27 2c0a 2020 2020 6d75 6c74  click',.    mult
+00000770: 6946 6f6c 6465 723a 2066 616c 7365 0a20  iFolder: false. 
+00000780: 2020 207d 2c0a 2020 2020 6675 6e63 7469     },.    functi
+00000790: 6f6e 2866 696c 6529 207b 0a20 2020 2020  on(file) {.     
+000007a0: 2024 2822 2366 702d 7365 6c65 6374 6564   $("#fp-selected
+000007b0: 2229 2e74 6578 7428 2243 7572 7265 6e74  ").text("Current
+000007c0: 6c79 2073 656c 6563 7465 643a 2022 202b  ly selected: " +
+000007d0: 2066 696c 6529 3b0a 2020 2020 2020 2428   file);.      $(
+000007e0: 2223 6869 6464 656e 2d70 6174 6822 292e  "#hidden-path").
+000007f0: 7661 6c28 6669 6c65 293b 0a20 2020 207d  val(file);.    }
+00000800: 0a20 2029 3b0a 0a20 2024 2827 666f 726d  .  );..  $('form
+00000810: 5b6e 616d 653d 7061 7468 2d66 6f72 6d5d  [name=path-form]
+00000820: 2729 2e73 7562 6d69 7428 2066 756e 6374  ').submit( funct
+00000830: 696f 6e20 2865 2920 7b0a 2020 2020 652e  ion (e) {.    e.
+00000840: 7072 6576 656e 7444 6566 6175 6c74 2829  preventDefault()
+00000850: 3b0a 2020 2020 6966 2028 2824 2822 2364  ;.    if (($("#d
+00000860: 6972 2d66 696c 6522 292e 7661 6c28 2920  ir-file").val() 
+00000870: 213d 2027 2729 2026 2620 2824 2822 2368  != '') && ($("#h
+00000880: 6964 6465 6e2d 7061 7468 2229 2e76 616c  idden-path").val
+00000890: 2829 2021 3d20 2727 2929 207b 0a20 2020  () != '')) {.   
+000008a0: 2020 2024 2822 2369 6e2d 7375 626d 6973     $("#in-submis
+000008b0: 7369 6f6e 2229 2e73 686f 7728 293b 0a20  sion").show();. 
+000008c0: 2020 2020 2024 2822 2373 656c 6563 742d       $("#select-
+000008d0: 7061 7468 2229 2e68 6964 6528 293b 0a20  path").hide();. 
+000008e0: 2020 2020 2024 2e61 6a61 7828 7b0a 2020       $.ajax({.  
+000008f0: 2020 2020 2020 7479 7065 3a20 2250 4f53        type: "POS
+00000900: 5422 2c0a 2020 2020 2020 2020 7572 6c3a  T",.        url:
+00000910: 2027 7b7b 2075 726c 5f66 6f72 2827 696d   '{{ url_for('im
+00000920: 706f 7274 5f64 6174 6162 6173 6527 2920  port_database') 
+00000930: 7d7d 272c 0a20 2020 2020 2020 2064 6174  }}',.        dat
+00000940: 613a 2024 2874 6869 7329 2e73 6572 6961  a: $(this).seria
+00000950: 6c69 7a65 2829 2c0a 2020 2020 2020 2020  lize(),.        
+00000960: 7375 6363 6573 733a 2066 756e 6374 696f  success: functio
+00000970: 6e20 2829 207b 0a20 2020 2020 2020 2020  n () {.         
+00000980: 2064 6f63 756d 656e 742e 6c6f 6361 7469   document.locati
+00000990: 6f6e 2e68 7265 663d 277b 7b20 7572 6c5f  on.href='{{ url_
+000009a0: 666f 7228 2769 6e64 6578 2729 207d 7d27  for('index') }}'
+000009b0: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
+000009c0: 2020 7d29 3b0a 2020 2020 7d20 656c 7365    });.    } else
+000009d0: 207b 0a20 2020 2020 2024 2822 236d 6973   {.      $("#mis
+000009e0: 7369 6e67 2d6e 616d 6522 292e 6874 6d6c  sing-name").html
+000009f0: 2827 3c70 2073 7479 6c65 3d22 636f 6c6f  ('<p style="colo
+00000a00: 723a 2072 6564 223e 596f 7520 6d75 7374  r: red">You must
+00000a10: 2066 6972 7374 2073 656c 6563 7420 626f   first select bo
+00000a20: 7468 2061 2066 696c 652f 6469 7265 6374  th a file/direct
+00000a30: 6f72 7920 616e 6420 656e 7465 7220 6120  ory and enter a 
+00000a40: 6e61 6d65 3c2f 703e 2729 3b0a 2020 2020  name</p>');.    
+00000a50: 7d0a 2020 7d29 3b0a 7d29 3b0a 0a24 2866  }.  });.});..$(f
+00000a60: 756e 6374 696f 6e28 2920 7b0a 2020 2428  unction() {.  $(
+00000a70: 2223 6472 6976 656c 6574 7465 7222 292e  "#driveletter").
+00000a80: 6368 616e 6765 2866 756e 6374 696f 6e28  change(function(
+00000a90: 2920 7b0a 2020 2020 2020 7661 7220 6c65  ) {.      var le
+00000aa0: 7474 6572 203d 2024 2874 6869 7329 2e76  tter = $(this).v
+00000ab0: 616c 2829 3b0a 2020 2020 2020 2428 2723  al();.      $('#
+00000ac0: 6670 2729 2e68 746d 6c28 2222 293b 0a20  fp').html("");. 
+00000ad0: 2020 2020 2024 2827 2366 7027 292e 6669       $('#fp').fi
+00000ae0: 6c65 5472 6565 287b 0a20 2020 2020 2020  leTree({.       
+00000af0: 2072 6f6f 743a 206c 6574 7465 722c 0a20   root: letter,. 
+00000b00: 2020 2020 2020 2073 6372 6970 743a 2027         script: '
+00000b10: 2f66 702d 6170 6927 2c0a 2020 2020 2020  /fp-api',.      
+00000b20: 2020 666f 6c64 6572 4576 656e 743a 2027    folderEvent: '
+00000b30: 636c 6963 6b27 2c0a 2020 2020 2020 2020  click',.        
+00000b40: 6d75 6c74 6946 6f6c 6465 723a 2066 616c  multiFolder: fal
+00000b50: 7365 0a20 2020 2020 2020 207d 2c0a 2020  se.        },.  
+00000b60: 2020 2020 2020 6675 6e63 7469 6f6e 2866        function(f
+00000b70: 696c 6529 207b 2063 6f6e 736f 6c65 2e6c  ile) { console.l
+00000b80: 6f67 2866 696c 6529 3b20 7d0a 2020 2020  og(file); }.    
+00000b90: 2020 293b 0a20 207d 290a 7d29 3b0a 3c2f    );.  }).});.</
+00000ba0: 7363 7269 7074 3e0a 7b25 2065 6e64 626c  script>.{% endbl
+00000bb0: 6f63 6b20 257d 0a                        ock %}.
```

### Comparing `bw2ui-0.8/bw2ui/web/templates/import-method.html` & `bw2ui-0.8.1/bw2ui/web/templates/import-method.html`

 * *Files 17% similar despite different names*

```diff
@@ -20,119 +20,157 @@
 00000130: 636f 6c62 6f72 6465 7222 3e0a 2020 2020  colborder">.    
 00000140: 3c68 3320 6964 3d22 6670 2d73 656c 6563  <h3 id="fp-selec
 00000150: 7465 6422 3e43 6c69 636b 2074 6f20 7365  ted">Click to se
 00000160: 6c65 6374 2074 6865 2064 6972 6563 746f  lect the directo
 00000170: 7279 2074 6861 7420 7468 6520 584d 4c20  ry that the XML 
 00000180: 6669 6c65 7320 6172 6520 696e 2c20 6f72  files are in, or
 00000190: 2061 2073 696e 676c 6520 584d 4c20 6669   a single XML fi
-000001a0: 6c65 2e3c 2f68 333e 0a20 2020 203c 6469  le.</h3>.    <di
-000001b0: 7620 6964 3d22 6670 223e 3c2f 6469 763e  v id="fp"></div>
-000001c0: 0a20 203c 2f64 6976 3e0a 2020 3c64 6976  .  </div>.  <div
-000001d0: 2063 6c61 7373 3d22 7370 616e 2d38 206c   class="span-8 l
-000001e0: 6173 7422 3e0a 2020 2020 3c66 6f72 6d20  ast">.    <form 
-000001f0: 6e61 6d65 3d22 7061 7468 2d66 6f72 6d22  name="path-form"
-00000200: 3e0a 2020 2020 2020 3c69 6e70 7574 2069  >.      <input i
-00000210: 643d 2268 6964 6465 6e2d 7061 7468 2220  d="hidden-path" 
-00000220: 6e61 6d65 3d22 7061 7468 2220 7479 7065  name="path" type
-00000230: 3d22 6869 6464 656e 2220 7661 6c75 653d  ="hidden" value=
-00000240: 2222 3e0a 2020 2020 2020 3c64 6976 2069  "">.      <div i
-00000250: 643d 226d 6973 7369 6e67 2d6e 616d 6522  d="missing-name"
-00000260: 3e3c 2f64 6976 3e0a 2020 2020 2020 3c62  ></div>.      <b
-00000270: 7574 746f 6e20 6964 3d22 7375 626d 6974  utton id="submit
-00000280: 2d70 6174 6822 2074 7970 653d 2273 7562  -path" type="sub
-00000290: 6d69 7422 2073 7479 6c65 3d22 223e 496d  mit" style="">Im
-000002a0: 706f 7274 204c 4349 4120 6d65 7468 6f64  port LCIA method
-000002b0: 2873 293c 2f62 7574 746f 6e3e 0a20 2020  (s)</button>.   
-000002c0: 203c 2f66 6f72 6d3e 0a20 203c 2f64 6976   </form>.  </div
-000002d0: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2069  >.</div>..<div i
-000002e0: 643d 2269 6e2d 7375 626d 6973 7369 6f6e  d="in-submission
-000002f0: 2220 636c 6173 733d 2273 7061 6e2d 3234  " class="span-24
-00000300: 2063 6c65 6172 223e 0a20 203c 6833 3e59   clear">.  <h3>Y
-00000310: 6f75 7220 636f 6d70 7574 6572 2069 7320  our computer is 
-00000320: 6e6f 7720 776f 726b 696e 6720 6173 2066  now working as f
-00000330: 6173 7420 6173 2069 7420 6361 6e20 696d  ast as it can im
-00000340: 706f 7274 696e 6720 7468 6520 4c43 4941  porting the LCIA
-00000350: 206d 6574 686f 6428 7329 2e3c 2f68 333e   method(s).</h3>
-00000360: 0a20 203c 703e 506c 6561 7365 2062 6520  .  <p>Please be 
-00000370: 7061 7469 656e 742e 2e2e 2079 6f75 2077  patient... you w
-00000380: 696c 6c20 6265 2072 6564 6972 6563 7465  ill be redirecte
-00000390: 6420 746f 2074 6865 2068 6f6d 6520 7061  d to the home pa
-000003a0: 6765 2061 7320 736f 6f6e 2061 7320 7468  ge as soon as th
-000003b0: 6520 696d 706f 7274 2069 7320 6669 6e69  e import is fini
-000003c0: 7368 6564 2e3c 2f70 3e0a 3c2f 6469 763e  shed.</p>.</div>
-000003d0: 0a0a 3c73 6372 6970 7420 7479 7065 3d22  ..<script type="
-000003e0: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-000003f0: 3e0a 6675 6e63 7469 6f6e 2066 7073 656c  >.function fpsel
-00000400: 6563 746f 7220 2861 2920 7b0a 2020 2428  ector (a) {.  $(
-00000410: 2223 6670 2d73 656c 6563 7465 6422 292e  "#fp-selected").
-00000420: 7465 7874 2822 4375 7272 656e 746c 7920  text("Currently 
-00000430: 7365 6c65 6374 6564 3a20 2220 2b20 612e  selected: " + a.
-00000440: 6174 7472 2827 7265 6c27 2929 3b0a 2020  attr('rel'));.  
-00000450: 2428 2223 6869 6464 656e 2d70 6174 6822  $("#hidden-path"
-00000460: 292e 7661 6c28 612e 6174 7472 2827 7265  ).val(a.attr('re
-00000470: 6c27 2929 3b0a 7d3b 0a3c 2f73 6372 6970  l'));.};.</scrip
-00000480: 743e 0a3c 7363 7269 7074 2073 7263 3d22  t>.<script src="
-00000490: 7b7b 2075 726c 5f66 6f72 2827 7374 6174  {{ url_for('stat
-000004a0: 6963 272c 2066 696c 656e 616d 653d 226a  ic', filename="j
-000004b0: 7175 6572 7946 696c 6554 7265 652f 6a71  queryFileTree/jq
-000004c0: 7565 7279 4669 6c65 5472 6565 2e6a 7322  ueryFileTree.js"
-000004d0: 2920 7d7d 223e 3c2f 7363 7269 7074 3e0a  ) }}"></script>.
-000004e0: 3c73 6372 6970 7420 7479 7065 3d22 7465  <script type="te
-000004f0: 7874 2f6a 6176 6173 6372 6970 7422 3e20  xt/javascript"> 
-00000500: 2020 2020 200a 2428 646f 6375 6d65 6e74       .$(document
-00000510: 292e 7265 6164 7928 2066 756e 6374 696f  ).ready( functio
-00000520: 6e28 2920 7b20 2020 2020 2020 200a 2020  n() {        .  
-00000530: 2428 2223 696e 2d73 7562 6d69 7373 696f  $("#in-submissio
-00000540: 6e22 292e 6869 6465 2829 3b0a 0a20 2024  n").hide();..  $
-00000550: 2827 2366 7027 292e 6669 6c65 5472 6565  ('#fp').fileTree
-00000560: 287b 0a20 2020 2072 6f6f 743a 2027 2f27  ({.    root: '/'
-00000570: 2c20 0a20 2020 2073 6372 6970 743a 2027  , .    script: '
-00000580: 7b7b 2075 726c 5f66 6f72 2827 6670 5f61  {{ url_for('fp_a
-00000590: 7069 2729 207d 7d3f 6675 6c6c 3d31 272c  pi') }}?full=1',
-000005a0: 200a 2020 2020 666f 6c64 6572 4576 656e   .    folderEven
-000005b0: 743a 2027 636c 6963 6b27 2c20 0a20 2020  t: 'click', .   
-000005c0: 206d 756c 7469 466f 6c64 6572 3a20 6661   multiFolder: fa
-000005d0: 6c73 6520 0a20 2020 207d 2c20 0a20 2020  lse .    }, .   
-000005e0: 2066 756e 6374 696f 6e28 6669 6c65 2920   function(file) 
-000005f0: 7b20 0a20 2020 2020 2024 2822 2366 702d  { .      $("#fp-
-00000600: 7365 6c65 6374 6564 2229 2e74 6578 7428  selected").text(
-00000610: 2243 7572 7265 6e74 6c79 2073 656c 6563  "Currently selec
-00000620: 7465 643a 2022 202b 2066 696c 6529 3b0a  ted: " + file);.
-00000630: 2020 2020 2020 2428 2223 6869 6464 656e        $("#hidden
-00000640: 2d70 6174 6822 292e 7661 6c28 6669 6c65  -path").val(file
-00000650: 293b 0a20 2020 207d 0a20 2029 3b0a 0a20  );.    }.  );.. 
-00000660: 2024 2827 666f 726d 5b6e 616d 653d 7061   $('form[name=pa
-00000670: 7468 2d66 6f72 6d5d 2729 2e73 7562 6d69  th-form]').submi
-00000680: 7428 2066 756e 6374 696f 6e20 2865 2920  t( function (e) 
-00000690: 7b0a 2020 2020 652e 7072 6576 656e 7444  {.    e.preventD
-000006a0: 6566 6175 6c74 2829 3b0a 2020 2020 6966  efault();.    if
-000006b0: 2028 2428 2223 6869 6464 656e 2d70 6174   ($("#hidden-pat
-000006c0: 6822 292e 7661 6c28 2920 213d 2027 2729  h").val() != '')
-000006d0: 207b 0a20 2020 2020 2024 2822 2369 6e2d   {.      $("#in-
-000006e0: 7375 626d 6973 7369 6f6e 2229 2e73 686f  submission").sho
-000006f0: 7728 293b 0a20 2020 2020 2024 2822 2373  w();.      $("#s
-00000700: 656c 6563 742d 7061 7468 2229 2e68 6964  elect-path").hid
-00000710: 6528 293b 0a20 2020 2020 2024 2e61 6a61  e();.      $.aja
-00000720: 7828 7b0a 2020 2020 2020 2020 7479 7065  x({.        type
-00000730: 3a20 2250 4f53 5422 2c0a 2020 2020 2020  : "POST",.      
-00000740: 2020 7572 6c3a 2027 7b7b 2075 726c 5f66    url: '{{ url_f
-00000750: 6f72 2827 696d 706f 7274 5f6d 6574 686f  or('import_metho
-00000760: 6427 2920 7d7d 272c 0a20 2020 2020 2020  d') }}',.       
-00000770: 2064 6174 613a 2024 2874 6869 7329 2e73   data: $(this).s
-00000780: 6572 6961 6c69 7a65 2829 2c0a 2020 2020  erialize(),.    
-00000790: 2020 2020 7375 6363 6573 733a 2066 756e      success: fun
-000007a0: 6374 696f 6e20 2829 207b 0a20 2020 2020  ction () {.     
-000007b0: 2020 2020 2064 6f63 756d 656e 742e 6c6f       document.lo
-000007c0: 6361 7469 6f6e 2e68 7265 663d 277b 7b20  cation.href='{{ 
-000007d0: 7572 6c5f 666f 7228 2769 6e64 6578 2729  url_for('index')
-000007e0: 207d 7d27 3b0a 2020 2020 2020 2020 7d0a   }}';.        }.
-000007f0: 2020 2020 2020 7d29 3b0a 2020 2020 7d20        });.    } 
-00000800: 656c 7365 207b 0a20 2020 2020 2024 2822  else {.      $("
-00000810: 236d 6973 7369 6e67 2d6e 616d 6522 292e  #missing-name").
-00000820: 6874 6d6c 2827 3c70 2073 7479 6c65 3d22  html('<p style="
-00000830: 636f 6c6f 723a 2072 6564 223e 596f 7520  color: red">You 
-00000840: 6d75 7374 2066 6972 7374 2073 656c 6563  must first selec
-00000850: 7420 626f 7468 2061 2066 696c 652f 6469  t both a file/di
-00000860: 7265 6374 6f72 793c 2f70 3e27 293b 0a20  rectory</p>');. 
-00000870: 2020 207d 0a20 207d 293b 0a7d 293b 0a3c     }.  });.});.<
-00000880: 2f73 6372 6970 743e 0a7b 2520 656e 6462  /script>.{% endb
-00000890: 6c6f 636b 2025 7d                        lock %}
+000001a0: 6c65 2e3c 2f68 333e 0a20 2020 207b 2520  le.</h3>.    {% 
+000001b0: 6966 2077 696e 646f 7773 2025 7d0a 2020  if windows %}.  
+000001c0: 2020 2020 3c68 333e 4368 616e 6765 2074      <h3>Change t
+000001d0: 6865 2064 7269 7665 2028 5769 6e64 6f77  he drive (Window
+000001e0: 7320 6f6e 6c79 293c 2f68 333e 0a20 2020  s only)</h3>.   
+000001f0: 2020 203c 7365 6c65 6374 2069 643d 2264     <select id="d
+00000200: 7269 7665 6c65 7474 6572 223e 0a20 2020  riveletter">.   
+00000210: 2020 207b 2520 666f 7220 6c65 7474 6572     {% for letter
+00000220: 2069 6e20 6472 6976 655f 6c65 7474 6572   in drive_letter
+00000230: 7320 257d 0a20 2020 2020 2020 203c 6f70  s %}.        <op
+00000240: 7469 6f6e 2076 616c 7565 3d22 7b7b 206c  tion value="{{ l
+00000250: 6574 7465 7220 7d7d 2220 7b25 2069 6620  etter }}" {% if 
+00000260: 6c65 7474 6572 5b3a 325d 203d 3d20 6375  letter[:2] == cu
+00000270: 7272 656e 745f 6472 6976 6520 257d 7365  rrent_drive %}se
+00000280: 6c65 6374 6564 7b25 2065 6e64 6966 2025  lected{% endif %
+00000290: 7d3e 7b7b 206c 6574 7465 7220 7d7d 3c2f  }>{{ letter }}</
+000002a0: 6f70 7469 6f6e 3e0a 2020 2020 2020 7b25  option>.      {%
+000002b0: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+000002c0: 203c 2f73 656c 6563 743e 0a20 2020 207b   </select>.    {
+000002d0: 2520 656e 6469 6620 257d 0a20 2020 203c  % endif %}.    <
+000002e0: 6469 7620 6964 3d22 6670 223e 3c2f 6469  div id="fp"></di
+000002f0: 763e 0a20 203c 2f64 6976 3e0a 2020 3c64  v>.  </div>.  <d
+00000300: 6976 2063 6c61 7373 3d22 7370 616e 2d38  iv class="span-8
+00000310: 206c 6173 7422 3e0a 2020 2020 3c66 6f72   last">.    <for
+00000320: 6d20 6e61 6d65 3d22 7061 7468 2d66 6f72  m name="path-for
+00000330: 6d22 3e0a 2020 2020 2020 3c69 6e70 7574  m">.      <input
+00000340: 2069 643d 2268 6964 6465 6e2d 7061 7468   id="hidden-path
+00000350: 2220 6e61 6d65 3d22 7061 7468 2220 7479  " name="path" ty
+00000360: 7065 3d22 6869 6464 656e 2220 7661 6c75  pe="hidden" valu
+00000370: 653d 2222 3e0a 2020 2020 2020 3c64 6976  e="">.      <div
+00000380: 2069 643d 226d 6973 7369 6e67 2d6e 616d   id="missing-nam
+00000390: 6522 3e3c 2f64 6976 3e0a 2020 2020 2020  e"></div>.      
+000003a0: 3c62 7574 746f 6e20 6964 3d22 7375 626d  <button id="subm
+000003b0: 6974 2d70 6174 6822 2074 7970 653d 2273  it-path" type="s
+000003c0: 7562 6d69 7422 2073 7479 6c65 3d22 223e  ubmit" style="">
+000003d0: 496d 706f 7274 204c 4349 4120 6d65 7468  Import LCIA meth
+000003e0: 6f64 2873 293c 2f62 7574 746f 6e3e 0a20  od(s)</button>. 
+000003f0: 2020 203c 2f66 6f72 6d3e 0a20 203c 2f64     </form>.  </d
+00000400: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
+00000410: 2069 643d 2269 6e2d 7375 626d 6973 7369   id="in-submissi
+00000420: 6f6e 2220 636c 6173 733d 2273 7061 6e2d  on" class="span-
+00000430: 3234 2063 6c65 6172 223e 0a20 203c 6833  24 clear">.  <h3
+00000440: 3e59 6f75 7220 636f 6d70 7574 6572 2069  >Your computer i
+00000450: 7320 6e6f 7720 776f 726b 696e 6720 6173  s now working as
+00000460: 2066 6173 7420 6173 2069 7420 6361 6e20   fast as it can 
+00000470: 696d 706f 7274 696e 6720 7468 6520 4c43  importing the LC
+00000480: 4941 206d 6574 686f 6428 7329 2e3c 2f68  IA method(s).</h
+00000490: 333e 0a20 203c 703e 506c 6561 7365 2062  3>.  <p>Please b
+000004a0: 6520 7061 7469 656e 742e 2e2e 2079 6f75  e patient... you
+000004b0: 2077 696c 6c20 6265 2072 6564 6972 6563   will be redirec
+000004c0: 7465 6420 746f 2074 6865 2068 6f6d 6520  ted to the home 
+000004d0: 7061 6765 2061 7320 736f 6f6e 2061 7320  page as soon as 
+000004e0: 7468 6520 696d 706f 7274 2069 7320 6669  the import is fi
+000004f0: 6e69 7368 6564 2e3c 2f70 3e0a 3c2f 6469  nished.</p>.</di
+00000500: 763e 0a0a 3c73 6372 6970 7420 7479 7065  v>..<script type
+00000510: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
+00000520: 7422 3e0a 6675 6e63 7469 6f6e 2066 7073  t">.function fps
+00000530: 656c 6563 746f 7220 2861 2920 7b0a 2020  elector (a) {.  
+00000540: 2428 2223 6670 2d73 656c 6563 7465 6422  $("#fp-selected"
+00000550: 292e 7465 7874 2822 4375 7272 656e 746c  ).text("Currentl
+00000560: 7920 7365 6c65 6374 6564 3a20 2220 2b20  y selected: " + 
+00000570: 612e 6174 7472 2827 7265 6c27 2929 3b0a  a.attr('rel'));.
+00000580: 2020 2428 2223 6869 6464 656e 2d70 6174    $("#hidden-pat
+00000590: 6822 292e 7661 6c28 612e 6174 7472 2827  h").val(a.attr('
+000005a0: 7265 6c27 2929 3b0a 7d3b 0a3c 2f73 6372  rel'));.};.</scr
+000005b0: 6970 743e 0a3c 7363 7269 7074 2073 7263  ipt>.<script src
+000005c0: 3d22 7b7b 2075 726c 5f66 6f72 2827 7374  ="{{ url_for('st
+000005d0: 6174 6963 272c 2066 696c 656e 616d 653d  atic', filename=
+000005e0: 226a 7175 6572 7946 696c 6554 7265 652f  "jqueryFileTree/
+000005f0: 6a71 7565 7279 4669 6c65 5472 6565 2e6a  jqueryFileTree.j
+00000600: 7322 2920 7d7d 223e 3c2f 7363 7269 7074  s") }}"></script
+00000610: 3e0a 3c73 6372 6970 7420 7479 7065 3d22  >.<script type="
+00000620: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00000630: 3e0a 2428 646f 6375 6d65 6e74 292e 7265  >.$(document).re
+00000640: 6164 7928 2066 756e 6374 696f 6e28 2920  ady( function() 
+00000650: 7b0a 2020 2428 2223 696e 2d73 7562 6d69  {.  $("#in-submi
+00000660: 7373 696f 6e22 292e 6869 6465 2829 3b0a  ssion").hide();.
+00000670: 0a20 2024 2827 2366 7027 292e 6669 6c65  .  $('#fp').file
+00000680: 5472 6565 287b 0a20 2020 2072 6f6f 743a  Tree({.    root:
+00000690: 2027 2f27 2c0a 2020 2020 7363 7269 7074   '/',.    script
+000006a0: 3a20 277b 7b20 7572 6c5f 666f 7228 2766  : '{{ url_for('f
+000006b0: 705f 6170 6927 2920 7d7d 3f66 756c 6c3d  p_api') }}?full=
+000006c0: 3127 2c0a 2020 2020 666f 6c64 6572 4576  1',.    folderEv
+000006d0: 656e 743a 2027 636c 6963 6b27 2c0a 2020  ent: 'click',.  
+000006e0: 2020 6d75 6c74 6946 6f6c 6465 723a 2066    multiFolder: f
+000006f0: 616c 7365 0a20 2020 207d 2c0a 2020 2020  alse.    },.    
+00000700: 6675 6e63 7469 6f6e 2866 696c 6529 207b  function(file) {
+00000710: 0a20 2020 2020 2024 2822 2366 702d 7365  .      $("#fp-se
+00000720: 6c65 6374 6564 2229 2e74 6578 7428 2243  lected").text("C
+00000730: 7572 7265 6e74 6c79 2073 656c 6563 7465  urrently selecte
+00000740: 643a 2022 202b 2066 696c 6529 3b0a 2020  d: " + file);.  
+00000750: 2020 2020 2428 2223 6869 6464 656e 2d70      $("#hidden-p
+00000760: 6174 6822 292e 7661 6c28 6669 6c65 293b  ath").val(file);
+00000770: 0a20 2020 207d 0a20 2029 3b0a 0a20 2024  .    }.  );..  $
+00000780: 2827 666f 726d 5b6e 616d 653d 7061 7468  ('form[name=path
+00000790: 2d66 6f72 6d5d 2729 2e73 7562 6d69 7428  -form]').submit(
+000007a0: 2066 756e 6374 696f 6e20 2865 2920 7b0a   function (e) {.
+000007b0: 2020 2020 652e 7072 6576 656e 7444 6566      e.preventDef
+000007c0: 6175 6c74 2829 3b0a 2020 2020 6966 2028  ault();.    if (
+000007d0: 2428 2223 6869 6464 656e 2d70 6174 6822  $("#hidden-path"
+000007e0: 292e 7661 6c28 2920 213d 2027 2729 207b  ).val() != '') {
+000007f0: 0a20 2020 2020 2024 2822 2369 6e2d 7375  .      $("#in-su
+00000800: 626d 6973 7369 6f6e 2229 2e73 686f 7728  bmission").show(
+00000810: 293b 0a20 2020 2020 2024 2822 2373 656c  );.      $("#sel
+00000820: 6563 742d 7061 7468 2229 2e68 6964 6528  ect-path").hide(
+00000830: 293b 0a20 2020 2020 2024 2e61 6a61 7828  );.      $.ajax(
+00000840: 7b0a 2020 2020 2020 2020 7479 7065 3a20  {.        type: 
+00000850: 2250 4f53 5422 2c0a 2020 2020 2020 2020  "POST",.        
+00000860: 7572 6c3a 2027 7b7b 2075 726c 5f66 6f72  url: '{{ url_for
+00000870: 2827 696d 706f 7274 5f6d 6574 686f 6427  ('import_method'
+00000880: 2920 7d7d 272c 0a20 2020 2020 2020 2064  ) }}',.        d
+00000890: 6174 613a 2024 2874 6869 7329 2e73 6572  ata: $(this).ser
+000008a0: 6961 6c69 7a65 2829 2c0a 2020 2020 2020  ialize(),.      
+000008b0: 2020 7375 6363 6573 733a 2066 756e 6374    success: funct
+000008c0: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
+000008d0: 2020 2064 6f63 756d 656e 742e 6c6f 6361     document.loca
+000008e0: 7469 6f6e 2e68 7265 663d 277b 7b20 7572  tion.href='{{ ur
+000008f0: 6c5f 666f 7228 2769 6e64 6578 2729 207d  l_for('index') }
+00000900: 7d27 3b0a 2020 2020 2020 2020 7d0a 2020  }';.        }.  
+00000910: 2020 2020 7d29 3b0a 2020 2020 7d20 656c      });.    } el
+00000920: 7365 207b 0a20 2020 2020 2024 2822 236d  se {.      $("#m
+00000930: 6973 7369 6e67 2d6e 616d 6522 292e 6874  issing-name").ht
+00000940: 6d6c 2827 3c70 2073 7479 6c65 3d22 636f  ml('<p style="co
+00000950: 6c6f 723a 2072 6564 223e 596f 7520 6d75  lor: red">You mu
+00000960: 7374 2066 6972 7374 2073 656c 6563 7420  st first select 
+00000970: 626f 7468 2061 2066 696c 652f 6469 7265  both a file/dire
+00000980: 6374 6f72 793c 2f70 3e27 293b 0a20 2020  ctory</p>');.   
+00000990: 207d 0a20 207d 293b 0a7d 293b 0a0a 2428   }.  });.});..$(
+000009a0: 6675 6e63 7469 6f6e 2829 207b 0a20 2024  function() {.  $
+000009b0: 2822 2364 7269 7665 6c65 7474 6572 2229  ("#driveletter")
+000009c0: 2e63 6861 6e67 6528 6675 6e63 7469 6f6e  .change(function
+000009d0: 2829 207b 0a20 2020 2020 2076 6172 206c  () {.      var l
+000009e0: 6574 7465 7220 3d20 2428 7468 6973 292e  etter = $(this).
+000009f0: 7661 6c28 293b 0a20 2020 2020 2024 2827  val();.      $('
+00000a00: 2366 7027 292e 6874 6d6c 2822 2229 3b0a  #fp').html("");.
+00000a10: 2020 2020 2020 2428 2723 6670 2729 2e66        $('#fp').f
+00000a20: 696c 6554 7265 6528 7b0a 2020 2020 2020  ileTree({.      
+00000a30: 2020 726f 6f74 3a20 6c65 7474 6572 2c0a    root: letter,.
+00000a40: 2020 2020 2020 2020 7363 7269 7074 3a20          script: 
+00000a50: 272f 6670 2d61 7069 272c 0a20 2020 2020  '/fp-api',.     
+00000a60: 2020 2066 6f6c 6465 7245 7665 6e74 3a20     folderEvent: 
+00000a70: 2763 6c69 636b 272c 0a20 2020 2020 2020  'click',.       
+00000a80: 206d 756c 7469 466f 6c64 6572 3a20 6661   multiFolder: fa
+00000a90: 6c73 650a 2020 2020 2020 2020 7d2c 0a20  lse.        },. 
+00000aa0: 2020 2020 2020 2066 756e 6374 696f 6e28         function(
+00000ab0: 6669 6c65 2920 7b20 636f 6e73 6f6c 652e  file) { console.
+00000ac0: 6c6f 6728 6669 6c65 293b 207d 0a20 2020  log(file); }.   
+00000ad0: 2020 2029 3b0a 2020 7d29 0a7d 293b 0a3c     );.  }).});.<
+00000ae0: 2f73 6372 6970 743e 0a7b 2520 656e 6462  /script>.{% endb
+00000af0: 6c6f 636b 2025 7d0a                      lock %}.
```

### Comparing `bw2ui-0.8/bw2ui/web/templates/index.html` & `bw2ui-0.8.1/bw2ui/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/jsoneditor.html` & `bw2ui-0.8.1/bw2ui/web/templates/jsoneditor.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/method.html` & `bw2ui-0.8.1/bw2ui/web/templates/method.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/progress.html` & `bw2ui-0.8.1/bw2ui/web/templates/progress.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/report.html` & `bw2ui-0.8.1/bw2ui/web/templates/report.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/select.html` & `bw2ui-0.8.1/bw2ui/web/templates/select.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/settings.html` & `bw2ui-0.8.1/bw2ui/web/templates/settings.html`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/bw2ui/web/templates/start.html` & `bw2ui-0.8.1/bw2ui/web/templates/start.html`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     <h3 id="fp-selected">1. Click to select the directory that Brightway2 data will be saved in</h3>
     <p>You <b>must</b> have permission to write to this directory!</p>
     <p>Note: Not all files are shown! You are selecting a directory, not files...</p>
     {% if windows %}
       <h3>Change the drive (Windows only)</h3>
       <select id="driveletter">
       {% for letter in drive_letters %}
-        <option value="{{ letter }}">{{ letter }}</option>
+        <option value="{{ letter }}" {% if letter[:2] == current_drive %}selected{% endif %}>{{ letter }}</option>
       {% endfor %}
       </select>
     {% endif %}
     <div id="fp"></div>
   </div>
   <div class="span-8 last">
     <form name="path-form">
```

### Comparing `bw2ui-0.8/bw2ui.egg-info/PKG-INFO` & `bw2ui-0.8.1/bw2ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bw2ui
-Version: 0.8
+Version: 0.8.1
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/cmutel/brightway2-ui
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: Copyright (c) 2013, Chris Mutel and ETH Zürich
 All rights reserved.
```

### Comparing `bw2ui-0.8/bw2ui.egg-info/SOURCES.txt` & `bw2ui-0.8.1/bw2ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/LICENSE.txt` & `bw2ui-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2ui-0.8/PKG-INFO` & `bw2ui-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bw2ui
-Version: 0.8
+Version: 0.8.1
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/cmutel/brightway2-ui
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: Copyright (c) 2013, Chris Mutel and ETH Zürich
 All rights reserved.
```

### Comparing `bw2ui-0.8/setup.py` & `bw2ui-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bw2ui',
-    version="0.8",
+    version="0.8.1",
     packages=["bw2ui", "bw2ui.web"],
     package_data={'bw2ui.web': [
         "static/blueprint/*.css",
         "static/blueprint/plugins/buttons/*.css",
         "static/blueprint/plugins/fancy-type/*.css",
         "static/jqueryFileTree/*.css",
         "static/jqueryFileTree/*.js",
```

