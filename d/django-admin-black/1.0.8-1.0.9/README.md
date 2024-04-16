# Comparing `tmp/django-admin-black-1.0.8.tar.gz` & `tmp/django-admin-black-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-black-1.0.8.tar", last modified: Wed Jul 12 06:52:58 2023, max compression
+gzip compressed data, was "django-admin-black-1.0.9.tar", last modified: Tue Apr 16 16:20:59 2024, max compression
```

## Comparing `django-admin-black-1.0.8.tar` & `django-admin-black-1.0.9.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.719002 django-admin-black-1.0.8/
--rw-rw-rw-   0        0        0     1113 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      144 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8118 2023-07-12 06:52:58.717999 django-admin-black-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     7018 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.852244 django-admin-black-1.0.8/admin_black/
--rw-rw-rw-   0        0        0        0 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/admin_black/__init__.py
--rw-rw-rw-   0        0        0      120 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/admin_black/apps.py
--rw-rw-rw-   0        0        0     2696 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/forms.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.928635 django-admin-black-1.0.8/admin_black/migrations/
--rw-rw-rw-   0        0        0     1326 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/admin_black/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/admin_black/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.931154 django-admin-black-1.0.8/admin_black/static/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-black-1.0.8/admin_black/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.244859 django-admin-black-1.0.8/admin_black/static/assets/
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.965177 django-admin-black-1.0.8/admin_black/static/assets/css/
--rw-rw-rw-   0        0        0   423144 2023-07-12 06:48:36.000000 django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.css
--rw-rw-rw-   0        0        0   833336 2023-07-12 06:48:36.000000 django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.css.map
--rw-rw-rw-   0        0        0   310289 2023-07-12 06:48:36.000000 django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.min.css
--rw-rw-rw-   0        0        0     9616 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/css/forms.css
--rw-rw-rw-   0        0        0     8292 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/css/nucleo-icons.css
--rw-rw-rw-   0        0        0     1460 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/css/theme-switcher.css
--rw-rw-rw-   0        0        0    12535 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.982011 django-admin-black-1.0.8/admin_black/static/assets/demo/
--rw-rw-rw-   0        0        0      966 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/demo/demo.css
--rw-rw-rw-   0        0        0    19768 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/demo/demo.js
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.994270 django-admin-black-1.0.8/admin_black/static/assets/fonts/
--rw-rw-rw-   0        0        0    26524 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.eot
--rw-rw-rw-   0        0        0    26364 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.ttf
--rw-rw-rw-   0        0        0    15168 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.woff
--rw-rw-rw-   0        0        0    12616 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.woff2
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.116212 django-admin-black-1.0.8/admin_black/static/assets/img/
--rw-rw-rw-   0        0        0  1682267 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/12345.png
--rw-rw-rw-   0        0        0    37930 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/anime3.png
--rw-rw-rw-   0        0        0    39891 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/anime6.png
--rw-rw-rw-   0        0        0     2446 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/apple-icon.png
--rw-rw-rw-   0        0        0   213199 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/bg5.jpg
--rw-rw-rw-   0        0        0     2864 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/default-avatar.png
--rw-rw-rw-   0        0        0    86218 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/emilyz.jpg
--rw-rw-rw-   0        0        0     2761 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/favicon.png
--rw-rw-rw-   0        0        0   670266 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/header.jpg
--rw-rw-rw-   0        0        0      334 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icon-addlink.svg
--rw-rw-rw-   0        0        0     1095 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icon-calendar.svg
--rw-rw-rw-   0        0        0      686 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icon-clock.svg
--rw-rw-rw-   0        0        0      658 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icon-unknown-alt.svg
--rw-rw-rw-   0        0        0      658 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icon-unknown.svg
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.118217 django-admin-black-1.0.8/admin_black/static/assets/img/icons/
--rw-rw-rw-   0        0        0     1040 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/icons/add.svg
--rw-rw-rw-   0        0        0    38381 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/img_3115.jpg
--rw-rw-rw-   0        0        0    74556 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/james.jpg
--rw-rw-rw-   0        0        0    76654 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/mike.jpg
--rw-rw-rw-   0        0        0     8172 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/img/now-logo.png
--rw-rw-rw-   0        0        0      461 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/search.svg
--rw-rw-rw-   0        0        0     3325 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/static/assets/img/selector-icons.svg
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.130227 django-admin-black-1.0.8/admin_black/static/assets/js/
--rw-rw-rw-   0        0        0     7550 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.js
--rw-rw-rw-   0        0        0     4474 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.js.map
--rw-rw-rw-   0        0        0     4541 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.min.js
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.146141 django-admin-black-1.0.8/admin_black/static/assets/js/core/
--rw-rw-rw-   0        0        0    58037 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/core/bootstrap.min.js
--rw-rw-rw-   0        0        0    86663 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/core/jquery.min.js
--rw-rw-rw-   0        0        0    18998 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/core/popper.min.js
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.163120 django-admin-black-1.0.8/admin_black/static/assets/js/plugins/
--rw-rw-rw-   0        0        0    16043 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/plugins/bootstrap-notify.js
--rw-rw-rw-   0        0        0   157854 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/plugins/chartjs.min.js
--rw-rw-rw-   0        0        0    18298 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/plugins/perfect-scrollbar.jquery.min.js
--rw-rw-rw-   0        0        0     4916 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/js/themeSettings.js
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.166119 django-admin-black-1.0.8/admin_black/static/assets/scss/
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.183570 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/
--rw-rw-rw-   0        0        0       31 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/_buttons.scss
--rw-rw-rw-   0        0        0       41 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/_typography.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.276781 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/
--rw-rw-rw-   0        0        0     1199 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_alert.scss
--rw-rw-rw-   0        0        0     1173 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_badge.scss
--rw-rw-rw-   0        0        0     1319 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3787 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_button-group.scss
--rw-rw-rw-   0        0        0     2684 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_buttons.scss
--rw-rw-rw-   0        0        0     6161 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_card.scss
--rw-rw-rw-   0        0        0     4953 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_carousel.scss
--rw-rw-rw-   0        0        0      997 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_close.scss
--rw-rw-rw-   0        0        0     1061 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_code.scss
--rw-rw-rw-   0        0        0    15373 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss
--rw-rw-rw-   0        0        0     4554 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss
--rw-rw-rw-   0        0        0     9146 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_forms.scss
--rw-rw-rw-   0        0        0     2805 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_functions.scss
--rw-rw-rw-   0        0        0     1068 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_grid.scss
--rw-rw-rw-   0        0        0     1195 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_images.scss
--rw-rw-rw-   0        0        0     6048 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_input-group.scss
--rw-rw-rw-   0        0        0      422 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_jumbotron.scss
--rw-rw-rw-   0        0        0     3901 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_list-group.scss
--rw-rw-rw-   0        0        0       91 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_media.scss
--rw-rw-rw-   0        0        0     1106 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_mixins.scss
--rw-rw-rw-   0        0        0     6159 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_modal.scss
--rw-rw-rw-   0        0        0     2189 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_nav.scss
--rw-rw-rw-   0        0        0     6709 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_navbar.scss
--rw-rw-rw-   0        0        0     1813 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_pagination.scss
--rw-rw-rw-   0        0        0     4968 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_popover.scss
--rw-rw-rw-   0        0        0     3142 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_print.scss
--rw-rw-rw-   0        0        0     1111 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_progress.scss
--rw-rw-rw-   0        0        0    11667 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_reboot.scss
--rw-rw-rw-   0        0        0      591 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_root.scss
--rw-rw-rw-   0        0        0     1106 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_spinners.scss
--rw-rw-rw-   0        0        0     3705 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_tables.scss
--rw-rw-rw-   0        0        0     1034 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_toasts.scss
--rw-rw-rw-   0        0        0     2627 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss
--rw-rw-rw-   0        0        0      281 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_transitions.scss
--rw-rw-rw-   0        0        0     2369 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_type.scss
--rw-rw-rw-   0        0        0      519 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_utilities.scss
--rw-rw-rw-   0        0        0    48904 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_variables.scss
--rw-rw-rw-   0        0        0      601 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss
--rw-rw-rw-   0        0        0      423 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0      964 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.358461 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/
--rw-rw-rw-   0        0        0      255 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_alert.scss
--rw-rw-rw-   0        0        0      495 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_background-variant.scss
--rw-rw-rw-   0        0        0      335 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_badge.scss
--rw-rw-rw-   0        0        0     1403 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      552 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4605 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3476 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1468 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss
--rw-rw-rw-   0        0        0      100 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      623 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0      400 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_float.scss
--rw-rw-rw-   0        0        0     5104 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss
--rw-rw-rw-   0        0        0     2095 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     1894 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss
--rw-rw-rw-   0        0        0     1619 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss
--rw-rw-rw-   0        0        0      786 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss
--rw-rw-rw-   0        0        0     1195 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss
--rw-rw-rw-   0        0        0      452 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      175 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_lists.scss
--rw-rw-rw-   0        0        0      271 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_nav-divider.scss
--rw-rw-rw-   0        0        0      484 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      496 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      208 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_resize.scss
--rw-rw-rw-   0        0        0      766 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss
--rw-rw-rw-   0        0        0      155 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_size.scss
--rw-rw-rw-   0        0        0      831 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss
--rw-rw-rw-   0        0        0      380 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-emphasis.scss
--rw-rw-rw-   0        0        0      337 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-hide.scss
--rw-rw-rw-   0        0        0      176 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      380 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_transition.scss
--rw-rw-rw-   0        0        0      197 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_visibility.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.395559 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/
--rw-rw-rw-   0        0        0      428 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_align.scss
--rw-rw-rw-   0        0        0      416 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_background.scss
--rw-rw-rw-   0        0        0     1840 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss
--rw-rw-rw-   0        0        0       40 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_clearfix.scss
--rw-rw-rw-   0        0        0      545 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss
--rw-rw-rw-   0        0        0      885 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss
--rw-rw-rw-   0        0        0     2820 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss
--rw-rw-rw-   0        0        0      387 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_float.scss
--rw-rw-rw-   0        0        0      138 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_overflow.scss
--rw-rw-rw-   0        0        0      516 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss
--rw-rw-rw-   0        0        0      126 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_screenreaders.scss
--rw-rw-rw-   0        0        0      255 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_shadows.scss
--rw-rw-rw-   0        0        0      518 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss
--rw-rw-rw-   0        0        0     2174 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss
--rw-rw-rw-   0        0        0      450 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_stretched-link.scss
--rw-rw-rw-   0        0        0     2082 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss
--rw-rw-rw-   0        0        0      187 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_visibility.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.397558 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/
--rw-rw-rw-   0        0        0     6677 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.474175 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/
--rw-rw-rw-   0        0        0     1689 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_alerts.scss
--rw-rw-rw-   0        0        0     5270 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_buttons.scss
--rw-rw-rw-   0        0        0     5330 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_card.scss
--rw-rw-rw-   0        0        0     3799 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss
--rw-rw-rw-   0        0        0     7959 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_dropdown.scss
--rw-rw-rw-   0        0        0     4818 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_example-pages.scss
--rw-rw-rw-   0        0        0     7185 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss
--rw-rw-rw-   0        0        0     1500 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_footer.scss
--rw-rw-rw-   0        0        0     3011 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_forms.scss
--rw-rw-rw-   0        0        0      590 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_functions.scss
--rw-rw-rw-   0        0        0      124 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_images.scss
--rw-rw-rw-   0        0        0     7743 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_input-group.scss
--rw-rw-rw-   0        0        0     3802 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_misc.scss
--rw-rw-rw-   0        0        0      493 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_mixins.scss
--rw-rw-rw-   0        0        0     2979 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_modal.scss
--rw-rw-rw-   0        0        0     7679 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_navbar.scss
--rw-rw-rw-   0        0        0     3615 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_rtl.scss
--rw-rw-rw-   0        0        0    19722 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss
--rw-rw-rw-   0        0        0     3649 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_tables.scss
--rw-rw-rw-   0        0        0     2940 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_type.scss
--rw-rw-rw-   0        0        0      318 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_utilities.scss
--rw-rw-rw-   0        0        0    37819 2023-05-03 04:15:59.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_variables.scss
--rw-rw-rw-   0        0        0     6509 2023-05-03 04:12:12.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_white-content.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.493227 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/
--rw-rw-rw-   0        0        0     1054 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss
--rw-rw-rw-   0        0        0       29 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-map.scss
--rw-rw-rw-   0        0        0      286 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-plain.scss
--rw-rw-rw-   0        0        0      451 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-task.scss
--rw-rw-rw-   0        0        0     1780 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-user.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.522841 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/
--rw-rw-rw-   0        0        0      345 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_alert.scss
--rw-rw-rw-   0        0        0      467 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_background-variant.scss
--rw-rw-rw-   0        0        0      295 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_badges.scss
--rw-rw-rw-   0        0        0     9876 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss
--rw-rw-rw-   0        0        0      542 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss
--rw-rw-rw-   0        0        0     2805 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_forms.scss
--rw-rw-rw-   0        0        0      150 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_icon.scss
--rw-rw-rw-   0        0        0     6623 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss
--rw-rw-rw-   0        0        0      319 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_modals.scss
--rw-rw-rw-   0        0        0      481 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_page-header.scss
--rw-rw-rw-   0        0        0      728 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss
--rw-rw-rw-   0        0        0     7426 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss
--rw-rw-rw-   0        0        0      655 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss
--rw-rw-rw-   0        0        0      160 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/opacity.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.543932 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/
--rw-rw-rw-   0        0        0      840 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss
--rw-rw-rw-   0        0        0      862 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_floating.scss
--rw-rw-rw-   0        0        0      877 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_helper.scss
--rw-rw-rw-   0        0        0      260 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_position.scss
--rw-rw-rw-   0        0        0      358 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_shadows.scss
--rw-rw-rw-   0        0        0       69 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_sizing.scss
--rw-rw-rw-   0        0        0     2144 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss
--rw-rw-rw-   0        0        0     1022 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_text.scss
--rw-rw-rw-   0        0        0      284 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_transform.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.548929 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/vendor/
--rw-rw-rw-   0        0        0     3542 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss
--rw-rw-rw-   0        0        0     2714 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.549929 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/plugins/
--rw-rw-rw-   0        0        0     2714 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss
--rw-rw-rw-   0        0        0     3680 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard.scss
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.553451 django-admin-black-1.0.8/admin_black/templates/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-black-1.0.8/admin_black/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.590006 django-admin-black-1.0.8/admin_black/templates/accounts/
--rw-rw-rw-   0        0        0     4821 2023-02-27 04:31:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/auth-signin.html
--rw-rw-rw-   0        0        0     4429 2023-02-27 04:31:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/auth-signup.html
--rw-rw-rw-   0        0        0     4007 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/forgot-password.html
--rw-rw-rw-   0        0        0     4382 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/password_change.html
--rw-rw-rw-   0        0        0     3172 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/password_change_done.html
--rw-rw-rw-   0        0        0     3267 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/password_reset_complete.html
--rw-rw-rw-   0        0        0     3414 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/password_reset_done.html
--rw-rw-rw-   0        0        0     4466 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/accounts/recover-password.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.625142 django-admin-black-1.0.8/admin_black/templates/admin/
--rw-rw-rw-   0        0        0     1606 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:57.260903 django-admin-black-1.0.8/admin_black/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.631668 django-admin-black-1.0.8/admin_black/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      334 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5385 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     6206 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      556 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     5584 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      470 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3204 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     7159 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     6802 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.636665 django-admin-black-1.0.8/admin_black/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7834 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      506 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.640171 django-admin-black-1.0.8/admin_black/templates/admin/includes/
--rw-rw-rw-   0        0        0     2572 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      339 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    19323 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/index.html
--rw-rw-rw-   0        0        0     2717 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     5985 2023-02-27 04:31:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/login.html
--rw-rw-rw-   0        0        0     3895 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2180 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     1882 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1481 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.668982 django-admin-black-1.0.8/admin_black/templates/includes/
--rw-rw-rw-   0        0        0     2390 2023-02-26 17:37:05.000000 django-admin-black-1.0.8/admin_black/templates/includes/fixed-plugin.html
--rw-rw-rw-   0        0        0      928 2023-02-26 17:23:59.000000 django-admin-black-1.0.8/admin_black/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1016 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/head.html
--rw-rw-rw-   0        0        0     4120 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/menu-list.html
--rw-rw-rw-   0        0        0     5888 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/navigation.html
--rw-rw-rw-   0        0        0     4207 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/navigationrtl.html
--rw-rw-rw-   0        0        0     1950 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/rtlsidebar.html
--rw-rw-rw-   0        0        0     1563 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/scripts.html
--rw-rw-rw-   0        0        0      522 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/includes/sidebar.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.670495 django-admin-black-1.0.8/admin_black/templates/layouts/
--rw-rw-rw-   0        0        0     1186 2023-07-12 06:48:41.000000 django-admin-black-1.0.8/admin_black/templates/layouts/base.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.691266 django-admin-black-1.0.8/admin_black/templates/pages/
--rw-rw-rw-   0        0        0    20662 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/dashboard.html
--rw-rw-rw-   0        0        0    27773 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/icons.html
--rw-rw-rw-   0        0        0      620 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/map.html
--rw-rw-rw-   0        0        0     6204 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/notifications.html
--rw-rw-rw-   0        0        0    16074 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/rtl.html
--rw-rw-rw-   0        0        0     7405 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/tables.html
--rw-rw-rw-   0        0        0     6313 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/typography.html
--rw-rw-rw-   0        0        0     3504 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/upgrade.html
--rw-rw-rw-   0        0        0     5360 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/pages/user.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.699852 django-admin-black-1.0.8/admin_black/templates/registration/
--rw-rw-rw-   0        0        0     1761 2023-02-27 04:31:26.000000 django-admin-black-1.0.8/admin_black/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     2767 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     4179 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templates/registration/password_change_form.html
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.702809 django-admin-black-1.0.8/admin_black/templatetags/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/templatetags/admin_black.py
--rw-rw-rw-   0        0        0     1833 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/urls.py
--rw-rw-rw-   0        0        0    16512 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/utils.py
--rw-rw-rw-   0        0        0     3478 2023-02-26 16:09:26.000000 django-admin-black-1.0.8/admin_black/views.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.714007 django-admin-black-1.0.8/django_admin_black.egg-info/
--rw-rw-rw-   0        0        0     8118 2023-07-12 06:52:56.000000 django-admin-black-1.0.8/django_admin_black.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16123 2023-07-12 06:52:57.000000 django-admin-black-1.0.8/django_admin_black.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 06:52:56.000000 django-admin-black-1.0.8/django_admin_black.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-26 16:25:01.000000 django-admin-black-1.0.8/django_admin_black.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-07-12 06:52:57.000000 django-admin-black-1.0.8/django_admin_black.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 06:52:58.716000 django-admin-black-1.0.8/docs/
--rw-rw-rw-   0        0        0       13 2023-02-18 07:53:39.000000 django-admin-black-1.0.8/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 06:52:58.719002 django-admin-black-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-07-12 06:49:22.000000 django-admin-black-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:59.056833 django-admin-black-1.0.9/
+-rw-rw-rw-   0        0        0     1113 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      144 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8118 2024-04-16 16:20:59.055833 django-admin-black-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7018 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.768797 django-admin-black-1.0.9/admin_black/
+-rw-rw-rw-   0        0        0        0 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/admin_black/__init__.py
+-rw-rw-rw-   0        0        0      120 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/admin_black/apps.py
+-rw-rw-rw-   0        0        0     2696 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.772331 django-admin-black-1.0.9/admin_black/migrations/
+-rw-rw-rw-   0        0        0     1326 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/admin_black/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/admin_black/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.774327 django-admin-black-1.0.9/admin_black/static/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-black-1.0.9/admin_black/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.697080 django-admin-black-1.0.9/admin_black/static/assets/
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.924996 django-admin-black-1.0.9/admin_black/static/assets/css/
+-rw-rw-rw-   0        0        0   423144 2023-07-12 06:48:36.000000 django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.css
+-rw-rw-rw-   0        0        0   833336 2023-07-12 06:48:36.000000 django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.css.map
+-rw-rw-rw-   0        0        0   310289 2023-07-12 06:48:36.000000 django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.min.css
+-rw-rw-rw-   0        0        0     9616 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/css/forms.css
+-rw-rw-rw-   0        0        0     8292 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/css/nucleo-icons.css
+-rw-rw-rw-   0        0        0     1460 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/css/theme-switcher.css
+-rw-rw-rw-   0        0        0    12535 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.969254 django-admin-black-1.0.9/admin_black/static/assets/demo/
+-rw-rw-rw-   0        0        0      966 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/demo/demo.css
+-rw-rw-rw-   0        0        0    19768 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/demo/demo.js
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:56.000930 django-admin-black-1.0.9/admin_black/static/assets/fonts/
+-rw-rw-rw-   0        0        0    26524 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.eot
+-rw-rw-rw-   0        0        0    26364 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.ttf
+-rw-rw-rw-   0        0        0    15168 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.woff
+-rw-rw-rw-   0        0        0    12616 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.woff2
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:56.634503 django-admin-black-1.0.9/admin_black/static/assets/img/
+-rw-rw-rw-   0        0        0  1682267 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/12345.png
+-rw-rw-rw-   0        0        0    37930 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/anime3.png
+-rw-rw-rw-   0        0        0    39891 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/anime6.png
+-rw-rw-rw-   0        0        0     2446 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/apple-icon.png
+-rw-rw-rw-   0        0        0   213199 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/bg5.jpg
+-rw-rw-rw-   0        0        0     2864 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/default-avatar.png
+-rw-rw-rw-   0        0        0    86218 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/emilyz.jpg
+-rw-rw-rw-   0        0        0     2761 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/favicon.png
+-rw-rw-rw-   0        0        0   670266 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/header.jpg
+-rw-rw-rw-   0        0        0      334 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icon-addlink.svg
+-rw-rw-rw-   0        0        0     1095 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icon-calendar.svg
+-rw-rw-rw-   0        0        0      686 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icon-clock.svg
+-rw-rw-rw-   0        0        0      658 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icon-unknown-alt.svg
+-rw-rw-rw-   0        0        0      658 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icon-unknown.svg
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:56.646060 django-admin-black-1.0.9/admin_black/static/assets/img/icons/
+-rw-rw-rw-   0        0        0     1040 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/icons/add.svg
+-rw-rw-rw-   0        0        0    38381 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/img_3115.jpg
+-rw-rw-rw-   0        0        0    74556 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/james.jpg
+-rw-rw-rw-   0        0        0    76654 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/mike.jpg
+-rw-rw-rw-   0        0        0     8172 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/img/now-logo.png
+-rw-rw-rw-   0        0        0      461 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/search.svg
+-rw-rw-rw-   0        0        0     3325 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/static/assets/img/selector-icons.svg
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:56.759571 django-admin-black-1.0.9/admin_black/static/assets/js/
+-rw-rw-rw-   0        0        0     7550 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.js
+-rw-rw-rw-   0        0        0     4474 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.js.map
+-rw-rw-rw-   0        0        0     4541 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.min.js
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:56.886077 django-admin-black-1.0.9/admin_black/static/assets/js/core/
+-rw-rw-rw-   0        0        0    58037 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/core/bootstrap.min.js
+-rw-rw-rw-   0        0        0    86663 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/core/jquery.min.js
+-rw-rw-rw-   0        0        0    18998 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/core/popper.min.js
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.005765 django-admin-black-1.0.9/admin_black/static/assets/js/plugins/
+-rw-rw-rw-   0        0        0    16043 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/plugins/bootstrap-notify.js
+-rw-rw-rw-   0        0        0   157854 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/plugins/chartjs.min.js
+-rw-rw-rw-   0        0        0    18298 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/plugins/perfect-scrollbar.jquery.min.js
+-rw-rw-rw-   0        0        0     4916 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/js/themeSettings.js
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.025305 django-admin-black-1.0.9/admin_black/static/assets/scss/
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.043927 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/
+-rw-rw-rw-   0        0        0       31 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/_buttons.scss
+-rw-rw-rw-   0        0        0       41 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/_typography.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.454260 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/
+-rw-rw-rw-   0        0        0     1199 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_alert.scss
+-rw-rw-rw-   0        0        0     1173 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_badge.scss
+-rw-rw-rw-   0        0        0     1319 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3787 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_button-group.scss
+-rw-rw-rw-   0        0        0     2684 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_buttons.scss
+-rw-rw-rw-   0        0        0     6161 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_card.scss
+-rw-rw-rw-   0        0        0     4953 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_carousel.scss
+-rw-rw-rw-   0        0        0      997 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_close.scss
+-rw-rw-rw-   0        0        0     1061 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_code.scss
+-rw-rw-rw-   0        0        0    15373 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss
+-rw-rw-rw-   0        0        0     4554 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss
+-rw-rw-rw-   0        0        0     9146 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_forms.scss
+-rw-rw-rw-   0        0        0     2805 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_functions.scss
+-rw-rw-rw-   0        0        0     1068 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_grid.scss
+-rw-rw-rw-   0        0        0     1195 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_images.scss
+-rw-rw-rw-   0        0        0     6048 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_input-group.scss
+-rw-rw-rw-   0        0        0      422 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_jumbotron.scss
+-rw-rw-rw-   0        0        0     3901 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_list-group.scss
+-rw-rw-rw-   0        0        0       91 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_media.scss
+-rw-rw-rw-   0        0        0     1106 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_mixins.scss
+-rw-rw-rw-   0        0        0     6159 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_modal.scss
+-rw-rw-rw-   0        0        0     2189 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_nav.scss
+-rw-rw-rw-   0        0        0     6709 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_navbar.scss
+-rw-rw-rw-   0        0        0     1813 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_pagination.scss
+-rw-rw-rw-   0        0        0     4968 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_popover.scss
+-rw-rw-rw-   0        0        0     3142 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_print.scss
+-rw-rw-rw-   0        0        0     1111 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_progress.scss
+-rw-rw-rw-   0        0        0    11667 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_reboot.scss
+-rw-rw-rw-   0        0        0      591 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_root.scss
+-rw-rw-rw-   0        0        0     1106 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_spinners.scss
+-rw-rw-rw-   0        0        0     3705 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_tables.scss
+-rw-rw-rw-   0        0        0     1034 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_toasts.scss
+-rw-rw-rw-   0        0        0     2627 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss
+-rw-rw-rw-   0        0        0      281 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_transitions.scss
+-rw-rw-rw-   0        0        0     2369 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_type.scss
+-rw-rw-rw-   0        0        0      519 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_utilities.scss
+-rw-rw-rw-   0        0        0    48904 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_variables.scss
+-rw-rw-rw-   0        0        0      601 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0      423 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0      964 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.793813 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/
+-rw-rw-rw-   0        0        0      255 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      495 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_background-variant.scss
+-rw-rw-rw-   0        0        0      335 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_badge.scss
+-rw-rw-rw-   0        0        0     1403 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      552 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4605 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3476 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1468 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss
+-rw-rw-rw-   0        0        0      100 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      623 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0      400 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_float.scss
+-rw-rw-rw-   0        0        0     5104 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     2095 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     1894 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss
+-rw-rw-rw-   0        0        0     1619 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      786 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss
+-rw-rw-rw-   0        0        0     1195 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss
+-rw-rw-rw-   0        0        0      452 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      175 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      271 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_nav-divider.scss
+-rw-rw-rw-   0        0        0      484 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      496 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      208 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_resize.scss
+-rw-rw-rw-   0        0        0      766 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss
+-rw-rw-rw-   0        0        0      155 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_size.scss
+-rw-rw-rw-   0        0        0      831 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss
+-rw-rw-rw-   0        0        0      380 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-emphasis.scss
+-rw-rw-rw-   0        0        0      337 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-hide.scss
+-rw-rw-rw-   0        0        0      176 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      380 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_transition.scss
+-rw-rw-rw-   0        0        0      197 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_visibility.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.961312 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/
+-rw-rw-rw-   0        0        0      428 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_align.scss
+-rw-rw-rw-   0        0        0      416 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_background.scss
+-rw-rw-rw-   0        0        0     1840 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss
+-rw-rw-rw-   0        0        0       40 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_clearfix.scss
+-rw-rw-rw-   0        0        0      545 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss
+-rw-rw-rw-   0        0        0      885 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss
+-rw-rw-rw-   0        0        0     2820 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_float.scss
+-rw-rw-rw-   0        0        0      138 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_overflow.scss
+-rw-rw-rw-   0        0        0      516 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss
+-rw-rw-rw-   0        0        0      126 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_screenreaders.scss
+-rw-rw-rw-   0        0        0      255 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_shadows.scss
+-rw-rw-rw-   0        0        0      518 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss
+-rw-rw-rw-   0        0        0     2174 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss
+-rw-rw-rw-   0        0        0      450 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_stretched-link.scss
+-rw-rw-rw-   0        0        0     2082 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss
+-rw-rw-rw-   0        0        0      187 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_visibility.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:57.964385 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/
+-rw-rw-rw-   0        0        0     6677 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.207567 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/
+-rw-rw-rw-   0        0        0     1689 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_alerts.scss
+-rw-rw-rw-   0        0        0     5270 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_buttons.scss
+-rw-rw-rw-   0        0        0     5330 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_card.scss
+-rw-rw-rw-   0        0        0     3799 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss
+-rw-rw-rw-   0        0        0     7959 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_dropdown.scss
+-rw-rw-rw-   0        0        0     4818 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_example-pages.scss
+-rw-rw-rw-   0        0        0     7185 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss
+-rw-rw-rw-   0        0        0     1500 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_footer.scss
+-rw-rw-rw-   0        0        0     3011 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_forms.scss
+-rw-rw-rw-   0        0        0      590 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_functions.scss
+-rw-rw-rw-   0        0        0      124 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_images.scss
+-rw-rw-rw-   0        0        0     7743 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_input-group.scss
+-rw-rw-rw-   0        0        0     3802 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_misc.scss
+-rw-rw-rw-   0        0        0      493 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_mixins.scss
+-rw-rw-rw-   0        0        0     2979 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_modal.scss
+-rw-rw-rw-   0        0        0     7679 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_navbar.scss
+-rw-rw-rw-   0        0        0     3615 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_rtl.scss
+-rw-rw-rw-   0        0        0    19722 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss
+-rw-rw-rw-   0        0        0     3649 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_tables.scss
+-rw-rw-rw-   0        0        0     2940 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_type.scss
+-rw-rw-rw-   0        0        0      318 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_utilities.scss
+-rw-rw-rw-   0        0        0    37819 2023-05-03 04:15:59.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_variables.scss
+-rw-rw-rw-   0        0        0     6509 2023-05-03 04:12:12.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_white-content.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.233681 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/
+-rw-rw-rw-   0        0        0     1054 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss
+-rw-rw-rw-   0        0        0       29 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-map.scss
+-rw-rw-rw-   0        0        0      286 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-plain.scss
+-rw-rw-rw-   0        0        0      451 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-task.scss
+-rw-rw-rw-   0        0        0     1780 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-user.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.359587 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/
+-rw-rw-rw-   0        0        0      345 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      467 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_background-variant.scss
+-rw-rw-rw-   0        0        0      295 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_badges.scss
+-rw-rw-rw-   0        0        0     9876 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0      542 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss
+-rw-rw-rw-   0        0        0     2805 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_forms.scss
+-rw-rw-rw-   0        0        0      150 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_icon.scss
+-rw-rw-rw-   0        0        0     6623 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss
+-rw-rw-rw-   0        0        0      319 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_modals.scss
+-rw-rw-rw-   0        0        0      481 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_page-header.scss
+-rw-rw-rw-   0        0        0      728 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss
+-rw-rw-rw-   0        0        0     7426 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss
+-rw-rw-rw-   0        0        0      655 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss
+-rw-rw-rw-   0        0        0      160 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/opacity.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.434014 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/
+-rw-rw-rw-   0        0        0      840 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss
+-rw-rw-rw-   0        0        0      862 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_floating.scss
+-rw-rw-rw-   0        0        0      877 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_helper.scss
+-rw-rw-rw-   0        0        0      260 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_position.scss
+-rw-rw-rw-   0        0        0      358 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_shadows.scss
+-rw-rw-rw-   0        0        0       69 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_sizing.scss
+-rw-rw-rw-   0        0        0     2144 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss
+-rw-rw-rw-   0        0        0     1022 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_text.scss
+-rw-rw-rw-   0        0        0      284 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_transform.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.448044 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/vendor/
+-rw-rw-rw-   0        0        0     3542 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss
+-rw-rw-rw-   0        0        0     2714 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.450552 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/plugins/
+-rw-rw-rw-   0        0        0     2714 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss
+-rw-rw-rw-   0        0        0     3680 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard.scss
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.453562 django-admin-black-1.0.9/admin_black/templates/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-black-1.0.9/admin_black/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.581178 django-admin-black-1.0.9/admin_black/templates/accounts/
+-rw-rw-rw-   0        0        0     4821 2023-02-27 04:31:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/auth-signin.html
+-rw-rw-rw-   0        0        0     4429 2023-02-27 04:31:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/auth-signup.html
+-rw-rw-rw-   0        0        0     4007 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/forgot-password.html
+-rw-rw-rw-   0        0        0     4382 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/password_change.html
+-rw-rw-rw-   0        0        0     3172 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/password_change_done.html
+-rw-rw-rw-   0        0        0     3267 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/password_reset_complete.html
+-rw-rw-rw-   0        0        0     3414 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/password_reset_done.html
+-rw-rw-rw-   0        0        0     4466 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/accounts/recover-password.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.712760 django-admin-black-1.0.9/admin_black/templates/admin/
+-rw-rw-rw-   0        0        0     1606 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:55.708608 django-admin-black-1.0.9/admin_black/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.737672 django-admin-black-1.0.9/admin_black/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      334 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5385 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     6206 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      556 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     5584 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      470 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3204 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     7159 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     6802 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.755681 django-admin-black-1.0.9/admin_black/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7834 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      506 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.770817 django-admin-black-1.0.9/admin_black/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2572 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      339 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    19323 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2717 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     5985 2023-02-27 04:31:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/login.html
+-rw-rw-rw-   0        0        0     3895 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2180 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     1882 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1481 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.834647 django-admin-black-1.0.9/admin_black/templates/includes/
+-rw-rw-rw-   0        0        0     2390 2023-02-26 17:37:05.000000 django-admin-black-1.0.9/admin_black/templates/includes/fixed-plugin.html
+-rw-rw-rw-   0        0        0      928 2023-02-26 17:23:59.000000 django-admin-black-1.0.9/admin_black/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1016 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/head.html
+-rw-rw-rw-   0        0        0     4120 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/menu-list.html
+-rw-rw-rw-   0        0        0     5888 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/navigation.html
+-rw-rw-rw-   0        0        0     4207 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/navigationrtl.html
+-rw-rw-rw-   0        0        0     1950 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/rtlsidebar.html
+-rw-rw-rw-   0        0        0     1563 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0      522 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/includes/sidebar.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.853895 django-admin-black-1.0.9/admin_black/templates/layouts/
+-rw-rw-rw-   0        0        0     1186 2023-07-12 06:48:41.000000 django-admin-black-1.0.9/admin_black/templates/layouts/base.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:58.975501 django-admin-black-1.0.9/admin_black/templates/pages/
+-rw-rw-rw-   0        0        0    20891 2024-04-16 16:18:48.000000 django-admin-black-1.0.9/admin_black/templates/pages/dashboard.html
+-rw-rw-rw-   0        0        0    27773 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/icons.html
+-rw-rw-rw-   0        0        0      620 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/map.html
+-rw-rw-rw-   0        0        0     6204 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/notifications.html
+-rw-rw-rw-   0        0        0    16074 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/rtl.html
+-rw-rw-rw-   0        0        0     7405 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/tables.html
+-rw-rw-rw-   0        0        0     6313 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/typography.html
+-rw-rw-rw-   0        0        0     3504 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/upgrade.html
+-rw-rw-rw-   0        0        0     5360 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/pages/user.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:59.012118 django-admin-black-1.0.9/admin_black/templates/registration/
+-rw-rw-rw-   0        0        0     1761 2023-02-27 04:31:26.000000 django-admin-black-1.0.9/admin_black/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     2767 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     4179 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templates/registration/password_change_form.html
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:59.015124 django-admin-black-1.0.9/admin_black/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/templatetags/admin_black.py
+-rw-rw-rw-   0        0        0     1833 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/urls.py
+-rw-rw-rw-   0        0        0    16512 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/utils.py
+-rw-rw-rw-   0        0        0     3478 2023-02-26 16:09:26.000000 django-admin-black-1.0.9/admin_black/views.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:59.047966 django-admin-black-1.0.9/django_admin_black.egg-info/
+-rw-rw-rw-   0        0        0     8118 2024-04-16 16:20:54.000000 django-admin-black-1.0.9/django_admin_black.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16123 2024-04-16 16:20:55.000000 django-admin-black-1.0.9/django_admin_black.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:20:54.000000 django-admin-black-1.0.9/django_admin_black.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-26 16:25:01.000000 django-admin-black-1.0.9/django_admin_black.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-16 16:20:55.000000 django-admin-black-1.0.9/django_admin_black.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 16:20:59.054786 django-admin-black-1.0.9/docs/
+-rw-rw-rw-   0        0        0       13 2023-02-18 07:53:39.000000 django-admin-black-1.0.9/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:20:59.056833 django-admin-black-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2024-04-16 16:19:35.000000 django-admin-black-1.0.9/setup.py
```

### Comparing `django-admin-black-1.0.8/LICENSE.md` & `django-admin-black-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/PKG-INFO` & `django-admin-black-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-black
-Version: 1.0.8
+Version: 1.0.9
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/black-dashboard/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-black-1.0.8/README.md` & `django-admin-black-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/forms.py` & `django-admin-black-1.0.9/admin_black/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/migrations/0001_initial.py` & `django-admin-black-1.0.9/admin_black/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.css.map` & `django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/black-dashboard.min.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/black-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/forms.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/nucleo-icons.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/theme-switcher.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/theme-switcher.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/css/widgets.css` & `django-admin-black-1.0.9/admin_black/static/assets/css/widgets.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/demo/demo.css` & `django-admin-black-1.0.9/admin_black/static/assets/demo/demo.css`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/demo/demo.js` & `django-admin-black-1.0.9/admin_black/static/assets/demo/demo.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.eot` & `django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.ttf` & `django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.woff` & `django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/fonts/nucleo.woff2` & `django-admin-black-1.0.9/admin_black/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/12345.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/12345.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/anime3.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/anime3.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/anime6.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/anime6.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/apple-icon.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/apple-icon.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/bg5.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/bg5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/default-avatar.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/default-avatar.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/emilyz.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/emilyz.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/favicon.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/header.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/header.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/icon-calendar.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/icon-clock.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/icon-unknown-alt.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/icon-unknown.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/icons/add.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/icons/add.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/img_3115.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/img_3115.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/james.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/james.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/mike.jpg` & `django-admin-black-1.0.9/admin_black/static/assets/img/mike.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/now-logo.png` & `django-admin-black-1.0.9/admin_black/static/assets/img/now-logo.png`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/img/selector-icons.svg` & `django-admin-black-1.0.9/admin_black/static/assets/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.js.map` & `django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/black-dashboard.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/black-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/core/bootstrap.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/core/jquery.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/core/popper.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/plugins/bootstrap-notify.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/plugins/chartjs.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/plugins/perfect-scrollbar.jquery.min.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/plugins/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/js/themeSettings.js` & `django-admin-black-1.0.9/admin_black/static/assets/js/themeSettings.js`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_alert.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_badge.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_button-group.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_buttons.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_card.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_carousel.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_close.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_code.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_code.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_forms.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_functions.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_grid.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_images.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_input-group.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_list-group.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_mixins.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_modal.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_nav.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_navbar.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_pagination.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_popover.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_print.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_print.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_progress.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_reboot.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_root.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_spinners.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_tables.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_toasts.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_type.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_utilities.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/_variables.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_alerts.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_alerts.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_buttons.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_card.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_card.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_dropdown.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_example-pages.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_example-pages.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_footer.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_footer.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_forms.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_functions.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_input-group.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_misc.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_misc.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_modal.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_modal.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_navbar.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_rtl.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_rtl.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_tables.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_type.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_type.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_variables.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/_white-content.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/_white-content.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-user.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/cards/_card-user.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_forms.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_floating.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_floating.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_helper.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_helper.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/utilities/_text.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/static/assets/scss/black-dashboard.scss` & `django-admin-black-1.0.9/admin_black/static/assets/scss/black-dashboard.scss`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/auth-signin.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/auth-signin.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/auth-signup.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/auth-signup.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/forgot-password.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/forgot-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/password_change.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/password_change.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/password_change_done.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/password_reset_complete.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/password_reset_done.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/accounts/recover-password.html` & `django-admin-black-1.0.9/admin_black/templates/accounts/recover-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/actions.html` & `django-admin-black-1.0.9/admin_black/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/auth/user/change_password.html` & `django-admin-black-1.0.9/admin_black/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/change_form.html` & `django-admin-black-1.0.9/admin_black/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/change_form_object_tools.html` & `django-admin-black-1.0.9/admin_black/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/change_list.html` & `django-admin-black-1.0.9/admin_black/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/change_list_results.html` & `django-admin-black-1.0.9/admin_black/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/delete_confirmation.html` & `django-admin-black-1.0.9/admin_black/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/delete_selected_confirmation.html` & `django-admin-black-1.0.9/admin_black/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/edit_inline/stacked.html` & `django-admin-black-1.0.9/admin_black/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/edit_inline/tabular.html` & `django-admin-black-1.0.9/admin_black/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/includes/fieldset.html` & `django-admin-black-1.0.9/admin_black/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/index.html` & `django-admin-black-1.0.9/admin_black/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/invalid_setup.html` & `django-admin-black-1.0.9/admin_black/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/login.html` & `django-admin-black-1.0.9/admin_black/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/object_history.html` & `django-admin-black-1.0.9/admin_black/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/pagination.html` & `django-admin-black-1.0.9/admin_black/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/search_form.html` & `django-admin-black-1.0.9/admin_black/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/admin/submit_line.html` & `django-admin-black-1.0.9/admin_black/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/fixed-plugin.html` & `django-admin-black-1.0.9/admin_black/templates/includes/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/footer.html` & `django-admin-black-1.0.9/admin_black/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/head.html` & `django-admin-black-1.0.9/admin_black/templates/includes/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/menu-list.html` & `django-admin-black-1.0.9/admin_black/templates/includes/menu-list.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/navigation.html` & `django-admin-black-1.0.9/admin_black/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/navigationrtl.html` & `django-admin-black-1.0.9/admin_black/templates/includes/navigationrtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/rtlsidebar.html` & `django-admin-black-1.0.9/admin_black/templates/includes/rtlsidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/scripts.html` & `django-admin-black-1.0.9/admin_black/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/includes/sidebar.html` & `django-admin-black-1.0.9/admin_black/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/layouts/base.html` & `django-admin-black-1.0.9/admin_black/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/dashboard.html` & `django-admin-black-1.0.9/admin_black/templates/pages/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -378,8 +378,17 @@
                         </table>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 </div>
