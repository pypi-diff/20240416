# Comparing `tmp/analogic-framework-4.1.8.tar.gz` & `tmp/analogic-framework-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogic-framework-4.1.8.tar", last modified: Mon Aug 28 14:39:10 2023, max compression
+gzip compressed data, was "analogic-framework-4.1.9.tar", last modified: Thu Oct 12 15:32:31 2023, max compression
```

## Comparing `analogic-framework-4.1.8.tar` & `analogic-framework-4.1.9.tar`

### file list

```diff
@@ -1,263 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:10.012637 analogic-framework-4.1.8/
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-08-28 14:39:10.012637 analogic-framework-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    10066 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.960637 analogic-framework-4.1.8/analogic/
--rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    13027 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/analogic.py
--rw-r--r--   0 runner    (1001) docker     (999)    27489 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/analogic_tm1_service.py
--rw-r--r--   0 runner    (1001) docker     (999)    14633 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (999)     8086 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/cam.py
--rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/camsecure.py
--rw-r--r--   0 runner    (1001) docker     (999)      150 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/condition.py
--rw-r--r--   0 runner    (1001) docker     (999)     1772 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/core_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (999)     2540 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/email.py
--rw-r--r--   0 runner    (1001) docker     (999)     2245 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (999)      616 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)      524 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/loader.py
--rw-r--r--   0 runner    (1001) docker     (999)     3604 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/logging.json
--rw-r--r--   0 runner    (1001) docker     (999)     4442 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/loginbasic.py
--rw-r--r--   0 runner    (1001) docker     (999)      742 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/logincam.py
--rw-r--r--   0 runner    (1001) docker     (999)     1195 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/nologin.py
--rw-r--r--   0 runner    (1001) docker     (999)    14761 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/pivot.py
--rw-r--r--   0 runner    (1001) docker     (999)     5373 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.952637 analogic-framework-4.1.8/analogic/static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.952637 analogic-framework-4.1.8/analogic/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.960637 analogic-framework-4.1.8/analogic/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (999)    48488 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (999)   108539 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/bootstrap-grid.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.960637 analogic-framework-4.1.8/analogic/static/assets/css/lib/
--rw-r--r--   0 runner    (1001) docker     (999)      521 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/lib/Chart-2.9.3.min.css
--rw-r--r--   0 runner    (1001) docker     (999)     4220 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/lib/nouislider.min.css
--rw-r--r--   0 runner    (1001) docker     (999)    65538 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.960637 analogic-framework-4.1.8/analogic/static/assets/css/widgets/
--rw-r--r--   0 runner    (1001) docker     (999)      288 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/widgets/loader.css
--rw-r--r--   0 runner    (1001) docker     (999)     2000 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/css/widgets/simulation-panel-slider.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.964637 analogic-framework-4.1.8/analogic/static/assets/images/
--rw-r--r--   0 runner    (1001) docker     (999)    10487 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (999)   120349 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/images/loading2.gif
--rw-r--r--   0 runner    (1001) docker     (999)    55508 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/images/loading2_transparent.gif
--rw-r--r--   0 runner    (1001) docker     (999)     1074 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/images/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.952637 analogic-framework-4.1.8/analogic/static/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.964637 analogic-framework-4.1.8/analogic/static/assets/js/framework/
--rw-r--r--   0 runner    (1001) docker     (999)    20738 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/api.js
--rw-r--r--   0 runner    (1001) docker     (999)     3271 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/app.js
--rw-r--r--   0 runner    (1001) docker     (999)     3484 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/authentication.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.964637 analogic-framework-4.1.8/analogic/static/assets/js/framework/extensions/
--rw-r--r--   0 runner    (1001) docker     (999)       74 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/extensions/app-initialization.js
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/extensions/authentication-provider.js
--rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/extensions/page-render.js
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/extensions/write-executor.js
--rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/listener.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.968637 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/
--rw-r--r--   0 runner    (1001) docker     (999)     2385 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/array.js
--rw-r--r--   0 runner    (1001) docker     (999)     3788 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (999)      155 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/default.js
--rw-r--r--   0 runner    (1001) docker     (999)     3885 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/skip.js
--rw-r--r--   0 runner    (1001) docker     (999)      244 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/state.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.968637 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/
--rw-r--r--   0 runner    (1001) docker     (999)      591 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/base.js
--rw-r--r--   0 runner    (1001) docker     (999)     1397 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/factory.js
--rw-r--r--   0 runner    (1001) docker     (999)      457 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/list.js
--rw-r--r--   0 runner    (1001) docker     (999)      780 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/matrix.js
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/object.js
--rw-r--r--   0 runner    (1001) docker     (999)      234 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/script.js
--rw-r--r--   0 runner    (1001) docker     (999)      135 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/skip.js
--rw-r--r--   0 runner    (1001) docker     (999)      579 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/pivot.js
--rw-r--r--   0 runner    (1001) docker     (999)     3606 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/query-builder.js
--rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/redirect.js
--rw-r--r--   0 runner    (1001) docker     (999)      381 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/render.js
--rw-r--r--   0 runner    (1001) docker     (999)      176 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/rest-request.js
--rw-r--r--   0 runner    (1001) docker     (999)     1523 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/server.js
--rw-r--r--   0 runner    (1001) docker     (999)    22944 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.972637 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/
--rw-r--r--   0 runner    (1001) docker     (999)     4733 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (999)      177 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/download.js
--rw-r--r--   0 runner    (1001) docker     (999)     5735 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (999)      715 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/function.js
--rw-r--r--   0 runner    (1001) docker     (999)     2054 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (999)      352 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/skip.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.972637 analogic-framework-4.1.8/analogic/static/assets/js/lib/
--rw-r--r--   0 runner    (1001) docker     (999)   172689 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/Chart-2.9.3.min.js
--rw-r--r--   0 runner    (1001) docker     (999)    44136 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/Sortable.min.js
--rw-r--r--   0 runner    (1001) docker     (999)    12908 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
--rw-r--r--   0 runner    (1001) docker     (999)    21295 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.976637 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/
--rw-r--r--   0 runner    (1001) docker     (999)   204509 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (999)   950937 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chart.umd.js.map
--rw-r--r--   0 runner    (1001) docker     (999)    12937 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/init.js
--rw-r--r--   0 runner    (1001) docker     (999)     1154 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.976637 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/
--rw-r--r--   0 runner    (1001) docker     (999)    89411 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (999)     1239 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
--rw-r--r--   0 runner    (1001) docker     (999)     2981 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (999)      896 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
--rw-r--r--   0 runner    (1001) docker     (999)     1460 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/tableSort.js
--rw-r--r--   0 runner    (1001) docker     (999)    26460 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/lib/nouislider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.984637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.984637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (999)    23394 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/base/widget.js
--rw-r--r--   0 runner    (1001) docker     (999)    12486 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/button.js
--rw-r--r--   0 runner    (1001) docker     (999)    27762 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)     1709 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/container.js
--rw-r--r--   0 runner    (1001) docker     (999)    18887 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/datepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.992637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ButtonWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ContainerWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/DatePickerWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/DropBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/GaugeWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/GridCellWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/GridRowWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/GridWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        3 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ImageWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/PanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/PieChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/PopupWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)     1054 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SideBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/SwipeWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/TextAreaWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/TextBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/TextWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ToggleWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        3 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/WaterFallWidget.json
--rw-r--r--   0 runner    (1001) docker     (999)    11440 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/dropbox.js
--rw-r--r--   0 runner    (1001) docker     (999)     9323 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.992637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/
--rw-r--r--   0 runner    (1001) docker     (999)     1109 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid-cell.js
--rw-r--r--   0 runner    (1001) docker     (999)     1094 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid-row.js
--rw-r--r--   0 runner    (1001) docker     (999)      994 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.992637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/
--rw-r--r--   0 runner    (1001) docker     (999)     4822 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
--rw-r--r--   0 runner    (1001) docker     (999)     2683 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
--rw-r--r--   0 runner    (1001) docker     (999)     1626 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
--rw-r--r--   0 runner    (1001) docker     (999)    19047 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (999)    18115 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/histogram-combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)     2502 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontal-bar-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)    25693 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontal-table.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.996637 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/
--rw-r--r--   0 runner    (1001) docker     (999)     1138 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
--rw-r--r--   0 runner    (1001) docker     (999)      953 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
--rw-r--r--   0 runner    (1001) docker     (999)      962 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
--rw-r--r--   0 runner    (1001) docker     (999)     1295 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/image.js
--rw-r--r--   0 runner    (1001) docker     (999)    20015 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/line-area-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)    26764 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/line-scatter-combo.js
--rw-r--r--   0 runner    (1001) docker     (999)     1186 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/loader.js
--rw-r--r--   0 runner    (1001) docker     (999)     1328 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/page.js
--rw-r--r--   0 runner    (1001) docker     (999)      309 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/panel.js
--rw-r--r--   0 runner    (1001) docker     (999)     6271 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/pie-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)    81168 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/pivot-table.js
--rw-r--r--   0 runner    (1001) docker     (999)     7777 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/popup.js
--rw-r--r--   0 runner    (1001) docker     (999)     8149 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/radar-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)    36449 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/scroll-table.js
--rw-r--r--   0 runner    (1001) docker     (999)     2741 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-bar.js
--rw-r--r--   0 runner    (1001) docker     (999)      828 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-control-item.js
--rw-r--r--   0 runner    (1001) docker     (999)     4953 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-control.js
--rw-r--r--   0 runner    (1001) docker     (999)      184 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/shadow.js
--rw-r--r--   0 runner    (1001) docker     (999)     2067 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/simulation-panel-slider.js
--rw-r--r--   0 runner    (1001) docker     (999)     4840 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/simulation-panel.js
--rw-r--r--   0 runner    (1001) docker     (999)    19961 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/slider.js
--rw-r--r--   0 runner    (1001) docker     (999)    38388 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/stacked-column-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)     4956 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/swipe.js
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/system-popup.js
--rw-r--r--   0 runner    (1001) docker     (999)    21662 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/text.js
--rw-r--r--   0 runner    (1001) docker     (999)     4679 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/textarea.js
--rw-r--r--   0 runner    (1001) docker     (999)     5734 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/textbox.js
--rw-r--r--   0 runner    (1001) docker     (999)     7898 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/toggle.js
--rw-r--r--   0 runner    (1001) docker     (999)     4921 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/tornado-chart.js
--rw-r--r--   0 runner    (1001) docker     (999)     2779 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/vertical-line-box.js
--rw-r--r--   0 runner    (1001) docker     (999)    13579 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/js/widgets/water-fall.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:09.952637 analogic-framework-4.1.8/analogic/static/assets/skin/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:10.000637 analogic-framework-4.1.8/analogic/static/assets/skin/css/
--rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-button.css
--rw-r--r--   0 runner    (1001) docker     (999)      125 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-combo-chart.css
--rw-r--r--   0 runner    (1001) docker     (999)     1462 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-container.css
--rw-r--r--   0 runner    (1001) docker     (999)     3783 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (999)     1805 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-dropbox.css
--rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-gauge.css
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-general.css
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid-cell.css
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid-row.css
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid-table-cell.css
--rw-r--r--   0 runner    (1001) docker     (999)     1665 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid-table.css
--rw-r--r--   0 runner    (1001) docker     (999)     1310 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid.css
--rw-r--r--   0 runner    (1001) docker     (999)     2149 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-horizontal-table.css
--rw-r--r--   0 runner    (1001) docker     (999)     3706 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-horizontalbarchart.css
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-image.css
--rw-r--r--   0 runner    (1001) docker     (999)      175 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-legend.css
--rw-r--r--   0 runner    (1001) docker     (999)       75 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-line-area-chart.css
--rw-r--r--   0 runner    (1001) docker     (999)     1601 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-line-scatter-combo.css
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-page.css
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-panel.css
--rw-r--r--   0 runner    (1001) docker     (999)      292 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-pie-chart.css
--rw-r--r--   0 runner    (1001) docker     (999)    20239 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-pivot-table.css
--rw-r--r--   0 runner    (1001) docker     (999)     1388 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-popup.css
--rw-r--r--   0 runner    (1001) docker     (999)      332 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-radar-chart.css
--rw-r--r--   0 runner    (1001) docker     (999)     1655 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-scrolltable.css
--rw-r--r--   0 runner    (1001) docker     (999)      363 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-segmented.css
--rw-r--r--   0 runner    (1001) docker     (999)     1215 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-segmentedbar.css
--rw-r--r--   0 runner    (1001) docker     (999)      879 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-slider-touch.css
--rw-r--r--   0 runner    (1001) docker     (999)     1242 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-slider.css
--rw-r--r--   0 runner    (1001) docker     (999)      741 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-text.css
--rw-r--r--   0 runner    (1001) docker     (999)      765 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-textarea.css
--rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-textbox.css
--rw-r--r--   0 runner    (1001) docker     (999)      841 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-toggle.css
--rw-r--r--   0 runner    (1001) docker     (999)     2133 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-tornado.css
--rw-r--r--   0 runner    (1001) docker     (999)      667 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-vertical-line-box.css
--rw-r--r--   0 runner    (1001) docker     (999)     3553 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-waterfall.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:10.008637 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/
--rw-r--r--   0 runner    (1001) docker     (999)    75822 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (999)   253851 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
--rw-r--r--   0 runner    (1001) docker     (999)    75604 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    32032 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (999)    23076 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (999)    75582 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (999)   256592 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
--rw-r--r--   0 runner    (1001) docker     (999)    75356 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    32152 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (999)    23124 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (999)    26192 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.eot
--rw-r--r--   0 runner    (1001) docker     (999)   108091 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.svg
--rw-r--r--   0 runner    (1001) docker     (999)    26028 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    26104 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.woff
--rw-r--r--   0 runner    (1001) docker     (999)       70 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/task.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:10.008637 analogic-framework-4.1.8/analogic/templates/
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (999)      181 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (999)     2135 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/authenticated.html
--rw-r--r--   0 runner    (1001) docker     (999)      721 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (999)    10533 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (999)    12002 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/javascripts.html
--rw-r--r--   0 runner    (1001) docker     (999)     2972 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (999)      585 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/redirect.html
--rw-r--r--   0 runner    (1001) docker     (999)     2195 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/sso_error.html
--rw-r--r--   0 runner    (1001) docker     (999)      149 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/templates/unauthorized.html
--rw-r--r--   0 runner    (1001) docker     (999)        6 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/version.config
--rw-r--r--   0 runner    (1001) docker     (999)      181 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/analogic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:39:10.008637 analogic-framework-4.1.8/analogic_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-08-28 14:39:09.000000 analogic-framework-4.1.8/analogic_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    11515 2023-08-28 14:39:09.000000 analogic-framework-4.1.8/analogic_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:39:09.000000 analogic-framework-4.1.8/analogic_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      256 2023-08-28 14:39:09.000000 analogic-framework-4.1.8/analogic_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        9 2023-08-28 14:39:09.000000 analogic-framework-4.1.8/analogic_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       84 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 14:39:10.012637 analogic-framework-4.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      853 2023-08-28 14:38:45.000000 analogic-framework-4.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.309054 analogic-framework-4.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-12 15:32:31.309054 analogic-framework-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.253053 analogic-framework-4.1.9/analogic/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/__cli__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/analogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27489 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/analogic_tm1_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/cam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/camsecure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/core_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/logged_in_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/logging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/loginbasic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/logincam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/multi_authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/multi_authentication_provider_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/multi_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/nologin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.241053 analogic-framework-4.1.9/analogic/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.245053 analogic-framework-4.1.9/analogic/static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.253053 analogic-framework-4.1.9/analogic/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    48488 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   108539 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/bootstrap-grid.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.253053 analogic-framework-4.1.9/analogic/static/assets/css/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/lib/Chart-2.9.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/lib/nouislider.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    65538 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.253053 analogic-framework-4.1.9/analogic/static/assets/css/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/widgets/loader.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/css/widgets/simulation-panel-slider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.253053 analogic-framework-4.1.9/analogic/static/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   120349 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/images/loading2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    55508 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/images/loading2_transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/images/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.245053 analogic-framework-4.1.9/analogic/static/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.257053 analogic-framework-4.1.9/analogic/static/assets/js/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)    21218 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/api.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/authentication.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.261053 analogic-framework-4.1.9/analogic/static/assets/js/framework/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/extensions/app-initialization.js
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/extensions/authentication-provider.js
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/extensions/page-render.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/extensions/write-executor.js
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/listener.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.261053 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/default.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/skip.js
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/state.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.265053 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/factory.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/matrix.js
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/object.js
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/skip.js
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/query-builder.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/redirect.js
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/render.js
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/rest-request.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/server.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23044 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.265053 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/download.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/function.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/skip.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.265053 analogic-framework-4.1.9/analogic/static/assets/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)   172689 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/Chart-2.9.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44136 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/Sortable.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21295 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.269054 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/
+-rw-r--r--   0 runner    (1001) docker     (127)   204509 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)   950937 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chart.umd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.273054 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)    89411 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/tableSort.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26460 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/lib/nouislider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.281054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.281054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    23396 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/base/widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/button.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27762 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/container.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/datepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.289054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ButtonWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ContainerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/DatePickerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/DropBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/GaugeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/GridCellWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/GridRowWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/GridWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ImageWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/PanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/PieChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/PopupWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SideBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/SwipeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/TextAreaWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/TextBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/TextWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ToggleWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/WaterFallWidget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/dropbox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.289054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid-cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.293054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19047 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/histogram-combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontal-bar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontal-table.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.293054 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/image.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/line-area-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26764 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/line-scatter-combo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/page.js
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/panel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/pie-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81193 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/pivot-table.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/popup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/radar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36449 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/scroll-table.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-bar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-control-item.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-control.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/shadow.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/simulation-panel-slider.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/simulation-panel.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/slider.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38388 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/stacked-column-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/swipe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/system-popup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21662 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/text.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/textarea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/textbox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/toggle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/tornado-chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/vertical-line-box.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/js/widgets/water-fall.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.245053 analogic-framework-4.1.9/analogic/static/assets/skin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.301054 analogic-framework-4.1.9/analogic/static/assets/skin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-button.css
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-combo-chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-container.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-dropbox.css
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-gauge.css
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-general.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid-cell.css
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid-row.css
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid-table-cell.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid-table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-horizontal-table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-horizontalbarchart.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-image.css
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-legend.css
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-line-area-chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-line-scatter-combo.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-page.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-panel.css
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-pie-chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20239 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-pivot-table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-popup.css
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-radar-chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-scrolltable.css
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-segmented.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-segmentedbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-slider-touch.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-slider.css
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-text.css
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-textarea.css
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-textbox.css
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-toggle.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-tornado.css
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-vertical-line-box.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-waterfall.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.305054 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    75822 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   253851 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    75604 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    32032 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    23076 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    75582 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   256592 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    75356 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    32152 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    23124 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108091 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26028 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26104 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.woff
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.305054 analogic-framework-4.1.9/analogic/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/authenticated.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/javascripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/sso_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/templates/unauthorized.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/version.config
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/analogic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 15:32:31.309054 analogic-framework-4.1.9/analogic_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 15:32:31.000000 analogic-framework-4.1.9/analogic_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 15:32:31.309054 analogic-framework-4.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-12 15:32:10.000000 analogic-framework-4.1.9/setup.py
```

### Comparing `analogic-framework-4.1.8/LICENSE` & `analogic-framework-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/README.md` & `analogic-framework-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/analogic.py` & `analogic-framework-4.1.9/analogic/analogic.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from analogic.endpoint import AnalogicEndpoint
 import logging.config
 import json
 import sys
 from importlib import resources
 from analogic.core_endpoints import core_endpoints
 from analogic.authentication_provider import AuthenticationProvider
-from analogic.condition import Condition
 import inspect
 from analogic.setting import SettingManager
 from datetime import timedelta
 import importlib
 from analogic.task import scheduler
 import atexit
 
@@ -34,20 +33,22 @@
 
         self.endpoint_rules = []
         self.authentication_providers = {
             'Cam': 'analogic',
             'CamSecure': 'analogic',
             'LoginBasic': 'analogic',
             'LoginCam': 'analogic',
+            'MultiAuthenticationProvider': 'analogic',
             'NoLogin': 'analogic'
         }
         self.conditions = {}
         self.extension_assets = {}
         self.add_url_rule('/extension_asset', methods=['GET'], view_func=self.extension_asset)
         self.analogic_applications = {}
+        self.initialize_auth_providers = True
 
     def register_analogic_url_rules(self, instance):
         for url_rule in self.endpoint_rules:
             self.add_url_rule(instance + url_rule['rule'],
                               url_rule['endpoint'],
                               view_func=url_rule['view_func'],
                               provide_automatic_options=url_rule['provide_automatic_options'],
@@ -68,43 +69,49 @@
         return self.conditions[name]
 
     def get_authentication_provider_module_name(self, name):
         return self.authentication_providers[name]
 
     def register_application(self, application_dir, blueprint: "Blueprint", **options: t.Any) -> None:
         try:
+
             instance = '/' + blueprint.name
+
             self.register_analogic_url_rules(instance)
 
             self.analogic_applications[blueprint.name] = self.create_authentication_provider(blueprint.name,
-                                                                                         application_dir)
+                                                                                             application_dir)
 
             super().register_blueprint(blueprint, **options)
         except Exception as e:
             logging.getLogger(__name__).error('Error registering application ' + blueprint.name + ': ' + str(e))
+            logging.getLogger(__name__).error(e, exc_info=True)
 
     def create_authentication_provider(self, analogic_application, analogic_application_path):
         with self.app_context():
             setting = SettingManager(analogic_application_path, analogic_application)
-            config = setting.config
+            return self.create_authentication_provider_by_setting(setting)
+
+    def create_authentication_provider_by_setting(self, setting, initialize=True):
 
-            class_name = config['authenticationMode']
-            module_name = self.get_authentication_provider_module_name(class_name)
+        class_name = setting.config['authenticationMode']
+        module_name = self.get_authentication_provider_module_name(class_name)
 
-            if module_name in sys.modules:
-                module = sys.modules[module_name]
-            else:
-                module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
+        if module_name in sys.modules:
+            module = sys.modules[module_name]
+        else:
+            module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
 
-            authentication_provider_class = getattr(module, class_name)
-            authentication_provider = authentication_provider_class(setting)
+        authentication_provider_class = getattr(module, class_name)
+        authentication_provider = authentication_provider_class(setting)
 
+        if initialize and self.initialize_auth_providers:
             authentication_provider.initialize()
 
-            return authentication_provider
+        return authentication_provider
 
     def get_analogic_application(self):
         s = request.path.split('/')
         if len(s) > 2 and s[1] in self.analogic_applications:
             return self.analogic_applications[s[1]]
         else:
             return self.analogic_applications['default']
@@ -128,33 +135,24 @@
         return list(filter(lambda x: x.endswith(ext), list(self.extension_assets.keys())))
 
     def get_authentication_provider(self):
         authentication_provider = self.get_analogic_application()
 
         session.permanent = True
         config = authentication_provider.get_setting().get_config()
+
         if config['authenticationMode'] != 'Cam':
             self.permanent_session_lifetime = timedelta(minutes=config['sessionExpiresInMinutes'] - 1)
         else:
             self.permanent_session_lifetime = timedelta(days=31)
 
-        return authentication_provider
-
-    def evaluate_condition(self, config):
-        class_name = config.get('authenticationModeCondition')
-        module_name = self.get_condition_module_name(class_name)
+        if config['authenticationMode'] == 'MultiAuthenticationProvider':
+            return authentication_provider.get_authentication_provider_by_request()
 
-        if module_name in sys.modules:
-            module = sys.modules[module_name]
-        else:
-            module = importlib.import_module(module_name)
-
-        condition_class = getattr(module, class_name)
-        condition = condition_class()
-        return condition.get_authentication_provider_name(config)
+        return authentication_provider
 
     def on_exit(self):
         print('on_exit')
         for app_name in self.analogic_applications:
             self.analogic_applications[app_name].on_exit()
 
 
@@ -165,16 +163,17 @@
 def page_error(e):
     message = ''
     if e.original_exception:
         message += str(e.original_exception)
     return render_template('500.html', message=message), 500
 
 
-def create_app(instance_path):
+def create_app(instance_path, start_scheduler=True, initialize_auth_providers=True):
     app = Analogic(__name__, instance_path=instance_path)
+    app.initialize_auth_providers = initialize_auth_providers
 
     app.secret_key = b'\x18m\x18\\]\xec\xcf\xbd\xf2\x89\xb9\xa3\x06N\x07\xfd'
 
     _load_logging(app)  # Todo overwrite
 
     app.register_analogic_endpoint(core_endpoints)
 
@@ -185,15 +184,15 @@
 
     if EXTENSIONS_EXTRA:
         for extension_path in EXTENSIONS_EXTRA:
             extension_abs_path = os.path.abspath(os.path.normpath(extension_path))
             extension_folder = os.path.dirname(extension_abs_path)
             extension_name = os.path.basename(extension_abs_path)
             _append_extension_dir_to_path(app, extension_folder)
-            _load_module(app, True, extension_name, extension_folder, _register_extension)
+            _load_module(app, False, extension_name, extension_folder, _register_extension)
 
     _load_applications(app, register_func=_register_application, module_dirs=APPLICATIONS_DIR)
 
     if APPLICATIONS_DIR_EXTRA != '':
         _load_applications(app, register_func=_register_application, module_dirs=APPLICATIONS_DIR_EXTRA)
 
     if APPLICATIONS_EXTRA:
@@ -207,15 +206,16 @@
     app.register_analogic_url_rules('')
 
     app.register_error_handler(404, page_not_found)
     app.register_error_handler(500, page_error)
 
     scheduler.init_app(app)
 
-    scheduler.start()
+    if start_scheduler:
+        scheduler.start()
 
     atexit.register(app.on_exit)
 
     return app
 
 
 def _load_logging(app):
@@ -245,15 +245,14 @@
     modules_dir = os.path.join(app.instance_path, modules_dir_name)
     if modules_dir not in sys.path and os.path.exists(modules_dir) and len(os.listdir(modules_dir)) != 0:
         sys.path.append(modules_dir)
 
 
 def _register_extension(app, extension_dir, extension_dir_name, modules):
     _register_extension_components(app, extension_dir_name, modules)
-
     _register_extension_assets(app, extension_dir)
 
 
 def _register_extension_assets(app, extension_dir):
     assets = _fast_scan_dir(extension_dir, ['.css', '.js'])[1]
     app.register_extension_assets(assets)
 
@@ -265,67 +264,75 @@
         if module not in sys.modules:
             print(module + ' not loaded')
             continue
 
         for name, obj in inspect.getmembers(sys.modules[module]):
             if inspect.isclass(obj) and \
                     not inspect.isabstract(obj) and \
-                    issubclass(obj, AuthenticationProvider):
+                    issubclass(obj, AuthenticationProvider) and \
+                    app.authentication_providers.get(name) is None:
+                logging.getLogger(__name__).info('Registering authentication provider ' + extension_name + "." + name)
                 app.register_authentication_provider(name, extension_name)
 
-            if inspect.isclass(obj) and \
-                    not inspect.isabstract(obj) and \
-                    issubclass(obj, Condition):
-                app.register_condition(name, extension_name)
-
             if isinstance(obj, AnalogicEndpoint):
+                logging.getLogger(__name__).info('Registering analogic endpoing ' + name)
                 app.register_analogic_endpoint(obj)
 
 
 def _load_applications(app, register_func, module_dirs):
     for module_dir in module_dirs.split(";"):
         modules_dir_path = os.path.join(app.instance_path, module_dir)
 
         _append_extension_dir_to_path(app, module_dir)
 
         _load_modules(app, modules_dir_path, False, register_func)
 
 
 def _load_modules(app, modules_dir, check_prefix, register_func):
-    for module_dir_name in os.listdir(modules_dir):
-        _load_module(app, check_prefix, module_dir_name, modules_dir, register_func)
+    if os.path.isdir(modules_dir):
+        for module_dir_name in os.listdir(modules_dir):
+            _load_module(app, check_prefix, module_dir_name, modules_dir, register_func)
 
 
 def _load_module(app, check_prefix, module_dir_name, modules_dir, register_func):
     module_dir = os.path.join(modules_dir, module_dir_name)
     if os.path.isdir(module_dir) and module_dir_name != '.git' and module_dir_name != 'tests' and (
             check_prefix is False or (
-            module_dir_name.startswith(ALLOWED_EXTENSION_PREFIX) and not module_dir_name.endswith('dist-info'))):
+            module_dir_name.startswith(ALLOWED_EXTENSION_PREFIX) and not module_dir_name.endswith(
+        'dist-info') and not module_dir_name.endswith('egg-info'))):
 
         # workaround to handle repeating names in module path
-        if module_dir_name == modules_dir.rsplit('/', 1)[-1]:
+        if module_dir_name == modules_dir.rsplit('/', 1)[-1]:  # or module_dir_name == modules_dir.rsplit('\\', 1)[-1]:
             module_dir_name = module_dir_name + '.' + module_dir_name
 
         files = resources.contents(module_dir_name)
 
         modules = [f[:-3] for f in files if f.endswith(".py") and f[0] != "_" and 'setup' not in f]
         register_func(app, module_dir, module_dir_name, modules)
 
 
 def _register_application(app, application_dir, application_name, files):
+    _register_extension_components(app, application_name, files)
+    assets_extra_dir = os.path.join(application_dir, 'static', 'assets', 'extra')
+    if os.path.exists(assets_extra_dir):
+        assets_extra = _fast_scan_dir(assets_extra_dir, ['.css', '.js'])[1]
+        app.register_extension_assets(assets_extra)
+
     for file in files:
         module = application_name + '.' + file
 
         if module not in sys.modules:
             print(module + ' not loaded')
             continue
 
         for name, obj in inspect.getmembers(sys.modules[module]):
-            if isinstance(obj, Blueprint):
+            if isinstance(obj, Blueprint) and app.analogic_applications.get(obj.name) is None:
                 app.register_application(application_dir=application_dir, blueprint=obj)
+                logging.getLogger(__name__).info(
+                    'Registering application ' + application_name + " with blueprint " + name)
 
 
 def _fast_scan_dir(directory, ext):
     sub_folders, files = [], {}
     if '.git' in directory or 'tests' in directory:
         return sub_folders, files
```

### Comparing `analogic-framework-4.1.8/analogic/analogic_tm1_service.py` & `analogic-framework-4.1.9/analogic/analogic_tm1_service.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/authentication_provider.py` & `analogic-framework-4.1.9/analogic/authentication_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from flask import session, current_app, send_file, request, jsonify
+from flask import session, current_app, send_file, request, jsonify, Response
 from analogic.loader import ClassLoader
 import analogic.pivot as PivotApi
 from analogic.exceptions import AnalogicProxyException, AnalogicAccessDeniedException
+from analogic.session_handler import SessionHandler
 import logging
 import pandas as pd
 from abc import ABC, abstractmethod
 from functools import wraps
 import orjson
 
 pd.set_option('display.float_format', lambda x: '%.3f' % x)
@@ -55,30 +56,28 @@
     HEADERS = {'Connection': 'keep-alive',
                'User-Agent': 'Analogic',
                'Content-Type': 'application/json; odata.streaming=true; charset=utf-8',
                'Accept': 'application/json;odata.metadata=none,text/plain',
                'Accept-Encoding': 'gzip, deflate, br',
                'TM1-SessionContext': 'Analogic'}
 
-    PERMISSION_QUERIES_KEY = 'analogic_permissions'
-    PERMISSIONS_SESSION_NAME = 'analogic_permission'
-
     def __init__(self, setting):
         self.setting = setting
-        self.logged_in_user_session_name = self.setting.get_instance() + '_logged_in_user_name'
+        self.logged_in_user_session_name = '_logged_in_user_name'
         self._logger = logging.getLogger(self.setting.get_instance())
+        self.session_handler = SessionHandler(self.setting.get_instance_and_name())
 
     def initialize(self):
         self.setting.initialize()
 
     def get_setting(self):
         return self.setting
 
     def get_logged_in_user_name(self):
-        return session.get(self.logged_in_user_session_name)
+        return self.session_handler.get(self.logged_in_user_session_name)
 
     @login_required
     def pivot(self):
         username = self.get_logged_in_user_name()
 
         v = request.values
         cube_name = v.get('cube_name')
@@ -131,20 +130,22 @@
 
         return ClassLoader().call(description, request, self.get_tm1_service(), self.setting, self)
 
     def _get_check_access_mdx(self, force_server_side_query=False):
         if request.args.get('server') is not None or force_server_side_query is True:
             if request.method == 'GET':
                 body = request.args
+            elif len(request.form) > 0:
+                body = request.form.to_dict()
             else:
                 body = orjson.loads(request.data)
             key = body.get('key')
             if body.get('key_suffix') is not None:
                 key = key + '_' + body['key_suffix']
-            key = key + '_analogic_check_access'
+            key = key + self.get_setting().get_check_access_repository_yml_suffix()
             mdx = self.setting.get_mdx(key)
 
             if mdx is None:
                 return None
             else:
                 mdx = self._set_custom_mdx_data(mdx)
 
@@ -155,14 +156,16 @@
 
         return None
 
     def _get_server_side_mdx(self, force_server_side_query=False):
         if request.args.get('server') is not None or force_server_side_query is True:
             if request.method == 'GET':
                 body = request.args
+            elif len(request.form) > 0:
+                body = request.form.to_dict()
             else:
                 body = orjson.loads(request.data)
             key = body['key']
             if body.get('key_suffix') is not None:
                 key = key + '_' + body['key_suffix']
             mdx = self.setting.get_mdx(key)
 
@@ -176,25 +179,22 @@
             for k in body:
                 mdx = mdx.replace('$' + k, body[k].replace('"', '\\"'))
 
             return mdx.encode('utf-8')
         else:
             return ''.encode('utf-8')
 
-    @abstractmethod
     def index(self):
         pass
 
-    @abstractmethod
     def check_app_authenticated(self):
-        return True
+        return self.session_handler.is_exist(self.logged_in_user_session_name)
 
-    @abstractmethod
     def get_authentication_required_response(self):
-        pass
+        return Response('', 401)
 
     def get_not_found_response(self):
         return 'Not found', 404, {'Content-Type': 'application/json'}
 
     def _add_authenticated_cookies(self, response, max_age=None):
         m = max_age
         if max_age is None:
@@ -245,20 +245,27 @@
 
         if len(resp.get('Cells')) < 1:
             return False
 
         return resp.get('Cells')[0].get('Value') == 1
 
     def check_permission(self, required_permissions):
-        available_permissions = session.get(self.PERMISSIONS_SESSION_NAME)
-        available_permissions_list = available_permissions.split(',') if available_permissions is not None else []
+        available_permissions_list = self.get_permission_list()
         return any(permission in required_permissions for permission in available_permissions_list)
 
+    def get_permission_list(self):
+        available_permissions = self.session_handler.get(self.setting.get_permission_session_name())
+        available_permissions_list = available_permissions.split(',') if available_permissions is not None else []
+        return available_permissions_list
+
+    def set_permissions(self, permissions_str):
+        self.session_handler.set(self.setting.get_permission_session_name(), permissions_str)
+
     def load_permissions(self):
-        permission_queries = self.setting.get_mdx(self.PERMISSION_QUERIES_KEY)
+        permission_queries = self.setting.get_mdx(self.setting.get_permission_query_repository_yml_key())
         if permission_queries is not None:
             for permission_query_params in permission_queries:
                 self.execute_permission_query(permission_query_params)
 
     def execute_permission_query(self, params):
         try:
             target_url = self.setting.get_proxy_target_url()
@@ -268,27 +275,31 @@
 
             headers: dict[str, str] = self.HEADERS.copy()
             cookies: dict[str, str] = {}
 
             response = self.do_proxy_request(url, params['method'], body.encode('utf-8'), headers, cookies, True)
 
             if response.status_code > 300:
+                self._logger.error(
+                    'Unable to load permissions {0} {1}'.format(self.setting.get_instance(), self.setting.get_name()))
                 self._logger.error('MDX error: ' + response.text)
-                self._logger.error('MDX: ' + body.decode('utf-8'))
+                self._logger.error('MDX: ' + body)
             else:
                 r = response.json()
                 permissions = [str(x['Value']) for x in r['Cells']]
 
-                existing_permissions = session.get(self.PERMISSIONS_SESSION_NAME)
+                existing_permissions = self.session_handler.get(self.setting.get_permission_session_name())
                 existing_permissions_list = existing_permissions.split(',') if existing_permissions is not None else []
 
                 union = list(set(existing_permissions_list + permissions))
-                session[self.PERMISSIONS_SESSION_NAME] = ','.join(union)
+                self.set_permissions(','.join(union))
 
         except Exception as e:
+            self._logger.error(
+                'Unable to load permissions {0} {1}'.format(self.setting.get_instance(), self.setting.get_name()))
             self.getLogger().error(e, exc_info=True)
 
     @login_required
     @check_access
     def proxy(self, sub_path, encode_content=False, method=None, force_server_side_query=False,
               forward_query_string=True):
 
@@ -342,39 +353,53 @@
 
         return self._create_request_with_authenticated_user(url, method, mdx, headers, cookies, decode_content)
 
     @abstractmethod
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
         pass
 
-    @abstractmethod
     def _extend_login_session(self):
-        pass
+        session.modified = True
 
     @abstractmethod
     def get_tm1_service(self):
         pass
 
     @login_required
     def active_user(self):
         return jsonify({'username': self.get_logged_in_user_name()})
 
     def login(self):
-        pass
+        self.session_handler.set(self.logged_in_user_session_name, '')
 
     def logout(self):
-        session.clear()
+        self.session_handler.clear()
         return 'ok'
 
+    def clear_cache(self):
+        return self.get_setting().clear_cache()
+
     def getLogger(self):
         return self._logger
 
     def on_exit(self):
         pass
 
