# Comparing `tmp/bw25ui-0.36.0.tar.gz` & `tmp/bw25ui-0.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw25ui-0.36.0.tar", last modified: Mon Mar 18 13:59:18 2024, max compression
+gzip compressed data, was "bw25ui-0.37.0.tar", last modified: Tue Apr 16 10:31:48 2024, max compression
```

## Comparing `bw25ui-0.36.0.tar` & `bw25ui-0.37.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.602828 bw25ui-0.36.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-18 13:59:10.000000 bw25ui-0.36.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-18 13:59:10.000000 bw25ui-0.36.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-18 13:59:18.602828 bw25ui-0.36.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-18 13:59:10.000000 bw25ui-0.36.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-18 13:59:10.000000 bw25ui-0.36.0/TODO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.602828 bw25ui-0.36.0/bw25ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 13:59:18.000000 bw25ui-0.36.0/bw25ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.586828 bw25ui-0.36.0/bw2ui/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59353 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/bin/bw2_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/bin/bw2_web.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.586828 bw25ui-0.36.0/bw2ui/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/backgrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid-table.js
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid.css
--rw-r--r--   0 runner    (1001) docker     (127)    93706 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/blueprint/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/blueprint/ie.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.586828 bw25ui-0.36.0/bw2ui/web/static/blueprint/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/blueprint/plugins/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/blueprint/plugins/buttons/screen.css
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/blueprint/print.css
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/blueprint/screen.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/css/hypertree.css
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/css/pure-bw2.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/d3-tip/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/d3-tip/d3-tip.css
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/d3-tip/d3-tip.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/img/light_wool.png
--rw-r--r--   0 runner    (1001) docker     (127)    77595 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/img/linedpaper.png
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/img/llama.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/img/monster.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.590828 bw25ui-0.36.0/bw2ui/web/static/jit/
--rw-r--r--   0 runner    (1001) docker     (127)   162463 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jit/jit-yc.js
--rw-r--r--   0 runner    (1001) docker     (127)   490615 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jit/jit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.594828 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.598828 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/application.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/code.png
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/css.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/db.png
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/directory.png
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/doc.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/file.png
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/film.png
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/flash.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/folder_open.png
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/html.png
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/java.png
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/linux.png
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/music.png
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/pdf.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/php.png
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/picture.png
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/ppt.png
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/psd.png
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/ruby.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/script.png
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/spinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/txt.png
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/xls.png
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/zip.png
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.598828 bw25ui-0.36.0/bw2ui/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/hinton.js
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/hypertree.js
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/interp-histogram.js
--rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/mustache.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/stepped-histogram.js
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/js/treemap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.598828 bw25ui-0.36.0/bw2ui/web/static/jstree/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3121 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jstree/32px.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1880 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jstree/40px.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   108473 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jstree/jstree.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    24311 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jstree/style.min.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/static/jstree/throbber.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:59:18.602828 bw25ui-0.36.0/bw2ui/web/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/activity.html
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/database.html
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/database_tree.html
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/facets.html
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/fp-select.html
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/fp.html
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/health-check.html
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/hist.html
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/import-database.html
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/import-method.html
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/jsoneditor.html
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/method.html
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/templates/start.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-03-18 13:59:10.000000 bw25ui-0.36.0/bw2ui/web/web_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-18 13:59:15.000000 bw25ui-0.36.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 13:59:18.602828 bw25ui-0.36.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-18 13:59:10.000000 bw25ui-0.36.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.641583 bw25ui-0.37.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 10:31:43.000000 bw25ui-0.37.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 10:31:43.000000 bw25ui-0.37.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 10:31:48.641583 bw25ui-0.37.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-16 10:31:43.000000 bw25ui-0.37.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-16 10:31:43.000000 bw25ui-0.37.0/TODO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.637583 bw25ui-0.37.0/bw25ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 10:31:48.000000 bw25ui-0.37.0/bw25ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60283 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/bin/bw2_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/bin/bw2_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.621583 bw25ui-0.37.0/bw2ui/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/static/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid-table.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid.css
+-rw-r--r--   0 runner    (1001) docker     (127)    93706 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/static/blueprint/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/blueprint/ie.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.621583 bw25ui-0.37.0/bw2ui/web/static/blueprint/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/static/blueprint/plugins/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/blueprint/plugins/buttons/screen.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/blueprint/print.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/blueprint/screen.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/css/hypertree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/css/pure-bw2.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.625583 bw25ui-0.37.0/bw2ui/web/static/d3-tip/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/d3-tip/d3-tip.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/d3-tip/d3-tip.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.629583 bw25ui-0.37.0/bw2ui/web/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/img/light_wool.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77595 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/img/linedpaper.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/img/llama.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/img/monster.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.629583 bw25ui-0.37.0/bw2ui/web/static/jit/
+-rw-r--r--   0 runner    (1001) docker     (127)   162463 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jit/jit-yc.js
+-rw-r--r--   0 runner    (1001) docker     (127)   490615 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jit/jit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.629583 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.633583 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/application.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/code.png
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/css.png
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/db.png
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/directory.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/film.png
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/flash.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/folder_open.png
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/html.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/java.png
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/linux.png
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/music.png
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/pdf.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/php.png
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/ppt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/psd.png
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/ruby.png
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/script.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/txt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/xls.png
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/zip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.633583 bw25ui-0.37.0/bw2ui/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/hinton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/hypertree.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/interp-histogram.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/mustache.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/stepped-histogram.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/js/treemap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.633583 bw25ui-0.37.0/bw2ui/web/static/jstree/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3121 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jstree/32px.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1880 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jstree/40px.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108473 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jstree/jstree.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24311 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jstree/style.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/static/jstree/throbber.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:31:48.637583 bw25ui-0.37.0/bw2ui/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/activity.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/database.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/database_tree.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/facets.html
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/fp-select.html
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/fp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/health-check.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/hist.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/import-database.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/import-method.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/jsoneditor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/method.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/templates/start.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-04-16 10:31:43.000000 bw25ui-0.37.0/bw2ui/web/web_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-16 10:31:46.000000 bw25ui-0.37.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:31:48.641583 bw25ui-0.37.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 10:31:43.000000 bw25ui-0.37.0/setup.py
```

### Comparing `bw25ui-0.36.0/LICENSE` & `bw25ui-0.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/PKG-INFO` & `bw25ui-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw25ui
-Version: 0.36.0
+Version: 0.37.0
 Summary: A web and command line user interface, part of the Brightway2 LCA framework https://brightway.dev.
 Author-email: Chris Mutel <cmutel@gmail.com>
 Maintainer-email: Tomás NAVARRETE GUTIÉRREZ <tngTUDOR@users.noreply.github.com>
 Project-URL: source, https://github.com/brightway-lca/brightway2-ui
 Project-URL: homepage, https://github.com/brightway-lca/brightway2-ui
 Project-URL: tracker, https://github.com/brightway-lca/brightway2-ui/issues
 Classifier: Development Status :: 4 - Beta