-{% endblock content %}
+{% endblock content %}
+{% block extrajs %}
+<script>
+    $(document).ready(function () {
+        // Javascript method's body can be found in assets/js/demos.js
+        demo.initDashboardPageCharts();
+
+    });
+</script>
+{% endblock extrajs %}
```

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/icons.html` & `django-admin-black-1.0.9/admin_black/templates/pages/icons.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/map.html` & `django-admin-black-1.0.9/admin_black/templates/pages/map.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/notifications.html` & `django-admin-black-1.0.9/admin_black/templates/pages/notifications.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/rtl.html` & `django-admin-black-1.0.9/admin_black/templates/pages/rtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/tables.html` & `django-admin-black-1.0.9/admin_black/templates/pages/tables.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/typography.html` & `django-admin-black-1.0.9/admin_black/templates/pages/typography.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/upgrade.html` & `django-admin-black-1.0.9/admin_black/templates/pages/upgrade.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/pages/user.html` & `django-admin-black-1.0.9/admin_black/templates/pages/user.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/registration/logged_out.html` & `django-admin-black-1.0.9/admin_black/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/registration/password_change_done.html` & `django-admin-black-1.0.9/admin_black/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templates/registration/password_change_form.html` & `django-admin-black-1.0.9/admin_black/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/templatetags/admin_black.py` & `django-admin-black-1.0.9/admin_black/templatetags/admin_black.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/urls.py` & `django-admin-black-1.0.9/admin_black/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/utils.py` & `django-admin-black-1.0.9/admin_black/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/admin_black/views.py` & `django-admin-black-1.0.9/admin_black/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/django_admin_black.egg-info/PKG-INFO` & `django-admin-black-1.0.9/django_admin_black.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-black
-Version: 1.0.8
+Version: 1.0.9
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/black-dashboard/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-black-1.0.8/django_admin_black.egg-info/SOURCES.txt` & `django-admin-black-1.0.9/django_admin_black.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-black-1.0.8/setup.py` & `django-admin-black-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-black',
-version='1.0.8',
+version='1.0.9',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/black-dashboard/django/',
```

