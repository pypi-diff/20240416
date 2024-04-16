# Comparing `tmp/red_web_dashboard-1.2.0.tar.gz` & `tmp/red_web_dashboard-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_web_dashboard-1.2.0.tar", last modified: Sun Apr 14 22:44:29 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.3.0.tar", last modified: Mon Apr 15 21:21:38 2024, max compression
```

## Comparing `red_web_dashboard-1.2.0.tar` & `red_web_dashboard-1.3.0.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.722575 red_web_dashboard-1.2.0/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42435 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.718575 red_web_dashboard-1.2.0/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.730575 red_web_dashboard-1.2.0/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/simplemde.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.738575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.738575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.742575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.750575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.750575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.754575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.722575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.762575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    28545 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    30505 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27213 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.648548 red_web_dashboard-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-15 21:21:38.648548 red_web_dashboard-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 21:21:38.000000 red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.592547 red_web_dashboard-1.3.0/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.592547 red_web_dashboard-1.3.0/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.592547 red_web_dashboard-1.3.0/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42844 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.596547 red_web_dashboard-1.3.0/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.588547 red_web_dashboard-1.3.0/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.600547 red_web_dashboard-1.3.0/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.604547 red_web_dashboard-1.3.0/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/css/simplemde.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.604547 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.604547 red_web_dashboard-1.3.0/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.608547 red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.608547 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.608547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.616547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.624547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.624547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.628547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.632547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.636547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.588547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.636547 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.640548 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.640548 red_web_dashboard-1.3.0/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.640548 red_web_dashboard-1.3.0/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    29014 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:21:38.644548 red_web_dashboard-1.3.0/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26892 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-15 21:21:38.648548 red_web_dashboard-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 21:21:34.000000 red_web_dashboard-1.3.0/setup.py
```

### Comparing `red_web_dashboard-1.2.0/LICENSE` & `red_web_dashboard-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/PKG-INFO` & `red_web_dashboard-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.2.0
+Version: 1.3.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.2.0/README.md` & `red_web_dashboard-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.2.0
+Version: 1.3.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.3.0/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/pyproject.toml` & `red_web_dashboard-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/__main__.py` & `red_web_dashboard-1.3.0/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/app.py` & `red_web_dashboard-1.3.0/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/base/routes.py` & `red_web_dashboard-1.3.0/reddash/app/base/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,17 @@
             result = await get_result(app, requeststr)
             if result["status"] == 0:
                 flash(_("Successfully left the guild."), category="success")
                 return redirect(url_for("base_blueprint.dashboard"))
             else:
                 flash(_("Failed to leave the guild."), category="danger")
                 return redirect(request.url)
+        elif leave_guild_form.submit.data and leave_guild_form.errors:
+            for field_name, error_messages in leave_guild_form.errors.items():
+                flash(f"{field_name}: {' '.join(error_messages)}", category="warning")
     else:
         leave_guild_form = None
 
     return {"guild": guild, "leave_guild_form": leave_guild_form}
 
 
 class PrefixesCheck:
@@ -353,44 +356,44 @@
         self.use_bot_color.default = self.use_bot_color.checked = guild["settings"]["use_bot_color"]
         self.fuzzy.default = self.fuzzy.checked = guild["settings"]["fuzzy"]
         self.delete_delay.default = guild["settings"]["delete_delay"]
         self.locale.default = guild["settings"]["locale"]
         self.regional_format.default = guild["settings"]["regional_format"]
 
     bot_nickname: wtforms.StringField = wtforms.StringField(
-        _("Bot Nickname"), validators=[wtforms.validators.Length(max=32)]
+        _("Bot Nickname:"), validators=[wtforms.validators.Length(max=32)]
     )
     prefixes: wtforms.StringField = wtforms.StringField(
-        _("Prefixes"), validators=[wtforms.validators.Optional(), PrefixesCheck()]
+        _("Prefixes:"), validators=[wtforms.validators.Optional(), PrefixesCheck()]
     )
     admin_roles: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
-        _("Admin Roles"), choices=[]
+        _("Admin Roles:"), choices=[]
     )
     mod_roles: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
-        _("Mod Roles"), choices=[]
+        _("Mod Roles:"), choices=[]
     )
     ignored: wtforms.BooleanField = wtforms.BooleanField(_("Ignore commands in this guild."))
     disabled_commands: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
-        _("Disabled Commands"), choices=[]
+        _("Disabled Commands:"), choices=[]
     )
     embeds: wtforms.BooleanField = wtforms.BooleanField(_("Use embeds in responses."))