+    def install(self, params):
+        pass
+
+    def uninstall(self, params):
+        pass
+
+    def add_command_line_parameters(self, ap):
+        pass
+
+    def get_available_backend_methods(self):
+        return ['install', 'uninstall']
+
     @staticmethod
     def get_setting_parameter_descriptions():
         result = {
             'projectName': {
                 'required': True,
                 'description': 'Free text, displayed on the header of html title.'
             },
```

### Comparing `analogic-framework-4.1.8/analogic/cam.py` & `analogic-framework-4.1.9/analogic/cam.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 from flask import render_template, request, make_response, redirect, session, Response, send_file
 from analogic.analogic_tm1_service import AnalogicTM1Service
 import orjson
 import analogic.pivot as PivotApi
 from analogic.exceptions import AnalogicTM1ServiceException
 from analogic.loader import ClassLoader
 from analogic.authentication_provider import login_required
+from analogic.logged_in_signal import logged_in
+from analogic.multi_authentication_provider_interface import MultiAuthenticationProviderInterface
 
 
-class Cam(AuthenticationProvider):
+class Cam(AuthenticationProvider, MultiAuthenticationProviderInterface):
 
     def __init__(self, setting):
         super().__init__(setting)
 
     def index(self):
         authenticated = request.cookies.get('authenticated') is not None and self.check_app_authenticated()
         return render_template('index.html', authenticated=authenticated, cnf=self.setting.get_config())
 
     def auth(self):
         resp = make_response(redirect(self.setting.get_base_url()))
         resp.set_cookie('camPassport', request.form.get('c_pp'))
 
         cam_name = self.set_tm1_service(request.form.get('c_pp'))
-        session[self.logged_in_user_session_name] = cam_name
+        self.session_handler.set(self.logged_in_user_session_name, cam_name)
         self.load_permissions()
+        logged_in.send(self, user_name=cam_name, password='')
         return self._add_authenticated_cookies(resp)
 
+    def do_login(self, user_name, password):
+        raise Exception('Cam authentication mode must be the primary and only login endpoint')
+
     def get_base_url(self):
         return self.setting.get_config()['apiHost']
 
     def set_tm1_service(self, cam_passport):
         cnf = self.setting.get_config()
 
         tm1_service = AnalogicTM1Service(base_url=self.get_base_url(),
@@ -52,15 +58,15 @@
                 self._logger.error('exception while closing session: ' + str(e))
 
         self.setting.set_tm1_service(cam_name, tm1_service)
 
         return cam_name
 
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
-        tm1_service = self.setting.get_tm1_service(session.get(self.logged_in_user_session_name))
+        tm1_service = self.setting.get_tm1_service(self.get_logged_in_user_name())
         if tm1_service is None:
             return Response('Unauthorized', status=401, mimetype='application/json')
 
         response = tm1_service.get_session().request(method, url, data=mdx, headers=headers,
                                                      verify=self.setting.get_ssl_verify(), decode_content=decode_content)
         if response.status_code == 401:
             try:
@@ -85,16 +91,16 @@
                 mdx = mdx.replace('$' + k, body[k].replace('"', '\\"'))
 
             return mdx.encode('utf-8')
 
         return mdx
 
     def check_app_authenticated(self):
-        return session.get(self.logged_in_user_session_name, '') != '' and self.setting.get_tm1_service(
-            session.get(self.logged_in_user_session_name)) is not None
+        return self.session_handler.get(self.logged_in_user_session_name, '') != '' and self.setting.get_tm1_service(
+            self.get_logged_in_user_name()) is not None
 
     @login_required
     def pivot(self):
         username = self.get_logged_in_user_name()
 
         v = request.values
         cube_name = v.get('cube_name')
@@ -146,15 +152,15 @@
                          max_age=0,
                          mimetype='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
 
     def get_authentication_required_response(self):
         return 'Authentication required', 401, {'Content-Type': 'application/json'}
 
     def get_tm1_service(self):
-        tm1_service = self.setting.get_tm1_service(session[self.logged_in_user_session_name])
+        tm1_service = self.setting.get_tm1_service(self.get_logged_in_user_name())
         if tm1_service is None:
             raise AnalogicTM1ServiceException('Unauthorized')
 
         if tm1_service.connection.is_connected() is False:
             try:
                 tm1_service.re_authenticate()
             except Exception as e:
```

### Comparing `analogic-framework-4.1.8/analogic/camsecure.py` & `analogic-framework-4.1.9/analogic/camsecure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from analogic.cam import Cam
-from flask import request, make_response, redirect, session
+from flask import request, make_response, redirect
+from analogic.logged_in_signal import logged_in
 
 
 class CamSecure(Cam):
 
     def __init__(self, setting):
         super().__init__(setting)
 
     def auth(self):
         resp = make_response(redirect(self.setting.get_base_url()))
 
         cam_name = self.set_tm1_service(request.form.get('c_pp'))
-        session[self.logged_in_user_session_name] = cam_name
+        self.session_handler.set(self.logged_in_user_session_name, cam_name)
         self.load_permissions()
+        logged_in.send(self, user_name=cam_name, password='')
         return self._add_authenticated_cookies(resp)
 
+    def do_login(self, user_name, password):
+        raise Exception('Cam authentication mode must be the primary and only login endpoint')
+
     def get_base_url(self):
         return self.setting.get_proxy_target_url()
 
     @staticmethod
     def get_setting_parameter_descriptions():
         result = super(CamSecure, CamSecure).get_setting_parameter_descriptions()
         del result['apiHost']
```

### Comparing `analogic-framework-4.1.8/analogic/core_endpoints.py` & `analogic-framework-4.1.9/analogic/core_endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 @core_endpoints.analogic_endpoint_route('/export', methods=['GET', 'POST'])
 def export():
     return get_authentication_provider().export()
 
 
 @core_endpoints.analogic_endpoint_route('/clearcache', methods=['GET'])
 def clear_cache():
-    return get_authentication_provider().setting.clear_cache()
+    return get_authentication_provider().clear_cache()
 
 
 # @core_endpoints.analogic_endpoint_route('/ping', methods=['GET'])
 # def ping():
 #     return get_authentication_provider().ping()
```

### Comparing `analogic-framework-4.1.8/analogic/email.py` & `analogic-framework-4.1.9/analogic/email.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/endpoint.py` & `analogic-framework-4.1.9/analogic/endpoint.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/exceptions.py` & `analogic-framework-4.1.9/analogic/exceptions.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/loader.py` & `analogic-framework-4.1.9/analogic/loader.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/logging.json` & `analogic-framework-4.1.9/analogic/logging.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/loginbasic.py` & `analogic-framework-4.1.9/analogic/loginbasic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,101 @@
 from analogic.authentication_provider import AuthenticationProvider
 from analogic.analogic_tm1_service import AnalogicTM1Service
 from analogic.exceptions import AnalogicTM1ServiceException
 from flask import render_template, request, make_response, redirect, session, Response
+from analogic.logged_in_signal import logged_in
+from analogic.multi_authentication_provider_interface import MultiAuthenticationProviderInterface
 
 
-class LoginBasic(AuthenticationProvider):
+class LoginBasic(AuthenticationProvider, MultiAuthenticationProviderInterface):
 
     def __init__(self, setting):
         super().__init__(setting)
 
     def index(self):
         cnf = self.setting.get_config()
-        if self.logged_in_user_session_name in session:
+        if self.session_handler.is_exist(self.logged_in_user_session_name):
             return render_template('index.html', authenticated=True, cnf=cnf)
         return redirect(self.setting.get_base_url('login'))
 
     def get_connection_params(self, user_name, password):
         return {
-                'base_url': self.setting.get_proxy_target_url(),
-                'ssl': self.setting.get_ssl_verify(),
-                'user': user_name,
-                'password': password
+            'base_url': self.setting.get_proxy_target_url(),
+            'ssl': self.setting.get_ssl_verify(),
+            'user': user_name,
+            'password': password
         }
+
     def login(self):
         cnf = self.setting.get_config()
+        message = ''
         if request.method == 'POST':
             user_name = request.form.get('username')
-            p = self.get_connection_params(user_name, request.form.get('password'))
-            p['connection_pool_size'] = 100
-
+            password = request.form.get('password')
             try:
-                tm1_service = self.setting.get_tm1_service(user_name)
-                is_connected = False
-                if tm1_service is not None:
-                    try:
-                        is_connected = tm1_service.connection.is_connected()
-                    except Exception as e:
-                        self._logger.error('exception while checking connection: ' + str(e))
-
-                if not is_connected:
-                    if tm1_service is not None:
-                        try:
-                            tm1_service.close_session()
-                        except Exception as e:
-                            self._logger.error('exception while closing session: ' + str(e))
-
-                    tm1_service = AnalogicTM1Service(**p)
-                    self.setting.set_tm1_service(user_name, tm1_service)
-
-                session[self.logged_in_user_session_name] = user_name
-                self.load_permissions()
+                self.do_login(user_name, password)
+                logged_in.send(self, user_name=user_name, password=password)
                 resp = make_response(redirect(self.setting.get_base_url()))
                 return self._add_authenticated_cookies(resp)
-
             except Exception as e:
                 self._logger.error(e, exc_info=True)
+                message = str(e)
+        return render_template('login.html', cnf=cnf, message=message)
 
-        return render_template('login.html', cnf=cnf)
+    def do_login(self, user_name, password):
+        p = self.get_connection_params(user_name, password)
+        p['connection_pool_size'] = 100
+
+        tm1_service = self.setting.get_tm1_service(user_name)
+        is_connected = False
+        if tm1_service is not None:
+            try:
+                is_connected = tm1_service.connection.is_connected()
+            except Exception as e:
+                self._logger.error('exception while checking connection: ' + str(e))
+
+        if not is_connected:
+            if tm1_service is not None:
+                try:
+                    tm1_service.close_session()
+                except Exception as e:
+                    self._logger.error('exception while closing session: ' + str(e))
+
+            tm1_service = AnalogicTM1Service(**p)
+            self.setting.set_tm1_service(user_name, tm1_service)
+
+        self.session_handler.set(self.logged_in_user_session_name, user_name)
+        self.load_permissions()
 
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
-        user_name = session[self.logged_in_user_session_name]
+        user_name = self.get_logged_in_user_name()
         tm1_service = self.setting.get_tm1_service(user_name)
         if tm1_service is None:
             return Response('Unauthorized', status=401, mimetype='application/json')
-        response = tm1_service.get_session().request(method, url, data=mdx, headers=headers, verify=self.setting.get_ssl_verify(), decode_content=decode_content)
+        response = tm1_service.get_session().request(method, url, data=mdx, headers=headers,
+                                                     verify=self.setting.get_ssl_verify(),
+                                                     decode_content=decode_content)
         if response.status_code == 401:
             tm1_service.re_authenticate()
-            response = tm1_service.get_session().request(method, url, data=mdx, headers=headers, verify=self.setting.get_ssl_verify(), decode_content=decode_content)
+            response = tm1_service.get_session().request(method, url, data=mdx, headers=headers,
+                                                         verify=self.setting.get_ssl_verify(),
+                                                         decode_content=decode_content)
         return response
 
     def check_app_authenticated(self):
-        if self.logged_in_user_session_name in session:
-            return True
-        return False
+        return self.session_handler.is_exist(self.logged_in_user_session_name)
 
     def get_authentication_required_response(self):
         return redirect(self.setting.get_base_url('login'))
 
     def _extend_login_session(self):
         session.modified = True
 
     def get_tm1_service(self):
-        tm1_service = self.setting.get_tm1_service(session[self.logged_in_user_session_name])
+        tm1_service = self.setting.get_tm1_service(self.get_logged_in_user_name())
         if tm1_service is None:
             raise AnalogicTM1ServiceException('Unauthorized')
 
         if tm1_service.connection.is_connected() is False:
             try:
                 tm1_service.re_authenticate()
             except Exception as e:
@@ -101,8 +111,7 @@
             'target': {
                 'required': True,
                 'description': 'Tm1 restapi url.'
             }
         }
 
         return result
-
```

### Comparing `analogic-framework-4.1.8/analogic/logincam.py` & `analogic-framework-4.1.9/analogic/logincam.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/nologin.py` & `analogic-framework-4.1.9/analogic/nologin.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         super().__init__(setting)
 
     def index(self):
         cnf = self.setting.get_config()
 
         resp = make_response(render_template('index.html', authenticated=True, cnf=cnf))
 
-        session[self.logged_in_user_session_name] = 'nologin'
+        self.session_handler.set(self.logged_in_user_session_name, 'nologin')
 
         return self._add_authenticated_cookies(resp, 86400)
 
     def login(self):
         return redirect(self.setting.get_base_url())
 
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies):
@@ -32,11 +32,11 @@
     def _extend_login_session(self):
         session.modified = True
 
     def get_tm1_service(self):
         return None
 
     def active_user(self):
-        return jsonify({'username': session[self.logged_in_user_session_name]})
+        return jsonify({'username': self.get_logged_in_user_name()})
 
     def getLogger(self):
         return logging.getLogger(__name__)
```

### Comparing `analogic-framework-4.1.8/analogic/pivot.py` & `analogic-framework-4.1.9/analogic/pivot.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/setting.py` & `analogic-framework-4.1.9/analogic/setting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import yaml
 import os
-from flask import json, current_app, url_for, request, render_template
+from flask import json, current_app, url_for, request, render_template, has_request_context
 import logging
 import uuid
 import sys
 import importlib
 
 
 class SettingManager:
 
     def __init__(self, analogic_application_path, instance='default'):
         self.site_root = analogic_application_path
         self.instance = instance
+        self.config_js_name = self.get_config_js_name()
         self.config = self._create_config()
         self.repository = self._create_repository()
         self.custom_objects = self._create_custom_objects()
         self._logger = logging.getLogger(self.get_instance())
         self.tm1_services = {}
 
     def initialize(self):
@@ -42,34 +43,34 @@
     def get_instance(self):
         return self.instance
 
     def _create_config(self):
         return self._get_json_setting('app')
 
     def get_config(self):
-        if not os.path.exists(os.path.join(self.site_root, 'static', 'assets', 'js', 'config.js')):
+        if not os.path.exists(os.path.join(self.site_root, 'static', 'assets', 'js', self.config_js_name)):
             self.save_config_js()
 
-        if self.config.get('authenticationModeCondition') is not None:
-            self.config['authenticationMode'] = current_app.evaluate_condition(self.config)
-
         if self.config is not None:
             return self.config
         self.config = self._get_json_setting('app')
         self.save_config_js()
         return self.config
 
     def _get_param(self, param_name):
         return self.config[param_name]
 
     def get_base_url(self, route=''):
-        base = url_for('core_endpoints.index')
-        url = request.environ.get('wsgi.url_scheme') + '://' + request.environ.get('HTTP_HOST')
-        sub_path = [base[:-1], self.instance, route]
-        return url + ('/'.join(filter(lambda x: x != 'default' and x is not None, sub_path)))
+        if has_request_context():
+            base = url_for('core_endpoints.index')
+            url = request.environ.get('wsgi.url_scheme') + '://' + request.environ.get('HTTP_HOST')
+            sub_path = [base[:-1], self.instance, route]
+            return url + ('/'.join(filter(lambda x: x != 'default' and x is not None, sub_path)))
+        else:
+            ''
 
     def _create_repository(self):
         return self._get_yaml_setting(os.path.join('server', 'configs', 'repository'))
 
     def _get_repository(self):
         if self.repository is not None:
             return self.repository
@@ -85,41 +86,47 @@
     def _get_json_setting(self, file_name):
 
         json_url = os.path.join(self.site_root, file_name + '.json')
         with open(json_url, encoding="utf-8") as f:
             setting = json.load(f)
 
         if file_name == 'app':
-            setting['instance'] = self.instance
-            setting['blueprint_static'] = self.instance + '.static'
-            setting['extension_css_asset_names'] = current_app.get_extension_css_asset_names()
-            setting['extension_js_asset_names'] = current_app.get_extension_js_asset_names()
-            setting['version'] = uuid.uuid4().hex[:6].upper()
-
-            if setting.get('apiSubPath') is None:
-                setting['apiSubPath'] = '/api/v1/'
-
-            if setting.get('authenticationBridge') is None:
-                setting['authenticationBridge'] = ''
+            return self.get_app_setting(setting)
+
+        return setting
 
-            if setting.get('sessionExpiresInMinutes') is None:
-                setting['sessionExpiresInMinutes'] = 20
+    def get_app_setting(self, setting):
+        setting['instance'] = self.instance
+        setting['blueprint_static'] = self.instance + '.static'
+        setting['extension_css_asset_names'] = current_app.get_extension_css_asset_names()
+        setting['extension_js_asset_names'] = current_app.get_extension_js_asset_names()
+        setting['version'] = uuid.uuid4().hex[:6].upper()
+
+        if setting.get('apiSubPath') is None:
+            setting['apiSubPath'] = '/api/v1/'
+
+        if setting.get('authenticationBridge') is None:
+            setting['authenticationBridge'] = ''
 
-            if setting.get('useMinifiedAssets') is None:
-                setting['useMinifiedAssets'] = False
+        if setting.get('sessionExpiresInMinutes') is None:
+            setting['sessionExpiresInMinutes'] = 20
 
-            if setting.get('ssl_verify') is None:
-                setting['ssl_verify'] = True
+        if setting.get('useMinifiedAssets') is None:
+            setting['useMinifiedAssets'] = False
+
+        if setting.get('ssl_verify') is None:
+            setting['ssl_verify'] = True
 
         return setting
 
     def save_config_js(self, exclude=[]):
-        js_url = os.path.join(self.site_root, 'static', 'assets', 'js', 'config.js')
-        with open(js_url, 'w', encoding="utf-8") as f:
-            f.write(render_template('config.html', cnf=self.config, exclude=exclude))
+        js_url = os.path.join(self.site_root, 'static', 'assets', 'js', self.config_js_name)
+        if has_request_context():
+            with open(js_url, 'w', encoding="utf-8") as f:
+                f.write(render_template('config.html', cnf=self.config, exclude=exclude))
 
     def _get_yaml_setting(self, file_path):
         with open(os.path.join(self.site_root, file_path + '.yml'), encoding="utf-8") as file:
             setting = yaml.safe_load(file)
         return setting
 
     def _create_custom_objects(self):
@@ -144,9 +151,27 @@
 
     def get_smtp_password(self):
         return self.config['smtp']['password']
 
     def get_ssl_verify(self):
         return self.config['ssl_verify']
 