@@ -45,15 +45,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: myst_parser==2.0.0; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
-Requires-Dist: sphinx-click==4.1.0; extra == "docs"
 
 # Brightway2-UI
 
 This is now the official repo for  Brightway2-UI:
 
 > a web and command line user interface, part of the **Brightway2 LCA framework** <https://brightway.dev>.
```

### Comparing `bw25ui-0.36.0/README.md` & `bw25ui-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw25ui.egg-info/PKG-INFO` & `bw25ui-0.37.0/bw25ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw25ui
-Version: 0.36.0
+Version: 0.37.0
 Summary: A web and command line user interface, part of the Brightway2 LCA framework https://brightway.dev.
 Author-email: Chris Mutel <cmutel@gmail.com>
 Maintainer-email: Tomás NAVARRETE GUTIÉRREZ <tngTUDOR@users.noreply.github.com>
 Project-URL: source, https://github.com/brightway-lca/brightway2-ui
 Project-URL: homepage, https://github.com/brightway-lca/brightway2-ui
 Project-URL: tracker, https://github.com/brightway-lca/brightway2-ui/issues
 Classifier: Development Status :: 4 - Beta
@@ -45,15 +45,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: myst_parser==2.0.0; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
-Requires-Dist: sphinx-click==4.1.0; extra == "docs"
 
 # Brightway2-UI
 
 This is now the official repo for  Brightway2-UI:
 
 > a web and command line user interface, part of the **Brightway2 LCA framework** <https://brightway.dev>.