-    use_bot_color: wtforms.BooleanField = wtforms.BooleanField(_("Use bot color in embeds."))
+    use_bot_color: wtforms.BooleanField = wtforms.BooleanField(_("Use bot set color in embeds."))
     fuzzy: wtforms.BooleanField = wtforms.BooleanField(_("Use fuzzy command search."))
     delete_delay: wtforms.IntegerField = wtforms.IntegerField(
-        _("Delay before deleting invocation messages (-1 to disable)"),
+        _("Delay before deleting invocation messages (-1 to disable):"),
         validators=[
             wtforms.validators.DataRequired(),
             wtforms.validators.NumberRange(min=-1, max=60),
         ],
     )
     locale: wtforms.StringField = wtforms.StringField(
-        _("Locale"), validators=[wtforms.validators.DataRequired(), BabelCheck(check_reset=True)]
+        _("Locale:"), validators=[wtforms.validators.DataRequired(), BabelCheck(check_reset=True)]
     )
     regional_format: wtforms.StringField = wtforms.StringField(
-        _("Region"), validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)]
+        _("Regional Format:"), validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 class MarkdownTextAreaField(wtforms.TextAreaField):
     def __call__(
         self,
@@ -543,14 +546,16 @@
             if result["status"] == 0:
                 flash(_("Successfully saved the modifications."), category="success")
             else:
                 for error in result["errors"]:
                     flash(error, category="warning")
                 flash(_("Failed to save the modifications."), category="danger")
             return redirect(request.url)
+    else:
+        custom_commands_form = None
 
     guild_settings_form: GuildSettingsForm = GuildSettingsForm(guild=return_guild["guild"])
     if (
         guild_settings_form.validate_on_submit()
         and return_guild["guild"]["settings"]["edit_permission"]
     ):
         requeststr = {
@@ -668,21 +673,21 @@
 
 class DiscordProfileForm(FlaskForm):
     def __init__(self) -> None:
         super().__init__(prefix="bot_profile_form_")
         self.username.default = app.variables["bot"]["name"]
         self.description.default = app.variables["bot"]["profile_description"]
 
-    avatar: FileField = FileField(_("Avatar"))
-    avatar_choice: wtforms.HiddenField = wtforms.HiddenField(_("Avatar choice"), default="keep")
+    avatar: FileField = FileField()
+    avatar_choice: wtforms.HiddenField = wtforms.HiddenField(default="keep")
     username: wtforms.StringField = wtforms.StringField(
-        _("Username"), validators=[wtforms.validators.Length(max=32)]
+        _("Username:"), validators=[wtforms.validators.Length(max=32)]
     )
     description: MarkdownTextAreaField = MarkdownTextAreaField(
-        _("Description"), validators=[wtforms.validators.Length(max=1024)]
+        _("Description:"), validators=[wtforms.validators.Length(max=1024)]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 class DashboardSettingsForm(FlaskForm):
     def __init__(self, settings: typing.Dict[str, typing.Any]) -> None:
         super().__init__(prefix="dashboard_settings_form_")
@@ -695,36 +700,36 @@
         self.default_background_theme.default = settings["default_background_theme"]
         self.default_sidebar_theme.default = settings["default_sidebar_theme"]
         self.disabled_third_parties.choices = [
             (third_party, third_party) for third_party in app.variables["third_parties"]
         ]
         self.disabled_third_parties.default = settings["disabled_third_parties"].copy()
 
-    title: wtforms.StringField = wtforms.StringField(_("Title"))
-    icon: wtforms.StringField = wtforms.StringField(_("Icon"))
-    website_description: wtforms.StringField = wtforms.StringField(_("Website Short Description"))
-    description: MarkdownTextAreaField = MarkdownTextAreaField(_("Description"))
-    support_server: wtforms.URLField = wtforms.URLField(_("Support Server"))
+    title: wtforms.StringField = wtforms.StringField(_("Title:"))
+    icon: wtforms.StringField = wtforms.StringField(_("Icon:"))
+    website_description: wtforms.StringField = wtforms.StringField(_("Website (Short) Description:"))
+    description: MarkdownTextAreaField = MarkdownTextAreaField(_("Description:"))
+    support_server: wtforms.URLField = wtforms.URLField(_("Support Server URL:"))
     default_color: wtforms.SelectField = wtforms.SelectField(
-        _("Default Color"),
+        _("Default Color:"),
         choices=[(color, color.capitalize()) for color in AVAILABLE_COLORS],
         validators=[wtforms.validators.DataRequired()],
     )
     default_background_theme: wtforms.SelectField = wtforms.SelectField(
-        _("Default Background Theme"),
+        _("Default Background Theme:"),
         choices=[("light", "Light"), ("dark", "Dark")],
         validators=[wtforms.validators.DataRequired()],
     )
     default_sidebar_theme: wtforms.SelectField = wtforms.SelectField(
-        _("Default Sidebar Theme"),
+        _("Default Sidebar Theme:"),
         choices=[("light", "Light"), ("dark", "Dark")],
         validators=[wtforms.validators.DataRequired()],
     )
     disabled_third_parties: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
-        _("Disabled Third Parties"), choices=[]
+        _("Disabled Third Parties:"), choices=[]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 class BotSettingsForm(FlaskForm):
     def __init__(self, settings: typing.Dict[str, typing.Any]) -> None:
         super().__init__(prefix="bot_settings_form_")
@@ -762,46 +767,46 @@
         self.invite_commands_scope.default = self.invite_commands_scope.checked = settings["invite_commands_scope"]
         self.invite_perms.validators.append(wtforms.validators.NumberRange(min=0, max=app.variables["constants"]["MAX_DISCORD_PERMISSIONS_VALUE"]))
         self.invite_perms.default = settings["invite_perms"]
         self.locale.default = settings["locale"]
         self.regional_format.default = settings["regional_format"]
 
     prefixes: wtforms.StringField = wtforms.StringField(
-        _("Prefixes"), validators=[wtforms.validators.DataRequired(), PrefixesCheck()]
+        _("Prefixes:"), validators=[wtforms.validators.DataRequired(), PrefixesCheck()]
     )
     invoke_error_msg: wtforms.StringField = wtforms.StringField(
-        _("Invoke Error Message"), validators=[wtforms.validators.Length(max=1000)]
+        _("Invoke Error Message:"), validators=[wtforms.validators.Length(max=1000)]
     )
     disabled_commands: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
-        _("Disabled Commands"), choices=[]
+        _("Disabled Commands:"), choices=[]
     )
     disabled_command_msg: wtforms.StringField = wtforms.StringField(_("Disabled Command Message"))
     description: wtforms.StringField = wtforms.StringField(
-        _("Description"), validators=[wtforms.validators.Length(max=250)]
+        _("Description:"), validators=[wtforms.validators.Length(max=250)]
     )
     custom_info: MarkdownTextAreaField = MarkdownTextAreaField(
-        _("Custom Info"), validators=[wtforms.validators.Length(max=1024)]
+        _("Custom Info:"), validators=[wtforms.validators.Length(max=1024)]
     )
-    embeds: wtforms.BooleanField = wtforms.BooleanField(_("Use Embeds"))
-    color: wtforms.ColorField = wtforms.ColorField(_("Color"))
-    fuzzy: wtforms.BooleanField = wtforms.BooleanField(_("Use Fuzzy"))
-    use_buttons: wtforms.BooleanField = wtforms.BooleanField(_("Use Buttons"))
-    invite_public: wtforms.BooleanField = wtforms.BooleanField(_("Invite Public"))
-    invite_commands_scope: wtforms.BooleanField = wtforms.BooleanField(_("Invite Commands Scope"))
+    embeds: wtforms.BooleanField = wtforms.BooleanField(_("Use Embeds in commands responses."))
+    color: wtforms.ColorField = wtforms.ColorField(_("Embeds Color:"))
+    fuzzy: wtforms.BooleanField = wtforms.BooleanField(_("Use Fuzzy Search when command invokation."))
+    use_buttons: wtforms.BooleanField = wtforms.BooleanField(_("Use Buttons instead of Reactions."))
+    invite_public: wtforms.BooleanField = wtforms.BooleanField(_("Make the invite public."))
+    invite_commands_scope: wtforms.BooleanField = wtforms.BooleanField(_("Use the Commands Scope in the invite."))
     invite_perms: wtforms.IntegerField = wtforms.IntegerField(
-        _("Invite Permissions (0 for nothing)"),
+        _("Invite Permissions (0 for nothing):"),
         validators=[
             wtforms.validators.DataRequired(),
         ],
     )
     locale: wtforms.StringField = wtforms.StringField(
-        _("Locale"), validators=[wtforms.validators.DataRequired(), BabelCheck()]
+        _("Locale:"), validators=[wtforms.validators.DataRequired(), BabelCheck()]
     )
     regional_format: wtforms.StringField = wtforms.StringField(
-        _("Regional Format"),
+        _("Regional Format:"),
         validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)],
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 @blueprint.route("/admin/<page>", methods=("GET", "POST"))
 @blueprint.route("/admin", methods=("GET", "POST"))
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/login/routes.py` & `red_web_dashboard-1.3.0/reddash/app/login/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/pagination.py` & `red_web_dashboard-1.3.0/reddash/app/pagination.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.3.0/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.3.0/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.3.0/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.3.0/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.3.0/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.3.0/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.3.0/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.3.0/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.3.0/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.3.0/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.3.0/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.3.0/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/tasks_manager.py` & `red_web_dashboard-1.3.0/reddash/app/tasks_manager.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.3.0/reddash/app/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.3.0/reddash/app/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.3.0/reddash/app/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.3.0/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.3.0/reddash/app/templates/errors/custom.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.3.0/reddash/app/templates/includes/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.3.0/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.3.0/reddash/app/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.3.0/reddash/app/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.3.0/reddash/app/templates/includes/sidenav.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="/">
         <img src="{{ variables["bot"]["avatar"] }}" class="navbar-brand-img border-radius-sm h-100" alt="main_logo">
         <span class="ms-1 text-dark font-weight-bold">{{ variables["bot"]["name"] }} {{ _("Dashboard") }}</span>
       </a>
     </div>
-    <hr class="horizontal dark mt-0">
+    <hr class="horizontal dark mt-0" style="height: 1px;">
     <div class="collapse navbar-collapse w-auto" style="height: 58%;" id="sidenav-collapse-main">
       <ul class="navbar-nav">
         {% for item in variables["sidebar"] %}
           <li class="{{ "active" if item["active"] else "" }}">
             <a class="nav-link{{ " active" if item["active"] else "" }}" href="{{ item["url"] }}"{{ ' target="blank"' if item["is_http"] }}{{ " data-scroll" if not item["active"] else "" }}>
               <div class="icon icon-shape icon-sm border-radius-md text-center me-2 d-flex align-items-center justify-content-center">
                 <i class="{{ item["icon"] }} text-primary text-lg opacity-10" style="margin-bottom: 5px;"></i>
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.3.0/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,19 @@
      <style>
        .dropzone {
          border: 1px solid #d2d6da;
        }
      </style>
      <link href="https://cdn.jsdelivr.net/npm/flatpickr/dist/flatpickr.min.css" rel="stylesheet" />
      <link href="https://cdn.jsdelivr.net/npm/choices.js/public/assets/styles/choices.min.css" rel="stylesheet" />
+     <style>
+      .choices:not([data-type*=select-one]) .choices__item:not(.choices__item--choice) {
+        background-color: #2dce89 !important;
+      }
+     </style>
      <link href="https://pagination.js.org/dist/2.6.0/pagination.css" rel="stylesheet" />
  
      <!-- Specific CSS goes HERE -->
      {% block stylesheets %}{% endblock %}
    </head>
  
    <body class="g-sidenav-show bg-gray-100">
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.3.0/reddash/app/templates/layouts/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,19 @@
     <style>
       .dropzone {
         border: 1px solid #d2d6da;
       }
     </style>
     <link href="https://cdn.jsdelivr.net/npm/flatpickr/dist/flatpickr.min.css" rel="stylesheet" />
     <link href="https://cdn.jsdelivr.net/npm/choices.js/public/assets/styles/choices.min.css" rel="stylesheet" />
+    <style>
+      .choices:not([data-type*=select-one]) .choices__item:not(.choices__item--choice) {
+        background-color: #2dce89 !important;
+      }
+    </style>
     <link href="https://pagination.js.org/dist/2.6.0/pagination.css" rel="stylesheet" />
 
     <!-- Specific CSS goes HERE -->
     {% block stylesheets %}{% endblock %}
   </head>
 
   <body class="g-sidenav-show bg-gray-100">
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/admin.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% extends "layouts/base.html" %}
-{% import "bootstrap/wtf.html" as wtf %}
 
 {% block title %}
   {{ _("Admin") }}
 {% endblock %}
 
 {% block stylesheets %}
     <style>