+    def get_config_js_name(self):
+        return 'config.js'
+
+    def get_name(self):
+        return ''
+
+    def get_instance_and_name(self):
+        return self.get_instance() + '_' + self.get_name()
+
+    def get_check_access_repository_yml_suffix(self):
+        return '_analogic_check_access'
+
+    def get_permission_query_repository_yml_key(self):
+        return 'analogic_permissions'
+
+    def get_permission_session_name(self):
+        return self.get_instance() + '_analogic_permissions'
+
     def getLogger(self):
         return self._logger
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/bootstrap-grid.min.css` & `analogic-framework-4.1.9/analogic/static/assets/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/bootstrap-grid.min.css.map` & `analogic-framework-4.1.9/analogic/static/assets/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/lib/Chart-2.9.3.min.css` & `analogic-framework-4.1.9/analogic/static/assets/css/lib/Chart-2.9.3.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/lib/nouislider.min.css` & `analogic-framework-4.1.9/analogic/static/assets/css/lib/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/style.css` & `analogic-framework-4.1.9/analogic/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/css/widgets/simulation-panel-slider.css` & `analogic-framework-4.1.9/analogic/static/assets/css/widgets/simulation-panel-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/images/loading.gif` & `analogic-framework-4.1.9/analogic/static/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/images/loading2.gif` & `analogic-framework-4.1.9/analogic/static/assets/images/loading2.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/images/loading2_transparent.gif` & `analogic-framework-4.1.9/analogic/static/assets/images/loading2_transparent.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/images/triangle.png` & `analogic-framework-4.1.9/analogic/static/assets/images/triangle.png`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/api.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/api.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -701,8 +701,23 @@
 
 Api.logout = function logout() {
     return Auth.logout();
 };
 
 Api.goToStartPage = function goToStartPage() {
     Auth.goToStartPage();
-};
+};
+
+Api.triggerWidgetEvent = function triggerWidgetEvent(widgetId, eventName) {
+    const widget = Widgets[widgetId],
+        triggerHandlerFunctionName = eventName + 'TriggerHandler';
+    if (!widget) {
+        console.error('Unable to find ' + widgetId);
+        return false;
+    }
+    if (!widget[triggerHandlerFunctionName]) {
+        console.error('Unable to find ' + triggerHandlerFunctionName);
+        return false;
+    }
+    widget[triggerHandlerFunctionName]();
+    return true;
+}
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/app.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/app.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/authentication.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/authentication.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/array.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/array.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/base.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/base.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
         return ParsingControlFactory.createExecutor(ctx, data).execute();
     }
 
     getUrl = p => {
         if (p.url) {
             const url = (typeof p.url === 'function' ? p.url(Widgets) : p.url);
             return {
-                url: QB.getUrl(url),
+                url: QB.getUrl(url, p.source),
                 type: p.type ? p.type : 'POST'
             };
         }
 
         L('error: url not found', p);
 
         return {
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/load-executor/factory.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/load-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/base.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/factory.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/parsing-control/matrix.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/parsing-control/matrix.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/pivot.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/pivot.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/query-builder.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/query-builder.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -95,13 +95,38 @@
 
     return {
         url: newUrl + subUrl,
         body: `{${params.join(',')}}`
     };
 };
 
-QB.getUrl = (url) => {
+QB.getUrl = (url, source = '') => {
+    let proxy_sub_path = 'proxy';
     if (url.includes('proxy')) {
-        return url;
+        proxy_sub_path = ''
     }
-    return app.apiHost ? app.apiHost + url : 'proxy' + url;
+
+    if (app.apiHost && !url.includes('proxy')) {
+        return app.apiHost + url;
+    }
+
+    if (app.auth_prov) {
+        if (app.auth_prov === 'primary') {
+            return source ? source + '/' + proxy_sub_path + url : proxy_sub_path + url;
+        } else {
+            let path = window.location.pathname.split('/').filter(s => s !== '');
+            path.pop();
+            if (source) {
+                path.push(source)
+            }
+            if (proxy_sub_path !== '') {
+                path.push(proxy_sub_path)
+            } else {
+                url = '/' + url;
+            }
+            return [window.location.origin, ...path].join('/') + url;
+        }
+    }
+
+    return proxy_sub_path + url;
+    //return app.apiHost ? app.apiHost + url : source ? source + '/proxy' + url : 'proxy' + url;
 };
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/server.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/server.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/utils.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/utils.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -415,16 +415,17 @@
     },
     getPropertyOrFunctionValue(object, property) {
         if (typeof object[property] === 'function') {
             return object[property]();
         }
         return object[property];
     },
-    getDecimalFromPercentString(value) {
-        return Utils.parseNumber(value.replace('%', '')) / 100;
+    getDecimalFromPercentString(value, replaceDecimal = false) {
+        let result = Utils.parseNumber(value.replace('%', '')) / 100;
+        return replaceDecimal ? Utils.replaceDecimal(result) : result;
     },
     filterUnique(arr) {
         return arr.filter((v, i, a) => a.indexOf(v) === i);
     },
     create_UUID() {
         let dt = new Date().getTime();
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/base.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/base.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -133,15 +133,15 @@
             type = this.getRestType();
         } else {
             type = eventHandler.type;
         }
 
         Loader.start(true);
 
-        return Auth.getAjaxRequest(QB.getUrl(url), body, type, widgetId, ctx.isResent(), ctx.getEventMapId()).then((d) => {
+        return Auth.getAjaxRequest(QB.getUrl(url, ctx.getEventHandler().source), body, type, widgetId, ctx.isResent(), ctx.getEventMapId()).then((d) => {
             Loader.stop(true);
             L('finished after ajax');
             instance.triggerRepositoryFinished(d);
             if (eventHandler.callback) {
                 eventHandler.callback({
                     ...{
                         getResponse() {
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/factory.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/function.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/function.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/framework/write-executor/grid-table.js` & `analogic-framework-4.1.9/analogic/static/assets/js/framework/write-executor/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/Chart-2.9.3.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/Chart-2.9.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/Sortable.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chart.umd.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chart.umd.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chart.umd.js.map` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chart.umd.js.map`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.actual.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.actual.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.cookie.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/jquery.doubletap.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/jquery.doubletap.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/jquery/tableSort.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/jquery/tableSort.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/lib/nouislider.min.js` & `analogic-framework-4.1.9/analogic/static/assets/js/lib/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/base/widget.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/base/widget.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (308)*

 * *Files 0% similar despite different names*

```diff
@@ -124,1340 +124,1340 @@
 000007b0: 2020 2020 2020 7d29 3b0a 2020 2020 7d0a        });.    }.
 000007c0: 0a20 2020 2072 6552 656e 6465 7257 6964  .    reRenderWid
 000007d0: 6765 7428 7769 7468 5374 6174 6520 3d20  get(withState = 
 000007e0: 6661 6c73 652c 2077 6974 684c 6f61 6465  false, withLoade
 000007f0: 7220 3d20 7472 7565 2c20 7072 6576 696f  r = true, previo
 00000800: 7573 6c79 4c6f 6164 6564 4461 7461 203d  uslyLoadedData =
 00000810: 2066 616c 7365 2920 7b0a 2020 2020 2020   false) {.      
-00000820: 2020 6966 2874 6869 732e 6973 5265 6e64    if(this.isRend
-00000830: 6572 696e 6729 207b 0a20 2020 2020 2020  ering) {.       
-00000840: 2020 2020 2074 6869 732e 7265 6e64 6572       this.render
-00000850: 4572 726f 7228 293b 0a20 2020 2020 2020  Error();.       
-00000860: 207d 0a20 2020 2020 2020 2074 6869 732e   }.        this.
-00000870: 6973 5265 6e64 6572 696e 6720 3d20 7472  isRendering = tr
-00000880: 7565 3b0a 0a20 2020 2020 2020 2063 6f6e  ue;..        con
-00000890: 7374 206f 203d 2074 6869 732e 6f70 7469  st o = this.opti
-000008a0: 6f6e 732c 2068 6f6c 6465 7220 3d20 7468  ons, holder = th
-000008b0: 6973 2e67 6574 486f 6c64 6572 286f 2e69  is.getHolder(o.i
-000008c0: 6429 2c20 696e 7374 616e 6365 203d 2074  d), instance = t
-000008d0: 6869 733b 0a0a 2020 2020 2020 2020 7468  his;..        th
-000008e0: 6973 2e72 656e 6465 7253 7461 7274 4c6f  is.renderStartLo
-000008f0: 6164 6572 2877 6974 684c 6f61 6465 7229  ader(withLoader)
-00000900: 3b0a 0a20 2020 2020 2020 204c 6973 7465  ;..        Liste
-00000910: 6e65 7273 2e6c 656e 6774 6820 3d20 303b  ners.length = 0;
-00000920: 0a0a 2020 2020 2020 2020 6c65 7420 686f  ..        let ho
-00000930: 6c64 6572 4865 6967 6874 203d 2068 6f6c  lderHeight = hol
-00000940: 6465 722e 6163 7475 616c 2827 6865 6967  der.actual('heig
-00000950: 6874 2729 3b0a 0a20 2020 2020 2020 2072  ht');..        r
-00000960: 6574 7572 6e20 686f 6c64 6572 2e65 6d70  eturn holder.emp
-00000970: 7479 2829 2e6f 6666 2829 2e70 726f 6d69  ty().off().promi
-00000980: 7365 2829 2e74 6865 6e28 2829 203d 3e20  se().then(() => 
-00000990: 7b0a 0a20 2020 2020 2020 2020 2020 2069  {..            i
-000009a0: 6e73 7461 6e63 652e 686f 6c64 6572 5374  nstance.holderSt
-000009b0: 6172 744c 6f61 6465 7228 293b 0a0a 2020  artLoader();..  
-000009c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000009d0: 2069 6e73 7461 6e63 652e 7265 6e64 6572   instance.render
-000009e0: 2877 6974 6853 7461 7465 2c20 7472 7565  (withState, true
-000009f0: 2c20 6661 6c73 652c 2051 422e 6c6f 6164  , false, QB.load
-00000a00: 4461 7461 2c20 7072 6576 696f 7573 6c79  Data, previously
-00000a10: 4c6f 6164 6564 4461 7461 292e 7468 656e  LoadedData).then
-00000a20: 2868 746d 6c20 3d3e 207b 0a20 2020 2020  (html => {.     
-00000a30: 2020 2020 2020 2020 2020 206c 6574 2069             let i
-00000a40: 7348 6569 6768 7455 7064 6174 6564 203d  sHeightUpdated =
-00000a50: 2066 616c 7365 2c20 6820 3d20 2428 6874   false, h = $(ht
-00000a60: 6d6c 292c 2069 3b0a 0a20 2020 2020 2020  ml), i;..       
-00000a70: 2020 2020 2020 2020 2069 6620 2868 6f6c           if (hol
-00000a80: 6465 7248 6569 6768 7420 3e20 3029 207b  derHeight > 0) {
-00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000aa0: 2020 2020 2069 7348 6569 6768 7455 7064       isHeightUpd
-00000ab0: 6174 6564 203d 2074 7275 653b 0a20 2020  ated = true;.   
+00000820: 2020 6966 2028 7468 6973 2e69 7352 656e    if (this.isRen
+00000830: 6465 7269 6e67 2920 7b0a 2020 2020 2020  dering) {.      
+00000840: 2020 2020 2020 7468 6973 2e72 656e 6465        this.rende
+00000850: 7245 7272 6f72 2829 3b0a 2020 2020 2020  rError();.      
+00000860: 2020 7d0a 2020 2020 2020 2020 7468 6973    }.        this
+00000870: 2e69 7352 656e 6465 7269 6e67 203d 2074  .isRendering = t
+00000880: 7275 653b 0a0a 2020 2020 2020 2020 636f  rue;..        co
+00000890: 6e73 7420 6f20 3d20 7468 6973 2e6f 7074  nst o = this.opt
+000008a0: 696f 6e73 2c20 686f 6c64 6572 203d 2074  ions, holder = t
+000008b0: 6869 732e 6765 7448 6f6c 6465 7228 6f2e  his.getHolder(o.
+000008c0: 6964 292c 2069 6e73 7461 6e63 6520 3d20  id), instance = 
+000008d0: 7468 6973 3b0a 0a20 2020 2020 2020 2074  this;..        t
+000008e0: 6869 732e 7265 6e64 6572 5374 6172 744c  his.renderStartL
+000008f0: 6f61 6465 7228 7769 7468 4c6f 6164 6572  oader(withLoader
+00000900: 293b 0a0a 2020 2020 2020 2020 4c69 7374  );..        List
+00000910: 656e 6572 732e 6c65 6e67 7468 203d 2030  eners.length = 0
+00000920: 3b0a 0a20 2020 2020 2020 206c 6574 2068  ;..        let h
+00000930: 6f6c 6465 7248 6569 6768 7420 3d20 686f  olderHeight = ho
+00000940: 6c64 6572 2e61 6374 7561 6c28 2768 6569  lder.actual('hei
+00000950: 6768 7427 293b 0a0a 2020 2020 2020 2020  ght');..        
+00000960: 7265 7475 726e 2068 6f6c 6465 722e 656d  return holder.em
+00000970: 7074 7928 292e 6f66 6628 292e 7072 6f6d  pty().off().prom
+00000980: 6973 6528 292e 7468 656e 2828 2920 3d3e  ise().then(() =>
+00000990: 207b 0a0a 2020 2020 2020 2020 2020 2020   {..            
+000009a0: 696e 7374 616e 6365 2e68 6f6c 6465 7253  instance.holderS
+000009b0: 7461 7274 4c6f 6164 6572 2829 3b0a 0a20  tartLoader();.. 
+000009c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000009d0: 6e20 696e 7374 616e 6365 2e72 656e 6465  n instance.rende
+000009e0: 7228 7769 7468 5374 6174 652c 2074 7275  r(withState, tru
+000009f0: 652c 2066 616c 7365 2c20 5142 2e6c 6f61  e, false, QB.loa
+00000a00: 6444 6174 612c 2070 7265 7669 6f75 736c  dData, previousl
+00000a10: 794c 6f61 6465 6444 6174 6129 2e74 6865  yLoadedData).the
+00000a20: 6e28 6874 6d6c 203d 3e20 7b0a 2020 2020  n(html => {.    
+00000a30: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+00000a40: 6973 4865 6967 6874 5570 6461 7465 6420  isHeightUpdated 
+00000a50: 3d20 6661 6c73 652c 2068 203d 2024 2868  = false, h = $(h
+00000a60: 746d 6c29 2c20 693b 0a0a 2020 2020 2020  tml), i;..      
+00000a70: 2020 2020 2020 2020 2020 6966 2028 686f            if (ho
+00000a80: 6c64 6572 4865 6967 6874 203e 2030 2920  lderHeight > 0) 
+00000a90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000aa0: 2020 2020 2020 6973 4865 6967 6874 5570        isHeightUp
+00000ab0: 6461 7465 6420 3d20 7472 7565 3b0a 2020  dated = true;.  
 00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2068 6f6c 6465 722e 6373 7328 7b6f 7061   holder.css({opa
-00000ae0: 6369 7479 3a20 302c 2027 6d69 6e2d 6865  city: 0, 'min-he
-00000af0: 6967 6874 273a 2068 6f6c 6465 7248 6569  ight': holderHei
-00000b00: 6768 747d 293b 0a20 2020 2020 2020 2020  ght});.         
-00000b10: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00000b20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000b30: 2068 6f6c 6465 722e 6874 6d6c 2868 2e68   holder.html(h.h
-00000b40: 746d 6c28 2929 2e70 726f 6d69 7365 2829  tml()).promise()
-00000b50: 2e74 6865 6e28 2829 203d 3e20 7b0a 0a20  .then(() => {.. 
+00000ad0: 2020 686f 6c64 6572 2e63 7373 287b 6f70    holder.css({op
+00000ae0: 6163 6974 793a 2030 2c20 276d 696e 2d68  acity: 0, 'min-h
+00000af0: 6569 6768 7427 3a20 686f 6c64 6572 4865  eight': holderHe
+00000b00: 6967 6874 7d29 3b0a 2020 2020 2020 2020  ight});.        
+00000b10: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00000b20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000b30: 6e20 686f 6c64 6572 2e68 746d 6c28 682e  n holder.html(h.
+00000b40: 6874 6d6c 2829 292e 7072 6f6d 6973 6528  html()).promise(
+00000b50: 292e 7468 656e 2828 2920 3d3e 207b 0a0a  ).then(() => {..
 00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2069 6e73 7461 6e63 652e 7265 6d6f     instance.remo
-00000b80: 7665 4c6f 6164 6572 4874 6d6c 2877 6974  veLoaderHtml(wit
-00000b90: 6853 7461 7465 293b 0a0a 2020 2020 2020  hState);..      
-00000ba0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000bb0: 2028 2168 6f6c 6465 722e 6861 7343 6c61   (!holder.hasCla
-00000bc0: 7373 2827 666f 7263 6564 4279 4576 656e  ss('forcedByEven
-00000bd0: 744d 6170 2729 2920 7b0a 2020 2020 2020  tMap')) {.      
+00000b70: 2020 2020 696e 7374 616e 6365 2e72 656d      instance.rem
+00000b80: 6f76 654c 6f61 6465 7248 746d 6c28 7769  oveLoaderHtml(wi
+00000b90: 7468 5374 6174 6529 3b0a 0a20 2020 2020  thState);..     
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000bb0: 6620 2821 686f 6c64 6572 2e68 6173 436c  f (!holder.hasCl
+00000bc0: 6173 7328 2766 6f72 6365 6442 7945 7665  ass('forcedByEve
+00000bd0: 6e74 4d61 7027 2929 207b 0a20 2020 2020  ntMap')) {.     
 00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 686f 6c64 6572 2e63 7373 2827 6469    holder.css('di
-00000c00: 7370 6c61 7927 2c20 682e 6373 7328 2764  splay', h.css('d
-00000c10: 6973 706c 6179 2729 2021 3d3d 2027 2720  isplay') !== '' 
-00000c20: 3f20 682e 6373 7328 2764 6973 706c 6179  ? h.css('display
-00000c30: 2729 203a 2027 756e 7365 7427 293b 0a20  ') : 'unset');. 
+00000bf0: 2020 2068 6f6c 6465 722e 6373 7328 2764     holder.css('d
+00000c00: 6973 706c 6179 272c 2068 2e63 7373 2827  isplay', h.css('
+00000c10: 6469 7370 6c61 7927 2920 213d 3d20 2727  display') !== ''
+00000c20: 203f 2068 2e63 7373 2827 6469 7370 6c61   ? h.css('displa
+00000c30: 7927 2920 3a20 2775 6e73 6574 2729 3b0a  y') : 'unset');.
 00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00000c60: 2020 2020 2020 2020 2020 6966 2028 6973            if (is
-00000c70: 4865 6967 6874 5570 6461 7465 6429 207b  HeightUpdated) {
-00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c90: 2020 2020 2020 2020 2068 6f6c 6465 722e           holder.
-00000ca0: 6373 7328 276f 7061 6369 7479 272c 2031  css('opacity', 1
-00000cb0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-00000cc0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00000ce0: 7374 616e 6365 2e69 6e69 7445 7665 6e74  stance.initEvent
-00000cf0: 7328 7769 7468 5374 6174 6529 3b0a 0a0a  s(withState);...
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 2020 2020 666f 7220 2869 206f 6620 4c69      for (i of Li
-00000d20: 7374 656e 6572 732e 6669 6c74 6572 2865  steners.filter(e
-00000d30: 203d 3e20 652e 6d65 7468 6f64 203d 3d3d   => e.method ===
-00000d40: 2027 7265 6672 6573 6847 7269 6443 656c   'refreshGridCel
-00000d50: 6c27 2026 2620 652e 6f70 7469 6f6e 732e  l' && e.options.
-00000d60: 6964 2e69 6e63 6c75 6465 7328 686f 6c64  id.includes(hold
-00000d70: 6572 2e61 7474 7228 2769 6427 2929 2929  er.attr('id'))))
-00000d80: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000d90: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00000da0: 2065 7665 6e74 203d 2069 2e65 7665 6e74   event = i.event
-00000db0: 4e61 6d65 2e73 706c 6974 2827 2e27 295b  Name.split('.')[
-00000dc0: 305d 3b0a 2020 2020 2020 2020 2020 2020  0];.            
-00000dd0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00000de0: 242e 5f64 6174 6128 456c 2e62 6f64 795b  $._data(El.body[
-00000df0: 305d 2c20 2265 7665 6e74 7322 2920 2626  0], "events") &&
-00000e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e10: 2020 2020 2020 2020 2020 2020 2024 2e5f               $._
-00000e20: 6461 7461 2845 6c2e 626f 6479 5b30 5d2c  data(El.body[0],
-00000e30: 2022 6576 656e 7473 2229 5b65 7665 6e74   "events")[event
-00000e40: 5d20 2626 0a20 2020 2020 2020 2020 2020  ] &&.           
+00000c50: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00000c60: 2020 2020 2020 2020 2020 2069 6620 2869             if (i
+00000c70: 7348 6569 6768 7455 7064 6174 6564 2920  sHeightUpdated) 
+00000c80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000c90: 2020 2020 2020 2020 2020 686f 6c64 6572            holder
+00000ca0: 2e63 7373 2827 6f70 6163 6974 7927 2c20  .css('opacity', 
+00000cb0: 3129 3b0a 2020 2020 2020 2020 2020 2020  1);.            
+00000cc0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000ce0: 6e73 7461 6e63 652e 696e 6974 4576 656e  nstance.initEven
+00000cf0: 7473 2877 6974 6853 7461 7465 293b 0a0a  ts(withState);..
+00000d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d10: 2020 2020 2066 6f72 2028 6920 6f66 204c       for (i of L
+00000d20: 6973 7465 6e65 7273 2e66 696c 7465 7228  isteners.filter(
+00000d30: 6520 3d3e 2065 2e6d 6574 686f 6420 3d3d  e => e.method ==
+00000d40: 3d20 2772 6566 7265 7368 4772 6964 4365  = 'refreshGridCe
+00000d50: 6c6c 2720 2626 2065 2e6f 7074 696f 6e73  ll' && e.options
+00000d60: 2e69 642e 696e 636c 7564 6573 2868 6f6c  .id.includes(hol
+00000d70: 6465 722e 6174 7472 2827 6964 2729 2929  der.attr('id')))
+00000d80: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00000d90: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000da0: 7420 6576 656e 7420 3d20 692e 6576 656e  t event = i.even
+00000db0: 744e 616d 652e 7370 6c69 7428 272e 2729  tName.split('.')
+00000dc0: 5b30 5d3b 0a20 2020 2020 2020 2020 2020  [0];.           
+00000dd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000de0: 2824 2e5f 6461 7461 2845 6c2e 626f 6479  ($._data(El.body
+00000df0: 5b30 5d2c 2022 6576 656e 7473 2229 2026  [0], "events") &
+00000e00: 260a 2020 2020 2020 2020 2020 2020 2020  &.              
+00000e10: 2020 2020 2020 2020 2020 2020 2020 242e                $.
+00000e20: 5f64 6174 6128 456c 2e62 6f64 795b 305d  _data(El.body[0]
+00000e30: 2c20 2265 7665 6e74 7322 295b 6576 656e  , "events")[even
+00000e40: 745d 2026 260a 2020 2020 2020 2020 2020  t] &&.          
 00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2024 2e5f 6461 7461 2845 6c2e 626f 6479   $._data(El.body
-00000e70: 5b30 5d2c 2022 6576 656e 7473 2229 5b65  [0], "events")[e
-00000e80: 7665 6e74 5d2e 6669 6c74 6572 2865 203d  vent].filter(e =
-00000e90: 3e20 652e 6461 7461 2e6d 6574 686f 6420  > e.data.method 
-00000ea0: 3d3d 3d20 2772 6566 7265 7368 4772 6964  === 'refreshGrid
-00000eb0: 4365 6c6c 2720 2626 0a20 2020 2020 2020  Cell' &&.       
+00000e60: 2020 242e 5f64 6174 6128 456c 2e62 6f64    $._data(El.bod
+00000e70: 795b 305d 2c20 2265 7665 6e74 7322 295b  y[0], "events")[
+00000e80: 6576 656e 745d 2e66 696c 7465 7228 6520  event].filter(e 
+00000e90: 3d3e 2065 2e64 6174 612e 6d65 7468 6f64  => e.data.method
+00000ea0: 203d 3d3d 2027 7265 6672 6573 6847 7269   === 'refreshGri
+00000eb0: 6443 656c 6c27 2026 260a 2020 2020 2020  dCell' &&.      
 00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 2020 2020 2065 2e64 6174 612e           e.data.
-00000ee0: 6f70 7469 6f6e 732e 6964 203d 3d3d 2069  options.id === i
-00000ef0: 2e6f 7074 696f 6e73 2e69 6429 2e6c 656e  .options.id).len
-00000f00: 6774 6820 3d3d 3d20 3029 207b 0a20 2020  gth === 0) {.   
+00000ed0: 2020 2020 2020 2020 2020 652e 6461 7461            e.data
+00000ee0: 2e6f 7074 696f 6e73 2e69 6420 3d3d 3d20  .options.id === 
+00000ef0: 692e 6f70 7469 6f6e 732e 6964 292e 6c65  i.options.id).le
+00000f00: 6e67 7468 203d 3d3d 2030 2920 7b0a 2020  ngth === 0) {.  
 00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 2020 2045 6c2e 626f 6479           El.body
-00000f30: 2e6f 6e28 692e 6576 656e 744e 616d 652c  .on(i.eventName,
-00000f40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000f20: 2020 2020 2020 2020 2020 456c 2e62 6f64            El.bod
+00000f30: 792e 6f6e 2869 2e65 7665 6e74 4e61 6d65  y.on(i.eventName
+00000f40: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
 00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 2020 206f 7074 696f 6e73 3a20 692e 6f70     options: i.op
-00000f70: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00000f60: 2020 2020 6f70 7469 6f6e 733a 2069 2e6f      options: i.o
+00000f70: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
 00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 206d 6574 686f 643a 2069         method: i
-00000fa0: 2e6d 6574 686f 642c 0a20 2020 2020 2020  .method,.       
+00000f90: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+00000fa0: 692e 6d65 7468 6f64 2c0a 2020 2020 2020  i.method,.      
 00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
-00000fd0: 6572 733a 2069 2e70 6172 616d 6574 6572  ers: i.parameter
-00000fe0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00001000: 2069 2e68 616e 646c 6572 293b 0a20 2020   i.handler);.   
+00000fc0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00000fd0: 7465 7273 3a20 692e 7061 7261 6d65 7465  ters: i.paramete
+00000fe0: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
+00000ff0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001000: 2c20 692e 6861 6e64 6c65 7229 3b0a 2020  , i.handler);.  
 00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00001030: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001020: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001030: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
 00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2069 6620 2821 7769 7468 5374 6174 6529   if (!withState)
-00001060: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001070: 2020 2020 2020 2020 2020 2045 6c2e 626f             El.bo
-00001080: 6479 2e74 7269 6767 6572 2827 7265 6e64  dy.trigger('rend
-00001090: 6572 6564 2e27 202b 206f 2e69 6429 3b0a  ered.' + o.id);.
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2020 2020 696e 7374 616e 6365          instance
-000010c0: 2e72 6566 7265 7368 4669 6e69 7368 6564  .refreshFinished
-000010d0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-000010e0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00001100: 7069 2e73 686f 7754 6f6f 6c54 6970 7343  pi.showToolTipsC
-00001110: 6861 6e67 6564 2829 3b0a 0a20 2020 2020  hanged();..     
-00001120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001130: 6e73 7461 6e63 652e 7265 6e64 6572 4c6f  nstance.renderLo
-00001140: 6164 6572 5374 6f70 2877 6974 684c 6f61  aderStop(withLoa
-00001150: 6465 7229 3b0a 0a20 2020 2020 2020 2020  der);..         
-00001160: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001170: 6e20 2772 6572 656e 6465 7265 6427 3b0a  n 'rerendered';.
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
-000011a0: 7d29 3b0a 2020 2020 2020 2020 7d29 3b0a  });.        });.
-000011b0: 2020 2020 7d0a 0a20 2020 2072 656e 6465      }..    rende
-000011c0: 7245 7272 6f72 2829 207b 0a20 2020 2020  rError() {.     
-000011d0: 2020 2063 6f6e 736f 6c65 2e65 7272 6f72     console.error
-000011e0: 2827 4475 706c 6963 6174 6520 7265 6e64  ('Duplicate rend
-000011f0: 6572 2063 616c 6c73 2061 7420 7468 6520  er calls at the 
-00001200: 7361 6d65 2074 696d 6520 666f 7220 7468  same time for th
-00001210: 6520 2720 2b20 7468 6973 2e6f 7074 696f  e ' + this.optio
-00001220: 6e73 2e69 6420 2b20 2720 7769 6467 6574  ns.id + ' widget
-00001230: 2127 293b 0a20 2020 2020 2020 2063 6f6e  !');.        con
-00001240: 736f 6c65 2e65 7272 6f72 2827 506c 6561  sole.error('Plea
-00001250: 7365 2063 6865 636b 2074 6865 2066 6f72  se check the for
-00001260: 6365 5265 6672 6573 6820 6675 6e63 7469  ceRefresh functi
-00001270: 6f6e 2063 616c 6c27 293b 0a20 2020 207d  on call');.    }
-00001280: 0a0a 2020 2020 7265 6e64 6572 5769 6467  ..    renderWidg
-00001290: 6574 2877 6974 6853 7461 7465 203d 2066  et(withState = f
-000012a0: 616c 7365 2c20 7769 7468 4c6f 6164 6572  alse, withLoader
-000012b0: 203d 2074 7275 652c 2070 7265 7669 6f75   = true, previou
-000012c0: 736c 794c 6f61 6465 6444 6174 6120 3d20  slyLoadedData = 
-000012d0: 6661 6c73 6529 207b 0a20 2020 2020 2020  false) {.       
-000012e0: 2069 6628 7468 6973 2e69 7352 656e 6465   if(this.isRende
-000012f0: 7269 6e67 2920 7b0a 2020 2020 2020 2020  ring) {.        
-00001300: 2020 2020 7468 6973 2e72 656e 6465 7245      this.renderE
-00001310: 7272 6f72 2829 3b0a 2020 2020 2020 2020  rror();.        
-00001320: 7d0a 2020 2020 2020 2020 7468 6973 2e69  }.        this.i
-00001330: 7352 656e 6465 7269 6e67 203d 2074 7275  sRendering = tru
-00001340: 653b 0a0a 2020 2020 2020 2020 636f 6e73  e;..        cons
-00001350: 7420 6f20 3d20 7468 6973 2e6f 7074 696f  t o = this.optio
-00001360: 6e73 2c20 686f 6c64 6572 203d 2074 6869  ns, holder = thi
-00001370: 732e 6765 7448 6f6c 6465 7228 6f2e 6964  s.getHolder(o.id
-00001380: 292c 2069 6e73 7461 6e63 6520 3d20 7468  ), instance = th
-00001390: 6973 3b0a 0a20 2020 2020 2020 2074 6869  is;..        thi
-000013a0: 732e 7265 6e64 6572 5374 6172 744c 6f61  s.renderStartLoa
-000013b0: 6465 7228 7769 7468 4c6f 6164 6572 293b  der(withLoader);
-000013c0: 0a0a 2020 2020 2020 2020 4c69 7374 656e  ..        Listen
-000013d0: 6572 732e 6c65 6e67 7468 203d 2030 3b0a  ers.length = 0;.
-000013e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000013f0: 686f 6c64 6572 2e65 6d70 7479 2829 2e6f  holder.empty().o
-00001400: 6666 2829 2e70 726f 6d69 7365 2829 2e74  ff().promise().t
-00001410: 6865 6e28 2829 203d 3e20 7b0a 0a20 2020  hen(() => {..   
-00001420: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
-00001430: 652e 686f 6c64 6572 5374 6172 744c 6f61  e.holderStartLoa
-00001440: 6465 7228 293b 0a0a 2020 2020 2020 2020  der();..        
-00001450: 2020 2020 7265 7475 726e 2069 6e73 7461      return insta
-00001460: 6e63 652e 7265 6e64 6572 2877 6974 6853  nce.render(withS
-00001470: 7461 7465 2c20 6661 6c73 652c 2066 616c  tate, false, fal
-00001480: 7365 2c20 5142 2e6c 6f61 6444 6174 612c  se, QB.loadData,
-00001490: 2070 7265 7669 6f75 736c 794c 6f61 6465   previouslyLoade
-000014a0: 6444 6174 6129 2e74 6865 6e28 6874 6d6c  dData).then(html
-000014b0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-000014c0: 2020 2020 2020 6c65 7420 6820 3d20 2428        let h = $(
-000014d0: 6874 6d6c 292c 2069 3b0a 0a20 2020 2020  html), i;..     
-000014e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000014f0: 6e20 686f 6c64 6572 2e68 746d 6c28 682e  n holder.html(h.
-00001500: 6874 6d6c 2829 292e 7072 6f6d 6973 6528  html()).promise(
-00001510: 292e 7468 656e 2828 2920 3d3e 207b 0a0a  ).then(() => {..
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2020 696e 7374 616e 6365 2e72 656d      instance.rem
-00001540: 6f76 654c 6f61 6465 7248 746d 6c28 7769  oveLoaderHtml(wi
-00001550: 7468 5374 6174 6529 3b0a 0a20 2020 2020  thState);..     
-00001560: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001570: 6e73 7461 6e63 652e 696e 6974 4576 656e  nstance.initEven
-00001580: 7473 2866 616c 7365 293b 0a0a 2020 2020  ts(false);..    
+00001050: 2020 6966 2028 2177 6974 6853 7461 7465    if (!withState
+00001060: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00001070: 2020 2020 2020 2020 2020 2020 456c 2e62              El.b
+00001080: 6f64 792e 7472 6967 6765 7228 2772 656e  ody.trigger('ren
+00001090: 6465 7265 642e 2720 2b20 6f2e 6964 293b  dered.' + o.id);
+000010a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010b0: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
+000010c0: 652e 7265 6672 6573 6846 696e 6973 6865  e.refreshFinishe
+000010d0: 6428 293b 0a20 2020 2020 2020 2020 2020  d();.           
+000010e0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 4170 692e 7368 6f77 546f 6f6c 5469 7073  Api.showToolTips
+00001110: 4368 616e 6765 6428 293b 0a0a 2020 2020  Changed();..    
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 696e 7374 616e 6365 2e72 656e 6465 724c  instance.renderL
+00001140: 6f61 6465 7253 746f 7028 7769 7468 4c6f  oaderStop(withLo
+00001150: 6164 6572 293b 0a0a 2020 2020 2020 2020  ader);..        
+00001160: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001170: 726e 2027 7265 7265 6e64 6572 6564 273b  rn 'rerendered';
+00001180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001190: 207d 293b 0a20 2020 2020 2020 2020 2020   });.           
+000011a0: 207d 293b 0a20 2020 2020 2020 207d 293b   });.        });
+000011b0: 0a20 2020 207d 0a0a 2020 2020 7265 6e64  .    }..    rend
+000011c0: 6572 4572 726f 7228 2920 7b0a 2020 2020  erError() {.    
+000011d0: 2020 2020 636f 6e73 6f6c 652e 6572 726f      console.erro
+000011e0: 7228 2744 7570 6c69 6361 7465 2072 656e  r('Duplicate ren
+000011f0: 6465 7220 6361 6c6c 7320 6174 2074 6865  der calls at the
+00001200: 2073 616d 6520 7469 6d65 2066 6f72 2074   same time for t
+00001210: 6865 2027 202b 2074 6869 732e 6f70 7469  he ' + this.opti
+00001220: 6f6e 732e 6964 202b 2027 2077 6964 6765  ons.id + ' widge
+00001230: 7421 2729 3b0a 2020 2020 2020 2020 636f  t!');.        co
+00001240: 6e73 6f6c 652e 6572 726f 7228 2750 6c65  nsole.error('Ple
+00001250: 6173 6520 6368 6563 6b20 7468 6520 666f  ase check the fo
+00001260: 7263 6552 6566 7265 7368 2066 756e 6374  rceRefresh funct
+00001270: 696f 6e20 6361 6c6c 2729 3b0a 2020 2020  ion call');.    
+00001280: 7d0a 0a20 2020 2072 656e 6465 7257 6964  }..    renderWid
+00001290: 6765 7428 7769 7468 5374 6174 6520 3d20  get(withState = 
+000012a0: 6661 6c73 652c 2077 6974 684c 6f61 6465  false, withLoade
+000012b0: 7220 3d20 7472 7565 2c20 7072 6576 696f  r = true, previo
+000012c0: 7573 6c79 4c6f 6164 6564 4461 7461 203d  uslyLoadedData =
+000012d0: 2066 616c 7365 2920 7b0a 2020 2020 2020   false) {.      
+000012e0: 2020 6966 2028 7468 6973 2e69 7352 656e    if (this.isRen
+000012f0: 6465 7269 6e67 2920 7b0a 2020 2020 2020  dering) {.      
+00001300: 2020 2020 2020 7468 6973 2e72 656e 6465        this.rende
+00001310: 7245 7272 6f72 2829 3b0a 2020 2020 2020  rError();.      
+00001320: 2020 7d0a 2020 2020 2020 2020 7468 6973    }.        this
+00001330: 2e69 7352 656e 6465 7269 6e67 203d 2074  .isRendering = t
+00001340: 7275 653b 0a0a 2020 2020 2020 2020 636f  rue;..        co
+00001350: 6e73 7420 6f20 3d20 7468 6973 2e6f 7074  nst o = this.opt
+00001360: 696f 6e73 2c20 686f 6c64 6572 203d 2074  ions, holder = t
+00001370: 6869 732e 6765 7448 6f6c 6465 7228 6f2e  his.getHolder(o.
+00001380: 6964 292c 2069 6e73 7461 6e63 6520 3d20  id), instance = 
+00001390: 7468 6973 3b0a 0a20 2020 2020 2020 2074  this;..        t
+000013a0: 6869 732e 7265 6e64 6572 5374 6172 744c  his.renderStartL
+000013b0: 6f61 6465 7228 7769 7468 4c6f 6164 6572  oader(withLoader
+000013c0: 293b 0a0a 2020 2020 2020 2020 4c69 7374  );..        List
+000013d0: 656e 6572 732e 6c65 6e67 7468 203d 2030  eners.length = 0
+000013e0: 3b0a 0a20 2020 2020 2020 2072 6574 7572  ;..        retur
+000013f0: 6e20 686f 6c64 6572 2e65 6d70 7479 2829  n holder.empty()
+00001400: 2e6f 6666 2829 2e70 726f 6d69 7365 2829  .off().promise()
+00001410: 2e74 6865 6e28 2829 203d 3e20 7b0a 0a20  .then(() => {.. 
+00001420: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001430: 6e63 652e 686f 6c64 6572 5374 6172 744c  nce.holderStartL
+00001440: 6f61 6465 7228 293b 0a0a 2020 2020 2020  oader();..      
+00001450: 2020 2020 2020 7265 7475 726e 2069 6e73        return ins
+00001460: 7461 6e63 652e 7265 6e64 6572 2877 6974  tance.render(wit
+00001470: 6853 7461 7465 2c20 6661 6c73 652c 2066  hState, false, f
+00001480: 616c 7365 2c20 5142 2e6c 6f61 6444 6174  alse, QB.loadDat
+00001490: 612c 2070 7265 7669 6f75 736c 794c 6f61  a, previouslyLoa
+000014a0: 6465 6444 6174 6129 2e74 6865 6e28 6874  dedData).then(ht
+000014b0: 6d6c 203d 3e20 7b0a 2020 2020 2020 2020  ml => {.        
+000014c0: 2020 2020 2020 2020 6c65 7420 6820 3d20          let h = 
+000014d0: 2428 6874 6d6c 292c 2069 3b0a 0a20 2020  $(html), i;..   
+000014e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000014f0: 7572 6e20 686f 6c64 6572 2e68 746d 6c28  urn holder.html(
+00001500: 682e 6874 6d6c 2829 292e 7072 6f6d 6973  h.html()).promis
+00001510: 6528 292e 7468 656e 2828 2920 3d3e 207b  e().then(() => {
+00001520: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001530: 2020 2020 2020 696e 7374 616e 6365 2e72        instance.r
+00001540: 656d 6f76 654c 6f61 6465 7248 746d 6c28  emoveLoaderHtml(
+00001550: 7769 7468 5374 6174 6529 3b0a 0a20 2020  withState);..   
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2069 6e73 7461 6e63 652e 696e 6974 4576   instance.initEv
+00001580: 656e 7473 2866 616c 7365 293b 0a0a 2020  ents(false);..  
 00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 666f 7220 2869 206f 6620 4c69 7374 656e  for (i of Listen
-000015b0: 6572 7329 207b 0a20 2020 2020 2020 2020  ers) {.         
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2045                 E
-000015d0: 6c2e 626f 6479 2e6f 6e28 692e 6576 656e  l.body.on(i.even
-000015e0: 744e 616d 652c 207b 0a20 2020 2020 2020  tName, {.       
+000015a0: 2020 666f 7220 2869 206f 6620 4c69 7374    for (i of List
+000015b0: 656e 6572 7329 207b 0a20 2020 2020 2020  eners) {.       
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 2045 6c2e 626f 6479 2e6f 6e28 692e 6576   El.body.on(i.ev
+000015e0: 656e 744e 616d 652c 207b 0a20 2020 2020  entName, {.     
 000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 206f 7074 696f 6e73 3a20 692e       options: i.
-00001610: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
+00001600: 2020 2020 2020 206f 7074 696f 6e73 3a20         options: 
+00001610: 692e 6f70 7469 6f6e 732c 0a20 2020 2020  i.options,.     
 00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 206d 6574 686f 643a 2069 2e6d       method: i.m
-00001640: 6574 686f 642c 0a20 2020 2020 2020 2020  ethod,.         
+00001630: 2020 2020 2020 206d 6574 686f 643a 2069         method: i
+00001640: 2e6d 6574 686f 642c 0a20 2020 2020 2020  .method,.       
 00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2070 6172 616d 6574 6572 733a 2069     parameters: i
-00001670: 2e70 6172 616d 6574 6572 730a 2020 2020  .parameters.    
+00001660: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
+00001670: 2069 2e70 6172 616d 6574 6572 730a 2020   i.parameters.  
 00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 2020 7d2c 2069 2e68 616e 646c 6572      }, i.handler
-000016a0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000016b0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000016c0: 2020 2020 2020 2020 2020 2020 2045 6c2e               El.
-000016d0: 626f 6479 2e74 7269 6767 6572 2827 626f  body.trigger('bo
-000016e0: 6479 5265 6164 7927 293b 0a20 2020 2020  dyReady');.     
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001700: 6620 2821 7769 7468 5374 6174 6529 207b  f (!withState) {
-00001710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001720: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
-00001730: 652e 696e 6974 4669 6e69 7368 6564 2829  e.initFinished()
-00001740: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00001750: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00001760: 2020 2020 2020 2020 2020 2020 2041 7069               Api
-00001770: 2e73 686f 7754 6f6f 6c54 6970 7343 6861  .showToolTipsCha
-00001780: 6e67 6564 2829 3b0a 0a20 2020 2020 2020  nged();..       
-00001790: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
-000017a0: 7461 6e63 652e 7265 6e64 6572 4c6f 6164  tance.renderLoad
-000017b0: 6572 5374 6f70 2877 6974 684c 6f61 6465  erStop(withLoade
-000017c0: 7229 3b0a 0a20 2020 2020 2020 2020 2020  r);..           
-000017d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000017e0: 2772 656e 6465 7265 6427 3b0a 2020 2020  'rendered';.    
-000017f0: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00001800: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00001810: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
-00001820: 7d0a 0a20 2020 2075 7064 6174 6557 6964  }..    updateWid
-00001830: 6765 7443 6f6e 7465 6e74 2877 6974 684c  getContent(withL
-00001840: 6f61 6465 7220 3d20 7472 7565 2920 7b0a  oader = true) {.
-00001850: 2020 2020 2020 2020 7769 7468 4c6f 6164          withLoad
-00001860: 6572 2026 2620 4c6f 6164 6572 2e73 7461  er && Loader.sta
-00001870: 7274 2874 7275 6529 3b0a 2020 2020 2020  rt(true);.      
-00001880: 2020 6c65 7420 696e 7374 616e 6365 203d    let instance =
-00001890: 2074 6869 733b 0a20 2020 2020 2020 2072   this;.        r
-000018a0: 6574 7572 6e20 7468 6973 2e75 7064 6174  eturn this.updat
-000018b0: 6543 6f6e 7465 6e74 2829 2e74 6865 6e28  eContent().then(
-000018c0: 2872 2920 3d3e 207b 0a20 2020 2020 2020  (r) => {.       
-000018d0: 2020 2020 2069 6620 2827 7570 6461 7465       if ('update
-000018e0: 2720 3d3d 3d20 7229 207b 0a20 2020 2020  ' === r) {.     
-000018f0: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
-00001900: 6e63 652e 7570 6461 7465 436f 6e74 656e  nce.updateConten
-00001910: 7446 696e 6973 6865 6428 293b 0a20 2020  tFinished();.   
-00001920: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001930: 2020 2020 2020 2077 6974 684c 6f61 6465         withLoade
-00001940: 7220 2626 204c 6f61 6465 722e 7374 6f70  r && Loader.stop
-00001950: 2874 7275 6529 3b0a 2020 2020 2020 2020  (true);.        
-00001960: 7d29 3b0a 2020 2020 7d0a 0a20 2020 2067  });.    }..    g
-00001970: 6574 5769 6467 6574 2877 6964 6765 744f  etWidget(widgetO
-00001980: 7074 696f 6e73 2920 7b0a 2020 2020 2020  ptions) {.      
-00001990: 2020 6966 2028 7769 6467 6574 4f70 7469    if (widgetOpti
-000019a0: 6f6e 732e 696d 706f 7274 2920 7b0a 2020  ons.import) {.  
-000019b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000019c0: 2057 6964 6765 7473 5b76 2877 6964 6765   Widgets[v(widge
-000019d0: 744f 7074 696f 6e73 2e69 6d70 6f72 742c  tOptions.import,
-000019e0: 2057 6964 6765 7443 6f6e 6669 6729 2e69   WidgetConfig).i
-000019f0: 645d 3b0a 2020 2020 2020 2020 7d0a 2020  d];.        }.  
-00001a00: 2020 2020 2020 7265 7475 726e 2057 6964        return Wid
-00001a10: 6765 7473 5b77 6964 6765 744f 7074 696f  gets[widgetOptio
-00001a20: 6e73 2e69 645d 3b0a 2020 2020 7d0a 0a20  ns.id];.    }.. 
-00001a30: 2020 2069 7343 6f6e 7465 6e74 5570 6461     isContentUpda
-00001a40: 7461 626c 6528 2920 7b0a 2020 2020 2020  table() {.      
-00001a50: 2020 7265 7475 726e 2074 7275 653b 0a20    return true;. 
-00001a60: 2020 207d 0a0a 2020 2020 7570 6461 7465     }..    update
-00001a70: 436f 6e74 656e 7428 6461 7461 203d 2066  Content(data = f
-00001a80: 616c 7365 2c20 6c6f 6164 4675 6e63 7469  alse, loadFuncti
-00001a90: 6f6e 203d 2051 422e 6c6f 6164 4461 7461  on = QB.loadData
-00001aa0: 2920 7b0a 2020 2020 2020 2020 636f 6e73  ) {.        cons
-00001ab0: 7420 6f20 3d20 7468 6973 2e6f 7074 696f  t o = this.optio
-00001ac0: 6e73 2c20 696e 7374 616e 6365 203d 2074  ns, instance = t
-00001ad0: 6869 733b 0a20 2020 2020 2020 206c 6574  his;.        let
-00001ae0: 2077 772c 2077 6964 6765 744f 7074 696f   ww, widgetOptio
-00001af0: 6e73 2c20 7072 6f63 6573 7365 6444 6174  ns, processedDat
-00001b00: 612c 2064 6566 6572 7265 6420 3d20 5b5d  a, deferred = []
-00001b10: 3b0a 0a20 2020 2020 2020 2066 6f72 2028  ;..        for (
-00001b20: 7769 6467 6574 4f70 7469 6f6e 7320 6f66  widgetOptions of
-00001b30: 206f 2e77 6964 6765 7473 207c 7c20 5b5d   o.widgets || []
-00001b40: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00001b50: 7777 203d 2074 6869 732e 6765 7457 6964  ww = this.getWid
-00001b60: 6765 7428 7769 6467 6574 4f70 7469 6f6e  get(widgetOption
-00001b70: 7329 3b0a 2020 2020 2020 2020 2020 2020  s);.            
-00001b80: 6465 6665 7272 6564 2e70 7573 6828 7777  deferred.push(ww
-00001b90: 2e75 7064 6174 6543 6f6e 7465 6e74 2829  .updateContent()
-00001ba0: 293b 0a20 2020 2020 2020 207d 0a0a 2020  );.        }..  
-00001bb0: 2020 2020 2020 6966 2028 6461 7461 2021        if (data !
-00001bc0: 3d3d 2066 616c 7365 2920 7b0a 2020 2020  == false) {.    
-00001bd0: 2020 2020 2020 2020 7265 7475 726e 2024          return $
-00001be0: 2e77 6865 6e2e 6170 706c 7928 242c 2064  .when.apply($, d
-00001bf0: 6566 6572 7265 6429 2e74 6865 6e28 6675  eferred).then(fu
-00001c00: 6e63 7469 6f6e 2028 2920 7b0a 2020 2020  nction () {.    
-00001c10: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00001c20: 6573 7365 6444 6174 6120 3d20 696e 7374  essedData = inst
-00001c30: 616e 6365 2e70 726f 6365 7373 4461 7461  ance.processData
-00001c40: 2864 6174 6129 3b0a 2020 2020 2020 2020  (data);.        
-00001c50: 2020 2020 2020 2020 696e 7374 616e 6365          instance
-00001c60: 2e75 7064 6174 6548 746d 6c28 7072 6f63  .updateHtml(proc
-00001c70: 6573 7365 6444 6174 6129 3b0a 2020 2020  essedData);.    
-00001c80: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
-00001c90: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
-00001ca0: 6574 7572 6e20 6c6f 6164 4675 6e63 7469  eturn loadFuncti
-00001cb0: 6f6e 286f 2e69 642c 2069 6e73 7461 6e63  on(o.id, instanc
-00001cc0: 652e 6e61 6d65 292e 7468 656e 2866 756e  e.name).then(fun
-00001cd0: 6374 696f 6e20 2864 2920 7b0a 2020 2020  ction (d) {.    
-00001ce0: 2020 2020 2020 2020 7265 7475 726e 2024          return $
-00001cf0: 2e77 6865 6e2e 6170 706c 7928 242c 2064  .when.apply($, d
-00001d00: 6566 6572 7265 6429 2e74 6865 6e28 6675  eferred).then(fu
-00001d10: 6e63 7469 6f6e 2028 2920 7b0a 2020 2020  nction () {.    
-00001d20: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00001d30: 6573 7365 6444 6174 6120 3d20 696e 7374  essedData = inst
-00001d40: 616e 6365 2e70 726f 6365 7373 4461 7461  ance.processData
-00001d50: 2864 293b 0a20 2020 2020 2020 2020 2020  (d);.           
-00001d60: 2020 2020 2069 6e73 7461 6e63 652e 7570       instance.up
-00001d70: 6461 7465 4874 6d6c 2870 726f 6365 7373  dateHtml(process
-00001d80: 6564 4461 7461 293b 0a20 2020 2020 2020  edData);.       
-00001d90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001da0: 2775 7064 6174 6527 3b0a 2020 2020 2020  'update';.      
-00001db0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00001dc0: 2020 7d29 3b0a 2020 2020 7d0a 0a20 2020    });.    }..   
-00001dd0: 2075 7064 6174 6548 746d 6c28 6461 7461   updateHtml(data
-00001de0: 2920 7b0a 0a20 2020 207d 0a0a 2020 2020  ) {..    }..    
-00001df0: 7265 6e64 6572 2877 6974 6853 7461 7465  render(withState
-00001e00: 2c20 7265 6672 6573 682c 2075 7365 4465  , refresh, useDe
-00001e10: 6661 756c 7444 6174 6120 3d20 6661 6c73  faultData = fals
-00001e20: 652c 206c 6f61 6446 756e 6374 696f 6e20  e, loadFunction 
-00001e30: 3d20 5142 2e6c 6f61 6444 6174 612c 2070  = QB.loadData, p
-00001e40: 7265 7669 6f75 736c 794c 6f61 6465 6444  reviouslyLoadedD
-00001e50: 6174 6120 3d20 6661 6c73 6529 207b 0a20  ata = false) {. 
-00001e60: 2020 2020 2020 2074 6869 732e 6973 5265         this.isRe
-00001e70: 6e64 6572 696e 6720 3d20 7472 7565 3b0a  ndering = true;.
-00001e80: 2020 2020 2020 2020 636f 6e73 7420 6f20          const o 
-00001e90: 3d20 7468 6973 2e6f 7074 696f 6e73 2c20  = this.options, 
-00001ea0: 696e 7374 616e 6365 203d 2074 6869 733b  instance = this;
-00001eb0: 0a20 2020 2020 2020 206c 6574 2077 773b  .        let ww;
-00001ec0: 0a0a 2020 2020 2020 2020 6c65 7420 7769  ..        let wi
-00001ed0: 6467 6574 4f70 7469 6f6e 732c 2077 6964  dgetOptions, wid
-00001ee0: 6765 7473 203d 205b 5d3b 0a0a 2020 2020  gets = [];..    
-00001ef0: 2020 2020 666f 7220 2877 6964 6765 744f      for (widgetO
-00001f00: 7074 696f 6e73 206f 6620 6f2e 7769 6467  ptions of o.widg
-00001f10: 6574 7320 7c7c 205b 5d29 207b 0a20 2020  ets || []) {.   
-00001f20: 2020 2020 2020 2020 2077 7720 3d20 7468           ww = th
-00001f30: 6973 2e67 6574 5769 6467 6574 2877 6964  is.getWidget(wid
-00001f40: 6765 744f 7074 696f 6e73 293b 0a20 2020  getOptions);.   
-00001f50: 2020 2020 2020 2020 2077 6964 6765 7473           widgets
-00001f60: 2e70 7573 6828 7777 293b 0a20 2020 2020  .push(ww);.     
-00001f70: 2020 207d 0a0a 2020 2020 2020 2020 7468     }..        th
-00001f80: 6973 2e61 6464 4c69 7374 656e 6572 7328  is.addListeners(
-00001f90: 6661 6c73 6529 3b0a 0a20 2020 2020 2020  false);..       
-00001fa0: 206c 6574 2075 7365 4465 6661 756c 7444   let useDefaultD
-00001fb0: 6174 6146 6f72 4368 696c 6472 656e 203d  ataForChildren =
-00001fc0: 2028 6f2e 7669 7369 626c 6520 3d3d 3d20   (o.visible === 
-00001fd0: 6661 6c73 6520 2626 2021 7265 6672 6573  false && !refres
-00001fe0: 6820 2626 206f 2e6e 6f74 4c6f 6164 4966  h && o.notLoadIf
-00001ff0: 4869 6464 656e 2920 7c7c 2075 7365 4465  Hidden) || useDe
-00002000: 6661 756c 7444 6174 613b 0a0a 2020 2020  faultData;..    
-00002010: 2020 2020 6c65 7420 6166 7465 724c 6f61      let afterLoa
-00002020: 6420 3d20 2864 6174 6129 203d 3e20 7b0a  d = (data) => {.
-00002030: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-00002040: 6465 6665 7272 6564 203d 205b 5d2c 2077  deferred = [], w
-00002050: 3b0a 2020 2020 2020 2020 2020 2020 666f  ;.            fo
-00002060: 7220 2877 206f 6620 7769 6467 6574 7329  r (w of widgets)
-00002070: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00002080: 2020 2064 6566 6572 7265 642e 7075 7368     deferred.push
-00002090: 2877 2e72 656e 6465 7228 7769 7468 5374  (w.render(withSt
-000020a0: 6174 652c 2072 6566 7265 7368 2c20 7573  ate, refresh, us
-000020b0: 6544 6566 6175 6c74 4461 7461 466f 7243  eDefaultDataForC
-000020c0: 6869 6c64 7265 6e29 293b 0a20 2020 2020  hildren));.     
-000020d0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000020e0: 2020 2020 2020 7265 7475 726e 2024 2e77        return $.w
-000020f0: 6865 6e2e 6170 706c 7928 242c 2064 6566  hen.apply($, def
-00002100: 6572 7265 6429 2e74 6865 6e28 6675 6e63  erred).then(func
-00002110: 7469 6f6e 2028 2e2e 2e72 6573 756c 7473  tion (...results
-00002120: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00002130: 2020 2020 6c65 7420 7769 6467 6574 4874      let widgetHt
-00002140: 6d6c 7320 3d20 5b5d 2c20 722c 2070 726f  mls = [], r, pro
-00002150: 6365 7373 6564 4461 7461 203d 2069 6e73  cessedData = ins
-00002160: 7461 6e63 652e 7072 6f63 6573 7344 6174  tance.processDat
-00002170: 6128 6461 7461 292c 2076 203d 2028 7072  a(data), v = (pr
-00002180: 6f63 6573 7365 6444 6174 6120 7c7c 207b  ocessedData || {
-00002190: 7d29 2e76 6973 6962 6c65 2c0a 2020 2020  }).visible,.    
+00001690: 2020 2020 2020 7d2c 2069 2e68 616e 646c        }, i.handl
+000016a0: 6572 293b 0a20 2020 2020 2020 2020 2020  er);.           
+000016b0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2045                 E
+000016d0: 6c2e 626f 6479 2e74 7269 6767 6572 2827  l.body.trigger('
+000016e0: 626f 6479 5265 6164 7927 293b 0a20 2020  bodyReady');.   
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2069 6620 2821 7769 7468 5374 6174 6529   if (!withState)
+00001710: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001720: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001730: 6e63 652e 696e 6974 4669 6e69 7368 6564  nce.initFinished
+00001740: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
+00001750: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001760: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00001770: 7069 2e73 686f 7754 6f6f 6c54 6970 7343  pi.showToolTipsC
+00001780: 6861 6e67 6564 2829 3b0a 0a20 2020 2020  hanged();..     
+00001790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000017a0: 6e73 7461 6e63 652e 7265 6e64 6572 4c6f  nstance.renderLo
+000017b0: 6164 6572 5374 6f70 2877 6974 684c 6f61  aderStop(withLoa
+000017c0: 6465 7229 3b0a 0a20 2020 2020 2020 2020  der);..         
+000017d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000017e0: 6e20 2772 656e 6465 7265 6427 3b0a 2020  n 'rendered';.  
+000017f0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+00001800: 3b0a 2020 2020 2020 2020 2020 2020 7d29  ;.            })
+00001810: 3b0a 2020 2020 2020 2020 7d29 3b0a 2020  ;.        });.  
+00001820: 2020 7d0a 0a20 2020 2075 7064 6174 6557    }..    updateW
+00001830: 6964 6765 7443 6f6e 7465 6e74 2877 6974  idgetContent(wit
+00001840: 684c 6f61 6465 7220 3d20 7472 7565 2920  hLoader = true) 
+00001850: 7b0a 2020 2020 2020 2020 7769 7468 4c6f  {.        withLo
+00001860: 6164 6572 2026 2620 4c6f 6164 6572 2e73  ader && Loader.s
+00001870: 7461 7274 2874 7275 6529 3b0a 2020 2020  tart(true);.    
+00001880: 2020 2020 6c65 7420 696e 7374 616e 6365      let instance
+00001890: 203d 2074 6869 733b 0a20 2020 2020 2020   = this;.       
+000018a0: 2072 6574 7572 6e20 7468 6973 2e75 7064   return this.upd
+000018b0: 6174 6543 6f6e 7465 6e74 2829 2e74 6865  ateContent().the
+000018c0: 6e28 2872 2920 3d3e 207b 0a20 2020 2020  n((r) => {.     
+000018d0: 2020 2020 2020 2069 6620 2827 7570 6461         if ('upda
+000018e0: 7465 2720 3d3d 3d20 7229 207b 0a20 2020  te' === r) {.   
+000018f0: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
+00001900: 7461 6e63 652e 7570 6461 7465 436f 6e74  tance.updateCont
+00001910: 656e 7446 696e 6973 6865 6428 293b 0a20  entFinished();. 
+00001920: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001930: 2020 2020 2020 2020 2077 6974 684c 6f61           withLoa
+00001940: 6465 7220 2626 204c 6f61 6465 722e 7374  der && Loader.st
+00001950: 6f70 2874 7275 6529 3b0a 2020 2020 2020  op(true);.      
+00001960: 2020 7d29 3b0a 2020 2020 7d0a 0a20 2020    });.    }..   
+00001970: 2067 6574 5769 6467 6574 2877 6964 6765   getWidget(widge
+00001980: 744f 7074 696f 6e73 2920 7b0a 2020 2020  tOptions) {.    
+00001990: 2020 2020 6966 2028 7769 6467 6574 4f70      if (widgetOp
+000019a0: 7469 6f6e 732e 696d 706f 7274 2920 7b0a  tions.import) {.
+000019b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000019c0: 726e 2057 6964 6765 7473 5b76 2877 6964  rn Widgets[v(wid
+000019d0: 6765 744f 7074 696f 6e73 2e69 6d70 6f72  getOptions.impor
+000019e0: 742c 2057 6964 6765 7443 6f6e 6669 6729  t, WidgetConfig)
+000019f0: 2e69 645d 3b0a 2020 2020 2020 2020 7d0a  .id];.        }.
+00001a00: 2020 2020 2020 2020 7265 7475 726e 2057          return W
+00001a10: 6964 6765 7473 5b77 6964 6765 744f 7074  idgets[widgetOpt
+00001a20: 696f 6e73 2e69 645d 3b0a 2020 2020 7d0a  ions.id];.    }.
+00001a30: 0a20 2020 2069 7343 6f6e 7465 6e74 5570  .    isContentUp
+00001a40: 6461 7461 626c 6528 2920 7b0a 2020 2020  datable() {.    
+00001a50: 2020 2020 7265 7475 726e 2074 7275 653b      return true;
+00001a60: 0a20 2020 207d 0a0a 2020 2020 7570 6461  .    }..    upda
+00001a70: 7465 436f 6e74 656e 7428 6461 7461 203d  teContent(data =
+00001a80: 2066 616c 7365 2c20 6c6f 6164 4675 6e63   false, loadFunc
+00001a90: 7469 6f6e 203d 2051 422e 6c6f 6164 4461  tion = QB.loadDa
+00001aa0: 7461 2920 7b0a 2020 2020 2020 2020 636f  ta) {.        co
+00001ab0: 6e73 7420 6f20 3d20 7468 6973 2e6f 7074  nst o = this.opt
+00001ac0: 696f 6e73 2c20 696e 7374 616e 6365 203d  ions, instance =
+00001ad0: 2074 6869 733b 0a20 2020 2020 2020 206c   this;.        l
+00001ae0: 6574 2077 772c 2077 6964 6765 744f 7074  et ww, widgetOpt
+00001af0: 696f 6e73 2c20 7072 6f63 6573 7365 6444  ions, processedD
+00001b00: 6174 612c 2064 6566 6572 7265 6420 3d20  ata, deferred = 
+00001b10: 5b5d 3b0a 0a20 2020 2020 2020 2066 6f72  [];..        for
+00001b20: 2028 7769 6467 6574 4f70 7469 6f6e 7320   (widgetOptions 
+00001b30: 6f66 206f 2e77 6964 6765 7473 207c 7c20  of o.widgets || 
+00001b40: 5b5d 2920 7b0a 2020 2020 2020 2020 2020  []) {.          
+00001b50: 2020 7777 203d 2074 6869 732e 6765 7457    ww = this.getW
+00001b60: 6964 6765 7428 7769 6467 6574 4f70 7469  idget(widgetOpti
+00001b70: 6f6e 7329 3b0a 2020 2020 2020 2020 2020  ons);.          
+00001b80: 2020 6465 6665 7272 6564 2e70 7573 6828    deferred.push(
+00001b90: 7777 2e75 7064 6174 6543 6f6e 7465 6e74  ww.updateContent
+00001ba0: 2829 293b 0a20 2020 2020 2020 207d 0a0a  ());.        }..
+00001bb0: 2020 2020 2020 2020 6966 2028 6461 7461          if (data
+00001bc0: 2021 3d3d 2066 616c 7365 2920 7b0a 2020   !== false) {.  
+00001bd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001be0: 2024 2e77 6865 6e2e 6170 706c 7928 242c   $.when.apply($,
+00001bf0: 2064 6566 6572 7265 6429 2e74 6865 6e28   deferred).then(
+00001c00: 6675 6e63 7469 6f6e 2028 2920 7b0a 2020  function () {.  
+00001c10: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001c20: 6f63 6573 7365 6444 6174 6120 3d20 696e  ocessedData = in
+00001c30: 7374 616e 6365 2e70 726f 6365 7373 4461  stance.processDa
+00001c40: 7461 2864 6174 6129 3b0a 2020 2020 2020  ta(data);.      
+00001c50: 2020 2020 2020 2020 2020 696e 7374 616e            instan
+00001c60: 6365 2e75 7064 6174 6548 746d 6c28 7072  ce.updateHtml(pr
+00001c70: 6f63 6573 7365 6444 6174 6129 3b0a 2020  ocessedData);.  
+00001c80: 2020 2020 2020 2020 2020 7d29 3b0a 2020            });.  
+00001c90: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00001ca0: 2072 6574 7572 6e20 6c6f 6164 4675 6e63   return loadFunc
+00001cb0: 7469 6f6e 286f 2e69 642c 2069 6e73 7461  tion(o.id, insta
+00001cc0: 6e63 652e 6e61 6d65 292e 7468 656e 2866  nce.name).then(f
+00001cd0: 756e 6374 696f 6e20 2864 2920 7b0a 2020  unction (d) {.  
+00001ce0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001cf0: 2024 2e77 6865 6e2e 6170 706c 7928 242c   $.when.apply($,
+00001d00: 2064 6566 6572 7265 6429 2e74 6865 6e28   deferred).then(
+00001d10: 6675 6e63 7469 6f6e 2028 2920 7b0a 2020  function () {.  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001d30: 6f63 6573 7365 6444 6174 6120 3d20 696e  ocessedData = in
+00001d40: 7374 616e 6365 2e70 726f 6365 7373 4461  stance.processDa
+00001d50: 7461 2864 293b 0a20 2020 2020 2020 2020  ta(d);.         
+00001d60: 2020 2020 2020 2069 6e73 7461 6e63 652e         instance.
+00001d70: 7570 6461 7465 4874 6d6c 2870 726f 6365  updateHtml(proce
+00001d80: 7373 6564 4461 7461 293b 0a20 2020 2020  ssedData);.     
+00001d90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001da0: 6e20 2775 7064 6174 6527 3b0a 2020 2020  n 'update';.    
+00001db0: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
+00001dc0: 2020 2020 7d29 3b0a 2020 2020 7d0a 0a20      });.    }.. 
+00001dd0: 2020 2075 7064 6174 6548 746d 6c28 6461     updateHtml(da
+00001de0: 7461 2920 7b0a 0a20 2020 207d 0a0a 2020  ta) {..    }..  
+00001df0: 2020 7265 6e64 6572 2877 6974 6853 7461    render(withSta
+00001e00: 7465 2c20 7265 6672 6573 682c 2075 7365  te, refresh, use
+00001e10: 4465 6661 756c 7444 6174 6120 3d20 6661  DefaultData = fa
+00001e20: 6c73 652c 206c 6f61 6446 756e 6374 696f  lse, loadFunctio
+00001e30: 6e20 3d20 5142 2e6c 6f61 6444 6174 612c  n = QB.loadData,
+00001e40: 2070 7265 7669 6f75 736c 794c 6f61 6465   previouslyLoade
+00001e50: 6444 6174 6120 3d20 6661 6c73 6529 207b  dData = false) {
+00001e60: 0a20 2020 2020 2020 2074 6869 732e 6973  .        this.is
+00001e70: 5265 6e64 6572 696e 6720 3d20 7472 7565  Rendering = true
+00001e80: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
+00001e90: 6f20 3d20 7468 6973 2e6f 7074 696f 6e73  o = this.options
+00001ea0: 2c20 696e 7374 616e 6365 203d 2074 6869  , instance = thi
+00001eb0: 733b 0a20 2020 2020 2020 206c 6574 2077  s;.        let w
+00001ec0: 773b 0a0a 2020 2020 2020 2020 6c65 7420  w;..        let 
+00001ed0: 7769 6467 6574 4f70 7469 6f6e 732c 2077  widgetOptions, w
+00001ee0: 6964 6765 7473 203d 205b 5d3b 0a0a 2020  idgets = [];..  
+00001ef0: 2020 2020 2020 666f 7220 2877 6964 6765        for (widge
+00001f00: 744f 7074 696f 6e73 206f 6620 6f2e 7769  tOptions of o.wi
+00001f10: 6467 6574 7320 7c7c 205b 5d29 207b 0a20  dgets || []) {. 
+00001f20: 2020 2020 2020 2020 2020 2077 7720 3d20             ww = 
+00001f30: 7468 6973 2e67 6574 5769 6467 6574 2877  this.getWidget(w
+00001f40: 6964 6765 744f 7074 696f 6e73 293b 0a20  idgetOptions);. 
+00001f50: 2020 2020 2020 2020 2020 2077 6964 6765             widge
+00001f60: 7473 2e70 7573 6828 7777 293b 0a20 2020  ts.push(ww);.   
+00001f70: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00001f80: 7468 6973 2e61 6464 4c69 7374 656e 6572  this.addListener
+00001f90: 7328 6661 6c73 6529 3b0a 0a20 2020 2020  s(false);..     
+00001fa0: 2020 206c 6574 2075 7365 4465 6661 756c     let useDefaul
+00001fb0: 7444 6174 6146 6f72 4368 696c 6472 656e  tDataForChildren
+00001fc0: 203d 2028 6f2e 7669 7369 626c 6520 3d3d   = (o.visible ==
+00001fd0: 3d20 6661 6c73 6520 2626 2021 7265 6672  = false && !refr
+00001fe0: 6573 6820 2626 206f 2e6e 6f74 4c6f 6164  esh && o.notLoad
+00001ff0: 4966 4869 6464 656e 2920 7c7c 2075 7365  IfHidden) || use
+00002000: 4465 6661 756c 7444 6174 613b 0a0a 2020  DefaultData;..  
+00002010: 2020 2020 2020 6c65 7420 6166 7465 724c        let afterL
+00002020: 6f61 6420 3d20 2864 6174 6129 203d 3e20  oad = (data) => 
+00002030: 7b0a 2020 2020 2020 2020 2020 2020 6c65  {.            le
+00002040: 7420 6465 6665 7272 6564 203d 205b 5d2c  t deferred = [],
+00002050: 2077 3b0a 2020 2020 2020 2020 2020 2020   w;.            
+00002060: 666f 7220 2877 206f 6620 7769 6467 6574  for (w of widget
+00002070: 7329 207b 0a20 2020 2020 2020 2020 2020  s) {.           
+00002080: 2020 2020 2064 6566 6572 7265 642e 7075       deferred.pu
+00002090: 7368 2877 2e72 656e 6465 7228 7769 7468  sh(w.render(with
+000020a0: 5374 6174 652c 2072 6566 7265 7368 2c20  State, refresh, 
+000020b0: 7573 6544 6566 6175 6c74 4461 7461 466f  useDefaultDataFo
+000020c0: 7243 6869 6c64 7265 6e29 293b 0a20 2020  rChildren));.   
+000020d0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+000020e0: 2020 2020 2020 2020 7265 7475 726e 2024          return $
+000020f0: 2e77 6865 6e2e 6170 706c 7928 242c 2064  .when.apply($, d
+00002100: 6566 6572 7265 6429 2e74 6865 6e28 6675  eferred).then(fu
+00002110: 6e63 7469 6f6e 2028 2e2e 2e72 6573 756c  nction (...resul
+00002120: 7473 2920 7b0a 2020 2020 2020 2020 2020  ts) {.          
+00002130: 2020 2020 2020 6c65 7420 7769 6467 6574        let widget
+00002140: 4874 6d6c 7320 3d20 5b5d 2c20 722c 2070  Htmls = [], r, p
+00002150: 726f 6365 7373 6564 4461 7461 203d 2069  rocessedData = i
+00002160: 6e73 7461 6e63 652e 7072 6f63 6573 7344  nstance.processD
+00002170: 6174 6128 6461 7461 292c 2076 203d 2028  ata(data), v = (
+00002180: 7072 6f63 6573 7365 6444 6174 6120 7c7c  processedData ||
+00002190: 207b 7d29 2e76 6973 6962 6c65 2c0a 2020   {}).visible,.  
 000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 7669 7369 626c 6520 3d20 756e 6465 6669  visible = undefi
-000021c0: 6e65 6420 213d 3d20 7620 3f20 7620 3a20  ned !== v ? v : 
-000021d0: 6f2e 7669 7369 626c 653b 0a0a 2020 2020  o.visible;..    
-000021e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000021f0: 2872 206f 6620 7265 7375 6c74 7329 207b  (r of results) {
-00002200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002210: 2020 2020 2077 6964 6765 7448 746d 6c73       widgetHtmls
-00002220: 2e70 7573 6828 7229 3b0a 2020 2020 2020  .push(r);.      
-00002230: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
-00002240: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002250: 7572 6e20 696e 7374 616e 6365 2e67 6574  urn instance.get
-00002260: 4d61 696e 4874 6d6c 456c 656d 656e 7428  MainHtmlElement(
-00002270: 6f2c 2070 726f 6365 7373 6564 4461 7461  o, processedData
-00002280: 2c20 7669 7369 626c 652c 2077 6964 6765  , visible, widge
-00002290: 7448 746d 6c73 2c20 7769 7468 5374 6174  tHtmls, withStat
-000022a0: 6529 3b0a 2020 2020 2020 2020 2020 2020  e);.            
-000022b0: 7d29 3b0a 2020 2020 2020 2020 7d3b 0a0a  });.        };..
-000022c0: 2020 2020 2020 2020 6966 2028 7072 6576          if (prev
-000022d0: 696f 7573 6c79 4c6f 6164 6564 4461 7461  iouslyLoadedData
-000022e0: 2021 3d3d 2066 616c 7365 2920 7b0a 2020   !== false) {.  
-000022f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002300: 2061 6674 6572 4c6f 6164 2870 7265 7669   afterLoad(previ
-00002310: 6f75 736c 794c 6f61 6465 6444 6174 6129  ouslyLoadedData)
-00002320: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
-00002330: 2020 2020 2072 6574 7572 6e20 6c6f 6164       return load
-00002340: 4675 6e63 7469 6f6e 286f 2e69 642c 2069  Function(o.id, i
-00002350: 6e73 7461 6e63 652e 6e61 6d65 2c20 7573  nstance.name, us
-00002360: 6544 6566 6175 6c74 4461 7461 466f 7243  eDefaultDataForC
-00002370: 6869 6c64 7265 6e29 2e74 6865 6e28 6675  hildren).then(fu
-00002380: 6e63 7469 6f6e 2028 6461 7461 2920 7b0a  nction (data) {.
-00002390: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000023a0: 726e 2061 6674 6572 4c6f 6164 2864 6174  rn afterLoad(dat
-000023b0: 6129 3b0a 2020 2020 2020 2020 7d29 3b0a  a);.        });.
-000023c0: 2020 2020 7d0a 0a20 2020 2067 6574 4d61      }..    getMa
-000023d0: 696e 4874 6d6c 456c 656d 656e 7428 6f2c  inHtmlElement(o,
-000023e0: 2064 6174 612c 2076 6973 6962 6c65 2c20   data, visible, 
-000023f0: 7769 6467 6574 4874 6d6c 732c 2077 6974  widgetHtmls, wit
-00002400: 6853 7461 7465 2920 7b0a 2020 2020 2020  hState) {.      
-00002410: 2020 6c65 7420 6773 203d 205b 5d2c 2068    let gs = [], h
-00002420: 746d 6c3b 0a0a 2020 2020 2020 2020 6966  tml;..        if
-00002430: 2028 6f2e 6170 706c 794d 6561 7375 7265   (o.applyMeasure
-00002440: 7354 6f53 6563 7469 6f6e 203d 3d3d 2074  sToSection === t
-00002450: 7275 6529 207b 0a20 2020 2020 2020 2020  rue) {.         
-00002460: 2020 2067 7320 3d20 7468 6973 2e67 6574     gs = this.get
-00002470: 5769 6474 6841 6e64 4865 6967 6874 2864  WidthAndHeight(d
-00002480: 6174 6129 3b0a 2020 2020 2020 2020 7d0a  ata);.        }.
-00002490: 0a20 2020 2020 2020 2069 6620 2876 6973  .        if (vis
-000024a0: 6962 6c65 203d 3d3d 2066 616c 7365 2920  ible === false) 
-000024b0: 7b0a 2020 2020 2020 2020 2020 2020 6773  {.            gs
-000024c0: 2e70 7573 6828 2764 6973 706c 6179 3a6e  .push('display:n
-000024d0: 6f6e 653b 2729 3b0a 2020 2020 2020 2020  one;');.        
-000024e0: 7d0a 0a20 2020 2020 2020 206c 6574 206f  }..        let o
-000024f0: 7269 6769 6e61 6c49 6420 3d20 6661 6c73  riginalId = fals
-00002500: 652c 2077 7269 7465 203d 2027 6f6e 273b  e, write = 'on';
-00002510: 0a20 2020 2020 2020 2069 6620 2864 6174  .        if (dat
-00002520: 6120 2626 2064 6174 612e 6f72 6967 696e  a && data.origin
-00002530: 616c 4964 2920 7b0a 2020 2020 2020 2020  alId) {.        
-00002540: 2020 2020 6f72 6967 696e 616c 4964 203d      originalId =
-00002550: 2064 6174 612e 6f72 6967 696e 616c 4964   data.originalId
-00002560: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
-00002570: 2020 2020 2069 6620 286f 2e77 7269 7465       if (o.write
-00002580: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00002590: 7772 6974 6520 3d20 6f2e 7772 6974 653b  write = o.write;
-000025a0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-000025b0: 2020 2020 6966 2028 6461 7461 2026 2620      if (data && 
-000025c0: 6461 7461 2e77 7269 7465 2920 7b0a 2020  data.write) {.  
-000025d0: 2020 2020 2020 2020 2020 7772 6974 6520            write 
-000025e0: 3d20 6461 7461 2e77 7269 7465 3b0a 2020  = data.write;.  
-000025f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002600: 6874 6d6c 203d 2074 6869 732e 6765 7448  html = this.getH
-00002610: 746d 6c28 7769 6467 6574 4874 6d6c 732c  tml(widgetHtmls,
-00002620: 2064 6174 612c 2077 6974 6853 7461 7465   data, withState
-00002630: 293b 0a0a 2020 2020 2020 2020 7265 7475  );..        retu
-00002640: 726e 2060 3c73 6563 7469 6f6e 2024 7b77  rn `<section ${w
-00002650: 7269 7465 203d 3d3d 2027 6f66 6627 203f  rite === 'off' ?
-00002660: 2060 6461 7461 2d77 7269 7465 3d22 6f66   `data-write="of
-00002670: 6622 6020 3a20 2727 7d20 247b 6f72 6967  f"` : ''} ${orig
-00002680: 696e 616c 4964 2021 3d3d 2066 616c 7365  inalId !== false
-00002690: 203f 2060 6461 7461 2d6f 7269 6769 6e61   ? `data-origina
-000026a0: 6c49 643d 2224 7b6f 2e6f 7269 6769 6e61  lId="${o.origina
-000026b0: 6c49 647d 2260 203a 2027 277d 2024 7b6f  lId}"` : ''} ${o
-000026c0: 2e6f 7264 696e 616c 203f 2060 6461 7461  .ordinal ? `data
-000026d0: 2d6f 7264 696e 616c 3d22 247b 6f2e 6f72  -ordinal="${o.or
-000026e0: 6469 6e61 6c7d 2260 203a 2027 277d 2024  dinal}"` : ''} $
-000026f0: 7b6f 2e6d 6172 6769 6e20 3f20 2763 6c61  {o.margin ? 'cla
-00002700: 7373 3d22 7772 6170 7065 7222 2720 3a20  ss="wrapper"' : 
-00002710: 2727 7d20 7374 796c 653d 2224 7b67 732e  ''} style="${gs.
-00002720: 6a6f 696e 2827 2729 7d22 2069 643d 2224  join('')}" id="$
-00002730: 7b6f 2e69 6420 3f20 6f2e 6964 203a 2055  {o.id ? o.id : U
-00002740: 7469 6c73 2e67 6574 5261 6e64 6f6d 4964  tils.getRandomId
-00002750: 2829 7d22 3e24 7b68 746d 6c7d 3c2f 7365  ()}">${html}</se
-00002760: 6374 696f 6e3e 603b 0a0a 2020 2020 7d0a  ction>`;..    }.
-00002770: 0a20 2020 2065 6d62 6564 6465 6452 656e  .    embeddedRen
-00002780: 6465 7228 7769 7468 5374 6174 652c 2064  der(withState, d
-00002790: 6174 612c 206c 6f61 6446 756e 6374 696f  ata, loadFunctio
-000027a0: 6e20 3d20 5142 2e6c 6f61 6444 6174 6129  n = QB.loadData)
-000027b0: 207b 0a20 2020 2020 2020 2074 6869 732e   {.        this.
-000027c0: 6973 5265 6e64 6572 696e 6720 3d20 7472  isRendering = tr
-000027d0: 7565 3b0a 2020 2020 2020 2020 636f 6e73  ue;.        cons
-000027e0: 7420 6f20 3d20 7b2e 2e2e 7468 6973 2e6f  t o = {...this.o
-000027f0: 7074 696f 6e73 2c20 2e2e 2e64 6174 617d  ptions, ...data}
-00002800: 2c20 696e 7374 616e 6365 203d 2074 6869  , instance = thi
-00002810: 732c 2068 203d 204c 6973 7465 6e65 7273  s, h = Listeners
-00002820: 2e68 616e 646c 653b 0a0a 2020 2020 2020  .handle;..      
-00002830: 2020 7468 6973 2e61 6464 4c69 7374 656e    this.addListen
-00002840: 6572 7328 6661 6c73 6529 3b0a 0a20 2020  ers(false);..   
-00002850: 2020 2020 2069 6620 286e 6577 206f 2e74       if (new o.t
-00002860: 7970 6528 6f29 2e61 6d49 4f6e 4147 7269  ype(o).amIOnAGri
-00002870: 6454 6162 6c65 2829 2920 7b0a 2020 2020  dTable()) {.    
-00002880: 2020 2020 2020 2020 4c69 7374 656e 6572          Listener
-00002890: 732e 7075 7368 287b 6f70 7469 6f6e 733a  s.push({options:
-000028a0: 206f 2c20 6d65 7468 6f64 3a20 2772 6566   o, method: 'ref
-000028b0: 7265 7368 4772 6964 4365 6c6c 272c 2065  reshGridCell', e
-000028c0: 7665 6e74 4e61 6d65 3a20 2766 6f72 6365  ventName: 'force
-000028d0: 7265 6672 6573 682e 2720 2b20 6f2e 6964  refresh.' + o.id
-000028e0: 2c20 6861 6e64 6c65 723a 2068 7d29 3b0a  , handler: h});.
-000028f0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00002900: 2020 206c 6574 2076 6973 6962 6c65 203d     let visible =
-00002910: 2064 6174 6120 2626 2074 7970 656f 6620   data && typeof 
-00002920: 6461 7461 2e76 6973 6962 6c65 2021 3d3d  data.visible !==
-00002930: 2027 756e 6465 6669 6e65 6427 203f 2064   'undefined' ? d
-00002940: 6174 612e 7669 7369 626c 6520 3a20 6f2e  ata.visible : o.
-00002950: 7669 7369 626c 653b 0a0a 2020 2020 2020  visible;..      
-00002960: 2020 7265 7475 726e 2069 6e73 7461 6e63    return instanc
-00002970: 652e 6765 744d 6169 6e48 746d 6c45 6c65  e.getMainHtmlEle
-00002980: 6d65 6e74 286f 2c20 6461 7461 2c20 7669  ment(o, data, vi
-00002990: 7369 626c 652c 205b 5d2c 2077 6974 6853  sible, [], withS
-000029a0: 7461 7465 290a 0a20 2020 207d 0a0a 2020  tate)..    }..  
-000029b0: 2020 6164 6444 6570 656e 6465 6e74 7328    addDependents(
-000029c0: 2920 7b0a 2020 2020 2020 2020 636f 6e73  ) {.        cons
-000029d0: 7420 6f20 3d20 7468 6973 2e6f 7074 696f  t o = this.optio
-000029e0: 6e73 2c20 6820 3d20 4c69 7374 656e 6572  ns, h = Listener
-000029f0: 732e 6861 6e64 6c65 3b0a 0a20 2020 2020  s.handle;..     
-00002a00: 2020 2069 6620 286f 2e64 6570 656e 6473     if (o.depends
-00002a10: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00002a20: 636f 6e73 7420 6620 3d20 6f2e 6964 2e73  const f = o.id.s
-00002a30: 706c 6974 2827 5f27 292c 2061 203d 2066  plit('_'), a = f
-00002a40: 5b30 5d2c 2062 203d 2066 5b31 5d3b 0a0a  [0], b = f[1];..
-00002a50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00002a60: 286c 6574 206c 206f 6620 6f2e 6465 7065  (let l of o.depe
-00002a70: 6e64 7329 207b 0a20 2020 2020 2020 2020  nds) {.         
-00002a80: 2020 2020 2020 204c 6973 7465 6e65 7273         Listeners
-00002a90: 2e70 7573 6828 7b0a 2020 2020 2020 2020  .push({.        
-00002aa0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00002ab0: 6f6e 733a 206f 2c0a 2020 2020 2020 2020  ons: o,.        
-00002ac0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00002ad0: 6f64 3a20 2772 6566 7265 7368 4772 6964  od: 'refreshGrid
-00002ae0: 4365 6c6c 272c 0a20 2020 2020 2020 2020  Cell',.         
-00002af0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
-00002b00: 4e61 6d65 3a20 6c2e 6576 656e 7420 3f20  Name: l.event ? 
-00002b10: 6c2e 6576 656e 7420 3a20 6c2e 6163 7469  l.event : l.acti
-00002b20: 6f6e 202b 2027 2e27 202b 2061 202b 2027  on + '.' + a + '
-00002b30: 5f27 202b 2062 202b 2027 5f27 202b 206c  _' + b + '_' + l
-00002b40: 2e63 6f6c 202b 2027 2e66 696e 6973 6865  .col + '.finishe
-00002b50: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-00002b60: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
-00002b70: 7273 3a20 6c2e 7061 7261 6d65 7465 7273  rs: l.parameters
-00002b80: 207c 7c20 5b5d 2c0a 2020 2020 2020 2020   || [],.        
-00002b90: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
-00002ba0: 6c65 723a 2068 0a20 2020 2020 2020 2020  ler: h.         
-00002bb0: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-00002bc0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002bd0: 207d 0a20 2020 207d 0a0a 2020 2020 6164   }.    }..    ad
-00002be0: 644c 6973 7465 6e65 7273 2872 6563 7572  dListeners(recur
-00002bf0: 7369 7665 203d 2074 7275 6529 207b 0a20  sive = true) {. 
-00002c00: 2020 2020 2020 2063 6f6e 7374 206f 203d         const o =
-00002c10: 2074 6869 732e 6f70 7469 6f6e 732c 2068   this.options, h
-00002c20: 203d 204c 6973 7465 6e65 7273 2e68 616e   = Listeners.han
-00002c30: 646c 653b 0a0a 2020 2020 2020 2020 6966  dle;..        if
-00002c40: 2028 6f2e 6c69 7374 656e 2920 7b0a 2020   (o.listen) {.  
-00002c50: 2020 2020 2020 2020 2020 666f 7220 286c            for (l
-00002c60: 6574 206c 206f 6620 6f2e 6c69 7374 656e  et l of o.listen
-00002c70: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00002c80: 2020 2020 4c69 7374 656e 6572 732e 7075      Listeners.pu
-00002c90: 7368 287b 0a20 2020 2020 2020 2020 2020  sh({.           
-00002ca0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00002cb0: 3a20 6f2c 0a20 2020 2020 2020 2020 2020  : o,.           
-00002cc0: 2020 2020 2020 2020 206d 6574 686f 643a           method:
-00002cd0: 206c 2e6d 6574 686f 642c 0a20 2020 2020   l.method,.     
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002cf0: 7665 6e74 4e61 6d65 3a20 6c2e 6576 656e  ventName: l.even
-00002d00: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00002d10: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-00002d20: 733a 206c 2e70 6172 616d 6574 6572 7320  s: l.parameters 
-00002d30: 7c7c 205b 5d2c 0a20 2020 2020 2020 2020  || [],.         
-00002d40: 2020 2020 2020 2020 2020 2068 616e 646c             handl
-00002d50: 6572 3a20 680a 2020 2020 2020 2020 2020  er: h.          
-00002d60: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00002d70: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002d80: 7d0a 0a20 2020 2020 2020 2069 6620 286f  }..        if (o
-00002d90: 2e64 6570 656e 6473 2026 2620 7265 6375  .depends && recu
-00002da0: 7273 6976 6520 3d3d 3d20 6661 6c73 6529  rsive === false)
-00002db0: 207b 0a20 2020 2020 2020 2020 2020 2074   {.            t
-00002dc0: 6869 732e 6164 6444 6570 656e 6465 6e74  his.addDependent
-00002dd0: 7328 293b 0a20 2020 2020 2020 207d 0a0a  s();.        }..
-00002de0: 2020 2020 2020 2020 7468 6973 2e61 7070          this.app
-00002df0: 656e 644c 6973 7465 6e65 7273 286f 2c20  endListeners(o, 
-00002e00: 6829 3b0a 0a20 2020 2020 2020 2069 6620  h);..        if 
-00002e10: 2872 6563 7572 7369 7665 2920 7b0a 2020  (recursive) {.  
-00002e20: 2020 2020 2020 2020 2020 6c65 7420 7769            let wi
-00002e30: 6467 6574 4f70 7469 6f6e 732c 2077 6964  dgetOptions, wid
-00002e40: 6765 7473 203d 205b 5d2c 2077 2c20 7777  gets = [], w, ww
-00002e50: 3b0a 0a20 2020 2020 2020 2020 2020 2066  ;..            f
-00002e60: 6f72 2028 7769 6467 6574 4f70 7469 6f6e  or (widgetOption
-00002e70: 7320 6f66 206f 2e77 6964 6765 7473 207c  s of o.widgets |
-00002e80: 7c20 5b5d 2920 7b0a 2020 2020 2020 2020  | []) {.        
-00002e90: 2020 2020 2020 2020 7777 203d 2074 6869          ww = thi
-00002ea0: 732e 6765 7457 6964 6765 7428 7769 6467  s.getWidget(widg
-00002eb0: 6574 4f70 7469 6f6e 7329 3b0a 2020 2020  etOptions);.    
-00002ec0: 2020 2020 2020 2020 2020 2020 7769 6467              widg
-00002ed0: 6574 732e 7075 7368 2877 7729 3b0a 2020  ets.push(ww);.  
-00002ee0: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
-00002ef0: 2020 2020 2020 2020 2069 6620 286f 2e74           if (o.t
-00002f00: 7970 652e 6e61 6d65 203d 3d3d 2027 4772  ype.name === 'Gr
-00002f10: 6964 5461 626c 6557 6964 6765 7427 2920  idTableWidget') 
-00002f20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002f30: 2020 7468 6973 2e61 6464 4772 6964 5461    this.addGridTa
-00002f40: 626c 654c 6973 7465 6e65 7273 2829 3b0a  bleListeners();.
-00002f50: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
-00002f60: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
-00002f70: 2020 2020 2066 6f72 2028 7720 6f66 2077       for (w of w
-00002f80: 6964 6765 7473 2920 7b0a 2020 2020 2020  idgets) {.      
-00002f90: 2020 2020 2020 2020 2020 2020 2020 772e                w.
-00002fa0: 6164 644c 6973 7465 6e65 7273 2829 3b0a  addListeners();.
-00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fc0: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-00002fd0: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00002fe0: 0a20 2020 2061 7070 656e 644c 6973 7465  .    appendListe
-00002ff0: 6e65 7273 286f 7074 696f 6e73 2c20 6861  ners(options, ha
-00003000: 6e64 6c65 7229 207b 0a0a 2020 2020 7d0a  ndler) {..    }.
-00003010: 0a20 2020 2069 6e69 7446 696e 6973 6865  .    initFinishe
-00003020: 6428 2920 7b0a 2020 2020 2020 2020 7468  d() {.        th
-00003030: 6973 2e74 7269 6767 6572 4669 6e69 7368  is.triggerFinish
-00003040: 6564 4576 656e 7428 293b 0a20 2020 207d  edEvent();.    }
-00003050: 0a0a 2020 2020 7570 6461 7465 436f 6e74  ..    updateCont
-00003060: 656e 7446 696e 6973 6865 6428 2920 7b0a  entFinished() {.
-00003070: 2020 2020 2020 2020 7468 6973 2e74 7269          this.tri
-00003080: 6767 6572 4669 6e69 7368 6564 4576 656e  ggerFinishedEven
-00003090: 7428 2775 7064 6174 6543 6f6e 7465 6e74  t('updateContent
-000030a0: 2729 3b0a 2020 2020 7d0a 0a20 2020 2072  ');.    }..    r
-000030b0: 6566 7265 7368 4669 6e69 7368 6564 2829  efreshFinished()
-000030c0: 207b 0a20 2020 2020 2020 2074 6869 732e   {.        this.
-000030d0: 7472 6967 6765 7246 696e 6973 6865 6445  triggerFinishedE
-000030e0: 7665 6e74 2827 7265 6672 6573 6827 293b  vent('refresh');
-000030f0: 0a20 2020 207d 0a0a 2020 2020 7472 6967  .    }..    trig
-00003100: 6765 7246 696e 6973 6865 6445 7665 6e74  gerFinishedEvent
-00003110: 2865 7665 6e74 5479 7065 203d 2027 696e  (eventType = 'in
-00003120: 6974 2729 207b 0a20 2020 2020 2020 2063  it') {.        c
-00003130: 6f6e 7374 206f 203d 2074 6869 732e 6f70  onst o = this.op
-00003140: 7469 6f6e 733b 0a0a 2020 2020 2020 2020  tions;..        
-00003150: 6c65 7420 7769 6467 6574 4f70 7469 6f6e  let widgetOption
-00003160: 732c 2077 6964 6765 7473 203d 205b 5d2c  s, widgets = [],
-00003170: 2077 2c20 7777 3b0a 0a20 2020 2020 2020   w, ww;..       
-00003180: 2066 6f72 2028 7769 6467 6574 4f70 7469   for (widgetOpti
-00003190: 6f6e 7320 6f66 206f 2e77 6964 6765 7473  ons of o.widgets
-000031a0: 207c 7c20 5b5d 2920 7b0a 2020 2020 2020   || []) {.      
-000031b0: 2020 2020 2020 7777 203d 2074 6869 732e        ww = this.
-000031c0: 6765 7457 6964 6765 7428 7769 6467 6574  getWidget(widget
-000031d0: 4f70 7469 6f6e 7329 3b0a 2020 2020 2020  Options);.      
-000031e0: 2020 2020 2020 7769 6467 6574 732e 7075        widgets.pu
-000031f0: 7368 2877 7729 3b0a 2020 2020 2020 2020  sh(ww);.        
-00003200: 7d0a 0a20 2020 2020 2020 2066 6f72 2028  }..        for (
-00003210: 7720 6f66 2077 6964 6765 7473 2920 7b0a  w of widgets) {.
-00003220: 2020 2020 2020 2020 2020 2020 772e 7472              w.tr
-00003230: 6967 6765 7246 696e 6973 6865 6445 7665  iggerFinishedEve
-00003240: 6e74 2865 7665 6e74 5479 7065 293b 0a20  nt(eventType);. 
-00003250: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00003260: 2020 456c 2e62 6f64 792e 7472 6967 6765    El.body.trigge
-00003270: 7248 616e 646c 6572 2865 7665 6e74 5479  rHandler(eventTy
-00003280: 7065 202b 2027 2e27 202b 206f 2e69 6420  pe + '.' + o.id 
-00003290: 2b20 272e 6669 6e69 7368 6564 2729 3b0a  + '.finished');.
-000032a0: 0a20 2020 2020 2020 206c 6574 2061 6374  .        let act
-000032b0: 696f 6e73 203d 2045 7665 6e74 4d61 705b  ions = EventMap[
-000032c0: 6576 656e 7454 7970 6520 2b20 272e 2720  eventType + '.' 
-000032d0: 2b20 6f2e 6964 202b 2027 2e66 696e 6973  + o.id + '.finis
-000032e0: 6865 6427 5d2c 2061 3b0a 2020 2020 2020  hed'], a;.      
-000032f0: 2020 6966 2028 6163 7469 6f6e 7329 207b    if (actions) {
-00003300: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00003310: 2028 6120 6f66 2061 6374 696f 6e73 2920   (a of actions) 
-00003320: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003330: 2020 612e 6163 7469 6f6e 2861 2e61 7267    a.action(a.arg
-00003340: 756d 656e 742c 207b 7d2c 207b 7d29 3b0a  ument, {}, {});.
-00003350: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003360: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003370: 6966 2028 5265 706f 7369 746f 7279 5b6f  if (Repository[o
-00003380: 2e69 645d 2026 2620 5265 706f 7369 746f  .id] && Reposito
-00003390: 7279 5b6f 2e69 645d 5b65 7665 6e74 5479  ry[o.id][eventTy
-000033a0: 7065 202b 2027 4669 6e69 7368 6564 275d  pe + 'Finished']
-000033b0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-000033c0: 5265 706f 7369 746f 7279 5b6f 2e69 645d  Repository[o.id]
-000033d0: 5b65 7665 6e74 5479 7065 202b 2027 4669  [eventType + 'Fi
-000033e0: 6e69 7368 6564 275d 2829 3b0a 2020 2020  nished']();.    
-000033f0: 2020 2020 7d0a 2020 2020 7d0a 0a20 2020      }.    }..   
-00003400: 2069 6e69 7445 7665 6e74 7328 7769 7468   initEvents(with
-00003410: 5374 6174 6529 207b 0a20 2020 2020 2020  State) {.       
-00003420: 2063 6f6e 7374 206f 203d 2074 6869 732e   const o = this.
-00003430: 6f70 7469 6f6e 732c 2073 6563 7469 6f6e  options, section
-00003440: 203d 2024 2827 2327 202b 206f 2e69 6429   = $('#' + o.id)
-00003450: 3b0a 0a20 2020 2020 2020 206c 6574 2077  ;..        let w
-00003460: 6964 6765 744f 7074 696f 6e73 2c20 7769  idgetOptions, wi
-00003470: 6467 6574 7320 3d20 5b5d 2c20 772c 2077  dgets = [], w, w
-00003480: 773b 0a0a 2020 2020 2020 2020 666f 7220  w;..        for 
-00003490: 2877 6964 6765 744f 7074 696f 6e73 206f  (widgetOptions o
-000034a0: 6620 6f2e 7769 6467 6574 7320 7c7c 205b  f o.widgets || [
-000034b0: 5d29 207b 0a20 2020 2020 2020 2020 2020  ]) {.           
-000034c0: 2077 7720 3d20 7468 6973 2e67 6574 5769   ww = this.getWi
-000034d0: 6467 6574 2877 6964 6765 744f 7074 696f  dget(widgetOptio
-000034e0: 6e73 293b 0a20 2020 2020 2020 2020 2020  ns);.           
-000034f0: 2077 6964 6765 7473 2e70 7573 6828 7777   widgets.push(ww
-00003500: 293b 0a20 2020 2020 2020 207d 0a0a 2020  );.        }..  
-00003510: 2020 2020 2020 666f 7220 2877 206f 6620        for (w of 
-00003520: 7769 6467 6574 7329 207b 0a20 2020 2020  widgets) {.     
-00003530: 2020 2020 2020 2077 2e69 6e69 7445 7665         w.initEve
-00003540: 6e74 7328 7769 7468 5374 6174 6529 3b0a  nts(withState);.
-00003550: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00003560: 2020 2074 6869 732e 696e 6974 4576 656e     this.initEven
-00003570: 7448 616e 646c 6572 7328 7769 7468 5374  tHandlers(withSt
-00003580: 6174 6529 3b0a 0a20 2020 2020 2020 2074  ate);..        t
-00003590: 6869 732e 6973 5265 6e64 6572 696e 6720  his.isRendering 
-000035a0: 3d20 6661 6c73 653b 0a20 2020 207d 0a0a  = false;.    }..
-000035b0: 2020 2020 696e 6974 4576 656e 7448 616e      initEventHan
-000035c0: 646c 6572 7328 2920 7b0a 0a20 2020 207d  dlers() {..    }
-000035d0: 0a0a 2020 2020 7072 6f63 6573 7344 6174  ..    processDat
-000035e0: 6128 6461 7461 2920 7b0a 2020 2020 2020  a(data) {.      
-000035f0: 2020 7265 7475 726e 2064 6174 613b 0a20    return data;. 
-00003600: 2020 207d 0a0a 2020 2020 616d 494f 6e41     }..    amIOnA
-00003610: 4772 6964 5461 626c 6528 2920 7b0a 2020  GridTable() {.  
-00003620: 2020 2020 2020 636f 6e73 7420 6f20 3d20        const o = 
-00003630: 7468 6973 2e6f 7074 696f 6e73 3b0a 2020  this.options;.  
-00003640: 2020 2020 2020 7265 7475 726e 2028 6f2e        return (o.
-00003650: 6964 2e73 706c 6974 2827 5f27 292e 6c65  id.split('_').le
-00003660: 6e67 7468 202d 2031 2920 3d3d 3d20 323b  ngth - 1) === 2;
-00003670: 0a20 2020 207d 0a0a 2020 2020 6765 7453  .    }..    getS
-00003680: 6563 7469 6f6e 2829 207b 0a20 2020 2020  ection() {.     
-00003690: 2020 2072 6574 7572 6e20 2428 2723 2720     return $('#' 
-000036a0: 2b20 7468 6973 2e69 6429 3b0a 2020 2020  + this.id);.    
-000036b0: 7d0a 0a20 2020 2073 7461 7469 6320 6861  }..    static ha
-000036c0: 6e64 6c65 5379 7374 656d 4576 656e 7428  ndleSystemEvent(
-000036d0: 656c 656d 656e 742c 2074 7269 6767 6572  element, trigger
-000036e0: 4576 656e 744e 616d 652c 2066 696c 7465  EventName, filte
-000036f0: 7253 656c 6563 746f 722c 2075 7064 6174  rSelector, updat
-00003700: 6556 616c 7565 203d 2074 7275 652c 2061  eValue = true, a
-00003710: 6c6c 6f77 4275 6262 6c69 6e67 5570 203d  llowBubblingUp =
-00003720: 2066 616c 7365 2920 7b0a 2020 2020 2020   false) {.      
-00003730: 2020 656c 656d 656e 742e 6f6e 2874 7269    element.on(tri
-00003740: 6767 6572 4576 656e 744e 616d 652c 2066  ggerEventName, f
-00003750: 696c 7465 7253 656c 6563 746f 722c 2065  ilterSelector, e
-00003760: 7665 6e74 203d 3e20 7b0a 2020 2020 2020  vent => {.      
-00003770: 2020 2020 2020 5769 6467 6574 2e64 6f48        Widget.doH
-00003780: 616e 646c 6553 7973 7465 6d45 7665 6e74  andleSystemEvent
-00003790: 2824 2865 7665 6e74 2e63 7572 7265 6e74  ($(event.current
-000037a0: 5461 7267 6574 292c 2065 7665 6e74 2c20  Target), event, 
-000037b0: 7570 6461 7465 5661 6c75 6529 3b0a 0a20  updateValue);.. 
-000037c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000037d0: 6e20 616c 6c6f 7742 7562 626c 696e 6755  n allowBubblingU
-000037e0: 703b 0a20 2020 2020 2020 207d 293b 0a20  p;.        });. 
-000037f0: 2020 207d 0a0a 2020 2020 7374 6174 6963     }..    static
-00003800: 2064 6f48 616e 646c 6553 7973 7465 6d45   doHandleSystemE
-00003810: 7665 6e74 2865 6c65 6d65 6e74 2c20 6576  vent(element, ev
-00003820: 656e 742c 2075 7064 6174 6556 616c 7565  ent, updateValue
-00003830: 203d 2074 7275 6529 207b 0a20 2020 2020   = true) {.     
-00003840: 2020 206c 6574 2061 203d 2065 6c65 6d65     let a = eleme
-00003850: 6e74 2e64 6174 6128 2761 6374 696f 6e27  nt.data('action'
-00003860: 292c 2069 203d 2065 6c65 6d65 6e74 2e64  ), i = element.d
-00003870: 6174 6128 2769 6427 292c 2073 6563 7469  ata('id'), secti
-00003880: 6f6e 203d 2065 6c65 6d65 6e74 2e63 6c6f  on = element.clo
-00003890: 7365 7374 2827 7365 6374 696f 6e27 293b  sest('section');
-000038a0: 0a0a 2020 2020 2020 2020 636f 6e73 7420  ..        const 
-000038b0: 6576 656e 744d 6170 4964 203d 2061 202b  eventMapId = a +
-000038c0: 2027 2e27 202b 2069 3b0a 0a20 2020 2020   '.' + i;..     
-000038d0: 2020 2069 6620 2827 7269 6768 7463 6c69     if ('rightcli
-000038e0: 636b 2720 3d3d 3d20 6129 207b 0a20 2020  ck' === a) {.   
-000038f0: 2020 2020 2020 2020 2057 6964 6765 7473           Widgets
-00003900: 5b27 7269 6768 7463 6c69 636b 275d 203d  ['rightclick'] =
-00003910: 2069 3b0a 2020 2020 2020 2020 7d0a 0a20   i;.        }.. 
-00003920: 2020 2020 2020 2045 6c2e 626f 6479 2e74         El.body.t
-00003930: 7269 6767 6572 4861 6e64 6c65 7228 6576  riggerHandler(ev
-00003940: 656e 744d 6170 4964 202b 2027 2e73 7461  entMapId + '.sta
-00003950: 7274 6564 2729 3b0a 0a20 2020 2020 2020  rted');..       
-00003960: 2069 6620 2857 6964 6765 7473 5b69 5d20   if (Widgets[i] 
-00003970: 2626 2075 7064 6174 6556 616c 7565 2920  && updateValue) 
-00003980: 7b0a 2020 2020 2020 2020 2020 2020 5769  {.            Wi
-00003990: 6467 6574 735b 695d 5b61 5d20 3d20 656c  dgets[i][a] = el
-000039a0: 656d 656e 742e 6461 7461 2829 3b0a 2020  ement.data();.  
-000039b0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-000039c0: 2063 6f6e 7374 2077 7269 7465 203d 2073   const write = s
-000039d0: 6563 7469 6f6e 2e64 6174 6128 2777 7269  ection.data('wri
-000039e0: 7465 2729 2021 3d3d 2027 6f66 6627 3b0a  te') !== 'off';.
-000039f0: 0a20 2020 2020 2020 2057 6964 6765 742e  .        Widget.
-00003a00: 6578 6563 7574 6545 7665 6e74 4d61 7041  executeEventMapA
-00003a10: 6374 696f 6e73 2865 7665 6e74 4d61 7049  ctions(eventMapI
-00003a20: 642c 2065 7665 6e74 2c20 656c 656d 656e  d, event, elemen
-00003a30: 742c 2077 7269 7465 293b 0a20 2020 207d  t, write);.    }
-00003a40: 0a0a 2020 2020 7374 6174 6963 2064 6f48  ..    static doH
-00003a50: 616e 646c 6547 7269 6454 6162 6c65 5379  andleGridTableSy
-00003a60: 7374 656d 4576 656e 7428 656c 656d 656e  stemEvent(elemen
-00003a70: 742c 2065 7665 6e74 2c20 7570 6461 7465  t, event, update
-00003a80: 5661 6c75 6520 3d20 7472 7565 2920 7b0a  Value = true) {.
-00003a90: 2020 2020 2020 2020 6c65 7420 6120 3d20          let a = 
-00003aa0: 656c 656d 656e 742e 6461 7461 2827 6163  element.data('ac
-00003ab0: 7469 6f6e 2729 2c20 6920 3d20 656c 656d  tion'), i = elem
-00003ac0: 656e 742e 6461 7461 2827 6964 2729 2c20  ent.data('id'), 
-00003ad0: 6964 5061 7274 7320 3d20 692e 7370 6c69  idParts = i.spli
-00003ae0: 7428 275f 2729 2c0a 2020 2020 2020 2020  t('_'),.        
-00003af0: 2020 2020 7365 6374 696f 6e20 3d20 656c      section = el
-00003b00: 656d 656e 742e 636c 6f73 6573 7428 2773  ement.closest('s
-00003b10: 6563 7469 6f6e 2729 3b0a 0a20 2020 2020  ection');..     
-00003b20: 2020 2063 6f6e 7374 2065 7665 6e74 4d61     const eventMa
-00003b30: 7049 6420 3d20 6120 2b20 272e 2720 2b20  pId = a + '.' + 
-00003b40: 6964 5061 7274 735b 305d 202b 2027 5f72  idParts[0] + '_r
-00003b50: 6f77 5f27 202b 2069 6450 6172 7473 5b32  ow_' + idParts[2
-00003b60: 5d2c 0a20 2020 2020 2020 2020 2020 2063  ],.            c
-00003b70: 6f6c 756d 6e45 7665 6e74 4d61 7049 6420  olumnEventMapId 
-00003b80: 3d20 6120 2b20 272e 2720 2b20 6964 5061  = a + '.' + idPa
-00003b90: 7274 735b 305d 202b 2027 5f27 202b 2069  rts[0] + '_' + i
-00003ba0: 6450 6172 7473 5b31 5d20 2b20 275f 2720  dParts[1] + '_' 
-00003bb0: 2b20 6964 5061 7274 735b 325d 202b 2027  + idParts[2] + '
-00003bc0: 5f27 202b 2073 6563 7469 6f6e 2e64 6174  _' + section.dat
-00003bd0: 6128 276f 7269 6769 6e61 6c69 6427 293b  a('originalid');
-00003be0: 0a0a 2020 2020 2020 2020 456c 2e62 6f64  ..        El.bod
-00003bf0: 792e 7472 6967 6765 7248 616e 646c 6572  y.triggerHandler
-00003c00: 2865 7665 6e74 4d61 7049 6420 2b20 272e  (eventMapId + '.
-00003c10: 7374 6172 7465 6427 293b 0a20 2020 2020  started');.     
-00003c20: 2020 2045 6c2e 626f 6479 2e74 7269 6767     El.body.trigg
-00003c30: 6572 4861 6e64 6c65 7228 636f 6c75 6d6e  erHandler(column
-00003c40: 4576 656e 744d 6170 4964 202b 2027 2e73  EventMapId + '.s
-00003c50: 7461 7274 6564 2729 3b0a 0a20 2020 2020  tarted');..     
-00003c60: 2020 2069 6620 2857 6964 6765 7473 5b69     if (Widgets[i
-00003c70: 5d20 2626 2075 7064 6174 6556 616c 7565  ] && updateValue
-00003c80: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00003c90: 5769 6467 6574 735b 695d 5b61 5d20 3d20  Widgets[i][a] = 
-00003ca0: 656c 656d 656e 742e 6461 7461 2829 3b0a  element.data();.
-00003cb0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00003cc0: 2020 2063 6f6e 7374 2077 7269 7465 203d     const write =
-00003cd0: 2073 6563 7469 6f6e 2e64 6174 6128 2777   section.data('w
-00003ce0: 7269 7465 2729 2021 3d3d 2027 6f66 6627  rite') !== 'off'
-00003cf0: 3b0a 0a20 2020 2020 2020 2057 6964 6765  ;..        Widge
-00003d00: 742e 6578 6563 7574 6545 7665 6e74 4d61  t.executeEventMa
-00003d10: 7041 6374 696f 6e73 2861 202b 2027 2e27  pActions(a + '.'
-00003d20: 202b 2069 6450 6172 7473 5b30 5d2c 2065   + idParts[0], e
-00003d30: 7665 6e74 2c20 656c 656d 656e 742c 2066  vent, element, f
-00003d40: 616c 7365 293b 0a20 2020 2020 2020 2057  alse);.        W
-00003d50: 6964 6765 742e 6578 6563 7574 6545 7665  idget.executeEve
-00003d60: 6e74 4d61 7041 6374 696f 6e73 2865 7665  ntMapActions(eve
-00003d70: 6e74 4d61 7049 642c 2065 7665 6e74 2c20  ntMapId, event, 
-00003d80: 656c 656d 656e 742c 2077 7269 7465 293b  element, write);
-00003d90: 0a20 2020 2020 2020 2057 6964 6765 742e  .        Widget.
-00003da0: 6578 6563 7574 6545 7665 6e74 4d61 7041  executeEventMapA
-00003db0: 6374 696f 6e73 2863 6f6c 756d 6e45 7665  ctions(columnEve
-00003dc0: 6e74 4d61 7049 642c 2065 7665 6e74 2c20  ntMapId, event, 
-00003dd0: 656c 656d 656e 742c 2077 7269 7465 293b  element, write);
-00003de0: 0a20 2020 207d 0a0a 2020 2020 7374 6174  .    }..    stat
-00003df0: 6963 2065 7865 6375 7465 4576 656e 744d  ic executeEventM
-00003e00: 6170 4163 7469 6f6e 7328 6576 656e 744d  apActions(eventM
-00003e10: 6170 4964 2c20 6576 656e 742c 2065 6c65  apId, event, ele
-00003e20: 6d65 6e74 2c20 7772 6974 6520 3d20 7472  ment, write = tr
-00003e30: 7565 2c20 2e2e 2e61 7267 7329 207b 0a20  ue, ...args) {. 
-00003e40: 2020 2020 2020 204c 2865 7665 6e74 4d61         L(eventMa
-00003e50: 7049 642c 2065 7665 6e74 2c20 656c 656d  pId, event, elem
-00003e60: 656e 742c 2061 7267 7329 3b0a 0a20 2020  ent, args);..   
-00003e70: 2020 2020 206c 6574 2061 6374 696f 6e73       let actions
-00003e80: 203d 2045 7665 6e74 4d61 705b 6576 656e   = EventMap[even
-00003e90: 744d 6170 4964 5d2c 2061 2c20 7772 6974  tMapId], a, writ
-00003ea0: 6552 6573 706f 6e73 6520 3d20 7472 7565  eResponse = true
-00003eb0: 3b0a 0a20 2020 2020 2020 2069 6620 2877  ;..        if (w
-00003ec0: 7269 7465 203d 3d3d 2074 7275 6529 207b  rite === true) {
-00003ed0: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00003ee0: 7465 5265 7370 6f6e 7365 203d 2051 422e  teResponse = QB.
-00003ef0: 7772 6974 6544 6174 6128 6576 656e 744d  writeData(eventM
-00003f00: 6170 4964 2c20 6576 656e 742c 2065 6c65  apId, event, ele
-00003f10: 6d65 6e74 293b 0a20 2020 2020 2020 207d  ment);.        }
-00003f20: 0a0a 2020 2020 2020 2020 6966 2028 6163  ..        if (ac
-00003f30: 7469 6f6e 7320 2626 2077 7269 7465 5265  tions && writeRe
-00003f40: 7370 6f6e 7365 2021 3d3d 2066 616c 7365  sponse !== false
-00003f50: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00003f60: 666f 7220 2861 206f 6620 6163 7469 6f6e  for (a of action
-00003f70: 7329 207b 0a20 2020 2020 2020 2020 2020  s) {.           
-00003f80: 2020 2020 2061 2e61 6374 696f 6e28 612e       a.action(a.
-00003f90: 6172 6775 6d65 6e74 2c20 6576 656e 742c  argument, event,
-00003fa0: 2065 6c65 6d65 6e74 293b 0a20 2020 2020   element);.     
-00003fb0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00003fc0: 207d 0a20 2020 207d 0a0a 2020 2020 6765   }.    }..    ge
-00003fd0: 7420 6964 2829 207b 0a20 2020 2020 2020  t id() {.       
-00003fe0: 2072 6574 7572 6e20 7468 6973 2e6f 7074   return this.opt
-00003ff0: 696f 6e73 2e69 643b 0a20 2020 207d 0a0a  ions.id;.    }..
-00004000: 2020 2020 6765 7420 7374 6174 6528 2920      get state() 
-00004010: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
-00004020: 2057 6964 6765 7453 7461 7465 5b74 6869   WidgetState[thi
-00004030: 732e 6964 5d20 7c7c 207b 7d3b 0a20 2020  s.id] || {};.   
-00004040: 207d 0a0a 2020 2020 7365 7420 7374 6174   }..    set stat
-00004050: 6528 7374 6174 654f 626a 6563 7429 207b  e(stateObject) {
-00004060: 0a20 2020 2020 2020 2057 6964 6765 7453  .        WidgetS
-00004070: 7461 7465 5b74 6869 732e 6964 5d20 3d20  tate[this.id] = 
-00004080: 7374 6174 654f 626a 6563 743b 0a20 2020  stateObject;.   
-00004090: 207d 0a0a 2020 2020 6765 7420 6e61 6d65   }..    get name
-000040a0: 2829 207b 0a20 2020 2020 2020 2072 6574  () {.        ret
-000040b0: 7572 6e20 7468 6973 2e63 6f6e 7374 7275  urn this.constru
-000040c0: 6374 6f72 2e6e 616d 653b 0a20 2020 207d  ctor.name;.    }
-000040d0: 0a0a 2020 2020 7365 7420 6e61 6d65 286e  ..    set name(n
-000040e0: 2920 7b0a 2020 2020 2020 2020 7468 726f  ) {.        thro
-000040f0: 7720 6e65 7720 4572 726f 7228 2744 6f6e  w new Error('Don
-00004100: 5c27 7420 6368 616e 6765 2074 6865 2022  \'t change the "
-00004110: 6e61 6d65 2220 7072 6f70 6572 7479 206f  name" property o
-00004120: 6e20 7468 6973 206f 626a 6563 7421 2729  n this object!')
-00004130: 3b0a 2020 2020 7d0a 0a20 2020 2067 6574  ;.    }..    get
-00004140: 5265 616c 5661 6c75 6528 6b65 792c 2064  RealValue(key, d
-00004150: 6174 6120 3d20 7b7d 2c20 6465 6661 756c  ata = {}, defaul
-00004160: 7456 616c 203d 2027 272c 2064 6174 6150  tVal = '', dataP
-00004170: 7265 6669 7820 3d20 2727 2920 7b0a 0a20  refix = '') {.. 
-00004180: 2020 2020 2020 2069 6620 2827 756e 6465         if ('unde
-00004190: 6669 6e65 6427 2021 3d3d 2074 7970 656f  fined' !== typeo
-000041a0: 6620 6461 7461 5b64 6174 6150 7265 6669  f data[dataPrefi
-000041b0: 7820 2b20 6b65 795d 2920 7b0a 2020 2020  x + key]) {.    
-000041c0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-000041d0: 6174 615b 6461 7461 5072 6566 6978 202b  ata[dataPrefix +
-000041e0: 206b 6579 5d3b 0a20 2020 2020 2020 207d   key];.        }
-000041f0: 0a0a 2020 2020 2020 2020 6966 2028 2775  ..        if ('u
-00004200: 6e64 6566 696e 6564 2720 213d 3d20 7479  ndefined' !== ty
-00004210: 7065 6f66 2074 6869 732e 6f70 7469 6f6e  peof this.option
-00004220: 735b 6b65 795d 2920 7b0a 2020 2020 2020  s[key]) {.      
-00004230: 2020 2020 2020 7265 7475 726e 2074 6869        return thi
-00004240: 732e 6f70 7469 6f6e 735b 6b65 795d 3b0a  s.options[key];.
-00004250: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00004260: 2020 2072 6574 7572 6e20 6465 6661 756c     return defaul
-00004270: 7456 616c 3b0a 2020 2020 7d0a 0a20 2020  tVal;.    }..   
-00004280: 2067 6574 4874 6d6c 436f 6d70 6f6e 656e   getHtmlComponen
-00004290: 7453 7479 6c65 7341 7272 6179 286b 6579  tStylesArray(key
-000042a0: 2c20 6461 7461 203d 207b 7d29 207b 0a20  , data = {}) {. 
-000042b0: 2020 2020 2020 206c 6574 2073 7479 6c65         let style
-000042c0: 734f 626a 203d 2074 6869 732e 6765 7448  sObj = this.getH
-000042d0: 746d 6c43 6f6d 706f 6e65 6e74 5374 796c  tmlComponentStyl
-000042e0: 6573 286b 6579 2c20 6461 7461 292c 2073  es(key, data), s
-000042f0: 7479 6c65 7320 3d20 5b5d 3b0a 2020 2020  tyles = [];.    
-00004300: 2020 2020 666f 7220 2863 6f6e 7374 205b      for (const [
-00004310: 6b65 792c 2076 616c 7565 5d20 6f66 204f  key, value] of O
-00004320: 626a 6563 742e 656e 7472 6965 7328 7374  bject.entries(st
-00004330: 796c 6573 4f62 6a29 2920 7b0a 2020 2020  ylesObj)) {.    
-00004340: 2020 2020 2020 2020 7374 796c 6573 2e70          styles.p
-00004350: 7573 6828 6024 7b6b 6579 2e72 6570 6c61  ush(`${key.repla
-00004360: 6365 416c 6c28 275f 272c 2027 2d27 297d  ceAll('_', '-')}
-00004370: 3a24 7b76 616c 7565 7d3b 6029 3b0a 2020  :${value};`);.  
-00004380: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004390: 7265 7475 726e 2073 7479 6c65 733b 0a20  return styles;. 
-000043a0: 2020 207d 0a0a 2020 2020 6765 7448 746d     }..    getHtm
-000043b0: 6c43 6f6d 706f 6e65 6e74 5374 796c 6573  lComponentStyles
-000043c0: 5374 7269 6e67 286b 6579 2c20 6461 7461  String(key, data
-000043d0: 203d 207b 7d29 207b 0a20 2020 2020 2020   = {}) {.       
-000043e0: 2072 6574 7572 6e20 7468 6973 2e67 6574   return this.get
-000043f0: 4874 6d6c 436f 6d70 6f6e 656e 7453 7479  HtmlComponentSty
-00004400: 6c65 7341 7272 6179 286b 6579 2c20 6461  lesArray(key, da
-00004410: 7461 292e 6a6f 696e 2827 2729 3b0a 2020  ta).join('');.  
-00004420: 2020 7d0a 0a20 2020 2067 6574 4874 6d6c    }..    getHtml
-00004430: 436f 6d70 6f6e 656e 7453 7479 6c65 7328  ComponentStyles(
-00004440: 6b65 792c 2064 6174 6120 3d20 7b7d 2920  key, data = {}) 
-00004450: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
-00004460: 2074 6869 732e 6765 7452 6561 6c56 616c   this.getRealVal
-00004470: 7565 286b 6579 202b 2027 5374 796c 6527  ue(key + 'Style'
-00004480: 2c20 6461 7461 2c20 7b7d 293b 0a20 2020  , data, {});.   
-00004490: 207d 0a0a 2020 2020 6765 7447 656e 6572   }..    getGener
-000044a0: 616c 5374 796c 6573 2864 6174 6120 3d20  alStyles(data = 
-000044b0: 7b7d 2c20 6465 6661 756c 7473 203d 207b  {}, defaults = {
-000044c0: 7d2c 2064 6174 6150 7265 6669 7820 3d20  }, dataPrefix = 
-000044d0: 2727 2920 7b0a 2020 2020 2020 2020 7265  '') {.        re
-000044e0: 7475 726e 205b 2e2e 2e74 6869 732e 6765  turn [...this.ge
-000044f0: 7457 6964 7468 416e 6448 6569 6768 7428  tWidthAndHeight(
-00004500: 6461 7461 2c20 6465 6661 756c 7473 2c20  data, defaults, 
-00004510: 6461 7461 5072 6566 6978 292c 202e 2e2e  dataPrefix), ...
-00004520: 7468 6973 2e67 6574 5061 6464 696e 6773  this.getPaddings
-00004530: 2864 6174 612c 2064 6566 6175 6c74 732c  (data, defaults,
-00004540: 2064 6174 6150 7265 6669 7829 2c20 2e2e   dataPrefix), ..
-00004550: 2e74 6869 732e 6765 744d 6172 6769 6e73  .this.getMargins
-00004560: 2864 6174 612c 2064 6566 6175 6c74 732c  (data, defaults,
-00004570: 2064 6174 6150 7265 6669 7829 5d3b 0a20   dataPrefix)];. 
-00004580: 2020 207d 0a0a 2020 2020 7570 6461 7465     }..    update
-00004590: 4874 6d6c 436f 6d70 6f6e 656e 7428 6b65  HtmlComponent(ke
-000045a0: 792c 2064 6174 612c 2065 6c65 6d65 6e74  y, data, element
-000045b0: 203d 206e 756c 6c2c 2073 6563 7469 6f6e   = null, section
-000045c0: 203d 206e 756c 6c29 207b 0a20 2020 2020   = null) {.     
-000045d0: 2020 2069 6620 2865 6c65 6d65 6e74 203d     if (element =
-000045e0: 3d3d 206e 756c 6c29 207b 0a20 2020 2020  == null) {.     
-000045f0: 2020 2020 2020 2065 6c65 6d65 6e74 203d         element =
-00004600: 2073 6563 7469 6f6e 2e66 696e 6428 272e   section.find('.
-00004610: 2720 2b20 7468 6973 2e67 6574 4373 7350  ' + this.getCssP
-00004620: 7265 6669 7828 2920 2b20 272d 2720 2b20  refix() + '-' + 
-00004630: 6b65 7929 3b0a 2020 2020 2020 2020 7d0a  key);.        }.
-00004640: 2020 2020 2020 2020 636f 6e73 7420 6b65          const ke
-00004650: 7953 7479 6c65 7320 3d20 7468 6973 2e67  yStyles = this.g
-00004660: 6574 4874 6d6c 436f 6d70 6f6e 656e 7453  etHtmlComponentS
-00004670: 7479 6c65 7341 7272 6179 286b 6579 2c20  tylesArray(key, 
-00004680: 6461 7461 293b 0a20 2020 2020 2020 2069  data);.        i
-00004690: 6620 286b 6579 5374 796c 6573 2e6c 656e  f (keyStyles.len
-000046a0: 6774 6820 3e20 3029 207b 0a20 2020 2020  gth > 0) {.     
-000046b0: 2020 2020 2020 2065 6c65 6d65 6e74 2e61         element.a
-000046c0: 7474 7228 2773 7479 6c65 272c 206b 6579  ttr('style', key
-000046d0: 5374 796c 6573 2e6a 6f69 6e28 2727 2929  Styles.join(''))
-000046e0: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
-000046f0: 7d0a 0a20 2020 2075 7064 6174 654d 6561  }..    updateMea
-00004700: 7375 7265 7328 6d61 696e 2c20 6765 6e65  sures(main, gene
-00004710: 7261 6c53 7479 6c65 7329 207b 0a20 2020  ralStyles) {.   
-00004720: 2020 2020 206c 6574 2073 7479 6c65 7320       let styles 
-00004730: 3d20 6d61 696e 2e61 7474 7228 2773 7479  = main.attr('sty
-00004740: 6c65 2729 3b0a 2020 2020 2020 2020 7374  le');.        st
-00004750: 796c 6573 202b 3d20 6765 6e65 7261 6c53  yles += generalS
-00004760: 7479 6c65 732e 6a6f 696e 2827 2729 3b0a  tyles.join('');.
-00004770: 2020 2020 2020 2020 6d61 696e 2e61 7474          main.att
-00004780: 7228 2773 7479 6c65 272c 2073 7479 6c65  r('style', style
-00004790: 7329 3b0a 2020 2020 7d0a 0a20 2020 2067  s);.    }..    g
-000047a0: 6574 4373 7350 7265 6669 7828 2920 7b0a  etCssPrefix() {.
-000047b0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-000047c0: 273b 0a20 2020 207d 0a0a 2020 2020 6765  ';.    }..    ge
-000047d0: 7457 6964 7468 416e 6448 6569 6768 7428  tWidthAndHeight(
-000047e0: 6461 7461 203d 207b 7d2c 2064 6566 6175  data = {}, defau
-000047f0: 6c74 7320 3d20 7b7d 2c20 6461 7461 5072  lts = {}, dataPr
-00004800: 6566 6978 203d 2027 2729 207b 0a20 2020  efix = '') {.   
-00004810: 2020 2020 2063 6f6e 7374 2073 203d 205b       const s = [
-00004820: 5d2c 0a20 2020 2020 2020 2020 2020 2068  ],.            h
-00004830: 6569 6768 7420 3d20 7468 6973 2e67 6574  eight = this.get
-00004840: 5265 616c 5661 6c75 6528 2768 6569 6768  RealValue('heigh
-00004850: 7427 2c20 6461 7461 2c20 6465 6661 756c  t', data, defaul
-00004860: 7473 2e68 6569 6768 742c 2064 6174 6150  ts.height, dataP
-00004870: 7265 6669 7829 2c0a 2020 2020 2020 2020  refix),.        
-00004880: 2020 2020 6d69 6e48 6569 6768 7420 3d20      minHeight = 
-00004890: 7468 6973 2e67 6574 5265 616c 5661 6c75  this.getRealValu
-000048a0: 6528 276d 696e 4865 6967 6874 272c 2064  e('minHeight', d
-000048b0: 6174 612c 2064 6566 6175 6c74 732e 6d69  ata, defaults.mi
-000048c0: 6e48 6569 6768 742c 2064 6174 6150 7265  nHeight, dataPre
-000048d0: 6669 7829 2c0a 2020 2020 2020 2020 2020  fix),.          
-000048e0: 2020 7769 6474 6820 3d20 7468 6973 2e67    width = this.g
-000048f0: 6574 5265 616c 5661 6c75 6528 2777 6964  etRealValue('wid
-00004900: 7468 272c 2064 6174 612c 2064 6566 6175  th', data, defau
-00004910: 6c74 732e 7769 6474 682c 2064 6174 6150  lts.width, dataP
-00004920: 7265 6669 7829 2c0a 2020 2020 2020 2020  refix),.        
-00004930: 2020 2020 6d69 6e57 6964 7468 203d 2074      minWidth = t
-00004940: 6869 732e 6765 7452 6561 6c56 616c 7565  his.getRealValue
-00004950: 2827 6d69 6e57 6964 7468 272c 2064 6174  ('minWidth', dat
-00004960: 612c 2064 6566 6175 6c74 732e 6d69 6e57  a, defaults.minW
-00004970: 6964 7468 2c20 6461 7461 5072 6566 6978  idth, dataPrefix
-00004980: 293b 0a0a 2020 2020 2020 2020 6865 6967  );..        heig
-00004990: 6874 2026 2620 732e 7075 7368 2827 6865  ht && s.push('he
-000049a0: 6967 6874 3a27 2c20 6865 6967 6874 2c20  ight:', height, 
-000049b0: 6973 4e61 4e28 6865 6967 6874 2920 3f20  isNaN(height) ? 
-000049c0: 273b 2720 3a20 2770 783b 2729 3b0a 2020  ';' : 'px;');.  
-000049d0: 2020 2020 2020 6d69 6e48 6569 6768 7420        minHeight 
-000049e0: 2626 2073 2e70 7573 6828 276d 696e 2d68  && s.push('min-h
-000049f0: 6569 6768 743a 272c 206d 696e 4865 6967  eight:', minHeig
-00004a00: 6874 2c20 6973 4e61 4e28 6d69 6e48 6569  ht, isNaN(minHei
-00004a10: 6768 7429 203f 2027 3b27 203a 2027 7078  ght) ? ';' : 'px
-00004a20: 3b27 293b 0a20 2020 2020 2020 2077 6964  ;');.        wid
-00004a30: 7468 2026 2620 732e 7075 7368 2827 7769  th && s.push('wi
-00004a40: 6474 683a 272c 2077 6964 7468 2c20 6973  dth:', width, is
-00004a50: 4e61 4e28 7769 6474 6829 203f 2027 3b27  NaN(width) ? ';'
-00004a60: 203a 2027 7078 3b27 293b 0a20 2020 2020   : 'px;');.     
-00004a70: 2020 206d 696e 5769 6474 6820 2626 2073     minWidth && s
-00004a80: 2e70 7573 6828 276d 696e 2d77 6964 7468  .push('min-width
-00004a90: 3a27 2c20 6d69 6e57 6964 7468 2c20 6973  :', minWidth, is
-00004aa0: 4e61 4e28 6d69 6e57 6964 7468 2920 3f20  NaN(minWidth) ? 
-00004ab0: 273b 2720 3a20 2770 783b 2729 3b0a 0a20  ';' : 'px;');.. 
-00004ac0: 2020 2020 2020 2072 6574 7572 6e20 733b         return s;
-00004ad0: 0a20 2020 207d 0a0a 2020 2020 6765 7450  .    }..    getP
-00004ae0: 6164 6469 6e67 7328 6461 7461 203d 207b  addings(data = {
-00004af0: 7d2c 2064 6566 6175 6c74 7320 3d20 7b7d  }, defaults = {}
-00004b00: 2c20 6461 7461 5072 6566 6978 203d 2027  , dataPrefix = '
-00004b10: 2729 207b 0a20 2020 2020 2020 2063 6f6e  ') {.        con
-00004b20: 7374 2073 203d 205b 5d2c 0a20 2020 2020  st s = [],.     
-00004b30: 2020 2020 2020 2070 6164 6469 6e67 426f         paddingBo
-00004b40: 7474 6f6d 203d 2074 6869 732e 6765 7452  ttom = this.getR
-00004b50: 6561 6c56 616c 7565 2827 7061 6464 696e  ealValue('paddin
-00004b60: 6742 6f74 746f 6d27 2c20 6461 7461 2c20  gBottom', data, 
-00004b70: 6465 6661 756c 7473 2e70 6164 6469 6e67  defaults.padding
-00004b80: 426f 7474 6f6d 2c20 6461 7461 5072 6566  Bottom, dataPref
-00004b90: 6978 292c 0a20 2020 2020 2020 2020 2020  ix),.           
-00004ba0: 2070 6164 6469 6e67 4c65 6674 203d 2074   paddingLeft = t
-00004bb0: 6869 732e 6765 7452 6561 6c56 616c 7565  his.getRealValue
-00004bc0: 2827 7061 6464 696e 674c 6566 7427 2c20  ('paddingLeft', 
-00004bd0: 6461 7461 2c20 6465 6661 756c 7473 2e70  data, defaults.p
-00004be0: 6164 6469 6e67 4c65 6674 2c20 6461 7461  addingLeft, data
-00004bf0: 5072 6566 6978 292c 0a20 2020 2020 2020  Prefix),.       
-00004c00: 2020 2020 2070 6164 6469 6e67 5269 6768       paddingRigh
-00004c10: 7420 3d20 7468 6973 2e67 6574 5265 616c  t = this.getReal
-00004c20: 5661 6c75 6528 2770 6164 6469 6e67 5269  Value('paddingRi
-00004c30: 6768 7427 2c20 6461 7461 2c20 6465 6661  ght', data, defa
-00004c40: 756c 7473 2e70 6164 6469 6e67 5269 6768  ults.paddingRigh
-00004c50: 742c 2064 6174 6150 7265 6669 7829 2c0a  t, dataPrefix),.
-00004c60: 2020 2020 2020 2020 2020 2020 7061 6464              padd
-00004c70: 696e 6754 6f70 203d 2074 6869 732e 6765  ingTop = this.ge
-00004c80: 7452 6561 6c56 616c 7565 2827 7061 6464  tRealValue('padd
-00004c90: 696e 6754 6f70 272c 2064 6174 612c 2064  ingTop', data, d
-00004ca0: 6566 6175 6c74 732e 7061 6464 696e 6754  efaults.paddingT
-00004cb0: 6f70 2c20 6461 7461 5072 6566 6978 293b  op, dataPrefix);
-00004cc0: 0a0a 2020 2020 2020 2020 7061 6464 696e  ..        paddin
-00004cd0: 6754 6f70 2026 2620 732e 7075 7368 2827  gTop && s.push('
-00004ce0: 7061 6464 696e 672d 746f 703a 272c 2070  padding-top:', p
-00004cf0: 6164 6469 6e67 546f 702c 2070 6164 6469  addingTop, paddi
-00004d00: 6e67 546f 7020 213d 3d20 2761 7574 6f27  ngTop !== 'auto'
-00004d10: 2026 2620 2169 734e 614e 2870 6164 6469   && !isNaN(paddi
-00004d20: 6e67 546f 7029 203f 2027 7078 3b27 203a  ngTop) ? 'px;' :
-00004d30: 2027 3b27 293b 0a20 2020 2020 2020 2070   ';');.        p
-00004d40: 6164 6469 6e67 4c65 6674 2026 2620 732e  addingLeft && s.
-00004d50: 7075 7368 2827 7061 6464 696e 672d 6c65  push('padding-le
-00004d60: 6674 3a27 2c20 7061 6464 696e 674c 6566  ft:', paddingLef
-00004d70: 742c 2070 6164 6469 6e67 4c65 6674 2021  t, paddingLeft !
-00004d80: 3d3d 2027 6175 746f 2720 2626 2021 6973  == 'auto' && !is
-00004d90: 4e61 4e28 7061 6464 696e 674c 6566 7429  NaN(paddingLeft)
-00004da0: 203f 2027 7078 3b27 203a 2027 3b27 293b   ? 'px;' : ';');
-00004db0: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-00004dc0: 5269 6768 7420 2626 2073 2e70 7573 6828  Right && s.push(
-00004dd0: 2770 6164 6469 6e67 2d72 6967 6874 3a27  'padding-right:'
-00004de0: 2c20 7061 6464 696e 6752 6967 6874 2c20  , paddingRight, 
-00004df0: 7061 6464 696e 6752 6967 6874 2021 3d3d  paddingRight !==
-00004e00: 2027 6175 746f 2720 2626 2021 6973 4e61   'auto' && !isNa
-00004e10: 4e28 7061 6464 696e 6752 6967 6874 2920  N(paddingRight) 
-00004e20: 3f20 2770 783b 2720 3a20 273b 2729 3b0a  ? 'px;' : ';');.
-00004e30: 2020 2020 2020 2020 7061 6464 696e 6742          paddingB
-00004e40: 6f74 746f 6d20 2626 2073 2e70 7573 6828  ottom && s.push(
-00004e50: 2770 6164 6469 6e67 2d62 6f74 746f 6d3a  'padding-bottom:
-00004e60: 272c 2070 6164 6469 6e67 426f 7474 6f6d  ', paddingBottom
-00004e70: 2c20 7061 6464 696e 6742 6f74 746f 6d20  , paddingBottom 
-00004e80: 213d 3d20 2761 7574 6f27 2026 2620 2169  !== 'auto' && !i
-00004e90: 734e 614e 2870 6164 6469 6e67 426f 7474  sNaN(paddingBott
-00004ea0: 6f6d 2920 3f20 2770 783b 2720 3a20 273b  om) ? 'px;' : ';
-00004eb0: 2729 3b0a 0a20 2020 2020 2020 2072 6574  ');..        ret
-00004ec0: 7572 6e20 733b 0a20 2020 207d 0a0a 2020  urn s;.    }..  
-00004ed0: 2020 6765 744d 6172 6769 6e73 2864 6174    getMargins(dat
-00004ee0: 6120 3d20 7b7d 2c20 6465 6661 756c 7473  a = {}, defaults
-00004ef0: 203d 207b 7d2c 2064 6174 6150 7265 6669   = {}, dataPrefi
-00004f00: 7820 3d20 2727 2920 7b0a 2020 2020 2020  x = '') {.      
-00004f10: 2020 636f 6e73 7420 7320 3d20 5b5d 2c0a    const s = [],.
-00004f20: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
-00004f30: 696e 426f 7474 6f6d 203d 2074 6869 732e  inBottom = this.
-00004f40: 6765 7452 6561 6c56 616c 7565 2827 6d61  getRealValue('ma
-00004f50: 7267 696e 426f 7474 6f6d 272c 2064 6174  rginBottom', dat
-00004f60: 612c 2064 6566 6175 6c74 732e 6d61 7267  a, defaults.marg
-00004f70: 696e 426f 7474 6f6d 2c20 6461 7461 5072  inBottom, dataPr
-00004f80: 6566 6978 292c 0a20 2020 2020 2020 2020  efix),.         
-00004f90: 2020 206d 6172 6769 6e4c 6566 7420 3d20     marginLeft = 
-00004fa0: 7468 6973 2e67 6574 5265 616c 5661 6c75  this.getRealValu
-00004fb0: 6528 276d 6172 6769 6e4c 6566 7427 2c20  e('marginLeft', 
-00004fc0: 6461 7461 2c20 6465 6661 756c 7473 2e6d  data, defaults.m
-00004fd0: 6172 6769 6e4c 6566 742c 2064 6174 6150  arginLeft, dataP
-00004fe0: 7265 6669 7829 2c0a 2020 2020 2020 2020  refix),.        
-00004ff0: 2020 2020 6d61 7267 696e 5269 6768 7420      marginRight 
-00005000: 3d20 7468 6973 2e67 6574 5265 616c 5661  = this.getRealVa
-00005010: 6c75 6528 276d 6172 6769 6e52 6967 6874  lue('marginRight
-00005020: 272c 2064 6174 612c 2064 6566 6175 6c74  ', data, default
-00005030: 732e 6d61 7267 696e 5269 6768 742c 2064  s.marginRight, d
-00005040: 6174 6150 7265 6669 7829 2c0a 2020 2020  ataPrefix),.    
-00005050: 2020 2020 2020 2020 6d61 7267 696e 546f          marginTo
-00005060: 7020 3d20 7468 6973 2e67 6574 5265 616c  p = this.getReal
-00005070: 5661 6c75 6528 276d 6172 6769 6e54 6f70  Value('marginTop
-00005080: 272c 2064 6174 612c 2064 6566 6175 6c74  ', data, default
-00005090: 732e 6d61 7267 696e 546f 702c 2064 6174  s.marginTop, dat
-000050a0: 6150 7265 6669 7829 3b0a 0a20 2020 2020  aPrefix);..     
-000050b0: 2020 206d 6172 6769 6e54 6f70 2026 2620     marginTop && 
-000050c0: 732e 7075 7368 2827 6d61 7267 696e 2d74  s.push('margin-t
-000050d0: 6f70 3a27 2c20 6d61 7267 696e 546f 702c  op:', marginTop,
-000050e0: 206d 6172 6769 6e54 6f70 2021 3d3d 2027   marginTop !== '
-000050f0: 6175 746f 2720 2626 2021 6973 4e61 4e28  auto' && !isNaN(
-00005100: 6d61 7267 696e 546f 7029 203f 2027 7078  marginTop) ? 'px
-00005110: 3b27 203a 2027 3b27 293b 0a20 2020 2020  ;' : ';');.     
-00005120: 2020 206d 6172 6769 6e4c 6566 7420 2626     marginLeft &&
-00005130: 2073 2e70 7573 6828 276d 6172 6769 6e2d   s.push('margin-
-00005140: 6c65 6674 3a27 2c20 6d61 7267 696e 4c65  left:', marginLe
-00005150: 6674 2c20 6d61 7267 696e 4c65 6674 2021  ft, marginLeft !
-00005160: 3d3d 2027 6175 746f 2720 2626 2021 6973  == 'auto' && !is
-00005170: 4e61 4e28 6d61 7267 696e 4c65 6674 2920  NaN(marginLeft) 
-00005180: 3f20 2770 783b 2720 3a20 273b 2729 3b0a  ? 'px;' : ';');.
-00005190: 2020 2020 2020 2020 6d61 7267 696e 5269          marginRi
-000051a0: 6768 7420 2626 2073 2e70 7573 6828 276d  ght && s.push('m
-000051b0: 6172 6769 6e2d 7269 6768 743a 272c 206d  argin-right:', m
-000051c0: 6172 6769 6e52 6967 6874 2c20 6d61 7267  arginRight, marg
-000051d0: 696e 5269 6768 7420 213d 3d20 2761 7574  inRight !== 'aut
-000051e0: 6f27 2026 2620 2169 734e 614e 286d 6172  o' && !isNaN(mar
-000051f0: 6769 6e52 6967 6874 2920 3f20 2770 783b  ginRight) ? 'px;
-00005200: 2720 3a20 273b 2729 3b0a 2020 2020 2020  ' : ';');.      
-00005210: 2020 6d61 7267 696e 426f 7474 6f6d 2026    marginBottom &
-00005220: 2620 732e 7075 7368 2827 6d61 7267 696e  & s.push('margin
-00005230: 2d62 6f74 746f 6d3a 272c 206d 6172 6769  -bottom:', margi
-00005240: 6e42 6f74 746f 6d2c 206d 6172 6769 6e42  nBottom, marginB
-00005250: 6f74 746f 6d20 213d 3d20 2761 7574 6f27  ottom !== 'auto'
-00005260: 2026 2620 2169 734e 614e 286d 6172 6769   && !isNaN(margi
-00005270: 6e42 6f74 746f 6d29 203f 2027 7078 3b27  nBottom) ? 'px;'
-00005280: 203a 2027 3b27 293b 0a0a 2020 2020 2020   : ';');..      
-00005290: 2020 7265 7475 726e 2073 3b0a 2020 2020    return s;.    
-000052a0: 7d0a 0a20 2020 2067 6574 5769 6474 6846  }..    getWidthF
-000052b0: 6f72 5365 6374 696f 6e28 6461 7461 203d  orSection(data =
-000052c0: 207b 7d2c 2064 6566 6175 6c74 7320 3d20   {}, defaults = 
-000052d0: 7b7d 2920 7b0a 2020 2020 2020 2020 636f  {}) {.        co
-000052e0: 6e73 7420 7320 3d20 5b5d 2c0a 2020 2020  nst s = [],.    
-000052f0: 2020 2020 2020 2020 7769 6474 6820 3d20          width = 
-00005300: 7468 6973 2e67 6574 5265 616c 5661 6c75  this.getRealValu
-00005310: 6528 2777 6964 7468 272c 2064 6174 612c  e('width', data,
-00005320: 2064 6566 6175 6c74 732e 7769 6474 6829   defaults.width)
-00005330: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
-00005340: 6e48 6569 6768 7420 3d20 7468 6973 2e67  nHeight = this.g
-00005350: 6574 5265 616c 5661 6c75 6528 276d 696e  etRealValue('min
-00005360: 4865 6967 6874 272c 2064 6174 612c 2064  Height', data, d
-00005370: 6566 6175 6c74 732e 6d69 6e48 6569 6768  efaults.minHeigh
-00005380: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-00005390: 6d69 6e57 6964 7468 203d 2074 6869 732e  minWidth = this.
-000053a0: 6765 7452 6561 6c56 616c 7565 2827 6d69  getRealValue('mi
-000053b0: 6e57 6964 7468 272c 2064 6174 612c 2064  nWidth', data, d
-000053c0: 6566 6175 6c74 732e 6d69 6e57 6964 7468  efaults.minWidth
-000053d0: 293b 0a0a 2020 2020 2020 2020 6966 2028  );..        if (
-000053e0: 2169 734e 614e 2877 6964 7468 2929 207b  !isNaN(width)) {
-000053f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005400: 7572 6e20 5b5d 3b0a 2020 2020 2020 2020  urn [];.        
-00005410: 7d0a 0a20 2020 2020 2020 2077 6964 7468  }..        width
-00005420: 2026 2620 732e 7075 7368 2827 7769 6474   && s.push('widt
-00005430: 683a 272c 2077 6964 7468 2c20 6973 4e61  h:', width, isNa
-00005440: 4e28 7769 6474 6829 203f 2027 3b27 203a  N(width) ? ';' :
-00005450: 2027 7078 3b27 293b 0a20 2020 2020 2020   'px;');.       
-00005460: 206d 696e 4865 6967 6874 2026 2620 732e   minHeight && s.
-00005470: 7075 7368 2827 6d69 6e2d 6865 6967 6874  push('min-height
-00005480: 3a27 2c20 6d69 6e48 6569 6768 742c 2069  :', minHeight, i
-00005490: 734e 614e 286d 696e 4865 6967 6874 2920  sNaN(minHeight) 
-000054a0: 3f20 273b 2720 3a20 2770 783b 2729 3b0a  ? ';' : 'px;');.
-000054b0: 2020 2020 2020 2020 6d69 6e57 6964 7468          minWidth
-000054c0: 2026 2620 732e 7075 7368 2827 6d69 6e2d   && s.push('min-
-000054d0: 7769 6474 683a 272c 206d 696e 5769 6474  width:', minWidt
-000054e0: 682c 2069 734e 614e 286d 696e 5769 6474  h, isNaN(minWidt
-000054f0: 6829 203f 2027 3b27 203a 2027 7078 3b27  h) ? ';' : 'px;'
-00005500: 293b 0a0a 2020 2020 2020 2020 7265 7475  );..        retu
-00005510: 726e 2073 3b0a 2020 2020 7d0a 0a20 2020  rn s;.    }..   
-00005520: 2067 6574 4865 6967 6874 466f 7253 6563   getHeightForSec
-00005530: 7469 6f6e 2864 6174 6120 3d20 7b7d 2c20  tion(data = {}, 
-00005540: 6465 6661 756c 7473 203d 207b 7d29 207b  defaults = {}) {
-00005550: 0a20 2020 2020 2020 2063 6f6e 7374 2073  .        const s
-00005560: 203d 205b 5d2c 2068 6569 6768 7420 3d20   = [], height = 
-00005570: 7468 6973 2e67 6574 5265 616c 5661 6c75  this.getRealValu
-00005580: 6528 2768 6569 6768 7427 2c20 6461 7461  e('height', data
-00005590: 2c20 6465 6661 756c 7473 2e68 6569 6768  , defaults.heigh
-000055a0: 7429 3b0a 0a20 2020 2020 2020 2069 6620  t);..        if 
-000055b0: 2821 6973 4e61 4e28 6865 6967 6874 2929  (!isNaN(height))
-000055c0: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
-000055d0: 6574 7572 6e20 5b5d 3b0a 2020 2020 2020  eturn [];.      
-000055e0: 2020 7d0a 0a20 2020 2020 2020 2068 6569    }..        hei
-000055f0: 6768 7420 2626 2073 2e70 7573 6828 2768  ght && s.push('h
-00005600: 6569 6768 743a 272c 2068 6569 6768 742c  eight:', height,
-00005610: 2069 734e 614e 2868 6569 6768 7429 203f   isNaN(height) ?
-00005620: 2027 3b27 203a 2027 7078 3b27 293b 0a0a   ';' : 'px;');..
-00005630: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005640: 3b0a 2020 2020 7d0a 0a20 2020 2073 7461  ;.    }..    sta
-00005650: 7469 6320 6765 7450 6572 6365 6e74 4f72  tic getPercentOr
-00005660: 5069 7865 6c28 7661 6c75 6529 207b 0a20  Pixel(value) {. 
-00005670: 2020 2020 2020 2072 6574 7572 6e20 6973         return is
-00005680: 4e61 4e28 7661 6c75 6529 203f 2076 616c  NaN(value) ? val
-00005690: 7565 203a 2076 616c 7565 202b 2027 7078  ue : value + 'px
-000056a0: 273b 0a20 2020 207d 0a0a 2020 2020 7374  ';.    }..    st
-000056b0: 6174 6963 2073 6574 536b 696e 2865 6c65  atic setSkin(ele
-000056c0: 6d65 6e74 2c20 736b 696e 5072 6566 6978  ment, skinPrefix
-000056d0: 2c20 6e65 7753 6b69 6e29 207b 0a20 2020  , newSkin) {.   
-000056e0: 2020 2020 2069 6620 2821 656c 656d 656e       if (!elemen
-000056f0: 742e 6861 7343 6c61 7373 2873 6b69 6e50  t.hasClass(skinP
-00005700: 7265 6669 7820 2b20 6e65 7753 6b69 6e29  refix + newSkin)
-00005710: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00005720: 6966 2028 656c 656d 656e 742e 6174 7472  if (element.attr
-00005730: 2827 636c 6173 7327 2929 207b 0a20 2020  ('class')) {.   
-00005740: 2020 2020 2020 2020 2020 2020 206c 6574               let
-00005750: 2072 6573 756c 742c 2063 6c61 7373 5769   result, classWi
-00005760: 7468 6f75 7453 6b69 6e2c 206f 7269 6769  thoutSkin, origi
-00005770: 6e61 6c43 6c61 7373 203d 2065 6c65 6d65  nalClass = eleme
-00005780: 6e74 2e61 7474 7228 2763 6c61 7373 2729  nt.attr('class')
-00005790: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000057a0: 2020 2020 2020 7320 3d20 6f72 6967 696e        s = origin
-000057b0: 616c 436c 6173 732e 696e 6465 784f 6628  alClass.indexOf(
-000057c0: 736b 696e 5072 6566 6978 293b 0a20 2020  skinPrefix);.   
-000057d0: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
-000057e0: 7373 5769 7468 6f75 7453 6b69 6e20 3d20  ssWithoutSkin = 
-000057f0: 7320 213d 3d20 2d31 203f 206f 7269 6769  s !== -1 ? origi
-00005800: 6e61 6c43 6c61 7373 2e73 7562 7374 7269  nalClass.substri
-00005810: 6e67 2830 2c20 7320 2d20 3129 203a 206f  ng(0, s - 1) : o
-00005820: 7269 6769 6e61 6c43 6c61 7373 3b0a 2020  riginalClass;.  
-00005830: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00005840: 7375 6c74 203d 2063 6c61 7373 5769 7468  sult = classWith
-00005850: 6f75 7453 6b69 6e2e 7370 6c69 7428 2720  outSkin.split(' 
-00005860: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
-00005870: 2020 2020 7265 7375 6c74 2e70 7573 6828      result.push(
-00005880: 736b 696e 5072 6566 6978 202b 206e 6577  skinPrefix + new
-00005890: 536b 696e 293b 0a20 2020 2020 2020 2020  Skin);.         
-000058a0: 2020 2020 2020 2065 6c65 6d65 6e74 2e61         element.a
-000058b0: 7474 7228 2763 6c61 7373 272c 2072 6573  ttr('class', res
-000058c0: 756c 742e 6a6f 696e 2827 2027 2929 3b0a  ult.join(' '));.
-000058d0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000058e0: 2020 2020 2020 7d0a 2020 2020 7d0a 0a20        }.    }.. 
-000058f0: 2020 2073 7461 7469 6320 7265 6d6f 7665     static remove
-00005900: 5374 796c 6528 656c 656d 656e 742c 2073  Style(element, s
-00005910: 7479 6c65 4e61 6d65 2920 7b0a 2020 2020  tyleName) {.    
-00005920: 2020 2020 6c65 7420 7320 3d20 656c 656d      let s = elem
-00005930: 656e 742e 7072 6f70 2827 7374 796c 6527  ent.prop('style'
-00005940: 293b 0a20 2020 2020 2020 2073 2026 2620  );.        s && 
-00005950: 732e 7265 6d6f 7665 5072 6f70 6572 7479  s.removeProperty
-00005960: 2873 7479 6c65 4e61 6d65 293b 0a20 2020  (styleName);.   
-00005970: 207d 0a0a 2020 2020 7374 6174 6963 2073   }..    static s
-00005980: 6574 4f72 5265 6d6f 7665 5374 796c 6528  etOrRemoveStyle(
-00005990: 656c 656d 656e 742c 2073 7479 6c65 4e61  element, styleNa
-000059a0: 6d65 2c20 7661 6c75 6529 207b 0a20 2020  me, value) {.   
-000059b0: 2020 2020 2076 616c 7565 203f 2065 6c65       value ? ele
-000059c0: 6d65 6e74 2e63 7373 2873 7479 6c65 4e61  ment.css(styleNa
-000059d0: 6d65 2c20 7661 6c75 6529 203a 2057 6964  me, value) : Wid
-000059e0: 6765 742e 7265 6d6f 7665 5374 796c 6528  get.removeStyle(
-000059f0: 656c 656d 656e 742c 2073 7479 6c65 4e61  element, styleNa
-00005a00: 6d65 293b 0a20 2020 207d 0a0a 2020 2020  me);.    }..    
-00005a10: 7374 6174 6963 2073 6574 4f72 5265 6d6f  static setOrRemo
-00005a20: 7665 4d65 6173 7572 6528 656c 656d 656e  veMeasure(elemen
-00005a30: 742c 206d 6561 7375 7265 4e61 6d65 2c20  t, measureName, 
-00005a40: 7661 6c75 6529 207b 0a20 2020 2020 2020  value) {.       
-00005a50: 2057 6964 6765 742e 7365 744f 7252 656d   Widget.setOrRem
-00005a60: 6f76 6553 7479 6c65 2865 6c65 6d65 6e74  oveStyle(element
-00005a70: 2c20 6d65 6173 7572 654e 616d 652c 2076  , measureName, v
-00005a80: 616c 7565 203f 2057 6964 6765 742e 6765  alue ? Widget.ge
-00005a90: 7450 6572 6365 6e74 4f72 5069 7865 6c28  tPercentOrPixel(
-00005aa0: 7661 6c75 6529 203a 2066 616c 7365 293b  value) : false);
-00005ab0: 0a20 2020 207d 0a0a 2020 2020 7374 6174  .    }..    stat
-00005ac0: 6963 2061 6464 4f72 5265 6d6f 7665 436c  ic addOrRemoveCl
-00005ad0: 6173 7328 656c 656d 656e 742c 2063 6c61  ass(element, cla
-00005ae0: 7373 4e61 6d65 2c20 6164 6429 207b 0a20  ssName, add) {. 
-00005af0: 2020 2020 2020 2061 6464 203f 2021 656c         add ? !el
-00005b00: 656d 656e 742e 6861 7343 6c61 7373 2863  ement.hasClass(c
-00005b10: 6c61 7373 4e61 6d65 2920 2626 2065 6c65  lassName) && ele
-00005b20: 6d65 6e74 2e61 6464 436c 6173 7328 636c  ment.addClass(cl
-00005b30: 6173 734e 616d 6529 203a 2065 6c65 6d65  assName) : eleme
-00005b40: 6e74 2e72 656d 6f76 6543 6c61 7373 2863  nt.removeClass(c
-00005b50: 6c61 7373 4e61 6d65 293b 0a20 2020 207d  lassName);.    }
-00005b60: 0a7d                                     .}
+000021b0: 2020 7669 7369 626c 6520 3d20 756e 6465    visible = unde
+000021c0: 6669 6e65 6420 213d 3d20 7620 3f20 7620  fined !== v ? v 
+000021d0: 3a20 6f2e 7669 7369 626c 653b 0a0a 2020  : o.visible;..  
+000021e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000021f0: 7220 2872 206f 6620 7265 7375 6c74 7329  r (r of results)
+00002200: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002210: 2020 2020 2020 2077 6964 6765 7448 746d         widgetHtm
+00002220: 6c73 2e70 7573 6828 7229 3b0a 2020 2020  ls.push(r);.    
+00002230: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+00002240: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002250: 6574 7572 6e20 696e 7374 616e 6365 2e67  eturn instance.g
+00002260: 6574 4d61 696e 4874 6d6c 456c 656d 656e  etMainHtmlElemen
+00002270: 7428 6f2c 2070 726f 6365 7373 6564 4461  t(o, processedDa
+00002280: 7461 2c20 7669 7369 626c 652c 2077 6964  ta, visible, wid
+00002290: 6765 7448 746d 6c73 2c20 7769 7468 5374  getHtmls, withSt
+000022a0: 6174 6529 3b0a 2020 2020 2020 2020 2020  ate);.          
+000022b0: 2020 7d29 3b0a 2020 2020 2020 2020 7d3b    });.        };
+000022c0: 0a0a 2020 2020 2020 2020 6966 2028 7072  ..        if (pr
+000022d0: 6576 696f 7573 6c79 4c6f 6164 6564 4461  eviouslyLoadedDa
+000022e0: 7461 2021 3d3d 2066 616c 7365 2920 7b0a  ta !== false) {.
+000022f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002300: 726e 2061 6674 6572 4c6f 6164 2870 7265  rn afterLoad(pre
+00002310: 7669 6f75 736c 794c 6f61 6465 6444 6174  viouslyLoadedDat
+00002320: 6129 3b0a 2020 2020 2020 2020 7d0a 0a20  a);.        }.. 
+00002330: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+00002340: 6164 4675 6e63 7469 6f6e 286f 2e69 642c  adFunction(o.id,
+00002350: 2069 6e73 7461 6e63 652e 6e61 6d65 2c20   instance.name, 
+00002360: 7573 6544 6566 6175 6c74 4461 7461 466f  useDefaultDataFo
+00002370: 7243 6869 6c64 7265 6e29 2e74 6865 6e28  rChildren).then(
+00002380: 6675 6e63 7469 6f6e 2028 6461 7461 2920  function (data) 
+00002390: 7b0a 2020 2020 2020 2020 2020 2020 7265  {.            re
+000023a0: 7475 726e 2061 6674 6572 4c6f 6164 2864  turn afterLoad(d
+000023b0: 6174 6129 3b0a 2020 2020 2020 2020 7d29  ata);.        })
+000023c0: 3b0a 2020 2020 7d0a 0a20 2020 2067 6574  ;.    }..    get
+000023d0: 4d61 696e 4874 6d6c 456c 656d 656e 7428  MainHtmlElement(
+000023e0: 6f2c 2064 6174 612c 2076 6973 6962 6c65  o, data, visible
+000023f0: 2c20 7769 6467 6574 4874 6d6c 732c 2077  , widgetHtmls, w
+00002400: 6974 6853 7461 7465 2920 7b0a 2020 2020  ithState) {.    
+00002410: 2020 2020 6c65 7420 6773 203d 205b 5d2c      let gs = [],
+00002420: 2068 746d 6c3b 0a0a 2020 2020 2020 2020   html;..        
+00002430: 6966 2028 6f2e 6170 706c 794d 6561 7375  if (o.applyMeasu
+00002440: 7265 7354 6f53 6563 7469 6f6e 203d 3d3d  resToSection ===
+00002450: 2074 7275 6529 207b 0a20 2020 2020 2020   true) {.       
+00002460: 2020 2020 2067 7320 3d20 7468 6973 2e67       gs = this.g
+00002470: 6574 5769 6474 6841 6e64 4865 6967 6874  etWidthAndHeight
+00002480: 2864 6174 6129 3b0a 2020 2020 2020 2020  (data);.        
+00002490: 7d0a 0a20 2020 2020 2020 2069 6620 2876  }..        if (v
+000024a0: 6973 6962 6c65 203d 3d3d 2066 616c 7365  isible === false
+000024b0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+000024c0: 6773 2e70 7573 6828 2764 6973 706c 6179  gs.push('display
+000024d0: 3a6e 6f6e 653b 2729 3b0a 2020 2020 2020  :none;');.      
+000024e0: 2020 7d0a 0a20 2020 2020 2020 206c 6574    }..        let
+000024f0: 206f 7269 6769 6e61 6c49 6420 3d20 6661   originalId = fa
+00002500: 6c73 652c 2077 7269 7465 203d 2027 6f6e  lse, write = 'on
+00002510: 273b 0a20 2020 2020 2020 2069 6620 2864  ';.        if (d
+00002520: 6174 6120 2626 2064 6174 612e 6f72 6967  ata && data.orig
+00002530: 696e 616c 4964 2920 7b0a 2020 2020 2020  inalId) {.      
+00002540: 2020 2020 2020 6f72 6967 696e 616c 4964        originalId
+00002550: 203d 2064 6174 612e 6f72 6967 696e 616c   = data.original
+00002560: 4964 3b0a 2020 2020 2020 2020 7d0a 0a20  Id;.        }.. 
+00002570: 2020 2020 2020 2069 6620 286f 2e77 7269         if (o.wri
+00002580: 7465 2920 7b0a 2020 2020 2020 2020 2020  te) {.          
+00002590: 2020 7772 6974 6520 3d20 6f2e 7772 6974    write = o.writ
+000025a0: 653b 0a20 2020 2020 2020 207d 0a0a 2020  e;.        }..  
+000025b0: 2020 2020 2020 6966 2028 6461 7461 2026        if (data &
+000025c0: 2620 6461 7461 2e77 7269 7465 2920 7b0a  & data.write) {.
+000025d0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+000025e0: 6520 3d20 6461 7461 2e77 7269 7465 3b0a  e = data.write;.
+000025f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002600: 2020 6874 6d6c 203d 2074 6869 732e 6765    html = this.ge
+00002610: 7448 746d 6c28 7769 6467 6574 4874 6d6c  tHtml(widgetHtml
+00002620: 732c 2064 6174 612c 2077 6974 6853 7461  s, data, withSta
+00002630: 7465 293b 0a0a 2020 2020 2020 2020 7265  te);..        re
+00002640: 7475 726e 2060 3c73 6563 7469 6f6e 2024  turn `<section $
+00002650: 7b77 7269 7465 203d 3d3d 2027 6f66 6627  {write === 'off'
+00002660: 203f 2060 6461 7461 2d77 7269 7465 3d22   ? `data-write="
+00002670: 6f66 6622 6020 3a20 2727 7d20 247b 6f72  off"` : ''} ${or
+00002680: 6967 696e 616c 4964 2021 3d3d 2066 616c  iginalId !== fal
+00002690: 7365 203f 2060 6461 7461 2d6f 7269 6769  se ? `data-origi
+000026a0: 6e61 6c49 643d 2224 7b6f 2e6f 7269 6769  nalId="${o.origi
+000026b0: 6e61 6c49 647d 2260 203a 2027 277d 2024  nalId}"` : ''} $
+000026c0: 7b6f 2e6f 7264 696e 616c 203f 2060 6461  {o.ordinal ? `da
+000026d0: 7461 2d6f 7264 696e 616c 3d22 247b 6f2e  ta-ordinal="${o.
+000026e0: 6f72 6469 6e61 6c7d 2260 203a 2027 277d  ordinal}"` : ''}
+000026f0: 2024 7b6f 2e6d 6172 6769 6e20 3f20 2763   ${o.margin ? 'c
+00002700: 6c61 7373 3d22 7772 6170 7065 7222 2720  lass="wrapper"' 
+00002710: 3a20 2727 7d20 7374 796c 653d 2224 7b67  : ''} style="${g
+00002720: 732e 6a6f 696e 2827 2729 7d22 2069 643d  s.join('')}" id=
+00002730: 2224 7b6f 2e69 6420 3f20 6f2e 6964 203a  "${o.id ? o.id :
+00002740: 2055 7469 6c73 2e67 6574 5261 6e64 6f6d   Utils.getRandom
+00002750: 4964 2829 7d22 3e24 7b68 746d 6c7d 3c2f  Id()}">${html}</
+00002760: 7365 6374 696f 6e3e 603b 0a0a 2020 2020  section>`;..    
+00002770: 7d0a 0a20 2020 2065 6d62 6564 6465 6452  }..    embeddedR
+00002780: 656e 6465 7228 7769 7468 5374 6174 652c  ender(withState,
+00002790: 2064 6174 612c 206c 6f61 6446 756e 6374   data, loadFunct
+000027a0: 696f 6e20 3d20 5142 2e6c 6f61 6444 6174  ion = QB.loadDat
+000027b0: 6129 207b 0a20 2020 2020 2020 2074 6869  a) {.        thi
+000027c0: 732e 6973 5265 6e64 6572 696e 6720 3d20  s.isRendering = 
+000027d0: 7472 7565 3b0a 2020 2020 2020 2020 636f  true;.        co
+000027e0: 6e73 7420 6f20 3d20 7b2e 2e2e 7468 6973  nst o = {...this
+000027f0: 2e6f 7074 696f 6e73 2c20 2e2e 2e64 6174  .options, ...dat
+00002800: 617d 2c20 696e 7374 616e 6365 203d 2074  a}, instance = t
+00002810: 6869 732c 2068 203d 204c 6973 7465 6e65  his, h = Listene
+00002820: 7273 2e68 616e 646c 653b 0a0a 2020 2020  rs.handle;..    
+00002830: 2020 2020 7468 6973 2e61 6464 4c69 7374      this.addList
+00002840: 656e 6572 7328 6661 6c73 6529 3b0a 0a20  eners(false);.. 
+00002850: 2020 2020 2020 2069 6620 286e 6577 206f         if (new o
+00002860: 2e74 7970 6528 6f29 2e61 6d49 4f6e 4147  .type(o).amIOnAG
+00002870: 7269 6454 6162 6c65 2829 2920 7b0a 2020  ridTable()) {.  
+00002880: 2020 2020 2020 2020 2020 4c69 7374 656e            Listen
+00002890: 6572 732e 7075 7368 287b 6f70 7469 6f6e  ers.push({option
+000028a0: 733a 206f 2c20 6d65 7468 6f64 3a20 2772  s: o, method: 'r
+000028b0: 6566 7265 7368 4772 6964 4365 6c6c 272c  efreshGridCell',
+000028c0: 2065 7665 6e74 4e61 6d65 3a20 2766 6f72   eventName: 'for
+000028d0: 6365 7265 6672 6573 682e 2720 2b20 6f2e  cerefresh.' + o.
+000028e0: 6964 2c20 6861 6e64 6c65 723a 2068 7d29  id, handler: h})
+000028f0: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
+00002900: 2020 2020 206c 6574 2076 6973 6962 6c65       let visible
+00002910: 203d 2064 6174 6120 2626 2074 7970 656f   = data && typeo
+00002920: 6620 6461 7461 2e76 6973 6962 6c65 2021  f data.visible !
+00002930: 3d3d 2027 756e 6465 6669 6e65 6427 203f  == 'undefined' ?
+00002940: 2064 6174 612e 7669 7369 626c 6520 3a20   data.visible : 
+00002950: 6f2e 7669 7369 626c 653b 0a0a 2020 2020  o.visible;..    
+00002960: 2020 2020 7265 7475 726e 2069 6e73 7461      return insta
+00002970: 6e63 652e 6765 744d 6169 6e48 746d 6c45  nce.getMainHtmlE
+00002980: 6c65 6d65 6e74 286f 2c20 6461 7461 2c20  lement(o, data, 
+00002990: 7669 7369 626c 652c 205b 5d2c 2077 6974  visible, [], wit
+000029a0: 6853 7461 7465 290a 0a20 2020 207d 0a0a  hState)..    }..
+000029b0: 2020 2020 6164 6444 6570 656e 6465 6e74      addDependent
+000029c0: 7328 2920 7b0a 2020 2020 2020 2020 636f  s() {.        co
+000029d0: 6e73 7420 6f20 3d20 7468 6973 2e6f 7074  nst o = this.opt
+000029e0: 696f 6e73 2c20 6820 3d20 4c69 7374 656e  ions, h = Listen
+000029f0: 6572 732e 6861 6e64 6c65 3b0a 0a20 2020  ers.handle;..   
+00002a00: 2020 2020 2069 6620 286f 2e64 6570 656e       if (o.depen
+00002a10: 6473 2920 7b0a 2020 2020 2020 2020 2020  ds) {.          
+00002a20: 2020 636f 6e73 7420 6620 3d20 6f2e 6964    const f = o.id
+00002a30: 2e73 706c 6974 2827 5f27 292c 2061 203d  .split('_'), a =
+00002a40: 2066 5b30 5d2c 2062 203d 2066 5b31 5d3b   f[0], b = f[1];
+00002a50: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00002a60: 7220 286c 6574 206c 206f 6620 6f2e 6465  r (let l of o.de
+00002a70: 7065 6e64 7329 207b 0a20 2020 2020 2020  pends) {.       
+00002a80: 2020 2020 2020 2020 204c 6973 7465 6e65           Listene
+00002a90: 7273 2e70 7573 6828 7b0a 2020 2020 2020  rs.push({.      
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+00002ab0: 7469 6f6e 733a 206f 2c0a 2020 2020 2020  tions: o,.      
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00002ad0: 7468 6f64 3a20 2772 6566 7265 7368 4772  thod: 'refreshGr
+00002ae0: 6964 4365 6c6c 272c 0a20 2020 2020 2020  idCell',.       
+00002af0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00002b00: 6e74 4e61 6d65 3a20 6c2e 6576 656e 7420  ntName: l.event 
+00002b10: 3f20 6c2e 6576 656e 7420 3a20 6c2e 6163  ? l.event : l.ac
+00002b20: 7469 6f6e 202b 2027 2e27 202b 2061 202b  tion + '.' + a +
+00002b30: 2027 5f27 202b 2062 202b 2027 5f27 202b   '_' + b + '_' +
+00002b40: 206c 2e63 6f6c 202b 2027 2e66 696e 6973   l.col + '.finis
+00002b50: 6865 6427 2c0a 2020 2020 2020 2020 2020  hed',.          
+00002b60: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00002b70: 7465 7273 3a20 6c2e 7061 7261 6d65 7465  ters: l.paramete
+00002b80: 7273 207c 7c20 5b5d 2c0a 2020 2020 2020  rs || [],.      
+00002b90: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00002ba0: 6e64 6c65 723a 2068 0a20 2020 2020 2020  ndler: h.       
+00002bb0: 2020 2020 2020 2020 207d 293b 0a20 2020           });.   
+00002bc0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002bd0: 2020 207d 0a20 2020 207d 0a0a 2020 2020     }.    }..    
+00002be0: 6164 644c 6973 7465 6e65 7273 2872 6563  addListeners(rec
+00002bf0: 7572 7369 7665 203d 2074 7275 6529 207b  ursive = true) {
+00002c00: 0a20 2020 2020 2020 2063 6f6e 7374 206f  .        const o
+00002c10: 203d 2074 6869 732e 6f70 7469 6f6e 732c   = this.options,
+00002c20: 2068 203d 204c 6973 7465 6e65 7273 2e68   h = Listeners.h
+00002c30: 616e 646c 653b 0a0a 2020 2020 2020 2020  andle;..        
+00002c40: 6966 2028 6f2e 6c69 7374 656e 2920 7b0a  if (o.listen) {.
+00002c50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002c60: 286c 6574 206c 206f 6620 6f2e 6c69 7374  (let l of o.list
+00002c70: 656e 2920 7b0a 2020 2020 2020 2020 2020  en) {.          
+00002c80: 2020 2020 2020 4c69 7374 656e 6572 732e        Listeners.
+00002c90: 7075 7368 287b 0a20 2020 2020 2020 2020  push({.         
+00002ca0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00002cb0: 6e73 3a20 6f2c 0a20 2020 2020 2020 2020  ns: o,.         
+00002cc0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+00002cd0: 643a 206c 2e6d 6574 686f 642c 0a20 2020  d: l.method,.   
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2065 7665 6e74 4e61 6d65 3a20 6c2e 6576   eventName: l.ev
+00002d00: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
+00002d10: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+00002d20: 6572 733a 206c 2e70 6172 616d 6574 6572  ers: l.parameter
+00002d30: 7320 7c7c 205b 5d2c 0a20 2020 2020 2020  s || [],.       
+00002d40: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00002d50: 646c 6572 3a20 680a 2020 2020 2020 2020  dler: h.        
+00002d60: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
+00002d70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002d80: 2020 7d0a 0a20 2020 2020 2020 2069 6620    }..        if 
+00002d90: 286f 2e64 6570 656e 6473 2026 2620 7265  (o.depends && re
+00002da0: 6375 7273 6976 6520 3d3d 3d20 6661 6c73  cursive === fals
+00002db0: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
+00002dc0: 2074 6869 732e 6164 6444 6570 656e 6465   this.addDepende
+00002dd0: 6e74 7328 293b 0a20 2020 2020 2020 207d  nts();.        }
+00002de0: 0a0a 2020 2020 2020 2020 7468 6973 2e61  ..        this.a
+00002df0: 7070 656e 644c 6973 7465 6e65 7273 286f  ppendListeners(o
+00002e00: 2c20 6829 3b0a 0a20 2020 2020 2020 2069  , h);..        i
+00002e10: 6620 2872 6563 7572 7369 7665 2920 7b0a  f (recursive) {.
+00002e20: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+00002e30: 7769 6467 6574 4f70 7469 6f6e 732c 2077  widgetOptions, w
+00002e40: 6964 6765 7473 203d 205b 5d2c 2077 2c20  idgets = [], w, 
+00002e50: 7777 3b0a 0a20 2020 2020 2020 2020 2020  ww;..           
+00002e60: 2066 6f72 2028 7769 6467 6574 4f70 7469   for (widgetOpti
+00002e70: 6f6e 7320 6f66 206f 2e77 6964 6765 7473  ons of o.widgets
+00002e80: 207c 7c20 5b5d 2920 7b0a 2020 2020 2020   || []) {.      
+00002e90: 2020 2020 2020 2020 2020 7777 203d 2074            ww = t
+00002ea0: 6869 732e 6765 7457 6964 6765 7428 7769  his.getWidget(wi
+00002eb0: 6467 6574 4f70 7469 6f6e 7329 3b0a 2020  dgetOptions);.  
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00002ed0: 6467 6574 732e 7075 7368 2877 7729 3b0a  dgets.push(ww);.
+00002ee0: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+00002ef0: 2020 2020 2020 2020 2020 2069 6620 286f             if (o
+00002f00: 2e74 7970 652e 6e61 6d65 203d 3d3d 2027  .type.name === '
+00002f10: 4772 6964 5461 626c 6557 6964 6765 7427  GridTableWidget'
+00002f20: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00002f30: 2020 2020 7468 6973 2e61 6464 4772 6964      this.addGrid
+00002f40: 5461 626c 654c 6973 7465 6e65 7273 2829  TableListeners()
+00002f50: 3b0a 2020 2020 2020 2020 2020 2020 7d20  ;.            } 
+00002f60: 656c 7365 207b 0a20 2020 2020 2020 2020  else {.         
+00002f70: 2020 2020 2020 2066 6f72 2028 7720 6f66         for (w of
+00002f80: 2077 6964 6765 7473 2920 7b0a 2020 2020   widgets) {.    
+00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fa0: 772e 6164 644c 6973 7465 6e65 7273 2829  w.addListeners()
+00002fb0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00002fc0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00002fd0: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
+00002fe0: 7d0a 0a20 2020 2061 7070 656e 644c 6973  }..    appendLis
+00002ff0: 7465 6e65 7273 286f 7074 696f 6e73 2c20  teners(options, 
+00003000: 6861 6e64 6c65 7229 207b 0a0a 2020 2020  handler) {..    
+00003010: 7d0a 0a20 2020 2069 6e69 7446 696e 6973  }..    initFinis
+00003020: 6865 6428 2920 7b0a 2020 2020 2020 2020  hed() {.        
+00003030: 7468 6973 2e74 7269 6767 6572 4669 6e69  this.triggerFini
+00003040: 7368 6564 4576 656e 7428 293b 0a20 2020  shedEvent();.   
+00003050: 207d 0a0a 2020 2020 7570 6461 7465 436f   }..    updateCo
+00003060: 6e74 656e 7446 696e 6973 6865 6428 2920  ntentFinished() 
+00003070: 7b0a 2020 2020 2020 2020 7468 6973 2e74  {.        this.t
+00003080: 7269 6767 6572 4669 6e69 7368 6564 4576  riggerFinishedEv
+00003090: 656e 7428 2775 7064 6174 6543 6f6e 7465  ent('updateConte
+000030a0: 6e74 2729 3b0a 2020 2020 7d0a 0a20 2020  nt');.    }..   
+000030b0: 2072 6566 7265 7368 4669 6e69 7368 6564   refreshFinished
+000030c0: 2829 207b 0a20 2020 2020 2020 2074 6869  () {.        thi
+000030d0: 732e 7472 6967 6765 7246 696e 6973 6865  s.triggerFinishe
+000030e0: 6445 7665 6e74 2827 7265 6672 6573 6827  dEvent('refresh'
+000030f0: 293b 0a20 2020 207d 0a0a 2020 2020 7472  );.    }..    tr
+00003100: 6967 6765 7246 696e 6973 6865 6445 7665  iggerFinishedEve
+00003110: 6e74 2865 7665 6e74 5479 7065 203d 2027  nt(eventType = '
+00003120: 696e 6974 2729 207b 0a20 2020 2020 2020  init') {.       
+00003130: 2063 6f6e 7374 206f 203d 2074 6869 732e   const o = this.
+00003140: 6f70 7469 6f6e 733b 0a0a 2020 2020 2020  options;..      
+00003150: 2020 6c65 7420 7769 6467 6574 4f70 7469    let widgetOpti
+00003160: 6f6e 732c 2077 6964 6765 7473 203d 205b  ons, widgets = [
+00003170: 5d2c 2077 2c20 7777 3b0a 0a20 2020 2020  ], w, ww;..     
+00003180: 2020 2066 6f72 2028 7769 6467 6574 4f70     for (widgetOp
+00003190: 7469 6f6e 7320 6f66 206f 2e77 6964 6765  tions of o.widge
+000031a0: 7473 207c 7c20 5b5d 2920 7b0a 2020 2020  ts || []) {.    
+000031b0: 2020 2020 2020 2020 7777 203d 2074 6869          ww = thi
+000031c0: 732e 6765 7457 6964 6765 7428 7769 6467  s.getWidget(widg
+000031d0: 6574 4f70 7469 6f6e 7329 3b0a 2020 2020  etOptions);.    
+000031e0: 2020 2020 2020 2020 7769 6467 6574 732e          widgets.
+000031f0: 7075 7368 2877 7729 3b0a 2020 2020 2020  push(ww);.      
+00003200: 2020 7d0a 0a20 2020 2020 2020 2066 6f72    }..        for
+00003210: 2028 7720 6f66 2077 6964 6765 7473 2920   (w of widgets) 
+00003220: 7b0a 2020 2020 2020 2020 2020 2020 772e  {.            w.
+00003230: 7472 6967 6765 7246 696e 6973 6865 6445  triggerFinishedE
+00003240: 7665 6e74 2865 7665 6e74 5479 7065 293b  vent(eventType);
+00003250: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00003260: 2020 2020 456c 2e62 6f64 792e 7472 6967      El.body.trig
+00003270: 6765 7248 616e 646c 6572 2865 7665 6e74  gerHandler(event
+00003280: 5479 7065 202b 2027 2e27 202b 206f 2e69  Type + '.' + o.i
+00003290: 6420 2b20 272e 6669 6e69 7368 6564 2729  d + '.finished')
+000032a0: 3b0a 0a20 2020 2020 2020 206c 6574 2061  ;..        let a
+000032b0: 6374 696f 6e73 203d 2045 7665 6e74 4d61  ctions = EventMa
+000032c0: 705b 6576 656e 7454 7970 6520 2b20 272e  p[eventType + '.
+000032d0: 2720 2b20 6f2e 6964 202b 2027 2e66 696e  ' + o.id + '.fin
+000032e0: 6973 6865 6427 5d2c 2061 3b0a 2020 2020  ished'], a;.    
+000032f0: 2020 2020 6966 2028 6163 7469 6f6e 7329      if (actions)
+00003300: 207b 0a20 2020 2020 2020 2020 2020 2066   {.            f
+00003310: 6f72 2028 6120 6f66 2061 6374 696f 6e73  or (a of actions
+00003320: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00003330: 2020 2020 612e 6163 7469 6f6e 2861 2e61      a.action(a.a
+00003340: 7267 756d 656e 742c 207b 7d2c 207b 7d29  rgument, {}, {})
+00003350: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+00003360: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003370: 2020 6966 2028 5265 706f 7369 746f 7279    if (Repository
+00003380: 5b6f 2e69 645d 2026 2620 5265 706f 7369  [o.id] && Reposi
+00003390: 746f 7279 5b6f 2e69 645d 5b65 7665 6e74  tory[o.id][event
+000033a0: 5479 7065 202b 2027 4669 6e69 7368 6564  Type + 'Finished
+000033b0: 275d 2920 7b0a 2020 2020 2020 2020 2020  ']) {.          
+000033c0: 2020 5265 706f 7369 746f 7279 5b6f 2e69    Repository[o.i
+000033d0: 645d 5b65 7665 6e74 5479 7065 202b 2027  d][eventType + '
+000033e0: 4669 6e69 7368 6564 275d 2829 3b0a 2020  Finished']();.  
+000033f0: 2020 2020 2020 7d0a 2020 2020 7d0a 0a20        }.    }.. 
+00003400: 2020 2069 6e69 7445 7665 6e74 7328 7769     initEvents(wi
+00003410: 7468 5374 6174 6529 207b 0a20 2020 2020  thState) {.     
+00003420: 2020 2063 6f6e 7374 206f 203d 2074 6869     const o = thi
+00003430: 732e 6f70 7469 6f6e 732c 2073 6563 7469  s.options, secti
+00003440: 6f6e 203d 2024 2827 2327 202b 206f 2e69  on = $('#' + o.i
+00003450: 6429 3b0a 0a20 2020 2020 2020 206c 6574  d);..        let
+00003460: 2077 6964 6765 744f 7074 696f 6e73 2c20   widgetOptions, 
+00003470: 7769 6467 6574 7320 3d20 5b5d 2c20 772c  widgets = [], w,
+00003480: 2077 773b 0a0a 2020 2020 2020 2020 666f   ww;..        fo
+00003490: 7220 2877 6964 6765 744f 7074 696f 6e73  r (widgetOptions
+000034a0: 206f 6620 6f2e 7769 6467 6574 7320 7c7c   of o.widgets ||
+000034b0: 205b 5d29 207b 0a20 2020 2020 2020 2020   []) {.         
+000034c0: 2020 2077 7720 3d20 7468 6973 2e67 6574     ww = this.get
+000034d0: 5769 6467 6574 2877 6964 6765 744f 7074  Widget(widgetOpt
+000034e0: 696f 6e73 293b 0a20 2020 2020 2020 2020  ions);.         
+000034f0: 2020 2077 6964 6765 7473 2e70 7573 6828     widgets.push(
+00003500: 7777 293b 0a20 2020 2020 2020 207d 0a0a  ww);.        }..
+00003510: 2020 2020 2020 2020 666f 7220 2877 206f          for (w o
+00003520: 6620 7769 6467 6574 7329 207b 0a20 2020  f widgets) {.   
+00003530: 2020 2020 2020 2020 2077 2e69 6e69 7445           w.initE
+00003540: 7665 6e74 7328 7769 7468 5374 6174 6529  vents(withState)
+00003550: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
+00003560: 2020 2020 2074 6869 732e 696e 6974 4576       this.initEv
+00003570: 656e 7448 616e 646c 6572 7328 7769 7468  entHandlers(with
+00003580: 5374 6174 6529 3b0a 0a20 2020 2020 2020  State);..       
+00003590: 2074 6869 732e 6973 5265 6e64 6572 696e   this.isRenderin
+000035a0: 6720 3d20 6661 6c73 653b 0a20 2020 207d  g = false;.    }
+000035b0: 0a0a 2020 2020 696e 6974 4576 656e 7448  ..    initEventH
+000035c0: 616e 646c 6572 7328 2920 7b0a 0a20 2020  andlers() {..   
+000035d0: 207d 0a0a 2020 2020 7072 6f63 6573 7344   }..    processD
+000035e0: 6174 6128 6461 7461 2920 7b0a 2020 2020  ata(data) {.    
+000035f0: 2020 2020 7265 7475 726e 2064 6174 613b      return data;
+00003600: 0a20 2020 207d 0a0a 2020 2020 616d 494f  .    }..    amIO
+00003610: 6e41 4772 6964 5461 626c 6528 2920 7b0a  nAGridTable() {.
+00003620: 2020 2020 2020 2020 636f 6e73 7420 6f20          const o 
+00003630: 3d20 7468 6973 2e6f 7074 696f 6e73 3b0a  = this.options;.
+00003640: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00003650: 6f2e 6964 2e73 706c 6974 2827 5f27 292e  o.id.split('_').
+00003660: 6c65 6e67 7468 202d 2031 2920 3d3d 3d20  length - 1) === 
+00003670: 323b 0a20 2020 207d 0a0a 2020 2020 6765  2;.    }..    ge
+00003680: 7453 6563 7469 6f6e 2829 207b 0a20 2020  tSection() {.   
+00003690: 2020 2020 2072 6574 7572 6e20 2428 2723       return $('#
+000036a0: 2720 2b20 7468 6973 2e69 6429 3b0a 2020  ' + this.id);.  
+000036b0: 2020 7d0a 0a20 2020 2073 7461 7469 6320    }..    static 
+000036c0: 6861 6e64 6c65 5379 7374 656d 4576 656e  handleSystemEven
+000036d0: 7428 656c 656d 656e 742c 2074 7269 6767  t(element, trigg
+000036e0: 6572 4576 656e 744e 616d 652c 2066 696c  erEventName, fil
+000036f0: 7465 7253 656c 6563 746f 722c 2075 7064  terSelector, upd
+00003700: 6174 6556 616c 7565 203d 2074 7275 652c  ateValue = true,
+00003710: 2061 6c6c 6f77 4275 6262 6c69 6e67 5570   allowBubblingUp
+00003720: 203d 2066 616c 7365 2920 7b0a 2020 2020   = false) {.    
+00003730: 2020 2020 656c 656d 656e 742e 6f6e 2874      element.on(t
+00003740: 7269 6767 6572 4576 656e 744e 616d 652c  riggerEventName,
+00003750: 2066 696c 7465 7253 656c 6563 746f 722c   filterSelector,
+00003760: 2065 7665 6e74 203d 3e20 7b0a 2020 2020   event => {.    
+00003770: 2020 2020 2020 2020 5769 6467 6574 2e64          Widget.d
+00003780: 6f48 616e 646c 6553 7973 7465 6d45 7665  oHandleSystemEve
+00003790: 6e74 2824 2865 7665 6e74 2e63 7572 7265  nt($(event.curre
+000037a0: 6e74 5461 7267 6574 292c 2065 7665 6e74  ntTarget), event
+000037b0: 2c20 7570 6461 7465 5661 6c75 6529 3b0a  , updateValue);.
+000037c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000037d0: 7572 6e20 616c 6c6f 7742 7562 626c 696e  urn allowBubblin
+000037e0: 6755 703b 0a20 2020 2020 2020 207d 293b  gUp;.        });
+000037f0: 0a20 2020 207d 0a0a 2020 2020 7374 6174  .    }..    stat
+00003800: 6963 2064 6f48 616e 646c 6553 7973 7465  ic doHandleSyste
+00003810: 6d45 7665 6e74 2865 6c65 6d65 6e74 2c20  mEvent(element, 
+00003820: 6576 656e 742c 2075 7064 6174 6556 616c  event, updateVal
+00003830: 7565 203d 2074 7275 6529 207b 0a20 2020  ue = true) {.   
+00003840: 2020 2020 206c 6574 2061 203d 2065 6c65       let a = ele
+00003850: 6d65 6e74 2e64 6174 6128 2761 6374 696f  ment.data('actio
+00003860: 6e27 292c 2069 203d 2065 6c65 6d65 6e74  n'), i = element
+00003870: 2e64 6174 6128 2769 6427 292c 2073 6563  .data('id'), sec
+00003880: 7469 6f6e 203d 2065 6c65 6d65 6e74 2e63  tion = element.c
+00003890: 6c6f 7365 7374 2827 7365 6374 696f 6e27  losest('section'
+000038a0: 293b 0a0a 2020 2020 2020 2020 636f 6e73  );..        cons
+000038b0: 7420 6576 656e 744d 6170 4964 203d 2061  t eventMapId = a
+000038c0: 202b 2027 2e27 202b 2069 3b0a 0a20 2020   + '.' + i;..   
+000038d0: 2020 2020 2069 6620 2827 7269 6768 7463       if ('rightc
+000038e0: 6c69 636b 2720 3d3d 3d20 6129 207b 0a20  lick' === a) {. 
+000038f0: 2020 2020 2020 2020 2020 2057 6964 6765             Widge
+00003900: 7473 5b27 7269 6768 7463 6c69 636b 275d  ts['rightclick']
+00003910: 203d 2069 3b0a 2020 2020 2020 2020 7d0a   = i;.        }.
+00003920: 0a20 2020 2020 2020 2045 6c2e 626f 6479  .        El.body
+00003930: 2e74 7269 6767 6572 4861 6e64 6c65 7228  .triggerHandler(
+00003940: 6576 656e 744d 6170 4964 202b 2027 2e73  eventMapId + '.s
+00003950: 7461 7274 6564 2729 3b0a 0a20 2020 2020  tarted');..     
+00003960: 2020 2069 6620 2857 6964 6765 7473 5b69     if (Widgets[i
+00003970: 5d20 2626 2075 7064 6174 6556 616c 7565  ] && updateValue
+00003980: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00003990: 5769 6467 6574 735b 695d 5b61 5d20 3d20  Widgets[i][a] = 
+000039a0: 656c 656d 656e 742e 6461 7461 2829 3b0a  element.data();.
+000039b0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+000039c0: 2020 2063 6f6e 7374 2077 7269 7465 203d     const write =
+000039d0: 2073 6563 7469 6f6e 2e64 6174 6128 2777   section.data('w
+000039e0: 7269 7465 2729 2021 3d3d 2027 6f66 6627  rite') !== 'off'
+000039f0: 3b0a 0a20 2020 2020 2020 2057 6964 6765  ;..        Widge
+00003a00: 742e 6578 6563 7574 6545 7665 6e74 4d61  t.executeEventMa
+00003a10: 7041 6374 696f 6e73 2865 7665 6e74 4d61  pActions(eventMa
+00003a20: 7049 642c 2065 7665 6e74 2c20 656c 656d  pId, event, elem
+00003a30: 656e 742c 2077 7269 7465 293b 0a20 2020  ent, write);.   
+00003a40: 207d 0a0a 2020 2020 7374 6174 6963 2064   }..    static d
+00003a50: 6f48 616e 646c 6547 7269 6454 6162 6c65  oHandleGridTable
+00003a60: 5379 7374 656d 4576 656e 7428 656c 656d  SystemEvent(elem
+00003a70: 656e 742c 2065 7665 6e74 2c20 7570 6461  ent, event, upda
+00003a80: 7465 5661 6c75 6520 3d20 7472 7565 2920  teValue = true) 
+00003a90: 7b0a 2020 2020 2020 2020 6c65 7420 6120  {.        let a 
+00003aa0: 3d20 656c 656d 656e 742e 6461 7461 2827  = element.data('
+00003ab0: 6163 7469 6f6e 2729 2c20 6920 3d20 656c  action'), i = el
+00003ac0: 656d 656e 742e 6461 7461 2827 6964 2729  ement.data('id')
+00003ad0: 2c20 6964 5061 7274 7320 3d20 692e 7370  , idParts = i.sp
+00003ae0: 6c69 7428 275f 2729 2c0a 2020 2020 2020  lit('_'),.      
+00003af0: 2020 2020 2020 7365 6374 696f 6e20 3d20        section = 
+00003b00: 656c 656d 656e 742e 636c 6f73 6573 7428  element.closest(
+00003b10: 2773 6563 7469 6f6e 2729 3b0a 0a20 2020  'section');..   
+00003b20: 2020 2020 2063 6f6e 7374 2065 7665 6e74       const event
+00003b30: 4d61 7049 6420 3d20 6120 2b20 272e 2720  MapId = a + '.' 
+00003b40: 2b20 6964 5061 7274 735b 305d 202b 2027  + idParts[0] + '
+00003b50: 5f72 6f77 5f27 202b 2069 6450 6172 7473  _row_' + idParts
+00003b60: 5b32 5d2c 0a20 2020 2020 2020 2020 2020  [2],.           
+00003b70: 2063 6f6c 756d 6e45 7665 6e74 4d61 7049   columnEventMapI
+00003b80: 6420 3d20 6120 2b20 272e 2720 2b20 6964  d = a + '.' + id
+00003b90: 5061 7274 735b 305d 202b 2027 5f27 202b  Parts[0] + '_' +
+00003ba0: 2069 6450 6172 7473 5b31 5d20 2b20 275f   idParts[1] + '_
+00003bb0: 2720 2b20 6964 5061 7274 735b 325d 202b  ' + idParts[2] +
+00003bc0: 2027 5f27 202b 2073 6563 7469 6f6e 2e64   '_' + section.d
+00003bd0: 6174 6128 276f 7269 6769 6e61 6c69 6427  ata('originalid'
+00003be0: 293b 0a0a 2020 2020 2020 2020 456c 2e62  );..        El.b
+00003bf0: 6f64 792e 7472 6967 6765 7248 616e 646c  ody.triggerHandl
+00003c00: 6572 2865 7665 6e74 4d61 7049 6420 2b20  er(eventMapId + 
+00003c10: 272e 7374 6172 7465 6427 293b 0a20 2020  '.started');.   
+00003c20: 2020 2020 2045 6c2e 626f 6479 2e74 7269       El.body.tri
+00003c30: 6767 6572 4861 6e64 6c65 7228 636f 6c75  ggerHandler(colu
+00003c40: 6d6e 4576 656e 744d 6170 4964 202b 2027  mnEventMapId + '
+00003c50: 2e73 7461 7274 6564 2729 3b0a 0a20 2020  .started');..   
+00003c60: 2020 2020 2069 6620 2857 6964 6765 7473       if (Widgets
+00003c70: 5b69 5d20 2626 2075 7064 6174 6556 616c  [i] && updateVal
+00003c80: 7565 2920 7b0a 2020 2020 2020 2020 2020  ue) {.          
+00003c90: 2020 5769 6467 6574 735b 695d 5b61 5d20    Widgets[i][a] 
+00003ca0: 3d20 656c 656d 656e 742e 6461 7461 2829  = element.data()
+00003cb0: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
+00003cc0: 2020 2020 2063 6f6e 7374 2077 7269 7465       const write
+00003cd0: 203d 2073 6563 7469 6f6e 2e64 6174 6128   = section.data(
+00003ce0: 2777 7269 7465 2729 2021 3d3d 2027 6f66  'write') !== 'of
+00003cf0: 6627 3b0a 0a20 2020 2020 2020 2057 6964  f';..        Wid
+00003d00: 6765 742e 6578 6563 7574 6545 7665 6e74  get.executeEvent
+00003d10: 4d61 7041 6374 696f 6e73 2861 202b 2027  MapActions(a + '
+00003d20: 2e27 202b 2069 6450 6172 7473 5b30 5d2c  .' + idParts[0],
+00003d30: 2065 7665 6e74 2c20 656c 656d 656e 742c   event, element,
+00003d40: 2066 616c 7365 293b 0a20 2020 2020 2020   false);.       
+00003d50: 2057 6964 6765 742e 6578 6563 7574 6545   Widget.executeE
+00003d60: 7665 6e74 4d61 7041 6374 696f 6e73 2865  ventMapActions(e
+00003d70: 7665 6e74 4d61 7049 642c 2065 7665 6e74  ventMapId, event
+00003d80: 2c20 656c 656d 656e 742c 2077 7269 7465  , element, write
+00003d90: 293b 0a20 2020 2020 2020 2057 6964 6765  );.        Widge
+00003da0: 742e 6578 6563 7574 6545 7665 6e74 4d61  t.executeEventMa
+00003db0: 7041 6374 696f 6e73 2863 6f6c 756d 6e45  pActions(columnE
+00003dc0: 7665 6e74 4d61 7049 642c 2065 7665 6e74  ventMapId, event
+00003dd0: 2c20 656c 656d 656e 742c 2077 7269 7465  , element, write
+00003de0: 293b 0a20 2020 207d 0a0a 2020 2020 7374  );.    }..    st
+00003df0: 6174 6963 2065 7865 6375 7465 4576 656e  atic executeEven
+00003e00: 744d 6170 4163 7469 6f6e 7328 6576 656e  tMapActions(even
+00003e10: 744d 6170 4964 2c20 6576 656e 742c 2065  tMapId, event, e
+00003e20: 6c65 6d65 6e74 2c20 7772 6974 6520 3d20  lement, write = 
+00003e30: 7472 7565 2c20 2e2e 2e61 7267 7329 207b  true, ...args) {
+00003e40: 0a20 2020 2020 2020 204c 2865 7665 6e74  .        L(event
+00003e50: 4d61 7049 642c 2065 7665 6e74 2c20 656c  MapId, event, el
+00003e60: 656d 656e 742c 2061 7267 7329 3b0a 0a20  ement, args);.. 
+00003e70: 2020 2020 2020 206c 6574 2061 6374 696f         let actio
+00003e80: 6e73 203d 2045 7665 6e74 4d61 705b 6576  ns = EventMap[ev
+00003e90: 656e 744d 6170 4964 5d2c 2061 2c20 7772  entMapId], a, wr
+00003ea0: 6974 6552 6573 706f 6e73 6520 3d20 7472  iteResponse = tr
+00003eb0: 7565 3b0a 0a20 2020 2020 2020 2069 6620  ue;..        if 
+00003ec0: 2877 7269 7465 203d 3d3d 2074 7275 6529  (write === true)
+00003ed0: 207b 0a20 2020 2020 2020 2020 2020 2077   {.            w
+00003ee0: 7269 7465 5265 7370 6f6e 7365 203d 2051  riteResponse = Q
+00003ef0: 422e 7772 6974 6544 6174 6128 6576 656e  B.writeData(even
+00003f00: 744d 6170 4964 2c20 6576 656e 742c 2065  tMapId, event, e
+00003f10: 6c65 6d65 6e74 293b 0a20 2020 2020 2020  lement);.       
+00003f20: 207d 0a0a 2020 2020 2020 2020 6966 2028   }..        if (
+00003f30: 6163 7469 6f6e 7320 2626 2077 7269 7465  actions && write
+00003f40: 5265 7370 6f6e 7365 2021 3d3d 2066 616c  Response !== fal
+00003f50: 7365 2920 7b0a 2020 2020 2020 2020 2020  se) {.          
+00003f60: 2020 666f 7220 2861 206f 6620 6163 7469    for (a of acti
+00003f70: 6f6e 7329 207b 0a20 2020 2020 2020 2020  ons) {.         
+00003f80: 2020 2020 2020 2061 2e61 6374 696f 6e28         a.action(
+00003f90: 612e 6172 6775 6d65 6e74 2c20 6576 656e  a.argument, even
+00003fa0: 742c 2065 6c65 6d65 6e74 293b 0a20 2020  t, element);.   
+00003fb0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00003fc0: 2020 207d 0a20 2020 207d 0a0a 2020 2020     }.    }..    
+00003fd0: 6765 7420 6964 2829 207b 0a20 2020 2020  get id() {.     
+00003fe0: 2020 2072 6574 7572 6e20 7468 6973 2e6f     return this.o
+00003ff0: 7074 696f 6e73 2e69 643b 0a20 2020 207d  ptions.id;.    }
+00004000: 0a0a 2020 2020 6765 7420 7374 6174 6528  ..    get state(
+00004010: 2920 7b0a 2020 2020 2020 2020 7265 7475  ) {.        retu
+00004020: 726e 2057 6964 6765 7453 7461 7465 5b74  rn WidgetState[t
+00004030: 6869 732e 6964 5d20 7c7c 207b 7d3b 0a20  his.id] || {};. 
+00004040: 2020 207d 0a0a 2020 2020 7365 7420 7374     }..    set st
+00004050: 6174 6528 7374 6174 654f 626a 6563 7429  ate(stateObject)
+00004060: 207b 0a20 2020 2020 2020 2057 6964 6765   {.        Widge
+00004070: 7453 7461 7465 5b74 6869 732e 6964 5d20  tState[this.id] 
+00004080: 3d20 7374 6174 654f 626a 6563 743b 0a20  = stateObject;. 
+00004090: 2020 207d 0a0a 2020 2020 6765 7420 6e61     }..    get na
+000040a0: 6d65 2829 207b 0a20 2020 2020 2020 2072  me() {.        r
+000040b0: 6574 7572 6e20 7468 6973 2e63 6f6e 7374  eturn this.const
+000040c0: 7275 6374 6f72 2e6e 616d 653b 0a20 2020  ructor.name;.   
+000040d0: 207d 0a0a 2020 2020 7365 7420 6e61 6d65   }..    set name
+000040e0: 286e 2920 7b0a 2020 2020 2020 2020 7468  (n) {.        th
+000040f0: 726f 7720 6e65 7720 4572 726f 7228 2744  row new Error('D
+00004100: 6f6e 5c27 7420 6368 616e 6765 2074 6865  on\'t change the
+00004110: 2022 6e61 6d65 2220 7072 6f70 6572 7479   "name" property
+00004120: 206f 6e20 7468 6973 206f 626a 6563 7421   on this object!
+00004130: 2729 3b0a 2020 2020 7d0a 0a20 2020 2067  ');.    }..    g
+00004140: 6574 5265 616c 5661 6c75 6528 6b65 792c  etRealValue(key,
+00004150: 2064 6174 6120 3d20 7b7d 2c20 6465 6661   data = {}, defa
+00004160: 756c 7456 616c 203d 2027 272c 2064 6174  ultVal = '', dat
+00004170: 6150 7265 6669 7820 3d20 2727 2920 7b0a  aPrefix = '') {.
+00004180: 0a20 2020 2020 2020 2069 6620 2827 756e  .        if ('un
+00004190: 6465 6669 6e65 6427 2021 3d3d 2074 7970  defined' !== typ
+000041a0: 656f 6620 6461 7461 5b64 6174 6150 7265  eof data[dataPre
+000041b0: 6669 7820 2b20 6b65 795d 2920 7b0a 2020  fix + key]) {.  
+000041c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000041d0: 2064 6174 615b 6461 7461 5072 6566 6978   data[dataPrefix
+000041e0: 202b 206b 6579 5d3b 0a20 2020 2020 2020   + key];.       
+000041f0: 207d 0a0a 2020 2020 2020 2020 6966 2028   }..        if (
+00004200: 2775 6e64 6566 696e 6564 2720 213d 3d20  'undefined' !== 
+00004210: 7479 7065 6f66 2074 6869 732e 6f70 7469  typeof this.opti
+00004220: 6f6e 735b 6b65 795d 2920 7b0a 2020 2020  ons[key]) {.    
+00004230: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00004240: 6869 732e 6f70 7469 6f6e 735b 6b65 795d  his.options[key]
+00004250: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
+00004260: 2020 2020 2072 6574 7572 6e20 6465 6661       return defa
+00004270: 756c 7456 616c 3b0a 2020 2020 7d0a 0a20  ultVal;.    }.. 
+00004280: 2020 2067 6574 4874 6d6c 436f 6d70 6f6e     getHtmlCompon
+00004290: 656e 7453 7479 6c65 7341 7272 6179 286b  entStylesArray(k
+000042a0: 6579 2c20 6461 7461 203d 207b 7d29 207b  ey, data = {}) {
+000042b0: 0a20 2020 2020 2020 206c 6574 2073 7479  .        let sty
+000042c0: 6c65 734f 626a 203d 2074 6869 732e 6765  lesObj = this.ge
+000042d0: 7448 746d 6c43 6f6d 706f 6e65 6e74 5374  tHtmlComponentSt
+000042e0: 796c 6573 286b 6579 2c20 6461 7461 292c  yles(key, data),
+000042f0: 2073 7479 6c65 7320 3d20 5b5d 3b0a 2020   styles = [];.  
+00004300: 2020 2020 2020 666f 7220 2863 6f6e 7374        for (const
+00004310: 205b 6b65 792c 2076 616c 7565 5d20 6f66   [key, value] of
+00004320: 204f 626a 6563 742e 656e 7472 6965 7328   Object.entries(
+00004330: 7374 796c 6573 4f62 6a29 2920 7b0a 2020  stylesObj)) {.  
+00004340: 2020 2020 2020 2020 2020 7374 796c 6573            styles
+00004350: 2e70 7573 6828 6024 7b6b 6579 2e72 6570  .push(`${key.rep
+00004360: 6c61 6365 416c 6c28 275f 272c 2027 2d27  laceAll('_', '-'
+00004370: 297d 3a24 7b76 616c 7565 7d3b 6029 3b0a  )}:${value};`);.
+00004380: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00004390: 2020 7265 7475 726e 2073 7479 6c65 733b    return styles;
+000043a0: 0a20 2020 207d 0a0a 2020 2020 6765 7448  .    }..    getH
+000043b0: 746d 6c43 6f6d 706f 6e65 6e74 5374 796c  tmlComponentStyl
+000043c0: 6573 5374 7269 6e67 286b 6579 2c20 6461  esString(key, da
+000043d0: 7461 203d 207b 7d29 207b 0a20 2020 2020  ta = {}) {.     
+000043e0: 2020 2072 6574 7572 6e20 7468 6973 2e67     return this.g
+000043f0: 6574 4874 6d6c 436f 6d70 6f6e 656e 7453  etHtmlComponentS
+00004400: 7479 6c65 7341 7272 6179 286b 6579 2c20  tylesArray(key, 
+00004410: 6461 7461 292e 6a6f 696e 2827 2729 3b0a  data).join('');.
+00004420: 2020 2020 7d0a 0a20 2020 2067 6574 4874      }..    getHt
+00004430: 6d6c 436f 6d70 6f6e 656e 7453 7479 6c65  mlComponentStyle
+00004440: 7328 6b65 792c 2064 6174 6120 3d20 7b7d  s(key, data = {}
+00004450: 2920 7b0a 2020 2020 2020 2020 7265 7475  ) {.        retu
+00004460: 726e 2074 6869 732e 6765 7452 6561 6c56  rn this.getRealV
+00004470: 616c 7565 286b 6579 202b 2027 5374 796c  alue(key + 'Styl
+00004480: 6527 2c20 6461 7461 2c20 7b7d 293b 0a20  e', data, {});. 
+00004490: 2020 207d 0a0a 2020 2020 6765 7447 656e     }..    getGen
+000044a0: 6572 616c 5374 796c 6573 2864 6174 6120  eralStyles(data 
+000044b0: 3d20 7b7d 2c20 6465 6661 756c 7473 203d  = {}, defaults =
+000044c0: 207b 7d2c 2064 6174 6150 7265 6669 7820   {}, dataPrefix 
+000044d0: 3d20 2727 2920 7b0a 2020 2020 2020 2020  = '') {.        
+000044e0: 7265 7475 726e 205b 2e2e 2e74 6869 732e  return [...this.
+000044f0: 6765 7457 6964 7468 416e 6448 6569 6768  getWidthAndHeigh
+00004500: 7428 6461 7461 2c20 6465 6661 756c 7473  t(data, defaults
+00004510: 2c20 6461 7461 5072 6566 6978 292c 202e  , dataPrefix), .
+00004520: 2e2e 7468 6973 2e67 6574 5061 6464 696e  ..this.getPaddin
+00004530: 6773 2864 6174 612c 2064 6566 6175 6c74  gs(data, default
+00004540: 732c 2064 6174 6150 7265 6669 7829 2c20  s, dataPrefix), 
+00004550: 2e2e 2e74 6869 732e 6765 744d 6172 6769  ...this.getMargi
+00004560: 6e73 2864 6174 612c 2064 6566 6175 6c74  ns(data, default
+00004570: 732c 2064 6174 6150 7265 6669 7829 5d3b  s, dataPrefix)];
+00004580: 0a20 2020 207d 0a0a 2020 2020 7570 6461  .    }..    upda
+00004590: 7465 4874 6d6c 436f 6d70 6f6e 656e 7428  teHtmlComponent(
+000045a0: 6b65 792c 2064 6174 612c 2065 6c65 6d65  key, data, eleme
+000045b0: 6e74 203d 206e 756c 6c2c 2073 6563 7469  nt = null, secti
+000045c0: 6f6e 203d 206e 756c 6c29 207b 0a20 2020  on = null) {.   
+000045d0: 2020 2020 2069 6620 2865 6c65 6d65 6e74       if (element
+000045e0: 203d 3d3d 206e 756c 6c29 207b 0a20 2020   === null) {.   
+000045f0: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
+00004600: 203d 2073 6563 7469 6f6e 2e66 696e 6428   = section.find(
+00004610: 272e 2720 2b20 7468 6973 2e67 6574 4373  '.' + this.getCs
+00004620: 7350 7265 6669 7828 2920 2b20 272d 2720  sPrefix() + '-' 
+00004630: 2b20 6b65 7929 3b0a 2020 2020 2020 2020  + key);.        
+00004640: 7d0a 2020 2020 2020 2020 636f 6e73 7420  }.        const 
+00004650: 6b65 7953 7479 6c65 7320 3d20 7468 6973  keyStyles = this
+00004660: 2e67 6574 4874 6d6c 436f 6d70 6f6e 656e  .getHtmlComponen
+00004670: 7453 7479 6c65 7341 7272 6179 286b 6579  tStylesArray(key
+00004680: 2c20 6461 7461 293b 0a20 2020 2020 2020  , data);.       
+00004690: 2069 6620 286b 6579 5374 796c 6573 2e6c   if (keyStyles.l
+000046a0: 656e 6774 6820 3e20 3029 207b 0a20 2020  ength > 0) {.   
+000046b0: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
+000046c0: 2e61 7474 7228 2773 7479 6c65 272c 206b  .attr('style', k
+000046d0: 6579 5374 796c 6573 2e6a 6f69 6e28 2727  eyStyles.join(''
+000046e0: 2929 3b0a 2020 2020 2020 2020 7d0a 2020  ));.        }.  
+000046f0: 2020 7d0a 0a20 2020 2075 7064 6174 654d    }..    updateM
+00004700: 6561 7375 7265 7328 6d61 696e 2c20 6765  easures(main, ge
+00004710: 6e65 7261 6c53 7479 6c65 7329 207b 0a20  neralStyles) {. 
+00004720: 2020 2020 2020 206c 6574 2073 7479 6c65         let style
+00004730: 7320 3d20 6d61 696e 2e61 7474 7228 2773  s = main.attr('s
+00004740: 7479 6c65 2729 3b0a 2020 2020 2020 2020  tyle');.        
+00004750: 7374 796c 6573 202b 3d20 6765 6e65 7261  styles += genera
+00004760: 6c53 7479 6c65 732e 6a6f 696e 2827 2729  lStyles.join('')
+00004770: 3b0a 2020 2020 2020 2020 6d61 696e 2e61  ;.        main.a
+00004780: 7474 7228 2773 7479 6c65 272c 2073 7479  ttr('style', sty
+00004790: 6c65 7329 3b0a 2020 2020 7d0a 0a20 2020  les);.    }..   
+000047a0: 2067 6574 4373 7350 7265 6669 7828 2920   getCssPrefix() 
+000047b0: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
+000047c0: 2027 273b 0a20 2020 207d 0a0a 2020 2020   '';.    }..    
+000047d0: 6765 7457 6964 7468 416e 6448 6569 6768  getWidthAndHeigh
+000047e0: 7428 6461 7461 203d 207b 7d2c 2064 6566  t(data = {}, def
+000047f0: 6175 6c74 7320 3d20 7b7d 2c20 6461 7461  aults = {}, data
+00004800: 5072 6566 6978 203d 2027 2729 207b 0a20  Prefix = '') {. 
+00004810: 2020 2020 2020 2063 6f6e 7374 2073 203d         const s =
+00004820: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
+00004830: 2068 6569 6768 7420 3d20 7468 6973 2e67   height = this.g
+00004840: 6574 5265 616c 5661 6c75 6528 2768 6569  etRealValue('hei
+00004850: 6768 7427 2c20 6461 7461 2c20 6465 6661  ght', data, defa
+00004860: 756c 7473 2e68 6569 6768 742c 2064 6174  ults.height, dat
+00004870: 6150 7265 6669 7829 2c0a 2020 2020 2020  aPrefix),.      
+00004880: 2020 2020 2020 6d69 6e48 6569 6768 7420        minHeight 
+00004890: 3d20 7468 6973 2e67 6574 5265 616c 5661  = this.getRealVa
+000048a0: 6c75 6528 276d 696e 4865 6967 6874 272c  lue('minHeight',
+000048b0: 2064 6174 612c 2064 6566 6175 6c74 732e   data, defaults.
+000048c0: 6d69 6e48 6569 6768 742c 2064 6174 6150  minHeight, dataP
+000048d0: 7265 6669 7829 2c0a 2020 2020 2020 2020  refix),.        
+000048e0: 2020 2020 7769 6474 6820 3d20 7468 6973      width = this
+000048f0: 2e67 6574 5265 616c 5661 6c75 6528 2777  .getRealValue('w
+00004900: 6964 7468 272c 2064 6174 612c 2064 6566  idth', data, def
+00004910: 6175 6c74 732e 7769 6474 682c 2064 6174  aults.width, dat
+00004920: 6150 7265 6669 7829 2c0a 2020 2020 2020  aPrefix),.      
+00004930: 2020 2020 2020 6d69 6e57 6964 7468 203d        minWidth =
+00004940: 2074 6869 732e 6765 7452 6561 6c56 616c   this.getRealVal
+00004950: 7565 2827 6d69 6e57 6964 7468 272c 2064  ue('minWidth', d
+00004960: 6174 612c 2064 6566 6175 6c74 732e 6d69  ata, defaults.mi
+00004970: 6e57 6964 7468 2c20 6461 7461 5072 6566  nWidth, dataPref
+00004980: 6978 293b 0a0a 2020 2020 2020 2020 6865  ix);..        he
+00004990: 6967 6874 2026 2620 732e 7075 7368 2827  ight && s.push('
+000049a0: 6865 6967 6874 3a27 2c20 6865 6967 6874  height:', height
+000049b0: 2c20 6973 4e61 4e28 6865 6967 6874 2920  , isNaN(height) 
+000049c0: 3f20 273b 2720 3a20 2770 783b 2729 3b0a  ? ';' : 'px;');.
+000049d0: 2020 2020 2020 2020 6d69 6e48 6569 6768          minHeigh
+000049e0: 7420 2626 2073 2e70 7573 6828 276d 696e  t && s.push('min
+000049f0: 2d68 6569 6768 743a 272c 206d 696e 4865  -height:', minHe
+00004a00: 6967 6874 2c20 6973 4e61 4e28 6d69 6e48  ight, isNaN(minH
+00004a10: 6569 6768 7429 203f 2027 3b27 203a 2027  eight) ? ';' : '
+00004a20: 7078 3b27 293b 0a20 2020 2020 2020 2077  px;');.        w
+00004a30: 6964 7468 2026 2620 732e 7075 7368 2827  idth && s.push('
+00004a40: 7769 6474 683a 272c 2077 6964 7468 2c20  width:', width, 
+00004a50: 6973 4e61 4e28 7769 6474 6829 203f 2027  isNaN(width) ? '
+00004a60: 3b27 203a 2027 7078 3b27 293b 0a20 2020  ;' : 'px;');.   
+00004a70: 2020 2020 206d 696e 5769 6474 6820 2626       minWidth &&
+00004a80: 2073 2e70 7573 6828 276d 696e 2d77 6964   s.push('min-wid
+00004a90: 7468 3a27 2c20 6d69 6e57 6964 7468 2c20  th:', minWidth, 
+00004aa0: 6973 4e61 4e28 6d69 6e57 6964 7468 2920  isNaN(minWidth) 
+00004ab0: 3f20 273b 2720 3a20 2770 783b 2729 3b0a  ? ';' : 'px;');.
+00004ac0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004ad0: 733b 0a20 2020 207d 0a0a 2020 2020 6765  s;.    }..    ge
+00004ae0: 7450 6164 6469 6e67 7328 6461 7461 203d  tPaddings(data =
+00004af0: 207b 7d2c 2064 6566 6175 6c74 7320 3d20   {}, defaults = 
+00004b00: 7b7d 2c20 6461 7461 5072 6566 6978 203d  {}, dataPrefix =
+00004b10: 2027 2729 207b 0a20 2020 2020 2020 2063   '') {.        c
+00004b20: 6f6e 7374 2073 203d 205b 5d2c 0a20 2020  onst s = [],.   
+00004b30: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
+00004b40: 426f 7474 6f6d 203d 2074 6869 732e 6765  Bottom = this.ge
+00004b50: 7452 6561 6c56 616c 7565 2827 7061 6464  tRealValue('padd
+00004b60: 696e 6742 6f74 746f 6d27 2c20 6461 7461  ingBottom', data
+00004b70: 2c20 6465 6661 756c 7473 2e70 6164 6469  , defaults.paddi
+00004b80: 6e67 426f 7474 6f6d 2c20 6461 7461 5072  ngBottom, dataPr
+00004b90: 6566 6978 292c 0a20 2020 2020 2020 2020  efix),.         
+00004ba0: 2020 2070 6164 6469 6e67 4c65 6674 203d     paddingLeft =
+00004bb0: 2074 6869 732e 6765 7452 6561 6c56 616c   this.getRealVal
+00004bc0: 7565 2827 7061 6464 696e 674c 6566 7427  ue('paddingLeft'
+00004bd0: 2c20 6461 7461 2c20 6465 6661 756c 7473  , data, defaults
+00004be0: 2e70 6164 6469 6e67 4c65 6674 2c20 6461  .paddingLeft, da
+00004bf0: 7461 5072 6566 6978 292c 0a20 2020 2020  taPrefix),.     
+00004c00: 2020 2020 2020 2070 6164 6469 6e67 5269         paddingRi
+00004c10: 6768 7420 3d20 7468 6973 2e67 6574 5265  ght = this.getRe
+00004c20: 616c 5661 6c75 6528 2770 6164 6469 6e67  alValue('padding
+00004c30: 5269 6768 7427 2c20 6461 7461 2c20 6465  Right', data, de
+00004c40: 6661 756c 7473 2e70 6164 6469 6e67 5269  faults.paddingRi
+00004c50: 6768 742c 2064 6174 6150 7265 6669 7829  ght, dataPrefix)
+00004c60: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+00004c70: 6464 696e 6754 6f70 203d 2074 6869 732e  ddingTop = this.
+00004c80: 6765 7452 6561 6c56 616c 7565 2827 7061  getRealValue('pa
+00004c90: 6464 696e 6754 6f70 272c 2064 6174 612c  ddingTop', data,
+00004ca0: 2064 6566 6175 6c74 732e 7061 6464 696e   defaults.paddin
+00004cb0: 6754 6f70 2c20 6461 7461 5072 6566 6978  gTop, dataPrefix
+00004cc0: 293b 0a0a 2020 2020 2020 2020 7061 6464  );..        padd
+00004cd0: 696e 6754 6f70 2026 2620 732e 7075 7368  ingTop && s.push
+00004ce0: 2827 7061 6464 696e 672d 746f 703a 272c  ('padding-top:',
+00004cf0: 2070 6164 6469 6e67 546f 702c 2070 6164   paddingTop, pad
+00004d00: 6469 6e67 546f 7020 213d 3d20 2761 7574  dingTop !== 'aut
+00004d10: 6f27 2026 2620 2169 734e 614e 2870 6164  o' && !isNaN(pad
+00004d20: 6469 6e67 546f 7029 203f 2027 7078 3b27  dingTop) ? 'px;'
+00004d30: 203a 2027 3b27 293b 0a20 2020 2020 2020   : ';');.       
+00004d40: 2070 6164 6469 6e67 4c65 6674 2026 2620   paddingLeft && 
+00004d50: 732e 7075 7368 2827 7061 6464 696e 672d  s.push('padding-
+00004d60: 6c65 6674 3a27 2c20 7061 6464 696e 674c  left:', paddingL
+00004d70: 6566 742c 2070 6164 6469 6e67 4c65 6674  eft, paddingLeft
+00004d80: 2021 3d3d 2027 6175 746f 2720 2626 2021   !== 'auto' && !
+00004d90: 6973 4e61 4e28 7061 6464 696e 674c 6566  isNaN(paddingLef
+00004da0: 7429 203f 2027 7078 3b27 203a 2027 3b27  t) ? 'px;' : ';'
+00004db0: 293b 0a20 2020 2020 2020 2070 6164 6469  );.        paddi
+00004dc0: 6e67 5269 6768 7420 2626 2073 2e70 7573  ngRight && s.pus
+00004dd0: 6828 2770 6164 6469 6e67 2d72 6967 6874  h('padding-right
+00004de0: 3a27 2c20 7061 6464 696e 6752 6967 6874  :', paddingRight
+00004df0: 2c20 7061 6464 696e 6752 6967 6874 2021  , paddingRight !
+00004e00: 3d3d 2027 6175 746f 2720 2626 2021 6973  == 'auto' && !is
+00004e10: 4e61 4e28 7061 6464 696e 6752 6967 6874  NaN(paddingRight
+00004e20: 2920 3f20 2770 783b 2720 3a20 273b 2729  ) ? 'px;' : ';')
+00004e30: 3b0a 2020 2020 2020 2020 7061 6464 696e  ;.        paddin
+00004e40: 6742 6f74 746f 6d20 2626 2073 2e70 7573  gBottom && s.pus
+00004e50: 6828 2770 6164 6469 6e67 2d62 6f74 746f  h('padding-botto
+00004e60: 6d3a 272c 2070 6164 6469 6e67 426f 7474  m:', paddingBott
+00004e70: 6f6d 2c20 7061 6464 696e 6742 6f74 746f  om, paddingBotto
+00004e80: 6d20 213d 3d20 2761 7574 6f27 2026 2620  m !== 'auto' && 
+00004e90: 2169 734e 614e 2870 6164 6469 6e67 426f  !isNaN(paddingBo
+00004ea0: 7474 6f6d 2920 3f20 2770 783b 2720 3a20  ttom) ? 'px;' : 
+00004eb0: 273b 2729 3b0a 0a20 2020 2020 2020 2072  ';');..        r
+00004ec0: 6574 7572 6e20 733b 0a20 2020 207d 0a0a  eturn s;.    }..
+00004ed0: 2020 2020 6765 744d 6172 6769 6e73 2864      getMargins(d
+00004ee0: 6174 6120 3d20 7b7d 2c20 6465 6661 756c  ata = {}, defaul
+00004ef0: 7473 203d 207b 7d2c 2064 6174 6150 7265  ts = {}, dataPre
+00004f00: 6669 7820 3d20 2727 2920 7b0a 2020 2020  fix = '') {.    
+00004f10: 2020 2020 636f 6e73 7420 7320 3d20 5b5d      const s = []
+00004f20: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00004f30: 7267 696e 426f 7474 6f6d 203d 2074 6869  rginBottom = thi
+00004f40: 732e 6765 7452 6561 6c56 616c 7565 2827  s.getRealValue('
+00004f50: 6d61 7267 696e 426f 7474 6f6d 272c 2064  marginBottom', d
+00004f60: 6174 612c 2064 6566 6175 6c74 732e 6d61  ata, defaults.ma
+00004f70: 7267 696e 426f 7474 6f6d 2c20 6461 7461  rginBottom, data
+00004f80: 5072 6566 6978 292c 0a20 2020 2020 2020  Prefix),.       
+00004f90: 2020 2020 206d 6172 6769 6e4c 6566 7420       marginLeft 
+00004fa0: 3d20 7468 6973 2e67 6574 5265 616c 5661  = this.getRealVa
+00004fb0: 6c75 6528 276d 6172 6769 6e4c 6566 7427  lue('marginLeft'
+00004fc0: 2c20 6461 7461 2c20 6465 6661 756c 7473  , data, defaults
+00004fd0: 2e6d 6172 6769 6e4c 6566 742c 2064 6174  .marginLeft, dat
+00004fe0: 6150 7265 6669 7829 2c0a 2020 2020 2020  aPrefix),.      
+00004ff0: 2020 2020 2020 6d61 7267 696e 5269 6768        marginRigh
+00005000: 7420 3d20 7468 6973 2e67 6574 5265 616c  t = this.getReal
+00005010: 5661 6c75 6528 276d 6172 6769 6e52 6967  Value('marginRig
+00005020: 6874 272c 2064 6174 612c 2064 6566 6175  ht', data, defau
+00005030: 6c74 732e 6d61 7267 696e 5269 6768 742c  lts.marginRight,
+00005040: 2064 6174 6150 7265 6669 7829 2c0a 2020   dataPrefix),.  
+00005050: 2020 2020 2020 2020 2020 6d61 7267 696e            margin
+00005060: 546f 7020 3d20 7468 6973 2e67 6574 5265  Top = this.getRe
+00005070: 616c 5661 6c75 6528 276d 6172 6769 6e54  alValue('marginT
+00005080: 6f70 272c 2064 6174 612c 2064 6566 6175  op', data, defau
+00005090: 6c74 732e 6d61 7267 696e 546f 702c 2064  lts.marginTop, d
+000050a0: 6174 6150 7265 6669 7829 3b0a 0a20 2020  ataPrefix);..   
+000050b0: 2020 2020 206d 6172 6769 6e54 6f70 2026       marginTop &
+000050c0: 2620 732e 7075 7368 2827 6d61 7267 696e  & s.push('margin
+000050d0: 2d74 6f70 3a27 2c20 6d61 7267 696e 546f  -top:', marginTo
+000050e0: 702c 206d 6172 6769 6e54 6f70 2021 3d3d  p, marginTop !==
+000050f0: 2027 6175 746f 2720 2626 2021 6973 4e61   'auto' && !isNa
+00005100: 4e28 6d61 7267 696e 546f 7029 203f 2027  N(marginTop) ? '
+00005110: 7078 3b27 203a 2027 3b27 293b 0a20 2020  px;' : ';');.   
+00005120: 2020 2020 206d 6172 6769 6e4c 6566 7420       marginLeft 
+00005130: 2626 2073 2e70 7573 6828 276d 6172 6769  && s.push('margi
+00005140: 6e2d 6c65 6674 3a27 2c20 6d61 7267 696e  n-left:', margin
+00005150: 4c65 6674 2c20 6d61 7267 696e 4c65 6674  Left, marginLeft
+00005160: 2021 3d3d 2027 6175 746f 2720 2626 2021   !== 'auto' && !
+00005170: 6973 4e61 4e28 6d61 7267 696e 4c65 6674  isNaN(marginLeft
+00005180: 2920 3f20 2770 783b 2720 3a20 273b 2729  ) ? 'px;' : ';')
+00005190: 3b0a 2020 2020 2020 2020 6d61 7267 696e  ;.        margin
+000051a0: 5269 6768 7420 2626 2073 2e70 7573 6828  Right && s.push(
+000051b0: 276d 6172 6769 6e2d 7269 6768 743a 272c  'margin-right:',
+000051c0: 206d 6172 6769 6e52 6967 6874 2c20 6d61   marginRight, ma
+000051d0: 7267 696e 5269 6768 7420 213d 3d20 2761  rginRight !== 'a
+000051e0: 7574 6f27 2026 2620 2169 734e 614e 286d  uto' && !isNaN(m
+000051f0: 6172 6769 6e52 6967 6874 2920 3f20 2770  arginRight) ? 'p
+00005200: 783b 2720 3a20 273b 2729 3b0a 2020 2020  x;' : ';');.    
+00005210: 2020 2020 6d61 7267 696e 426f 7474 6f6d      marginBottom
+00005220: 2026 2620 732e 7075 7368 2827 6d61 7267   && s.push('marg
+00005230: 696e 2d62 6f74 746f 6d3a 272c 206d 6172  in-bottom:', mar
+00005240: 6769 6e42 6f74 746f 6d2c 206d 6172 6769  ginBottom, margi
+00005250: 6e42 6f74 746f 6d20 213d 3d20 2761 7574  nBottom !== 'aut
+00005260: 6f27 2026 2620 2169 734e 614e 286d 6172  o' && !isNaN(mar
+00005270: 6769 6e42 6f74 746f 6d29 203f 2027 7078  ginBottom) ? 'px
+00005280: 3b27 203a 2027 3b27 293b 0a0a 2020 2020  ;' : ';');..    
+00005290: 2020 2020 7265 7475 726e 2073 3b0a 2020      return s;.  
+000052a0: 2020 7d0a 0a20 2020 2067 6574 5769 6474    }..    getWidt
+000052b0: 6846 6f72 5365 6374 696f 6e28 6461 7461  hForSection(data
+000052c0: 203d 207b 7d2c 2064 6566 6175 6c74 7320   = {}, defaults 
+000052d0: 3d20 7b7d 2920 7b0a 2020 2020 2020 2020  = {}) {.        
+000052e0: 636f 6e73 7420 7320 3d20 5b5d 2c0a 2020  const s = [],.  
+000052f0: 2020 2020 2020 2020 2020 7769 6474 6820            width 
+00005300: 3d20 7468 6973 2e67 6574 5265 616c 5661  = this.getRealVa
+00005310: 6c75 6528 2777 6964 7468 272c 2064 6174  lue('width', dat
+00005320: 612c 2064 6566 6175 6c74 732e 7769 6474  a, defaults.widt
+00005330: 6829 2c0a 2020 2020 2020 2020 2020 2020  h),.            
+00005340: 6d69 6e48 6569 6768 7420 3d20 7468 6973  minHeight = this
+00005350: 2e67 6574 5265 616c 5661 6c75 6528 276d  .getRealValue('m
+00005360: 696e 4865 6967 6874 272c 2064 6174 612c  inHeight', data,
+00005370: 2064 6566 6175 6c74 732e 6d69 6e48 6569   defaults.minHei
+00005380: 6768 7429 2c0a 2020 2020 2020 2020 2020  ght),.          
+00005390: 2020 6d69 6e57 6964 7468 203d 2074 6869    minWidth = thi
+000053a0: 732e 6765 7452 6561 6c56 616c 7565 2827  s.getRealValue('
+000053b0: 6d69 6e57 6964 7468 272c 2064 6174 612c  minWidth', data,
+000053c0: 2064 6566 6175 6c74 732e 6d69 6e57 6964   defaults.minWid
+000053d0: 7468 293b 0a0a 2020 2020 2020 2020 6966  th);..        if
+000053e0: 2028 2169 734e 614e 2877 6964 7468 2929   (!isNaN(width))
+000053f0: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
+00005400: 6574 7572 6e20 5b5d 3b0a 2020 2020 2020  eturn [];.      
+00005410: 2020 7d0a 0a20 2020 2020 2020 2077 6964    }..        wid
+00005420: 7468 2026 2620 732e 7075 7368 2827 7769  th && s.push('wi
+00005430: 6474 683a 272c 2077 6964 7468 2c20 6973  dth:', width, is
+00005440: 4e61 4e28 7769 6474 6829 203f 2027 3b27  NaN(width) ? ';'
+00005450: 203a 2027 7078 3b27 293b 0a20 2020 2020   : 'px;');.     
+00005460: 2020 206d 696e 4865 6967 6874 2026 2620     minHeight && 
+00005470: 732e 7075 7368 2827 6d69 6e2d 6865 6967  s.push('min-heig
+00005480: 6874 3a27 2c20 6d69 6e48 6569 6768 742c  ht:', minHeight,
+00005490: 2069 734e 614e 286d 696e 4865 6967 6874   isNaN(minHeight
+000054a0: 2920 3f20 273b 2720 3a20 2770 783b 2729  ) ? ';' : 'px;')
+000054b0: 3b0a 2020 2020 2020 2020 6d69 6e57 6964  ;.        minWid
+000054c0: 7468 2026 2620 732e 7075 7368 2827 6d69  th && s.push('mi
+000054d0: 6e2d 7769 6474 683a 272c 206d 696e 5769  n-width:', minWi
+000054e0: 6474 682c 2069 734e 614e 286d 696e 5769  dth, isNaN(minWi
+000054f0: 6474 6829 203f 2027 3b27 203a 2027 7078  dth) ? ';' : 'px
+00005500: 3b27 293b 0a0a 2020 2020 2020 2020 7265  ;');..        re
+00005510: 7475 726e 2073 3b0a 2020 2020 7d0a 0a20  turn s;.    }.. 
+00005520: 2020 2067 6574 4865 6967 6874 466f 7253     getHeightForS
+00005530: 6563 7469 6f6e 2864 6174 6120 3d20 7b7d  ection(data = {}
+00005540: 2c20 6465 6661 756c 7473 203d 207b 7d29  , defaults = {})
+00005550: 207b 0a20 2020 2020 2020 2063 6f6e 7374   {.        const
+00005560: 2073 203d 205b 5d2c 2068 6569 6768 7420   s = [], height 
+00005570: 3d20 7468 6973 2e67 6574 5265 616c 5661  = this.getRealVa
+00005580: 6c75 6528 2768 6569 6768 7427 2c20 6461  lue('height', da
+00005590: 7461 2c20 6465 6661 756c 7473 2e68 6569  ta, defaults.hei
+000055a0: 6768 7429 3b0a 0a20 2020 2020 2020 2069  ght);..        i
+000055b0: 6620 2821 6973 4e61 4e28 6865 6967 6874  f (!isNaN(height
+000055c0: 2929 207b 0a20 2020 2020 2020 2020 2020  )) {.           
+000055d0: 2072 6574 7572 6e20 5b5d 3b0a 2020 2020   return [];.    
+000055e0: 2020 2020 7d0a 0a20 2020 2020 2020 2068      }..        h
+000055f0: 6569 6768 7420 2626 2073 2e70 7573 6828  eight && s.push(
+00005600: 2768 6569 6768 743a 272c 2068 6569 6768  'height:', heigh
+00005610: 742c 2069 734e 614e 2868 6569 6768 7429  t, isNaN(height)
+00005620: 203f 2027 3b27 203a 2027 7078 3b27 293b   ? ';' : 'px;');
+00005630: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005640: 2073 3b0a 2020 2020 7d0a 0a20 2020 2073   s;.    }..    s
+00005650: 7461 7469 6320 6765 7450 6572 6365 6e74  tatic getPercent
+00005660: 4f72 5069 7865 6c28 7661 6c75 6529 207b  OrPixel(value) {
+00005670: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005680: 6973 4e61 4e28 7661 6c75 6529 203f 2076  isNaN(value) ? v
+00005690: 616c 7565 203a 2076 616c 7565 202b 2027  alue : value + '
+000056a0: 7078 273b 0a20 2020 207d 0a0a 2020 2020  px';.    }..    
+000056b0: 7374 6174 6963 2073 6574 536b 696e 2865  static setSkin(e
+000056c0: 6c65 6d65 6e74 2c20 736b 696e 5072 6566  lement, skinPref
+000056d0: 6978 2c20 6e65 7753 6b69 6e29 207b 0a20  ix, newSkin) {. 
+000056e0: 2020 2020 2020 2069 6620 2821 656c 656d         if (!elem
+000056f0: 656e 742e 6861 7343 6c61 7373 2873 6b69  ent.hasClass(ski
+00005700: 6e50 7265 6669 7820 2b20 6e65 7753 6b69  nPrefix + newSki
+00005710: 6e29 2920 7b0a 2020 2020 2020 2020 2020  n)) {.          
+00005720: 2020 6966 2028 656c 656d 656e 742e 6174    if (element.at
+00005730: 7472 2827 636c 6173 7327 2929 207b 0a20  tr('class')) {. 
+00005740: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00005750: 6574 2072 6573 756c 742c 2063 6c61 7373  et result, class
+00005760: 5769 7468 6f75 7453 6b69 6e2c 206f 7269  WithoutSkin, ori
+00005770: 6769 6e61 6c43 6c61 7373 203d 2065 6c65  ginalClass = ele
+00005780: 6d65 6e74 2e61 7474 7228 2763 6c61 7373  ment.attr('class
+00005790: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+000057a0: 2020 2020 2020 2020 7320 3d20 6f72 6967          s = orig
+000057b0: 696e 616c 436c 6173 732e 696e 6465 784f  inalClass.indexO
+000057c0: 6628 736b 696e 5072 6566 6978 293b 0a20  f(skinPrefix);. 
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000057e0: 6c61 7373 5769 7468 6f75 7453 6b69 6e20  lassWithoutSkin 
+000057f0: 3d20 7320 213d 3d20 2d31 203f 206f 7269  = s !== -1 ? ori
+00005800: 6769 6e61 6c43 6c61 7373 2e73 7562 7374  ginalClass.subst
+00005810: 7269 6e67 2830 2c20 7320 2d20 3129 203a  ring(0, s - 1) :
+00005820: 206f 7269 6769 6e61 6c43 6c61 7373 3b0a   originalClass;.
+00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005840: 7265 7375 6c74 203d 2063 6c61 7373 5769  result = classWi
+00005850: 7468 6f75 7453 6b69 6e2e 7370 6c69 7428  thoutSkin.split(
+00005860: 2720 2729 3b0a 2020 2020 2020 2020 2020  ' ');.          
+00005870: 2020 2020 2020 7265 7375 6c74 2e70 7573        result.pus
+00005880: 6828 736b 696e 5072 6566 6978 202b 206e  h(skinPrefix + n
+00005890: 6577 536b 696e 293b 0a20 2020 2020 2020  ewSkin);.       
+000058a0: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
+000058b0: 2e61 7474 7228 2763 6c61 7373 272c 2072  .attr('class', r
+000058c0: 6573 756c 742e 6a6f 696e 2827 2027 2929  esult.join(' '))
+000058d0: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+000058e0: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
+000058f0: 0a20 2020 2073 7461 7469 6320 7265 6d6f  .    static remo
+00005900: 7665 5374 796c 6528 656c 656d 656e 742c  veStyle(element,
+00005910: 2073 7479 6c65 4e61 6d65 2920 7b0a 2020   styleName) {.  
+00005920: 2020 2020 2020 6c65 7420 7320 3d20 656c        let s = el
+00005930: 656d 656e 742e 7072 6f70 2827 7374 796c  ement.prop('styl
+00005940: 6527 293b 0a20 2020 2020 2020 2073 2026  e');.        s &
+00005950: 2620 732e 7265 6d6f 7665 5072 6f70 6572  & s.removeProper
+00005960: 7479 2873 7479 6c65 4e61 6d65 293b 0a20  ty(styleName);. 
+00005970: 2020 207d 0a0a 2020 2020 7374 6174 6963     }..    static
+00005980: 2073 6574 4f72 5265 6d6f 7665 5374 796c   setOrRemoveStyl
+00005990: 6528 656c 656d 656e 742c 2073 7479 6c65  e(element, style
+000059a0: 4e61 6d65 2c20 7661 6c75 6529 207b 0a20  Name, value) {. 
+000059b0: 2020 2020 2020 2076 616c 7565 203f 2065         value ? e
+000059c0: 6c65 6d65 6e74 2e63 7373 2873 7479 6c65  lement.css(style
+000059d0: 4e61 6d65 2c20 7661 6c75 6529 203a 2057  Name, value) : W
+000059e0: 6964 6765 742e 7265 6d6f 7665 5374 796c  idget.removeStyl
+000059f0: 6528 656c 656d 656e 742c 2073 7479 6c65  e(element, style
+00005a00: 4e61 6d65 293b 0a20 2020 207d 0a0a 2020  Name);.    }..  
+00005a10: 2020 7374 6174 6963 2073 6574 4f72 5265    static setOrRe
+00005a20: 6d6f 7665 4d65 6173 7572 6528 656c 656d  moveMeasure(elem
+00005a30: 656e 742c 206d 6561 7375 7265 4e61 6d65  ent, measureName
+00005a40: 2c20 7661 6c75 6529 207b 0a20 2020 2020  , value) {.     
+00005a50: 2020 2057 6964 6765 742e 7365 744f 7252     Widget.setOrR
+00005a60: 656d 6f76 6553 7479 6c65 2865 6c65 6d65  emoveStyle(eleme
+00005a70: 6e74 2c20 6d65 6173 7572 654e 616d 652c  nt, measureName,
+00005a80: 2076 616c 7565 203f 2057 6964 6765 742e   value ? Widget.
+00005a90: 6765 7450 6572 6365 6e74 4f72 5069 7865  getPercentOrPixe
+00005aa0: 6c28 7661 6c75 6529 203a 2066 616c 7365  l(value) : false
+00005ab0: 293b 0a20 2020 207d 0a0a 2020 2020 7374  );.    }..    st
+00005ac0: 6174 6963 2061 6464 4f72 5265 6d6f 7665  atic addOrRemove
+00005ad0: 436c 6173 7328 656c 656d 656e 742c 2063  Class(element, c
+00005ae0: 6c61 7373 4e61 6d65 2c20 6164 6429 207b  lassName, add) {
+00005af0: 0a20 2020 2020 2020 2061 6464 203f 2021  .        add ? !
+00005b00: 656c 656d 656e 742e 6861 7343 6c61 7373  element.hasClass
+00005b10: 2863 6c61 7373 4e61 6d65 2920 2626 2065  (className) && e
+00005b20: 6c65 6d65 6e74 2e61 6464 436c 6173 7328  lement.addClass(
+00005b30: 636c 6173 734e 616d 6529 203a 2065 6c65  className) : ele
+00005b40: 6d65 6e74 2e72 656d 6f76 6543 6c61 7373  ment.removeClass
+00005b50: 2863 6c61 7373 4e61 6d65 293b 0a20 2020  (className);.   
+00005b60: 207d 0a7d                                 }.}
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/button.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/button.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/combo-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/container.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/container.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/datepicker.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/datepicker.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/default/ScrollTableWidget.json` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/default/ScrollTableWidget.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/dropbox.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/dropbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/gauge.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/gauge.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid-cell.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid-row.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid/grid.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid/grid.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/grid-table/grid-table.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/grid-table/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/histogram-combo-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/histogram-combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontal-bar-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontal-bar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontal-table.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontal-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/image.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/image.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/line-area-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/line-area-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/line-scatter-combo.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/line-scatter-combo.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/loader.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/loader.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/page.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/page.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/pie-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/pie-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/pivot-table.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/pivot-table.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2288,15 +2288,15 @@
 
     saveContentCellValue() {
         let i = this.cellInput,
             p = i.parent(),
             url = "/api/v1/Cellsets('" + this.cellsetId + "')/Cells";
 
         let body = '{"Ordinal":' + this.getOrdinalOfCell(p) + ',"Value": \"' + Utils.convertValueToPost(i.val()) + '\"}';
-
+        //Todo add source
         Auth.getAjaxRequest(QB.getUrl(url), body, 'PATCH', this.id)
             .then(() => p.addClass('ok'))
             .fail(() => p.addClass('err'))
             .always(() => this.finishEditingContentCell());
     }
 
     finishEditingContentCell() {
```

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/popup.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/radar-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/radar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/scroll-table.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/scroll-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-bar.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-bar.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-control-item.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-control-item.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/segmented-control.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/segmented-control.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/simulation-panel-slider.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/simulation-panel-slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/simulation-panel.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/simulation-panel.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/slider.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/stacked-column-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/stacked-column-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/swipe.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/swipe.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/system-popup.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/system-popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/text.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/text.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/textarea.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/textarea.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/textbox.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/textbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/toggle.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/toggle.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/tornado-chart.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/tornado-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/vertical-line-box.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/vertical-line-box.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/js/widgets/water-fall.js` & `analogic-framework-4.1.9/analogic/static/assets/js/widgets/water-fall.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-button.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-button.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-container.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-container.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-datepicker.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-datepicker.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-dropbox.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-dropbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid-table.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-grid.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-grid.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-horizontal-table.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-horizontal-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-horizontalbarchart.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-horizontalbarchart.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-line-scatter-combo.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-line-scatter-combo.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-pivot-table.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-pivot-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-popup.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-popup.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-scrolltable.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-scrolltable.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-segmentedbar.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-segmentedbar.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-slider-touch.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-slider-touch.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-slider.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-text.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-text.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-textarea.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-textarea.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-textbox.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-textbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-toggle.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-toggle.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-tornado.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-tornado.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-vertical-line-box.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-vertical-line-box.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/css/ks-waterfall.css` & `analogic-framework-4.1.9/analogic/static/assets/skin/css/ks-waterfall.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.eot` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.svg` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.ttf` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/static/assets/skin/fonts/pivot.woff` & `analogic-framework-4.1.9/analogic/static/assets/skin/fonts/pivot.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/templates/authenticated.html` & `analogic-framework-4.1.9/analogic/templates/authenticated.html`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             <link href="{{ url_for(cnf.blueprint_static, filename='assets/skin/css/minified.css')}}?v={{ cnf.version }}" rel="stylesheet" type="text/css">
         {% else %}
             {% include 'css.html' %}
         {% endif %}
     </head>
     <body>
         {% if (cnf.useMinifiedAssets)%}
-            <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config.js')}}?v={{cnf.version}}"></script>
+            <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config' + cnf.get('auth_prov', '') + '.js')}}?v={{cnf.version}}"></script>
             <script src="{{ url_for('static', filename='assets/js/minified.js')}}?v={{ cnf.version }}" charset="UTF-8"></script>
             <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/minified.js')}}?v={{ cnf.version }}" charset="UTF-8"></script>
             <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/repository.js')}}')}}?v={{cnf.version}}"></script>
         {% else %}
             {% include 'javascripts.html' %}
         {% endif %}
     </body>
```

### Comparing `analogic-framework-4.1.8/analogic/templates/config.html` & `analogic-framework-4.1.9/analogic/templates/config.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 let app = {};
 app = {id: 0, isMobile: null, isTouched: false, url: {}};
 app.assetsUrl = '{{ url_for('static', filename='assets') }}';
 app.applicationAssetsUrl = '{{ url_for(cnf.blueprint_static, filename='assets') }}';
 app.tm1CellsetId = (cellsetId) => `Cellsets('${cellsetId}')?`;
 app.handled401 = false;
 app.pingTime = new Date().getTime();
-{% for key, value in cnf.items() if key not in exclude%}
+{% for key, value in cnf.items() if key not in exclude and not key.startswith('_')%}
     {% if value is string %}
         app['{{ key }}'] = '{{ value|safe }}';
     {% endif %}
 
     {% if value is integer %}
         app['{{ key }}'] = {{ value }};
     {% endif %}
```

### Comparing `analogic-framework-4.1.8/analogic/templates/css.html` & `analogic-framework-4.1.9/analogic/templates/css.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.8/analogic/templates/javascripts.html` & `analogic-framework-4.1.9/analogic/templates/javascripts.html`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.actual.min.js') }}"></script>
 <script src="{{ url_for('static', filename='assets/js/lib/Chart-2.9.3.min.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-datalabels.min.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-dragdata.min.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/lib/nouislider.min.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/lib/Sortable.min.js') }}?v={{ cnf.version }}"></script>
 
-<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config' + cnf.get('auth_prov','') + '.js') }}?v={{ cnf.version }}"></script>
 <!-- end libs -->
 
 <!-- framework -->
 <script src="{{ url_for('static', filename='assets/js/framework/app.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/framework/utils.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/framework/render.js') }}?v={{ cnf.version }}"></script>
 <script src="{{ url_for('static', filename='assets/js/framework/listener.js') }}?v={{ cnf.version }}"></script>
```

### Comparing `analogic-framework-4.1.8/analogic/templates/login.html` & `analogic-framework-4.1.9/analogic/templates/sso_error.html`

 * *Files 15% similar despite different names*

```diff
@@ -13,38 +13,25 @@
         <meta name="theme-color" content="#ffffff">
         <link href="{{ url_for('static', filename='assets/css/bootstrap-grid.min.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
         <link href="{{ url_for(cnf.blueprint_static, filename='assets/skin/css/ks-general.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
         <link href="{{ url_for('static', filename='assets/css/style.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
         <link href="{{ url_for('static', filename='assets/css/widgets/loader.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
     </head>
     <body>
-        <div class="main-content" style="padding-top: 100px;">
-            <form action="login" method="POST">
-                <div class="row">
-                    <div class="col-2 offset-5">
-                        <div class="form-row">
-                            <label>Username</label>
-                            <input name="username" type="text" class="widget-input textbox-widget" placeholder="Username">
-                        </div>
+           <div class="main-content" style="padding-top: 100px;">
+            <div class="row">
+                <div class="col-2 offset-5">
+                    <div class="form-row">
+                        <div style="color:red;">ERROR!</div>
                     </div>
                 </div>
-                <div class="row">
-                    <div class="col-2 offset-5">
-                        <div class="form-row">
-                            <label>Password</label>
-                            <input name="password" type="password" class="widget-input textbox-widget" placeholder="Password">
-                        </div>
+            </div>
+            <div class="row">
+                <div class="col-2 offset-5">
+                    <div class="form-row">
+                        <div style="color:red;">{{ msg }}</div>
                     </div>
                 </div>
-                <div class="row margin-bottom-row">
-                    <div class="col-2 offset-5">
-                        <div class="row">
-                            <div class="col-12">
-                                <input type="submit" class="widget-btn button-widget-url" value="Login" style="width: 100%;"/>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </form>
+            </div>
         </div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,2 @@
-Username[username            ]
-Password[********************]
-[Login]
+ERROR!
+{{ msg }}
```

### Comparing `analogic-framework-4.1.8/analogic/templates/redirect.html` & `analogic-framework-4.1.9/analogic/templates/redirect.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,11 +2,11 @@
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">
         <title>{{ cnf.projectName }}</title>
     </head>
     <body>
         <script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery-3.6.0.min.js')}}"></script>
-        <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config.js')}}?v={{cnf.version}}"></script>
+        <script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config' + cnf.get('auth_prov', '') + '.js')}}?v={{cnf.version}}"></script>
         <script src="{{ url_for('static', filename='assets/js/framework/redirect.js')}}"></script>
     </body>
 </html>
```

### Comparing `analogic-framework-4.1.8/analogic_framework.egg-info/SOURCES.txt` & `analogic-framework-4.1.9/analogic_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+analogic/__cli__.py
 analogic/__init__.py
 analogic/analogic.py
 analogic/analogic_tm1_service.py
 analogic/authentication_provider.py
 analogic/cam.py
 analogic/camsecure.py
-analogic/condition.py
+analogic/cli.py
 analogic/core_endpoints.py
 analogic/email.py
 analogic/endpoint.py
 analogic/exceptions.py
 analogic/loader.py
+analogic/logged_in_signal.py
 analogic/logging.json
 analogic/loginbasic.py
 analogic/logincam.py
+analogic/multi_authentication_provider.py
+analogic/multi_authentication_provider_interface.py
+analogic/multi_setting.py
 analogic/nologin.py
 analogic/pivot.py
+analogic/session_handler.py
 analogic/setting.py
 analogic/task.py
 analogic/version.config
 analogic/version.py
 analogic/static/assets/css/bootstrap-grid.min.css
 analogic/static/assets/css/bootstrap-grid.min.css.map
 analogic/static/assets/css/style.css
@@ -225,9 +231,10 @@
 analogic/templates/login.html
 analogic/templates/redirect.html
 analogic/templates/sso_error.html
 analogic/templates/unauthorized.html
 analogic_framework.egg-info/PKG-INFO
 analogic_framework.egg-info/SOURCES.txt
 analogic_framework.egg-info/dependency_links.txt
+analogic_framework.egg-info/entry_points.txt
 analogic_framework.egg-info/requires.txt
 analogic_framework.egg-info/top_level.txt
```

### Comparing `analogic-framework-4.1.8/setup.py` & `analogic-framework-4.1.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,10 +27,14 @@
         'PyYaml==6.0',
         'xlrd==2.0.1',
         'openpyxl==3.0.10',
         'Flask-Cors==3.0.10',
         'json_logging==1.3.0',
         'flask_talisman',
         'Flask-APScheduler==1.12.4',
-        'orjson==3.8.6'
+        'orjson==3.8.6',
+        'rich==13.3.5'
     ],
+    entry_points={
+        'console_scripts': ['analogic=analogic.__cli__:main'],
+    }
 )
```