```

### Comparing `bw25ui-0.36.0/bw25ui.egg-info/SOURCES.txt` & `bw25ui-0.37.0/bw25ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/bin/bw2_browser.py` & `bw25ui-0.37.0/bw2ui/bin/bw2_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 Options:
   -h --help     Show this screen.
   --version     Show version.
 
 """
 from __future__ import print_function, unicode_literals
 
-import bw2analyzer as bwa
 import cmd
 import codecs
 import itertools
 import math
 import os
 import pprint
 import re
 import textwrap
 import threading
 import time
 import traceback
 import uuid
 import warnings
 import webbrowser
+
+import bw2analyzer as bwa
 from bw2calc import MultiLCA
 from bw2data import (
     Database,
     Method,
     calculation_setups,
     config,
     databases,
@@ -46,14 +47,15 @@
 )
 from bw2data.parameters import (
     ActivityParameter,
     DatabaseParameter,
     Group,
     ProjectParameter,
 )
+from bw2data.query import Filter, Query
 from docopt import docopt
 from tabulate import tabulate
 
 warnings.filterwarnings("ignore", ".*Read only project.*")
 
 GRUMPY = itertools.cycle(
     (
@@ -1082,30 +1084,42 @@
             search_criterion = None
             if "-loc" in arg:
                 re1a = r"(-loc\s)"  # Any Single Whitespace Character 1
                 search_criterion = "location"
             elif "-cat" in arg:
                 re1a = r"(-cat\s)"  # Any Single Whitespace Character 1
                 search_criterion = "category"
+            elif "-cas" in arg:
+                re1a = r"(-cas\s)"  # Any Single Whitespace Character 1
+                search_criterion = "CAS number"
             elif "-rp" in arg:
                 re1a = r"(-rp\s)"  # Any Single Whitespace Character 1
                 search_criterion = "reference product"
             re1b = r"(\{.*\})"  # Curly Braces 1
             re2 = (
                 r"(?:\s(.+))?"  # at least a space, and then 1 to n chars, but optional
             )
             rg = re.compile(re1a + re1b + re2, re.IGNORECASE | re.DOTALL)
             m = rg.search(arg)
             needle = arg  # Find the needle in the haystack
             if m is None and "-loc" in arg:
                 print("Missing location in curly braces in command: -loc {MX} ...")
                 return
-            elif m is None and "-cat " in arg:
+            elif m is None and "-cat" in arg:
                 print("Missing category in curly braces in command: -cat {water} ...")
                 return
+            elif m is None and "-cas" in arg:
+                print(
+                    "Missing CAS Number in curly braces in command: -cas {000095-50-1} \
+                            ..."
+                )
+                return
+            elif "-cas" in arg and "biosphere" not in self.database:
+                print("CAS Number search only for biosphere dbs.")
+                return
             elif m is None and "-rp" in arg:
                 print(
                     "Missing reference product in curly braces in command: -rp "
                     "{electricity high voltage} ..."
                 )
                 return
             elif m:
@@ -1159,14 +1173,21 @@
                 else:
                     criteria = {"product": criterion_value}
                     results = Database(self.database).search(
                         needle,
                         filter=criteria,
                         limit=self.search_limit,
                     )
+            elif m and search_criterion == "CAS number":
+                q = Query()
+                filter_cas = Filter("CAS number", "is", criterion_value)
+                bio_db_data = Database(self.database).load()
+                q.add(filter_cas)
+                res = q(bio_db_data)
+                results = [get_activity(r) for r in res]
             else:
                 results = Database(self.database).search(
                     needle, limit=self.search_limit
                 )
             results_keys = [r.key for r in results]
             self.set_current_options(
                 {
```

### Comparing `bw25ui-0.36.0/bw2ui/bin/bw2_web.py` & `bw25ui-0.37.0/bw2ui/bin/bw2_web.py`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/notebook.py` & `bw25ui-0.37.0/bw2ui/notebook.py`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/jobs.py` & `bw25ui-0.37.0/bw2ui/web/jobs.py`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid-table.js` & `bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid-table.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid.css` & `bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/backgrid/backgrid.js` & `bw25ui-0.37.0/bw2ui/web/static/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/blueprint/ie.css` & `bw25ui-0.37.0/bw2ui/web/static/blueprint/ie.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/blueprint/plugins/buttons/screen.css` & `bw25ui-0.37.0/bw2ui/web/static/blueprint/plugins/buttons/screen.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/blueprint/print.css` & `bw25ui-0.37.0/bw2ui/web/static/blueprint/print.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/blueprint/screen.css` & `bw25ui-0.37.0/bw2ui/web/static/blueprint/screen.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/css/base.css` & `bw25ui-0.37.0/bw2ui/web/static/css/base.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/css/pure-bw2.css` & `bw25ui-0.37.0/bw2ui/web/static/css/pure-bw2.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/d3-tip/d3-tip.js` & `bw25ui-0.37.0/bw2ui/web/static/d3-tip/d3-tip.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/img/favicon.ico` & `bw25ui-0.37.0/bw2ui/web/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/img/light_wool.png` & `bw25ui-0.37.0/bw2ui/web/static/img/light_wool.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/img/linedpaper.png` & `bw25ui-0.37.0/bw2ui/web/static/img/linedpaper.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/img/llama.jpg` & `bw25ui-0.37.0/bw2ui/web/static/img/llama.jpg`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/img/monster.jpg` & `bw25ui-0.37.0/bw2ui/web/static/img/monster.jpg`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jit/jit-yc.js` & `bw25ui-0.37.0/bw2ui/web/static/jit/jit-yc.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jit/jit.js` & `bw25ui-0.37.0/bw2ui/web/static/jit/jit.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/code.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/code.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/css.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/css.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/db.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/db.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/directory.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/directory.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/doc.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/doc.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/film.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/film.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/flash.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/flash.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/folder_open.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/folder_open.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/html.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/html.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/java.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/java.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/linux.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/linux.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/pdf.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/pdf.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/php.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/php.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/picture.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/picture.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/ppt.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/ppt.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/psd.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/psd.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/ruby.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/ruby.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/script.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/script.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/spinner.gif` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/images/xls.png` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/images/xls.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js` & `bw25ui-0.37.0/bw2ui/web/static/jqueryFileTree/jqueryFileTree.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/hinton.js` & `bw25ui-0.37.0/bw2ui/web/static/js/hinton.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/hypertree.js` & `bw25ui-0.37.0/bw2ui/web/static/js/hypertree.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/interp-histogram.js` & `bw25ui-0.37.0/bw2ui/web/static/js/interp-histogram.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/mustache.js` & `bw25ui-0.37.0/bw2ui/web/static/js/mustache.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/stepped-histogram.js` & `bw25ui-0.37.0/bw2ui/web/static/js/stepped-histogram.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/js/treemap.js` & `bw25ui-0.37.0/bw2ui/web/static/js/treemap.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jstree/32px.png` & `bw25ui-0.37.0/bw2ui/web/static/jstree/32px.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jstree/40px.png` & `bw25ui-0.37.0/bw2ui/web/static/jstree/40px.png`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jstree/jstree.min.js` & `bw25ui-0.37.0/bw2ui/web/static/jstree/jstree.min.js`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jstree/style.min.css` & `bw25ui-0.37.0/bw2ui/web/static/jstree/style.min.css`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/static/jstree/throbber.gif` & `bw25ui-0.37.0/bw2ui/web/static/jstree/throbber.gif`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/activity.html` & `bw25ui-0.37.0/bw2ui/web/templates/activity.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/base.html` & `bw25ui-0.37.0/bw2ui/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/database.html` & `bw25ui-0.37.0/bw2ui/web/templates/database.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/database_tree.html` & `bw25ui-0.37.0/bw2ui/web/templates/database_tree.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/facets.html` & `bw25ui-0.37.0/bw2ui/web/templates/facets.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/fp.html` & `bw25ui-0.37.0/bw2ui/web/templates/fp.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/health-check.html` & `bw25ui-0.37.0/bw2ui/web/templates/health-check.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/hist.html` & `bw25ui-0.37.0/bw2ui/web/templates/hist.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/import-database.html` & `bw25ui-0.37.0/bw2ui/web/templates/import-database.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/import-method.html` & `bw25ui-0.37.0/bw2ui/web/templates/import-method.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/index.html` & `bw25ui-0.37.0/bw2ui/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/jsoneditor.html` & `bw25ui-0.37.0/bw2ui/web/templates/jsoneditor.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/method.html` & `bw25ui-0.37.0/bw2ui/web/templates/method.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/progress.html` & `bw25ui-0.37.0/bw2ui/web/templates/progress.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/report.html` & `bw25ui-0.37.0/bw2ui/web/templates/report.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/search.html` & `bw25ui-0.37.0/bw2ui/web/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/select.html` & `bw25ui-0.37.0/bw2ui/web/templates/select.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/settings.html` & `bw25ui-0.37.0/bw2ui/web/templates/settings.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/templates/start.html` & `bw25ui-0.37.0/bw2ui/web/templates/start.html`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/utils.py` & `bw25ui-0.37.0/bw2ui/web/utils.py`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/bw2ui/web/web_app.py` & `bw25ui-0.37.0/bw2ui/web/web_app.py`

 * *Files identical despite different names*

### Comparing `bw25ui-0.36.0/pyproject.toml` & `bw25ui-0.37.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "pytest-randomly",
     "setuptools",
 ]
 docs = [
     "furo==2024.1.29",
     "myst_parser==2.0.0",
     "sphinx==7.2.6",
-    "sphinx-click==4.1.0",
 ]
 
 [project.scripts]
 bw2-web = "bw2ui.bin.bw2_web:main"
 bw2-browser = "bw2ui.bin.bw2_browser:main"
 
 [tool.setuptools]
```