@@ -129,67 +128,67 @@
                                 </div>
                             </div>
                             <div class="mt-4">
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ dashboard_settings_form.hidden_tag() }}
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Title:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.title.label.text }}</label>
                                             {{ dashboard_settings_form.title(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Icon:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.icon.label.text }}</label>
                                             {{ dashboard_settings_form.icon(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Website Short Description:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.website_description.label.text }}</label>
                                             {{ dashboard_settings_form.website_description(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Description:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.description.label.text }}</label>
                                             {{ dashboard_settings_form.description(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Support Server URL:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.support_server.label.text }}</label>
                                             {{ dashboard_settings_form.support_server(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Default Color:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.default_color.label.text }}</label>
                                             {{ dashboard_settings_form.default_color(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="row mb-1">
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ _("Default Background Theme:") }}</label>
+                                                <label class="form-group-label">{{ dashboard_settings_form.default_background_theme.label.text }}</label>
                                                 {{ dashboard_settings_form.default_background_theme(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ _("Default SideBar Theme:") }}</label>
+                                                <label class="form-group-label">{{ dashboard_settings_form.default_sidebar_theme.label.text }}</label>
                                                 {{ dashboard_settings_form.default_sidebar_theme(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Disabled Third Parties:") }}</label>
+                                            <label class="form-group-label">{{ dashboard_settings_form.disabled_third_parties.label.text }}</label>
                                             {{ dashboard_settings_form.disabled_third_parties(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="text-center">
                                         {{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
                                     </div>
                                 </form>
@@ -209,75 +208,75 @@
                                 </div>
                             </div>
                             <div class="mt-4">
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ bot_settings_form.hidden_tag() }}
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Prefixes:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.prefixes.label.text }}</label>
                                             {{ bot_settings_form.prefixes(class="form-control form-control-default select-choices") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Invoke Error Message:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.invoke_error_msg.label.text }}</label>
                                             {{ bot_settings_form.invoke_error_msg(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Disabled Commands:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.disabled_commands.label.text }}</label>
                                             {{ bot_settings_form.disabled_commands(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Disabled Command Message:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.disabled_command_msg.label.text }}</label>
                                             {{ bot_settings_form.disabled_command_msg(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Description:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.description.label.text }}</label>
                                             {{ bot_settings_form.description(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Custom Info:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.custom_info.label.text }}</label>
                                             {{ bot_settings_form.custom_info(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="row mb-1">
                                         <div class="col-sm-6">
                                             <div class="form-check form-switch ps-0">
                                                 {{ bot_settings_form.embeds(class="form-check-input ms-0", type="checkbox") }}
                                                 <label class="form-check-label">{{ bot_settings_form.embeds.label.text }}</label>
                                             </div>
                                         </div>
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ _("Bot Color:") }}</label>
+                                                <label class="form-group-label">{{ bot_settings_form.color.label.text }}</label>
                                                 {{ bot_settings_form.color(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                     </div>
                                     <div class="row mb-1">
                                         <div class="col-sm-6">
                                             <div class="form-check form-switch ps-0">
                                                 {{ bot_settings_form.fuzzy(class="form-check-input ms-0", type="checkbox") }}
                                                 <label class="form-check-label">{{ bot_settings_form.fuzzy.label.text }}</label>
                                             </div>
                                         </div>
                                         <div class="col-sm-6">
                                             <div class="form-check form-switch ps-0">
                                                 {{ bot_settings_form.use_buttons(class="form-check-input ms-0", type="checkbox") }}
-                                                <label class="form-check-label">{{ _("Use Buttons instead of Reactions") }}</label>
+                                                <label class="form-check-label">{{ bot_settings_form.use_buttons.label.text }}</label>
                                             </div>
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="row mb-1">
                                         <div class="col-sm-6">
                                             <div class="form-check form-switch ps-0">
@@ -290,29 +289,29 @@
                                                 {{ bot_settings_form.invite_commands_scope(class="form-check-input ms-0", type="checkbox") }}
                                                 <label class="form-check-label">{{ bot_settings_form.invite_commands_scope.label.text }}</label>
                                             </div>
                                         </div>
                                     </div>
                                     <div class="mb-3">
                                         <div class="form-group">
-                                            <label class="form-group-label">{{ _("Invite Permissions:") }}</label>
+                                            <label class="form-group-label">{{ bot_settings_form.invite_perms.label.text }}</label>
                                             {{ bot_settings_form.invite_perms(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="row mb-1">
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ _("Locale:") }}</label>
+                                                <label class="form-group-label">{{ bot_settings_form.locale.label.text }}</label>
                                                 {{ bot_settings_form.locale(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ _("Regional Format:") }}</label>
+                                                <label class="form-group-label">{{ bot_settings_form.regional_format.label.text }}</label>
                                                 {{ bot_settings_form.regional_format(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                     </div>
                                     <div class="text-center">
                                         {{ bot_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
                                     </div>
@@ -349,21 +348,21 @@
                             <div class="text-center">
                                 <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "default"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["default_avatar"] }}"); this.style.display = "none"; this.parentElement.children[1].style.display = "";'>{{ _("Use default") }}</a>
                                 <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "keep"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["avatar"] }}"); this.style.display = "none"; this.parentElement.children[0].style.display = "";' style="display: none; margin-left: 8px;">{{ _("Keep current") }}</a>
                             </div>
                         </div>
                         <div class="mb-3">
                             <div class="form-group">
-                                <label class="form-group-label">{{ _("Username:") }}</label>
+                                <label class="form-group-label">{{ bot_profile_form.username.label.text }}</label>
                                 {{ bot_profile_form.username(class="form-control form-control-default") }}
                             </div>
                         </div>
                         <div class="mb-3">
                             <div class="form-group">
-                                <label class="form-group-label">{{ _("Description:") }}</label>
+                                <label class="form-group-label">{{ bot_profile_form.description.label.text }}</label>
                                 {{ bot_profile_form.description(class="form-control form-control-default") }}
                             </div>
                         </div>
                     </div>
                     <div class="modal-footer">
                         <a class="btn btn-secondary" data-dismiss="modal">{{ _("Fermer") }}</a>
                         {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-success btn-md w-30 mt-2 mb-4") }}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "layouts/base.html" %} {% import "bootstrap/wtf.html" as wtf %} {%
-block title %} {{ _("Admin") }} {% endblock %} {% block stylesheets %}
+{% extends "layouts/base.html" %} {% block title %} {{ _("Admin") }} {%
+endblock %} {% block stylesheets %}
 {% endblock %} {% block content %}
 }" class="shadow-sm border-radius-lg" />
 {{{{ vvaarriiaabblleess[[""bboott""]][[""nnaammee""]] }}}}
 **** {{{{ __((""OOwwnneedd bbyy"")) }}}} {{{{ vvaarriiaabblleess[[""bboott""]][[""oowwnneerr""]] }}}} ****
     * }show active{% endif %}" id="overview-tab" data-toggle="pill"
       href="#overview" role="tab" aria-controls="overview" aria-
       selected="true"> {{ _("Overview") }}
@@ -31,88 +31,95 @@
 btn-md my-4 mb-2", onclick="return confirmRefreshSessions(event);") }}
 {{ _("This will log out all active users and require them to re-authenticate,
 including website administrators.") }}
 }show active{% endif %}" id="dashboard-settings" role="tabpanel" aria-
 labelledby="dashboard-settings-tab">
 ********** {{{{ __((""DDaasshhbbooaarrdd SSeettttiinnggss"")) }}}} **********
 {{ dashboard_settings_form.hidden_tag() }}
-{{ _("Title:") }} {{ dashboard_settings_form.title(class="form-control form-
-control-default") }}
-{{ _("Icon:") }} {{ dashboard_settings_form.icon(class="form-control form-
-control-default") }}
-{{ _("Website Short Description:") }} {
+{{ dashboard_settings_form.title.label.text }} {{ dashboard_settings_form.title
+(class="form-control form-control-default") }}
+{{ dashboard_settings_form.icon.label.text }} {{ dashboard_settings_form.icon
+(class="form-control form-control-default") }}
+{{ dashboard_settings_form.website_description.label.text }} {
 { dashboard_settings_form.website_description(class="form-control form-control-
 default") }}
-{{ _("Description:") }} {{ dashboard_settings_form.description(class="form-
-control form-control-default") }}
-{{ _("Support Server URL:") }} {{ dashboard_settings_form.support_server
-(class="form-control form-control-default") }}
+{{ dashboard_settings_form.description.label.text }} {
+{ dashboard_settings_form.description(class="form-control form-control-
+default") }}
+{{ dashboard_settings_form.support_server.label.text }} {
+{ dashboard_settings_form.support_server(class="form-control form-control-
+default") }}
 ===============================================================================
-{{ _("Default Color:") }} {{ dashboard_settings_form.default_color(class="form-
-control form-control-default") }}
-{{ _("Default Background Theme:") }} {
+{{ dashboard_settings_form.default_color.label.text }} {
+{ dashboard_settings_form.default_color(class="form-control form-control-
+default") }}
+{{ dashboard_settings_form.default_background_theme.label.text }} {
 { dashboard_settings_form.default_background_theme(class="form-control form-
 control-default") }}
-{{ _("Default SideBar Theme:") }} {
+{{ dashboard_settings_form.default_sidebar_theme.label.text }} {
 { dashboard_settings_form.default_sidebar_theme(class="form-control form-
 control-default") }}
 ===============================================================================
-{{ _("Disabled Third Parties:") }} {
+{{ dashboard_settings_form.disabled_third_parties.label.text }} {
 { dashboard_settings_form.disabled_third_parties(class="form-control form-
 control-default") }}
 {{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-
 100 my-4 mb-2") }}
 }show active{% endif %}" id="bot-settings" role="tabpanel" aria-
 labelledby="bot-settings-tab">
 ********** {{{{ __((""BBoott SSeettttiinnggss"")) }}}} **********
 {{ bot_settings_form.hidden_tag() }}
-{{ _("Prefixes:") }} {{ bot_settings_form.prefixes(class="form-control form-
-control-default select-choices") }}
-{{ _("Invoke Error Message:") }} {{ bot_settings_form.invoke_error_msg
-(class="form-control form-control-default") }}
+{{ bot_settings_form.prefixes.label.text }} {{ bot_settings_form.prefixes
+(class="form-control form-control-default select-choices") }}
+{{ bot_settings_form.invoke_error_msg.label.text }} {
+{ bot_settings_form.invoke_error_msg(class="form-control form-control-default")
+}}
+===============================================================================
+{{ bot_settings_form.disabled_commands.label.text }} {
+{ bot_settings_form.disabled_commands(class="form-control form-control-
+default") }}
+{{ bot_settings_form.disabled_command_msg.label.text }} {
+{ bot_settings_form.disabled_command_msg(class="form-control form-control-
+default") }}
 ===============================================================================
-{{ _("Disabled Commands:") }} {{ bot_settings_form.disabled_commands
+{{ bot_settings_form.description.label.text }} {{ bot_settings_form.description
 (class="form-control form-control-default") }}
-{{ _("Disabled Command Message:") }} {{ bot_settings_form.disabled_command_msg
+{{ bot_settings_form.custom_info.label.text }} {{ bot_settings_form.custom_info
 (class="form-control form-control-default") }}
-===============================================================================
-{{ _("Description:") }} {{ bot_settings_form.description(class="form-control
-form-control-default") }}
-{{ _("Custom Info:") }} {{ bot_settings_form.custom_info(class="form-control
-form-control-default") }}
 {{ bot_settings_form.embeds(class="form-check-input ms-0", type="checkbox") }}
 {{ bot_settings_form.embeds.label.text }}
-{{ _("Bot Color:") }} {{ bot_settings_form.color(class="form-control form-
-control-default") }}
+{{ bot_settings_form.color.label.text }} {{ bot_settings_form.color
+(class="form-control form-control-default") }}
 {{ bot_settings_form.fuzzy(class="form-check-input ms-0", type="checkbox") }} {
 { bot_settings_form.fuzzy.label.text }}
 {{ bot_settings_form.use_buttons(class="form-check-input ms-0",
-type="checkbox") }} {{ _("Use Buttons instead of Reactions") }}
+type="checkbox") }} {{ bot_settings_form.use_buttons.label.text }}
 ===============================================================================
 {{ bot_settings_form.invite_public(class="form-check-input ms-0",
 type="checkbox") }} {{ bot_settings_form.invite_public.label.text }}
 {{ bot_settings_form.invite_commands_scope(class="form-check-input ms-0",
 type="checkbox") }} {{ bot_settings_form.invite_commands_scope.label.text }}
-{{ _("Invite Permissions:") }} {{ bot_settings_form.invite_perms(class="form-
-control form-control-default") }}
+{{ bot_settings_form.invite_perms.label.text }} {
+{ bot_settings_form.invite_perms(class="form-control form-control-default") }}
 ===============================================================================
-{{ _("Locale:") }} {{ bot_settings_form.locale(class="form-control form-
-control-default") }}
-{{ _("Regional Format:") }} {{ bot_settings_form.regional_format(class="form-
-control form-control-default") }}
+{{ bot_settings_form.locale.label.text }} {{ bot_settings_form.locale
+(class="form-control form-control-default") }}
+{{ bot_settings_form.regional_format.label.text }} {
+{ bot_settings_form.regional_format(class="form-control form-control-default")
+}}
 {{ bot_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100
 my-4 mb-2") }}
 **** {{{{ __((""EEddiitt DDiissccoorrdd BBoott PPrrooffiillee"")) }}}} ****
 ×
 {{ bot_profile_form.hidden_tag() }}
 }" />
 {{ bot_profile_form.avatar(class="file-upload", accept="image/png, image/jpg,
 image/jpeg, image/gif", onchange="readURL(this);", style="display: none;") }}
 _{_{_ ___(_"_U_s_e_ _d_e_f_a_u_l_t_"_)_ _}_} _{_{_ ___(_"_K_e_e_p_ _c_u_r_r_e_n_t_"_)_ _}_}
-{{ _("Username:") }} {{ bot_profile_form.username(class="form-control form-
-control-default") }}
-{{ _("Description:") }} {{ bot_profile_form.description(class="form-control
-form-control-default") }}
+{{ bot_profile_form.username.label.text }} {{ bot_profile_form.username
+(class="form-control form-control-default") }}
+{{ bot_profile_form.description.label.text }} {{ bot_profile_form.description
+(class="form-control form-control-default") }}
 {{ _("Fermer") }} {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-
 success btn-md w-30 mt-2 mb-4") }}
 {% endblock %} {% block javascripts %}
 {% endblock %}
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/commands.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/credits.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/dashboard.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard_guild.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/dashboard_guild.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% extends "layouts/base.html" %}
-{% import "bootstrap/wtf.html" as wtf %}
 
 {% block title %}
   {{ _("Guild") }} {{ guild.name }}
 {% endblock %}
 
 {% block stylesheets %}{% endblock %}
 
@@ -161,46 +160,46 @@
                                         </div>
                                     </div>
                                     <div class="mt-4">
                                         <form action="" method="POST" role="form" enctype="multipart/form-data">
                                             {{ guild_settings_form.hidden_tag() }}
                                             <div class="mb-3">
                                                 <div class="form-group">
-                                                    <label class="form-group-label">{{ _("Bot Nickname:") }}</label>
+                                                    <label class="form-group-label">{{ guild_settings_form.bot_nickname.label.text }}</label>
                                                     {{ guild_settings_form.bot_nickname(class="form-control form-control-default") }}
                                                 </div>
                                             </div>
                                             <div class="mb-3">
                                                 <div class="form-group">
-                                                    <label class="form-group-label">{{ _("Prefixes:") }}</label>
+                                                    <label class="form-group-label">{{ guild_settings_form.prefixes.label.text }}</label>
                                                     {{ guild_settings_form.prefixes(class="form-control form-control-default select-choices") }}
                                                 </div>
                                             </div>
                                             <div class="mb-3">
                                                 <div class="form-group">
-                                                    <label class="form-group-label">{{ _("Admin Roles:") }}</label>
+                                                    <label class="form-group-label">{{ guild_settings_form.admin_roles.label.text }}</label>
                                                     {{ guild_settings_form.admin_roles(class="form-control form-control-default") }}
                                                 </div>
                                             </div>
                                             <div class="mb-3">
                                                 <div class="form-group">
-                                                    <label class="form-group-label">{{ _("Mod Roles:") }}</label>
+                                                    <label class="form-group-label">{{ guild_settings_form.mod_roles.label.text }}</label>
                                                     {{ guild_settings_form.mod_roles(class="form-control form-control-default") }}
                                                 </div>
                                             </div>
                                             <hr class="horizontal dark" />
                                             <div class="mb-3">
                                                 <div class="form-check form-switch ps-0">
                                                     {{ guild_settings_form.ignored(class="form-check-input ms-0", type="checkbox") }}
                                                     <label class="form-check-label">{{ guild_settings_form.ignored.label.text }}</label>
                                                 </div>
                                             </div>
                                             <div class="mb-3">
                                                 <div class="form-group">
-                                                    <label class="form-group-label">{{ _("Disabled Commands:") }}</label>
+                                                    <label class="form-group-label">{{ guild_settings_form.disabled_commands.label.text }}</label>
                                                     {{ guild_settings_form.disabled_commands(class="form-control form-control-default") }}
                                                 </div>
                                             </div>
                                             <hr class="horizontal dark" />
                                             <div class="row mb-1">
                                                 <div class="col-sm-6">
                                                     <div class="form-check form-switch ps-0">
@@ -220,30 +219,30 @@
                                                     <div class="form-check form-switch ps-0">
                                                         {{ guild_settings_form.fuzzy(class="form-check-input ms-0", type="checkbox") }}
                                                         <label class="form-check-label">{{ guild_settings_form.fuzzy.label.text }}</label>
                                                     </div>
                                                 </div>
                                                 <div class="col-sm-6">
                                                     <div class="form-group">
-                                                        <label class="form-group-label">{{ _("Delay before deleting invocation messages (-1 to disable):") }}</label>
+                                                        <label class="form-group-label">{{ guild_settings_form.delete_delay.label.text }}</label>
                                                         {{ guild_settings_form.delete_delay(class="form-control form-control-default") }}
                                                     </div>
                                                 </div>
                                             </div>
                                             <hr class="horizontal dark" />
                                             <div class="row mb-1">
                                                 <div class="col-sm-6">
                                                     <div class="form-group">
-                                                        <label class="form-group-label">{{ _("Locale:") }}</label>
+                                                        <label class="form-group-label">{{ guild_settings_form.locale.label.text }}</label>
                                                         {{ guild_settings_form.locale(class="form-control form-control-default") }}
                                                     </div>
                                                 </div>
                                                 <div class="col-sm-6">
                                                     <div class="form-group">
-                                                        <label class="form-group-label">{{ _("Regional Format:") }}</label>
+                                                        <label class="form-group-label">{{ guild_settings_form.regional_format.label.text }}</label>
                                                         {{ guild_settings_form.regional_format(class="form-control form-control-default") }}
                                                     </div>
                                                 </div>
                                             </div>
                                             <div class="text-center">
                                                 {{ guild_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
                                             </div>
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/guild_profile.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/login/login.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% extends "layouts/base.html" %}
-{% import "bootstrap/wtf.html" as wtf %}
 
 {% block title %}
   {{ _("Login") }}
 {% endblock %}
 
 {% block stylesheets %}{% endblock %}
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_party.html` & `red_web_dashboard-1.3.0/reddash/app/templates/pages/third_parties/third_party.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% extends "layouts/base.html" %}
-{% import "bootstrap/wtf.html" as wtf %}
 
 {% block title %}
   {{ _("Third Party") }} {{ third_party }}{% if guild %} - {{ guild.name }}{% endif %}
 {% endblock %}
 
 {% block stylesheets %}{% endblock %}
 
@@ -51,15 +50,15 @@
                                                 {% endif %}
                                             {% else %}
                                                 <h2 class="card-title"><a href="{{ url_for("third_parties_blueprint.third_parties", third_party=name) }}">🔙 {{ name }}</a></h2>
                                             {% endif %}
                                         </div>
                                     </div>
                                 </div>
-                                <div class="container mt-4 d-flex">
+                                <div class="container mt-4">
                                     {{ source_content|safe }}
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-{% extends "layouts/base.html" %} {% import "bootstrap/wtf.html" as wtf %} {%
-block title %} {{ _("Third Party") }} {{ third_party }}{% if guild %} - {
-{ guild.name }}{% endif %} {% endblock %} {% block stylesheets %}{% endblock %}
-{% block content %}
+{% extends "layouts/base.html" %} {% block title %} {{ _("Third Party") }} {
+{ third_party }}{% if guild %} - {{ guild.name }}{% endif %} {% endblock %} {%
+block stylesheets %}{% endblock %} {% block content %}
 {% if guild and not fullscreen %} {% include "pages/guild_profile.html" %} {%
 endif %}
 % if guild and not fullscreen %} class="col-md-8 mt-4"{% endif %}> {% if guild
 and not fullscreen %}
     * }" class="nav-link"> {{ _("Overview") }}
 }}" class="nav-link"> {{ _("Settings") }}
 }}" class="nav-link show active" id="third-parties-tab"> {{ _("Third Parties")
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/third_parties/routes.py` & `red_web_dashboard-1.3.0/reddash/app/third_parties/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from reddash.app.app import app
 
-from flask import abort, flash, jsonify, redirect, render_template, render_template_string, url_for, request, session
+from flask import abort, flash, jsonify, redirect, render_template, render_template_string, url_for, request, session, g
 from flask_babel import _
 from flask_login import current_user, login_required
 from flask_login import login_url as make_login_url
 from pygments import highlight
 from pygments.formatters import HtmlFormatter
 from pygments.lexers import Python3TracebackLexer, get_lexer_by_name
 
+import base64
+
 from ..base.routes import get_guild, get_third_parties
 from ..utils import get_result  # , get_user_id
 from . import blueprint
 
 # <---------- Third Parties ---------->
 
 
@@ -173,43 +175,42 @@
             return render_template("errors/custom.html", error_title=f"Missing argument: `{key}`.")
         except ValueError:
             return render_template("errors/custom.html", error_title=f"Invalid argument: `{key}`.")
     for key in third_parties[name][_page]["required_kwargs"]:
         if key not in kwargs:
             return render_template("errors/custom.html", error_title=f"Missing argument: `{key}`.")
 
-    kwargs["data"] = request.json if request.method not in ("GET", "HEAD") else {}
     kwargs["form"] = request.form.copy()
+    kwargs["json"] = request.json if request.method not in ("GET", "HEAD") and request.content_type == "application/json" else {}
     
     try:
         requeststr = {
             "jsonrpc": "2.0",
             "id": 0,
             "method": "DASHBOARDRPC_THIRDPARTIES__DATA_RECEIVE",
             "params": [
                 request.method,
                 name,
                 page,
                 request.url,
-                session["csrf_token"],
+                (session["csrf_token"], g.csrf_token),
+                base64.urlsafe_b64encode(app.config["WTF_CSRF_SECRET_KEY"]).decode(),
                 context_ids,
                 kwargs,
                 app.extensions["babel"].locale_selector(),
             ],
         }
         with app.lock:
             result = await get_result(app, requeststr)
 
         if "data" in result:
             result = result["data"]
         if "notifications" in result:
             for notification in result["notifications"]:
                 flash(notification["message"], category=notification["category"])
-        if request.method not in ["HEAD", "GET"]:  # API request by JavaScript code or bot.
-            return result
         if "web_content" in result:
             if result["web_content"].get("standalone", False):
                 return render_template_string(
                     name=name, page=page, **return_guild, **result["web_content"]
                 )
             return render_template(
                 "pages/third_parties/third_party.html",
```

### Comparing `red_web_dashboard-1.2.0/reddash/app/utils.py` & `red_web_dashboard-1.3.0/reddash/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,18 +209,18 @@
     initial_protect = app.csrf_protect.protect
 
     def protect():
         initial_protect()
         g.csrf_valid = False
 
     app.csrf_protect.protect = protect
-    initial_init = Field.__init__
+    initial_init_field = Field.__init__
 
     def init_field(field, *args, **kwargs):
-        initial_init(field, *args, **kwargs)
+        initial_init_field(field, *args, **kwargs)
         if isinstance(field, FormField):
             return
         if hasattr(field, "_value"):
             field._real_value = field._value
         field._value = lambda: (field._real_value() if hasattr(field, "_real_value") else "") or (
             (str(field.default) if not isinstance(field.default, typing.List) else field.default)
             if field.default
@@ -496,97 +496,86 @@
             number_to_text_with_suffix=number_to_text_with_suffix,
         )
 
 
 def initialize_babel(app: Flask) -> None:
     app.config["BABEL_TRANSLATION_DIRECTORIES"]: str = "translations"
     app.config["LANGUAGES"]: typing.List[str] = [
-        "en",
-        "af_ZA",
-        "ar_SA",
-        "bg_BG",
-        "ca_ES",
-        "cs_CZ",
-        "da_DK",
-        "de_DE",
-        "el_GR",
-        "es_ES",
-        "fi_FI",
-        "fr_FR",
-        "he_IL",
-        "hu_HU",
-        "id_ID",
-        "it_IT",
-        "ja_JP",
-        "ko_KR",
-        "nl_NL",
-        "nb_NO",
-        "pl_PL",
-        "pt_BR",
-        "pt_PT",
-        "ro_RO",
-        "ru_RU",
-        "sk_SK",
-        "sv_SE",
-        "tr_TR",
-        "uk_UA",
-        "vi_VN",
-        "zh_CN",
-        "zh_HK",
-        "zh_TW",
+        "en-US",
+        "af-ZA",
+        "ar-SA",
+        "bg-BG",
+        "ca-ES",
+        "cs-CZ",
+        "da-DK",
+        "de-DE",
+        "el-GR",
+        "es-ES",
+        "fi-FI",
+        "fr-FR",
+        "he-IL",
+        "hu-HU",
+        "id-ID",
+        "it-IT",
+        "ja-JP",
+        "ko-KR",
+        "nl-NL",
+        "nb-NO",
+        "pl-PL",
+        "pt-BR",
+        "pt-PT",
+        "ro-RO",
+        "ru-RU",
+        "sk-SK",
+        "sv-SE",
+        "tr-TR",
+        "uk-UA",
+        "vi-VN",
+        "zh-CN",
+        "zh-HK",
+        "zh-TW",
     ]
     locale_dict: typing.Dict[str, str] = {}
     for locale in app.config["LANGUAGES"]:
-        loc = Locale.parse(locale)
-        lang = loc.get_language_name(locale)
-        if territory := loc.get_territory_name(locale):
+        loc = Locale.parse(locale, sep="-")
+        lang = loc.get_language_name()
+        if territory := loc.get_territory_name():
             lang = f"{lang} - {territory}"
         locale_dict[locale] = lang
     app.config["LOCALE_DICT"]: typing.Dict[str, str] = locale_dict
 
     @app.before_request
     def pull_locale() -> None:
         # Locale is determined in the following priority:
         # - `lang_code` kwarg
         # - `lang_code` cookie
         # - `lang_code` session value
         # - default from browser
+        locale = None
         lang = request.args.get("lang_code") or request.cookies.get(
             "lang_code"
         )  # Url is visible by user, so it's the priority.
+        lang = lang or session.get("lang_code")  # User either didn't have `lang_code` argument or wasnt able to match a locale. Let's check if theres something in the session.
         if lang:
-            # User had lang_code argument in request, lets check if its valid.
+            # User had `lang_code` argument in request, lets check if its valid.
             processed = process.extractOne(lang, app.config["LANGUAGES"])
             if processed[1] < 80:
                 # Too low of a match, abort lang_code argument and go to session value.
                 lang = None
             else:
-                # User had lang_code argument, and it closely matched a registered locale.
+                # User had `lang_code` argument, and it closely matched a registered locale.
                 locale = processed[0]
-
-        if not lang:
-            # User either didn't have lang_code argument or wasnt able to match a locale.
-            # Let's check if theres something in the session.
-            lang = session.get("lang_code")
-            if lang:
-                # User has a locale in session.
-                locale = lang
-            else:
-                # User doesn't have lang_code, and doesn't have a locale stored in session.
-                # Let's get the best one according to Flask.
-                locale = request.accept_languages.best_match(app.config["LANGUAGES"])
-
         # Let's save that so it will be used on next request as well.
         session["lang_code"] = locale
 
     # @app.babel.localeselector
     def get_locale() -> str:
-        return session.get(
-            "lang_code", request.accept_languages.best_match(app.config["LANGUAGES"])
-        )
+        return (
+            session.get("lang_code") or request.accept_languages.best_match(app.config["LANGUAGES"], default="en-US")
+        ).replace("-", "_")
 
     app.extensions["babel"].locale_selector = get_locale
 
 
 def initialize_websocket(app: Flask) -> bool:
     app.ws: websocket.WebSocket = websocket.WebSocket()
     try:
```

### Comparing `red_web_dashboard-1.2.0/setup.cfg` & `red_web_dashboard-1.3.0/setup.cfg`

 * *Files identical despite different names*

