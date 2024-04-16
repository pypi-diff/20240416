# Comparing `tmp/django-static-adminlte-3.2.0.1.tar.gz` & `tmp/django-static-adminlte-3.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-static-adminlte-3.2.0.1.tar", last modified: Mon Sep 18 06:48:15 2023, max compression
+gzip compressed data, was "django-static-adminlte-3.2.0.2.tar", last modified: Tue Apr 16 13:15:40 2024, max compression
```

## Comparing `django-static-adminlte-3.2.0.1.tar` & `django-static-adminlte-3.2.0.2.tar`

### file list

```diff
@@ -1,24 +1,105 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-18 06:48:15.374988 django-static-adminlte-3.2.0.1/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-09-18 06:18:26.000000 django-static-adminlte-3.2.0.1/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      163 2023-09-18 06:18:33.000000 django-static-adminlte-3.2.0.1/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2853 2023-09-18 06:48:15.374850 django-static-adminlte-3.2.0.1/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2156 2023-09-18 06:44:16.000000 django-static-adminlte-3.2.0.1/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-18 06:48:15.373172 django-static-adminlte-3.2.0.1/django_static_adminlte/
--rw-r--r--   0 test       (501) staff       (20)      143 2023-09-18 06:32:52.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:19.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/admin.py
--rw-r--r--   0 test       (501) staff       (20)      117 2018-03-27 01:14:03.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-18 06:48:15.374609 django-static-adminlte-3.2.0.1/django_static_adminlte/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2018-03-27 01:14:03.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/models.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:13.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/tests.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:11.000000 django-static-adminlte-3.2.0.1/django_static_adminlte/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-18 06:48:15.374472 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2853 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      570 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        7 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       23 2023-09-18 06:48:15.000000 django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        7 2018-03-27 01:07:34.000000 django-static-adminlte-3.2.0.1/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-18 06:48:15.375024 django-static-adminlte-3.2.0.1/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1192 2023-09-18 06:44:24.000000 django-static-adminlte-3.2.0.1/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.101572 django-static-adminlte-3.2.0.2/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-16 13:11:47.000000 django-static-adminlte-3.2.0.2/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      159 2024-04-16 09:19:38.000000 django-static-adminlte-3.2.0.2/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2247 2024-04-16 13:15:40.101417 django-static-adminlte-3.2.0.2/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1641 2024-04-16 13:10:35.000000 django-static-adminlte-3.2.0.2/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:39.994834 django-static-adminlte-3.2.0.2/django_static_adminlte/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-18 06:43:47.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/.DS_Store
+-rw-r--r--   0 test       (501) staff       (20)      142 2024-04-16 09:20:07.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:19.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      117 2018-03-27 01:14:03.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:39.995641 django-static-adminlte-3.2.0.2/django_static_adminlte/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2018-03-27 01:14:03.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:15.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:39.995731 django-static-adminlte-3.2.0.2/django_static_adminlte/static/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-18 07:41:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/.DS_Store
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:39.996034 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-18 07:41:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/.DS_Store
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.011355 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/
+-rw-rw-r--   0 test       (501) staff       (20)  1559615 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/adminlte.css
+-rw-rw-r--   0 test       (501) staff       (20)  2405822 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/adminlte.css.map
+-rw-rw-r--   0 test       (501) staff       (20)  1396747 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/adminlte.min.css
+-rw-rw-r--   0 test       (501) staff       (20)  3846965 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/adminlte.min.css.map
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.080927 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/
+-rw-rw-r--   0 test       (501) staff       (20)   393293 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.components.css
+-rw-rw-r--   0 test       (501) staff       (20)   601309 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.components.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   358450 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.components.min.css
+-rw-rw-r--   0 test       (501) staff       (20)   951543 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.components.min.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   812720 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.core.css
+-rw-rw-r--   0 test       (501) staff       (20)  1357088 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.core.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   715345 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.core.min.css
+-rw-rw-r--   0 test       (501) staff       (20)  2046784 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.core.min.css.map
+-rw-rw-r--   0 test       (501) staff       (20)    40433 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.extra-components.css
+-rw-rw-r--   0 test       (501) staff       (20)   138081 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.extra-components.css.map
+-rw-rw-r--   0 test       (501) staff       (20)    34347 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.extra-components.min.css
+-rw-rw-r--   0 test       (501) staff       (20)    89877 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.extra-components.min.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   993233 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.light.css
+-rw-rw-r--   0 test       (501) staff       (20)  1741831 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.light.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   875714 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.light.min.css
+-rw-rw-r--   0 test       (501) staff       (20)  2622810 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.light.min.css.map
+-rw-rw-r--   0 test       (501) staff       (20)    19814 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.pages.css
+-rw-rw-r--   0 test       (501) staff       (20)   104787 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.pages.css.map
+-rw-rw-r--   0 test       (501) staff       (20)    16448 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.pages.min.css
+-rw-rw-r--   0 test       (501) staff       (20)    60623 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.pages.min.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   317481 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.plugins.css
+-rw-rw-r--   0 test       (501) staff       (20)   489273 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.plugins.css.map
+-rw-rw-r--   0 test       (501) staff       (20)   290881 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.plugins.min.css
+-rw-rw-r--   0 test       (501) staff       (20)   436535 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/css/alt/adminlte.plugins.min.css.map
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.097781 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/
+-rw-rw-r--   0 test       (501) staff       (20)     2637 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/AdminLTELogo.png
+-rw-rw-r--   0 test       (501) staff       (20)     8118 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/avatar.png
+-rw-rw-r--   0 test       (501) staff       (20)     8265 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/avatar2.png
+-rw-rw-r--   0 test       (501) staff       (20)     9246 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/avatar3.png
+-rw-rw-r--   0 test       (501) staff       (20)    13543 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/avatar4.png
+-rw-rw-r--   0 test       (501) staff       (20)     7587 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/avatar5.png
+-rw-rw-r--   0 test       (501) staff       (20)   123766 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/boxed-bg.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    43676 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/boxed-bg.png
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.098959 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/
+-rw-rw-r--   0 test       (501) staff       (20)     2162 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/american-express.png
+-rw-rw-r--   0 test       (501) staff       (20)     1577 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/cirrus.png
+-rw-rw-r--   0 test       (501) staff       (20)     1575 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/mastercard.png
+-rw-rw-r--   0 test       (501) staff       (20)     1976 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/paypal.png
+-rw-rw-r--   0 test       (501) staff       (20)     1219 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/paypal2.png
+-rw-rw-r--   0 test       (501) staff       (20)     1062 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/credit/visa.png
+-rw-rw-r--   0 test       (501) staff       (20)      339 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/default-150x150.png
+-rw-rw-r--   0 test       (501) staff       (20)     1139 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/icons.png
+-rw-rw-r--   0 test       (501) staff       (20)   662169 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/photo1.png
+-rw-rw-r--   0 test       (501) staff       (20)   422537 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/photo2.png
+-rw-rw-r--   0 test       (501) staff       (20)   370563 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/photo3.jpg
+-rw-rw-r--   0 test       (501) staff       (20)  1145510 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/photo4.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    45269 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/prod-1.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    32224 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/prod-2.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    21025 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/prod-3.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    26459 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/prod-4.jpg
+-rw-rw-r--   0 test       (501) staff       (20)    32090 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/prod-5.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     2750 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user1-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     6905 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user2-160x160.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     3398 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user3-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     3455 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user4-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     6415 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user5-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     4250 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user6-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     6363 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user7-128x128.jpg
+-rw-rw-r--   0 test       (501) staff       (20)     4983 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/img/user8-128x128.jpg
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.100521 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/
+-rw-rw-r--   0 test       (501) staff       (20)     1171 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/.eslintrc.json
+-rw-rw-r--   0 test       (501) staff       (20)   104260 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/adminlte.js
+-rw-rw-r--   0 test       (501) staff       (20)   179858 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/adminlte.js.map
+-rw-rw-r--   0 test       (501) staff       (20)    46369 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/adminlte.min.js
+-rw-rw-r--   0 test       (501) staff       (20)   135565 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/adminlte.min.js.map
+-rw-rw-r--   0 test       (501) staff       (20)    22628 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/demo.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:40.101133 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/pages/
+-rw-rw-r--   0 test       (501) staff       (20)     7359 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/pages/dashboard.js
+-rw-rw-r--   0 test       (501) staff       (20)     6299 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/pages/dashboard2.js
+-rw-rw-r--   0 test       (501) staff       (20)     3487 2022-02-07 20:33:09.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/static/adminlte/js/pages/dashboard3.js
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:13.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/tests.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-18 06:28:11.000000 django-static-adminlte-3.2.0.2/django_static_adminlte/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-16 13:15:39.995519 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2247 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     5119 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)      102 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       23 2024-04-16 13:15:39.000000 django-static-adminlte-3.2.0.2/django_static_adminlte.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)      102 2024-04-16 13:12:58.000000 django-static-adminlte-3.2.0.2/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-04-16 13:15:40.101615 django-static-adminlte-3.2.0.2/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1249 2024-04-16 13:14:14.000000 django-static-adminlte-3.2.0.2/setup.py
```

### Comparing `django-static-adminlte-3.2.0.1/LICENSE` & `django-static-adminlte-3.2.0.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2017 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-static-adminlte-3.2.0.1/PKG-INFO` & `django-static-adminlte-3.2.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,179 +1,103 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
-00000020: 676f 2d73 7461 7469 632d 6164 6d69 6e6c  go-static-adminl
-00000030: 7465 0a56 6572 7369 6f6e 3a20 332e 322e  te.Version: 3.2.
-00000040: 302e 310a 5375 6d6d 6172 793a 2044 6a61  0.1.Summary: Dja
-00000050: 6e67 6f20 6170 706c 6963 6174 696f 6e20  ngo application 
-00000060: 636f 6e74 6169 6e20 6164 6d69 6e6c 7465  contain adminlte
-00000070: 2073 7461 7469 6320 6669 6c65 732e 0a41   static files..A
-00000080: 7574 686f 723a 2051 7561 6e20 5a69 4a69  uthor: Quan ZiJi
-00000090: 610a 4175 7468 6f72 2d65 6d61 696c 3a20  a.Author-email: 
-000000a0: 7175 616e 7a69 6a69 6140 7a65 6e63 6f72  quanzijia@zencor
-000000b0: 652e 636e 0a4d 6169 6e74 6169 6e65 723a  e.cn.Maintainer:
-000000c0: 2051 7561 6e20 5a69 4a69 610a 4d61 696e   Quan ZiJia.Main
-000000d0: 7461 696e 6572 2d65 6d61 696c 3a20 7175  tainer-email: qu
-000000e0: 616e 7a69 6a69 6140 7a65 6e63 6f72 652e  anzijia@zencore.
-000000f0: 636e 0a4c 6963 656e 7365 3a20 4d49 540a  cn.License: MIT.
-00000100: 4b65 7977 6f72 6473 3a20 646a 616e 676f  Keywords: django
-00000110: 2d73 7461 7469 632d 6164 6d69 6e6c 7465  -static-adminlte
-00000120: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000130: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000140: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-00000150: 6e2f 5374 6162 6c65 0a43 6c61 7373 6966  n/Stable.Classif
-00000160: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000170: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000180: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-00000190: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-000001a0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-000001b0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-000001c0: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-000001d0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000001e0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001f0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000200: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000210: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000220: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 203a 3a20 4f6e 6c79 0a52 6571 7569 7265   :: Only.Require
-00000270: 733a 2064 6a61 6e67 6f0a 4465 7363 7269  s: django.Descri
-00000280: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000290: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-000002a0: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-000002b0: 4c49 4345 4e53 450a 0a23 2064 6a61 6e67  LICENSE..# djang
-000002c0: 6f2d 7374 6174 6963 2d61 646d 696e 6c74  o-static-adminlt
-000002d0: 650a 0a44 6a61 6e67 6f20 6170 706c 6963  e..Django applic
-000002e0: 6174 696f 6e20 636f 6e74 6169 6e20 6164  ation contain ad
-000002f0: 6d69 6e6c 7465 2073 7461 7469 6320 6669  minlte static fi
-00000300: 6c65 732e 0a0a 2323 2049 6e73 7461 6c6c  les...## Install
-00000310: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
-00000320: 6c20 646a 616e 676f 2d73 7461 7469 632d  l django-static-
-00000330: 6164 6d69 6e6c 7465 0a60 6060 0a0a 2323  adminlte.```..##
-00000340: 204c 6963 656e 7365 730a 0a2d 2041 6c6c   Licenses..- All
-00000350: 2072 6573 6f75 7263 6520 6669 6c65 7320   resource files 
-00000360: 6f66 2041 444d 494e 4c54 4520 6172 6520  of ADMINLTE are 
-00000370: 756e 7a69 7020 6672 6f6d 2041 646d 696e  unzip from Admin
-00000380: 4c54 452d 782e 782e 782e 7461 722e 677a  LTE-x.x.x.tar.gz
-00000390: 2077 6869 6368 2064 6f77 6e6c 6f61 6420   which download 
-000003a0: 6672 6f6d 2068 7474 7073 3a2f 2f61 646d  from https://adm
-000003b0: 696e 6c74 652e 696f 2f20 7769 7468 6f75  inlte.io/ withou
-000003c0: 7420 616e 7920 6368 616e 6765 732e 0a2d  t any changes..-
-000003d0: 2041 6c6c 2072 6573 6f75 7263 6520 6669   All resource fi
-000003e0: 6c65 7320 6f66 2041 444d 494e 4c54 4520  les of ADMINLTE 
-000003f0: 6f62 6579 2041 444d 494e 4c54 4520 4c69  obey ADMINLTE Li
-00000400: 6365 6e73 652c 2073 6565 2064 6574 6169  cense, see detai
-00000410: 6c73 2061 7420 6874 7470 733a 2f2f 6769  ls at https://gi
-00000420: 7468 7562 2e63 6f6d 2f43 6f6c 6f72 6c69  thub.com/Colorli
-00000430: 6248 512f 4164 6d69 6e4c 5445 2f62 6c6f  bHQ/AdminLTE/blo
-00000440: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00000450: 2e0a 2d20 5765 2064 6f6e 2774 2067 7561  ..- We don't gua
-00000460: 7261 6e74 6565 2074 6865 206c 6174 6573  rantee the lates
-00000470: 7420 6a51 7565 7279 2076 6572 7369 6f6e  t jQuery version
-00000480: 2e0a 0a0a 2323 2055 7361 6765 0a0a 2a2a  ....## Usage..**
-00000490: 7072 6f2f 7365 7474 696e 6773 2e70 792a  pro/settings.py*
-000004a0: 2a0a 0a60 6060 7079 7468 6f6e 0a49 4e53  *..```python.INS
-000004b0: 5441 4c4c 4544 5f41 5050 5320 3d20 5b0a  TALLED_APPS = [.
-000004c0: 2020 2020 2e2e 2e0a 2020 2020 2264 6a61      ....    "dja
-000004d0: 6e67 6f5f 7374 6174 6963 5f66 6f6e 7461  ngo_static_fonta
-000004e0: 7765 736f 6d65 222c 0a20 2020 2022 646a  wesome",.    "dj
-000004f0: 616e 676f 5f73 7461 7469 635f 696f 6e69  ango_static_ioni
-00000500: 636f 6e73 222c 0a20 2020 2022 646a 616e  cons",.    "djan
-00000510: 676f 5f73 7461 7469 635f 6a71 7565 7279  go_static_jquery
-00000520: 3322 2c0a 2020 2020 2264 6a61 6e67 6f5f  3",.    "django_
-00000530: 7374 6174 6963 5f62 6f6f 7473 7472 6170  static_bootstrap
-00000540: 222c 0a20 2020 2022 646a 616e 676f 5f73  ",.    "django_s
-00000550: 7461 7469 635f 6164 6d69 6e6c 7465 222c  tatic_adminlte",
-00000560: 0a20 2020 202e 2e2e 0a5d 0a60 6060 0a0a  .    ....].```..
-00000570: 2a2a 6170 702f 7465 6d70 6c61 7465 2f61  **app/template/a
-00000580: 7070 2f69 6e64 6578 2e68 746d 6c2a 2a0a  pp/index.html**.
-00000590: 0a60 6060 6874 6d6c 0a7b 2520 6c6f 6164  .```html.{% load
-000005a0: 2073 7461 7469 6366 696c 6573 2025 7d0a   staticfiles %}.
-000005b0: 0a7b 2520 626c 6f63 6b20 7374 796c 6520  .{% block style 
-000005c0: 257d 0a20 2020 203c 6c69 6e6b 2072 656c  %}.    <link rel
-000005d0: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-000005e0: 6566 3d22 7b25 2073 7461 7469 6320 2262  ef="{% static "b
-000005f0: 6f6f 7473 7472 6170 2f63 7373 2f62 6f6f  ootstrap/css/boo
-00000600: 7473 7472 6170 2e6d 696e 2e63 7373 2220  tstrap.min.css" 
-00000610: 257d 223e 0a20 2020 203c 6c69 6e6b 2072  %}">.    <link r
-00000620: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
-00000630: 6872 6566 3d22 7b25 2073 7461 7469 6320  href="{% static 
-00000640: 2266 6f6e 7461 7765 736f 6d65 2f63 7373  "fontawesome/css
-00000650: 2f61 6c6c 2e6d 696e 2e63 7373 2220 257d  /all.min.css" %}
-00000660: 223e 0a20 2020 203c 6c69 6e6b 2072 656c  ">.    <link rel
-00000670: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-00000680: 6566 3d22 7b25 2073 7461 7469 6320 2269  ef="{% static "i
-00000690: 6f6e 6963 6f6e 732f 6373 732f 696f 6e69  onicons/css/ioni
-000006a0: 636f 6e73 2e63 7373 2220 257d 223e 0a20  cons.css" %}">. 
-000006b0: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
-000006c0: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
-000006d0: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
-000006e0: 6c74 652f 6373 732f 4164 6d69 6e4c 5445  lte/css/AdminLTE
-000006f0: 2e6d 696e 2e63 7373 2220 257d 223e 0a20  .min.css" %}">. 
-00000700: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
-00000710: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
-00000720: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
-00000730: 6c74 652f 6373 732f 736b 696e 732f 5f61  lte/css/skins/_a
-00000740: 6c6c 2d73 6b69 6e73 2e6d 696e 2e63 7373  ll-skins.min.css
-00000750: 2220 257d 223e 0a20 2020 203c 212d 2d5b  " %}">.    <!--[
-00000760: 6966 206c 7420 4945 2039 5d3e 0a20 2020  if lt IE 9]>.   
-00000770: 203c 7363 7269 7074 2073 7263 3d22 7b25   <script src="{%
-00000780: 2073 7461 7469 6320 2268 746d 6c35 7368   static "html5sh
-00000790: 6976 2f68 746d 6c35 7368 6976 2e6d 696e  iv/html5shiv.min
-000007a0: 2e6a 7322 2025 7d22 3e3c 2f73 6372 6970  .js" %}"></scrip
-000007b0: 743e 0a20 2020 203c 7363 7269 7074 2073  t>.    <script s
-000007c0: 7263 3d22 7b25 2073 7461 7469 6320 2272  rc="{% static "r
-000007d0: 6573 706f 6e64 2f72 6573 706f 6e64 2e6d  espond/respond.m
-000007e0: 696e 2e6a 7322 2025 7d22 3e3c 2f73 6372  in.js" %}"></scr
-000007f0: 6970 743e 0a20 2020 203c 215b 656e 6469  ipt>.    <![endi
-00000800: 665d 2d2d 3e0a 7b25 2065 6e64 626c 6f63  f]-->.{% endbloc
-00000810: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2073  k %}..{% block s
-00000820: 6372 6970 7420 257d 0a20 2020 203c 7363  cript %}.    <sc
-00000830: 7269 7074 2073 7263 3d22 7b25 2073 7461  ript src="{% sta
-00000840: 7469 6320 226a 7175 6572 792f 6a71 7565  tic "jquery/jque
-00000850: 7279 2e6a 7322 2025 7d22 3e3c 2f73 6372  ry.js" %}"></scr
-00000860: 6970 743e 0a20 2020 203c 7363 7269 7074  ipt>.    <script
-00000870: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
-00000880: 2262 6f6f 7473 7472 6170 2f6a 732f 626f  "bootstrap/js/bo
-00000890: 6f74 7374 7261 702e 6d69 6e2e 6a73 2220  otstrap.min.js" 
-000008a0: 257d 223e 3c2f 7363 7269 7074 3e0a 2020  %}"></script>.  
-000008b0: 2020 3c73 6372 6970 7420 7372 633d 227b    <script src="{
-000008c0: 2520 7374 6174 6963 2022 6a71 7565 7279  % static "jquery
-000008d0: 2d73 6c69 6d73 6372 6f6c 6c2f 6a71 7565  -slimscroll/jque
-000008e0: 7279 2e73 6c69 6d73 6372 6f6c 6c2e 6d69  ry.slimscroll.mi
-000008f0: 6e2e 6a73 2220 257d 223e 3c2f 7363 7269  n.js" %}"></scri
-00000900: 7074 3e0a 2020 2020 3c73 6372 6970 7420  pt>.    <script 
-00000910: 7372 633d 227b 2520 7374 6174 6963 2022  src="{% static "
-00000920: 6661 7374 636c 6963 6b2f 6661 7374 636c  fastclick/fastcl
-00000930: 6963 6b2e 6a73 2220 257d 223e 3c2f 7363  ick.js" %}"></sc
-00000940: 7269 7074 3e0a 2020 2020 3c73 6372 6970  ript>.    <scrip
-00000950: 7420 7372 633d 227b 2520 7374 6174 6963  t src="{% static
-00000960: 2022 6164 6d69 6e6c 7465 2f6a 732f 6164   "adminlte/js/ad
-00000970: 6d69 6e6c 7465 2e6d 696e 2e6a 7322 2025  minlte.min.js" %
-00000980: 7d22 3e3c 2f73 6372 6970 743e 0a20 2020  }"></script>.   
-00000990: 203c 7363 7269 7074 3e0a 2020 2020 2020   <script>.      
-000009a0: 2020 2428 646f 6375 6d65 6e74 292e 7265    $(document).re
-000009b0: 6164 7928 6675 6e63 7469 6f6e 2028 2920  ady(function () 
-000009c0: 7b0a 2020 2020 2020 2020 2020 2020 2428  {.            $(
-000009d0: 272e 7369 6465 6261 722d 6d65 6e75 2729  '.sidebar-menu')
-000009e0: 2e74 7265 6528 290a 2020 2020 2020 2020  .tree().        
-000009f0: 7d29 3b0a 2020 2020 3c2f 7363 7269 7074  });.    </script
-00000a00: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-00000a10: 0a60 6060 0a0a 2323 2041 626f 7574 2072  .```..## About r
-00000a20: 656c 6561 7365 730a 0a2d 2054 6865 2066  eleases..- The f
-00000a30: 6972 7374 206e 756d 6265 7220 6973 206f  irst number is o
-00000a40: 7572 2072 656c 6561 7365 206e 756d 6265  ur release numbe
-00000a50: 722e 0a2d 2054 6865 206f 7468 6572 2074  r..- The other t
-00000a60: 6872 6565 206e 756d 6265 7273 2061 7265  hree numbers are
-00000a70: 2074 6865 2073 616d 6520 7769 7468 2041   the same with A
-00000a80: 444d 494e 4c54 4527 7320 7265 6c65 6173  DMINLTE's releas
-00000a90: 6520 7665 7273 696f 6e2e 0a0a 2323 2052  e version...## R
-00000aa0: 656c 6561 7365 730a 0a23 2323 2032 2e34  eleases..### 2.4
-00000ab0: 2e33 0a0a 2d20 4669 7273 7420 7265 6c65  .3..- First rele
-00000ac0: 6173 652e 0a0a 2323 2320 322e 342e 332e  ase...### 2.4.3.
-00000ad0: 320a 0a2d 2055 7064 6174 652e 0a0a 2323  2..- Update...##
-00000ae0: 2320 322e 342e 332e 330a 0a2d 2044 6f63  # 2.4.3.3..- Doc
-00000af0: 2075 7064 6174 652e 0a0a 2323 2320 332e   update...### 3.
-00000b00: 322e 302e 310a 0a2d 2055 7067 7261 6465  2.0.1..- Upgrade
-00000b10: 2061 646d 696e 6c74 6520 746f 2033 2e32   adminlte to 3.2
-00000b20: 2e30 2e0a 0a                             .0...
+00000000: 2320 646a 616e 676f 2d73 7461 7469 632d  # django-static-
+00000010: 6164 6d69 6e6c 7465 0a0a 446a 616e 676f  adminlte..Django
+00000020: 2061 7070 6c69 6361 7469 6f6e 2063 6f6e   application con
+00000030: 7461 696e 2061 646d 696e 6c74 6520 7374  tain adminlte st
+00000040: 6174 6963 2066 696c 6573 2e0a 0a23 2320  atic files...## 
+00000050: 496e 7374 616c 6c0a 0a60 6060 0a70 6970  Install..```.pip
+00000060: 2069 6e73 7461 6c6c 2064 6a61 6e67 6f2d   install django-
+00000070: 7374 6174 6963 2d61 646d 696e 6c74 650a  static-adminlte.
+00000080: 6060 600a 0a23 2320 4c69 6365 6e73 6573  ```..## Licenses
+00000090: 0a0a 2d20 416c 6c20 7265 736f 7572 6365  ..- All resource
+000000a0: 2066 696c 6573 206f 6620 4144 4d49 4e4c   files of ADMINL
+000000b0: 5445 2061 7265 2075 6e7a 6970 2066 726f  TE are unzip fro
+000000c0: 6d20 4164 6d69 6e4c 5445 2d78 2e78 2e78  m AdminLTE-x.x.x
+000000d0: 2e74 6172 2e67 7a20 7768 6963 6820 646f  .tar.gz which do
+000000e0: 776e 6c6f 6164 2066 726f 6d20 6874 7470  wnload from http
+000000f0: 733a 2f2f 6164 6d69 6e6c 7465 2e69 6f2f  s://adminlte.io/
+00000100: 2077 6974 686f 7574 2061 6e79 2063 6861   without any cha
+00000110: 6e67 6573 2e0a 2d20 416c 6c20 7265 736f  nges..- All reso
+00000120: 7572 6365 2066 696c 6573 206f 6620 4144  urce files of AD
+00000130: 4d49 4e4c 5445 206f 6265 7920 4144 4d49  MINLTE obey ADMI
+00000140: 4e4c 5445 204c 6963 656e 7365 2c20 7365  NLTE License, se
+00000150: 6520 6465 7461 696c 7320 6174 2068 7474  e details at htt
+00000160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000170: 436f 6c6f 726c 6962 4851 2f41 646d 696e  ColorlibHQ/Admin
+00000180: 4c54 452f 626c 6f62 2f6d 6173 7465 722f  LTE/blob/master/
+00000190: 4c49 4345 4e53 452e 0a2d 2057 6520 646f  LICENSE..- We do
+000001a0: 6e27 7420 6775 6172 616e 7465 6520 7468  n't guarantee th
+000001b0: 6520 6c61 7465 7374 206a 5175 6572 7920  e latest jQuery 
+000001c0: 7665 7273 696f 6e2e 0a0a 0a23 2320 5573  version....## Us
+000001d0: 6167 650a 0a2a 2a70 726f 2f73 6574 7469  age..**pro/setti
+000001e0: 6e67 732e 7079 2a2a 0a0a 6060 6070 7974  ngs.py**..```pyt
+000001f0: 686f 6e0a 494e 5354 414c 4c45 445f 4150  hon.INSTALLED_AP
+00000200: 5053 203d 205b 0a20 2020 202e 2e2e 0a20  PS = [.    .... 
+00000210: 2020 2022 646a 616e 676f 5f73 7461 7469     "django_stati
+00000220: 635f 666f 6e74 6177 6573 6f6d 6522 2c0a  c_fontawesome",.
+00000230: 2020 2020 2264 6a61 6e67 6f5f 7374 6174      "django_stat
+00000240: 6963 5f69 6f6e 6963 6f6e 7322 2c0a 2020  ic_ionicons",.  
+00000250: 2020 2264 6a61 6e67 6f5f 7374 6174 6963    "django_static
+00000260: 5f6a 7175 6572 7933 222c 0a20 2020 2022  _jquery3",.    "
+00000270: 646a 616e 676f 5f73 7461 7469 635f 626f  django_static_bo
+00000280: 6f74 7374 7261 7022 2c0a 2020 2020 2264  otstrap",.    "d
+00000290: 6a61 6e67 6f5f 7374 6174 6963 5f61 646d  jango_static_adm
+000002a0: 696e 6c74 6522 2c0a 2020 2020 2e2e 2e0a  inlte",.    ....
+000002b0: 5d0a 6060 600a 0a2a 2a61 7070 2f74 656d  ].```..**app/tem
+000002c0: 706c 6174 652f 6170 702f 696e 6465 782e  plate/app/index.
+000002d0: 6874 6d6c 2a2a 0a0a 6060 6068 746d 6c0a  html**..```html.
+000002e0: 7b25 206c 6f61 6420 7374 6174 6963 2025  {% load static %
+000002f0: 7d0a 0a7b 2520 626c 6f63 6b20 7374 796c  }..{% block styl
+00000300: 6520 257d 0a3c 6c69 6e6b 2072 656c 3d22  e %}.<link rel="
+00000310: 7374 796c 6573 6865 6574 2220 6872 6566  stylesheet" href
+00000320: 3d22 7b25 2073 7461 7469 6320 2262 6f6f  ="{% static "boo
+00000330: 7473 7472 6170 2f63 7373 2f62 6f6f 7473  tstrap/css/boots
+00000340: 7472 6170 2e6d 696e 2e63 7373 2220 257d  trap.min.css" %}
+00000350: 223e 0a3c 6c69 6e6b 2072 656c 3d22 7374  ">.<link rel="st
+00000360: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
+00000370: 7b25 2073 7461 7469 6320 2266 6f6e 7461  {% static "fonta
+00000380: 7765 736f 6d65 2f63 7373 2f61 6c6c 2e6d  wesome/css/all.m
+00000390: 696e 2e63 7373 2220 257d 223e 0a3c 6c69  in.css" %}">.<li
+000003a0: 6e6b 2072 656c 3d22 7374 796c 6573 6865  nk rel="styleshe
+000003b0: 6574 2220 6872 6566 3d22 7b25 2073 7461  et" href="{% sta
+000003c0: 7469 6320 2269 6f6e 6963 6f6e 732f 6373  tic "ionicons/cs
+000003d0: 732f 696f 6e69 636f 6e73 2e63 7373 2220  s/ionicons.css" 
+000003e0: 257d 223e 0a3c 6c69 6e6b 2072 656c 3d22  %}">.<link rel="
+000003f0: 7374 796c 6573 6865 6574 2220 6872 6566  stylesheet" href
+00000400: 3d22 7b25 2073 7461 7469 6320 2261 646d  ="{% static "adm
+00000410: 696e 6c74 652f 6373 732f 6164 6d69 6e6c  inlte/css/adminl
+00000420: 7465 2e6d 696e 2e63 7373 2220 257d 223e  te.min.css" %}">
+00000430: 0a7b 2520 656e 6462 6c6f 636b 2025 7d0a  .{% endblock %}.
+00000440: 0a7b 2520 626c 6f63 6b20 7363 7269 7074  .{% block script
+00000450: 2025 7d0a 3c73 6372 6970 7420 7372 633d   %}.<script src=
+00000460: 227b 2520 7374 6174 6963 2022 6a71 7565  "{% static "jque
+00000470: 7279 2f6a 7175 6572 792e 6a73 2220 257d  ry/jquery.js" %}
+00000480: 223e 3c2f 7363 7269 7074 3e0a 3c73 6372  "></script>.<scr
+00000490: 6970 7420 7372 633d 227b 2520 7374 6174  ipt src="{% stat
+000004a0: 6963 2022 626f 6f74 7374 7261 702f 6a73  ic "bootstrap/js
+000004b0: 2f62 6f6f 7473 7472 6170 2e6d 696e 2e6a  /bootstrap.min.j
+000004c0: 7322 2025 7d22 3e3c 2f73 6372 6970 743e  s" %}"></script>
+000004d0: 0a3c 7363 7269 7074 2073 7263 3d22 7b25  .<script src="{%
+000004e0: 2073 7461 7469 6320 2261 646d 696e 6c74   static "adminlt
+000004f0: 652f 6a73 2f61 646d 696e 6c74 652e 6d69  e/js/adminlte.mi
+00000500: 6e2e 6a73 2220 257d 223e 3c2f 7363 7269  n.js" %}"></scri
+00000510: 7074 3e0a 7b25 2065 6e64 626c 6f63 6b20  pt>.{% endblock 
+00000520: 257d 0a0a 6060 600a 0a23 2320 4162 6f75  %}..```..## Abou
+00000530: 7420 7265 6c65 6173 6573 0a0a 2d20 5468  t releases..- Th
+00000540: 6520 6669 7273 7420 6e75 6d62 6572 2069  e first number i
+00000550: 7320 6f75 7220 7265 6c65 6173 6520 6e75  s our release nu
+00000560: 6d62 6572 2e0a 2d20 5468 6520 6f74 6865  mber..- The othe
+00000570: 7220 7468 7265 6520 6e75 6d62 6572 7320  r three numbers 
+00000580: 6172 6520 7468 6520 7361 6d65 2077 6974  are the same wit
+00000590: 6820 4144 4d49 4e4c 5445 2773 2072 656c  h ADMINLTE's rel
+000005a0: 6561 7365 2076 6572 7369 6f6e 2e0a 0a23  ease version...#
+000005b0: 2320 5265 6c65 6173 6573 0a0a 2323 2320  # Releases..### 
+000005c0: 322e 342e 330a 0a2d 2046 6972 7374 2072  2.4.3..- First r
+000005d0: 656c 6561 7365 2e0a 0a23 2323 2032 2e34  elease...### 2.4
+000005e0: 2e33 2e32 0a0a 2d20 5570 6461 7465 2e0a  .3.2..- Update..
+000005f0: 0a23 2323 2032 2e34 2e33 2e33 0a0a 2d20  .### 2.4.3.3..- 
+00000600: 446f 6320 7570 6461 7465 2e0a 0a23 2323  Doc update...###
+00000610: 2033 2e32 2e30 2e31 0a0a 2d20 5570 6772   3.2.0.1..- Upgr
+00000620: 6164 6520 6164 6d69 6e6c 7465 2074 6f20  ade adminlte to 
+00000630: 332e 322e 302e 0a0a 2323 2320 332e 322e  3.2.0...### 3.2.
+00000640: 302e 320a 0a2d 2046 6978 2073 7461 7469  0.2..- Fix stati
+00000650: 6320 6669 6c65 7320 6d69 7373 696e 6720  c files missing 
+00000660: 7072 6f62 6c65 6d2e 0a                   problem..
```

### Comparing `django-static-adminlte-3.2.0.1/django_static_adminlte.egg-info/PKG-INFO` & `django-static-adminlte-3.2.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,141 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d73 7461 7469 632d 6164 6d69 6e6c  go-static-adminl
 00000030: 7465 0a56 6572 7369 6f6e 3a20 332e 322e  te.Version: 3.2.
-00000040: 302e 310a 5375 6d6d 6172 793a 2044 6a61  0.1.Summary: Dja
+00000040: 302e 320a 5375 6d6d 6172 793a 2044 6a61  0.2.Summary: Dja
 00000050: 6e67 6f20 6170 706c 6963 6174 696f 6e20  ngo application 
 00000060: 636f 6e74 6169 6e20 6164 6d69 6e6c 7465  contain adminlte
 00000070: 2073 7461 7469 6320 6669 6c65 732e 0a41   static files..A
 00000080: 7574 686f 723a 2051 7561 6e20 5a69 4a69  uthor: Quan ZiJi
-00000090: 610a 4175 7468 6f72 2d65 6d61 696c 3a20  a.Author-email: 
-000000a0: 7175 616e 7a69 6a69 6140 7a65 6e63 6f72  quanzijia@zencor
-000000b0: 652e 636e 0a4d 6169 6e74 6169 6e65 723a  e.cn.Maintainer:
-000000c0: 2051 7561 6e20 5a69 4a69 610a 4d61 696e   Quan ZiJia.Main
-000000d0: 7461 696e 6572 2d65 6d61 696c 3a20 7175  tainer-email: qu
-000000e0: 616e 7a69 6a69 6140 7a65 6e63 6f72 652e  anzijia@zencore.
-000000f0: 636e 0a4c 6963 656e 7365 3a20 4d49 540a  cn.License: MIT.
-00000100: 4b65 7977 6f72 6473 3a20 646a 616e 676f  Keywords: django
-00000110: 2d73 7461 7469 632d 6164 6d69 6e6c 7465  -static-adminlte
-00000120: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000130: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000140: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-00000150: 6e2f 5374 6162 6c65 0a43 6c61 7373 6966  n/Stable.Classif
-00000160: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000170: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000180: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-00000190: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-000001a0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-000001b0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-000001c0: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-000001d0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000001e0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001f0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000200: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000210: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000220: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 203a 3a20 4f6e 6c79 0a52 6571 7569 7265   :: Only.Require
-00000270: 733a 2064 6a61 6e67 6f0a 4465 7363 7269  s: django.Descri
-00000280: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000290: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-000002a0: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-000002b0: 4c49 4345 4e53 450a 0a23 2064 6a61 6e67  LICENSE..# djang
-000002c0: 6f2d 7374 6174 6963 2d61 646d 696e 6c74  o-static-adminlt
-000002d0: 650a 0a44 6a61 6e67 6f20 6170 706c 6963  e..Django applic
-000002e0: 6174 696f 6e20 636f 6e74 6169 6e20 6164  ation contain ad
-000002f0: 6d69 6e6c 7465 2073 7461 7469 6320 6669  minlte static fi
-00000300: 6c65 732e 0a0a 2323 2049 6e73 7461 6c6c  les...## Install
-00000310: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
-00000320: 6c20 646a 616e 676f 2d73 7461 7469 632d  l django-static-
-00000330: 6164 6d69 6e6c 7465 0a60 6060 0a0a 2323  adminlte.```..##
-00000340: 204c 6963 656e 7365 730a 0a2d 2041 6c6c   Licenses..- All
-00000350: 2072 6573 6f75 7263 6520 6669 6c65 7320   resource files 
-00000360: 6f66 2041 444d 494e 4c54 4520 6172 6520  of ADMINLTE are 
-00000370: 756e 7a69 7020 6672 6f6d 2041 646d 696e  unzip from Admin
-00000380: 4c54 452d 782e 782e 782e 7461 722e 677a  LTE-x.x.x.tar.gz
-00000390: 2077 6869 6368 2064 6f77 6e6c 6f61 6420   which download 
-000003a0: 6672 6f6d 2068 7474 7073 3a2f 2f61 646d  from https://adm
-000003b0: 696e 6c74 652e 696f 2f20 7769 7468 6f75  inlte.io/ withou
-000003c0: 7420 616e 7920 6368 616e 6765 732e 0a2d  t any changes..-
-000003d0: 2041 6c6c 2072 6573 6f75 7263 6520 6669   All resource fi
-000003e0: 6c65 7320 6f66 2041 444d 494e 4c54 4520  les of ADMINLTE 
-000003f0: 6f62 6579 2041 444d 494e 4c54 4520 4c69  obey ADMINLTE Li
-00000400: 6365 6e73 652c 2073 6565 2064 6574 6169  cense, see detai
-00000410: 6c73 2061 7420 6874 7470 733a 2f2f 6769  ls at https://gi
-00000420: 7468 7562 2e63 6f6d 2f43 6f6c 6f72 6c69  thub.com/Colorli
-00000430: 6248 512f 4164 6d69 6e4c 5445 2f62 6c6f  bHQ/AdminLTE/blo
-00000440: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00000450: 2e0a 2d20 5765 2064 6f6e 2774 2067 7561  ..- We don't gua
-00000460: 7261 6e74 6565 2074 6865 206c 6174 6573  rantee the lates
-00000470: 7420 6a51 7565 7279 2076 6572 7369 6f6e  t jQuery version
-00000480: 2e0a 0a0a 2323 2055 7361 6765 0a0a 2a2a  ....## Usage..**
-00000490: 7072 6f2f 7365 7474 696e 6773 2e70 792a  pro/settings.py*
-000004a0: 2a0a 0a60 6060 7079 7468 6f6e 0a49 4e53  *..```python.INS
-000004b0: 5441 4c4c 4544 5f41 5050 5320 3d20 5b0a  TALLED_APPS = [.
-000004c0: 2020 2020 2e2e 2e0a 2020 2020 2264 6a61      ....    "dja
-000004d0: 6e67 6f5f 7374 6174 6963 5f66 6f6e 7461  ngo_static_fonta
-000004e0: 7765 736f 6d65 222c 0a20 2020 2022 646a  wesome",.    "dj
-000004f0: 616e 676f 5f73 7461 7469 635f 696f 6e69  ango_static_ioni
-00000500: 636f 6e73 222c 0a20 2020 2022 646a 616e  cons",.    "djan
-00000510: 676f 5f73 7461 7469 635f 6a71 7565 7279  go_static_jquery
-00000520: 3322 2c0a 2020 2020 2264 6a61 6e67 6f5f  3",.    "django_
-00000530: 7374 6174 6963 5f62 6f6f 7473 7472 6170  static_bootstrap
-00000540: 222c 0a20 2020 2022 646a 616e 676f 5f73  ",.    "django_s
-00000550: 7461 7469 635f 6164 6d69 6e6c 7465 222c  tatic_adminlte",
-00000560: 0a20 2020 202e 2e2e 0a5d 0a60 6060 0a0a  .    ....].```..
-00000570: 2a2a 6170 702f 7465 6d70 6c61 7465 2f61  **app/template/a
-00000580: 7070 2f69 6e64 6578 2e68 746d 6c2a 2a0a  pp/index.html**.
-00000590: 0a60 6060 6874 6d6c 0a7b 2520 6c6f 6164  .```html.{% load
-000005a0: 2073 7461 7469 6366 696c 6573 2025 7d0a   staticfiles %}.
-000005b0: 0a7b 2520 626c 6f63 6b20 7374 796c 6520  .{% block style 
-000005c0: 257d 0a20 2020 203c 6c69 6e6b 2072 656c  %}.    <link rel
-000005d0: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-000005e0: 6566 3d22 7b25 2073 7461 7469 6320 2262  ef="{% static "b
-000005f0: 6f6f 7473 7472 6170 2f63 7373 2f62 6f6f  ootstrap/css/boo
-00000600: 7473 7472 6170 2e6d 696e 2e63 7373 2220  tstrap.min.css" 
-00000610: 257d 223e 0a20 2020 203c 6c69 6e6b 2072  %}">.    <link r
-00000620: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
-00000630: 6872 6566 3d22 7b25 2073 7461 7469 6320  href="{% static 
-00000640: 2266 6f6e 7461 7765 736f 6d65 2f63 7373  "fontawesome/css
-00000650: 2f61 6c6c 2e6d 696e 2e63 7373 2220 257d  /all.min.css" %}
-00000660: 223e 0a20 2020 203c 6c69 6e6b 2072 656c  ">.    <link rel
-00000670: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-00000680: 6566 3d22 7b25 2073 7461 7469 6320 2269  ef="{% static "i
-00000690: 6f6e 6963 6f6e 732f 6373 732f 696f 6e69  onicons/css/ioni
-000006a0: 636f 6e73 2e63 7373 2220 257d 223e 0a20  cons.css" %}">. 
-000006b0: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
-000006c0: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
-000006d0: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
-000006e0: 6c74 652f 6373 732f 4164 6d69 6e4c 5445  lte/css/AdminLTE
-000006f0: 2e6d 696e 2e63 7373 2220 257d 223e 0a20  .min.css" %}">. 
-00000700: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
-00000710: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
-00000720: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
-00000730: 6c74 652f 6373 732f 736b 696e 732f 5f61  lte/css/skins/_a
-00000740: 6c6c 2d73 6b69 6e73 2e6d 696e 2e63 7373  ll-skins.min.css
-00000750: 2220 257d 223e 0a20 2020 203c 212d 2d5b  " %}">.    <!--[
-00000760: 6966 206c 7420 4945 2039 5d3e 0a20 2020  if lt IE 9]>.   
-00000770: 203c 7363 7269 7074 2073 7263 3d22 7b25   <script src="{%
-00000780: 2073 7461 7469 6320 2268 746d 6c35 7368   static "html5sh
-00000790: 6976 2f68 746d 6c35 7368 6976 2e6d 696e  iv/html5shiv.min
-000007a0: 2e6a 7322 2025 7d22 3e3c 2f73 6372 6970  .js" %}"></scrip
-000007b0: 743e 0a20 2020 203c 7363 7269 7074 2073  t>.    <script s
-000007c0: 7263 3d22 7b25 2073 7461 7469 6320 2272  rc="{% static "r
-000007d0: 6573 706f 6e64 2f72 6573 706f 6e64 2e6d  espond/respond.m
-000007e0: 696e 2e6a 7322 2025 7d22 3e3c 2f73 6372  in.js" %}"></scr
-000007f0: 6970 743e 0a20 2020 203c 215b 656e 6469  ipt>.    <![endi
-00000800: 665d 2d2d 3e0a 7b25 2065 6e64 626c 6f63  f]-->.{% endbloc
-00000810: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2073  k %}..{% block s
-00000820: 6372 6970 7420 257d 0a20 2020 203c 7363  cript %}.    <sc
-00000830: 7269 7074 2073 7263 3d22 7b25 2073 7461  ript src="{% sta
-00000840: 7469 6320 226a 7175 6572 792f 6a71 7565  tic "jquery/jque
-00000850: 7279 2e6a 7322 2025 7d22 3e3c 2f73 6372  ry.js" %}"></scr
-00000860: 6970 743e 0a20 2020 203c 7363 7269 7074  ipt>.    <script
-00000870: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
-00000880: 2262 6f6f 7473 7472 6170 2f6a 732f 626f  "bootstrap/js/bo
-00000890: 6f74 7374 7261 702e 6d69 6e2e 6a73 2220  otstrap.min.js" 
-000008a0: 257d 223e 3c2f 7363 7269 7074 3e0a 2020  %}"></script>.  
-000008b0: 2020 3c73 6372 6970 7420 7372 633d 227b    <script src="{
-000008c0: 2520 7374 6174 6963 2022 6a71 7565 7279  % static "jquery
-000008d0: 2d73 6c69 6d73 6372 6f6c 6c2f 6a71 7565  -slimscroll/jque
-000008e0: 7279 2e73 6c69 6d73 6372 6f6c 6c2e 6d69  ry.slimscroll.mi
-000008f0: 6e2e 6a73 2220 257d 223e 3c2f 7363 7269  n.js" %}"></scri
-00000900: 7074 3e0a 2020 2020 3c73 6372 6970 7420  pt>.    <script 
-00000910: 7372 633d 227b 2520 7374 6174 6963 2022  src="{% static "
-00000920: 6661 7374 636c 6963 6b2f 6661 7374 636c  fastclick/fastcl
-00000930: 6963 6b2e 6a73 2220 257d 223e 3c2f 7363  ick.js" %}"></sc
-00000940: 7269 7074 3e0a 2020 2020 3c73 6372 6970  ript>.    <scrip
-00000950: 7420 7372 633d 227b 2520 7374 6174 6963  t src="{% static
-00000960: 2022 6164 6d69 6e6c 7465 2f6a 732f 6164   "adminlte/js/ad
-00000970: 6d69 6e6c 7465 2e6d 696e 2e6a 7322 2025  minlte.min.js" %
-00000980: 7d22 3e3c 2f73 6372 6970 743e 0a20 2020  }"></script>.   
-00000990: 203c 7363 7269 7074 3e0a 2020 2020 2020   <script>.      
-000009a0: 2020 2428 646f 6375 6d65 6e74 292e 7265    $(document).re
-000009b0: 6164 7928 6675 6e63 7469 6f6e 2028 2920  ady(function () 
-000009c0: 7b0a 2020 2020 2020 2020 2020 2020 2428  {.            $(
-000009d0: 272e 7369 6465 6261 722d 6d65 6e75 2729  '.sidebar-menu')
-000009e0: 2e74 7265 6528 290a 2020 2020 2020 2020  .tree().        
-000009f0: 7d29 3b0a 2020 2020 3c2f 7363 7269 7074  });.    </script
-00000a00: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-00000a10: 0a60 6060 0a0a 2323 2041 626f 7574 2072  .```..## About r
-00000a20: 656c 6561 7365 730a 0a2d 2054 6865 2066  eleases..- The f
-00000a30: 6972 7374 206e 756d 6265 7220 6973 206f  irst number is o
-00000a40: 7572 2072 656c 6561 7365 206e 756d 6265  ur release numbe
-00000a50: 722e 0a2d 2054 6865 206f 7468 6572 2074  r..- The other t
-00000a60: 6872 6565 206e 756d 6265 7273 2061 7265  hree numbers are
-00000a70: 2074 6865 2073 616d 6520 7769 7468 2041   the same with A
-00000a80: 444d 494e 4c54 4527 7320 7265 6c65 6173  DMINLTE's releas
-00000a90: 6520 7665 7273 696f 6e2e 0a0a 2323 2052  e version...## R
-00000aa0: 656c 6561 7365 730a 0a23 2323 2032 2e34  eleases..### 2.4
-00000ab0: 2e33 0a0a 2d20 4669 7273 7420 7265 6c65  .3..- First rele
-00000ac0: 6173 652e 0a0a 2323 2320 322e 342e 332e  ase...### 2.4.3.
-00000ad0: 320a 0a2d 2055 7064 6174 652e 0a0a 2323  2..- Update...##
-00000ae0: 2320 322e 342e 332e 330a 0a2d 2044 6f63  # 2.4.3.3..- Doc
-00000af0: 2075 7064 6174 652e 0a0a 2323 2320 332e   update...### 3.
-00000b00: 322e 302e 310a 0a2d 2055 7067 7261 6465  2.0.1..- Upgrade
-00000b10: 2061 646d 696e 6c74 6520 746f 2033 2e32   adminlte to 3.2
-00000b20: 2e30 2e0a 0a                             .0...
+00000090: 610a 4d61 696e 7461 696e 6572 3a20 5175  a.Maintainer: Qu
+000000a0: 616e 205a 694a 6961 0a4c 6963 656e 7365  an ZiJia.License
+000000b0: 3a20 4d49 540a 4b65 7977 6f72 6473 3a20  : MIT.Keywords: 
+000000c0: 646a 616e 676f 2d73 7461 7469 632d 6164  django-static-ad
+000000d0: 6d69 6e6c 7465 0a43 6c61 7373 6966 6965  minlte.Classifie
+000000e0: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+000000f0: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00000100: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+00000110: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00000120: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000130: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+00000140: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000150: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
+00000160: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
+00000170: 7320 3a3a 2050 7974 686f 6e20 4d6f 6475  s :: Python Modu
+00000180: 6c65 730a 436c 6173 7369 6669 6572 3a20  les.Classifier: 
+00000190: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001b0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+000001c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001e0: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000001f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000210: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0a44  n :: 3 :: Only.D
+00000220: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000230: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000240: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000250: 696c 653a 204c 4943 454e 5345 0a0a 2320  ile: LICENSE..# 
+00000260: 646a 616e 676f 2d73 7461 7469 632d 6164  django-static-ad
+00000270: 6d69 6e6c 7465 0a0a 446a 616e 676f 2061  minlte..Django a
+00000280: 7070 6c69 6361 7469 6f6e 2063 6f6e 7461  pplication conta
+00000290: 696e 2061 646d 696e 6c74 6520 7374 6174  in adminlte stat
+000002a0: 6963 2066 696c 6573 2e0a 0a23 2320 496e  ic files...## In
+000002b0: 7374 616c 6c0a 0a60 6060 0a70 6970 2069  stall..```.pip i
+000002c0: 6e73 7461 6c6c 2064 6a61 6e67 6f2d 7374  nstall django-st
+000002d0: 6174 6963 2d61 646d 696e 6c74 650a 6060  atic-adminlte.``
+000002e0: 600a 0a23 2320 4c69 6365 6e73 6573 0a0a  `..## Licenses..
+000002f0: 2d20 416c 6c20 7265 736f 7572 6365 2066  - All resource f
+00000300: 696c 6573 206f 6620 4144 4d49 4e4c 5445  iles of ADMINLTE
+00000310: 2061 7265 2075 6e7a 6970 2066 726f 6d20   are unzip from 
+00000320: 4164 6d69 6e4c 5445 2d78 2e78 2e78 2e74  AdminLTE-x.x.x.t
+00000330: 6172 2e67 7a20 7768 6963 6820 646f 776e  ar.gz which down
+00000340: 6c6f 6164 2066 726f 6d20 6874 7470 733a  load from https:
+00000350: 2f2f 6164 6d69 6e6c 7465 2e69 6f2f 2077  //adminlte.io/ w
+00000360: 6974 686f 7574 2061 6e79 2063 6861 6e67  ithout any chang
+00000370: 6573 2e0a 2d20 416c 6c20 7265 736f 7572  es..- All resour
+00000380: 6365 2066 696c 6573 206f 6620 4144 4d49  ce files of ADMI
+00000390: 4e4c 5445 206f 6265 7920 4144 4d49 4e4c  NLTE obey ADMINL
+000003a0: 5445 204c 6963 656e 7365 2c20 7365 6520  TE License, see 
+000003b0: 6465 7461 696c 7320 6174 2068 7474 7073  details at https
+000003c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 436f  ://github.com/Co
+000003d0: 6c6f 726c 6962 4851 2f41 646d 696e 4c54  lorlibHQ/AdminLT
+000003e0: 452f 626c 6f62 2f6d 6173 7465 722f 4c49  E/blob/master/LI
+000003f0: 4345 4e53 452e 0a2d 2057 6520 646f 6e27  CENSE..- We don'
+00000400: 7420 6775 6172 616e 7465 6520 7468 6520  t guarantee the 
+00000410: 6c61 7465 7374 206a 5175 6572 7920 7665  latest jQuery ve
+00000420: 7273 696f 6e2e 0a0a 0a23 2320 5573 6167  rsion....## Usag
+00000430: 650a 0a2a 2a70 726f 2f73 6574 7469 6e67  e..**pro/setting
+00000440: 732e 7079 2a2a 0a0a 6060 6070 7974 686f  s.py**..```pytho
+00000450: 6e0a 494e 5354 414c 4c45 445f 4150 5053  n.INSTALLED_APPS
+00000460: 203d 205b 0a20 2020 202e 2e2e 0a20 2020   = [.    ....   
+00000470: 2022 646a 616e 676f 5f73 7461 7469 635f   "django_static_
+00000480: 666f 6e74 6177 6573 6f6d 6522 2c0a 2020  fontawesome",.  
+00000490: 2020 2264 6a61 6e67 6f5f 7374 6174 6963    "django_static
+000004a0: 5f69 6f6e 6963 6f6e 7322 2c0a 2020 2020  _ionicons",.    
+000004b0: 2264 6a61 6e67 6f5f 7374 6174 6963 5f6a  "django_static_j
+000004c0: 7175 6572 7933 222c 0a20 2020 2022 646a  query3",.    "dj
+000004d0: 616e 676f 5f73 7461 7469 635f 626f 6f74  ango_static_boot
+000004e0: 7374 7261 7022 2c0a 2020 2020 2264 6a61  strap",.    "dja
+000004f0: 6e67 6f5f 7374 6174 6963 5f61 646d 696e  ngo_static_admin
+00000500: 6c74 6522 2c0a 2020 2020 2e2e 2e0a 5d0a  lte",.    ....].
+00000510: 6060 600a 0a2a 2a61 7070 2f74 656d 706c  ```..**app/templ
+00000520: 6174 652f 6170 702f 696e 6465 782e 6874  ate/app/index.ht
+00000530: 6d6c 2a2a 0a0a 6060 6068 746d 6c0a 7b25  ml**..```html.{%
+00000540: 206c 6f61 6420 7374 6174 6963 2025 7d0a   load static %}.
+00000550: 0a7b 2520 626c 6f63 6b20 7374 796c 6520  .{% block style 
+00000560: 257d 0a3c 6c69 6e6b 2072 656c 3d22 7374  %}.<link rel="st
+00000570: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
+00000580: 7b25 2073 7461 7469 6320 2262 6f6f 7473  {% static "boots
+00000590: 7472 6170 2f63 7373 2f62 6f6f 7473 7472  trap/css/bootstr
+000005a0: 6170 2e6d 696e 2e63 7373 2220 257d 223e  ap.min.css" %}">
+000005b0: 0a3c 6c69 6e6b 2072 656c 3d22 7374 796c  .<link rel="styl
+000005c0: 6573 6865 6574 2220 6872 6566 3d22 7b25  esheet" href="{%
+000005d0: 2073 7461 7469 6320 2266 6f6e 7461 7765   static "fontawe
+000005e0: 736f 6d65 2f63 7373 2f61 6c6c 2e6d 696e  some/css/all.min
+000005f0: 2e63 7373 2220 257d 223e 0a3c 6c69 6e6b  .css" %}">.<link
+00000600: 2072 656c 3d22 7374 796c 6573 6865 6574   rel="stylesheet
+00000610: 2220 6872 6566 3d22 7b25 2073 7461 7469  " href="{% stati
+00000620: 6320 2269 6f6e 6963 6f6e 732f 6373 732f  c "ionicons/css/
+00000630: 696f 6e69 636f 6e73 2e63 7373 2220 257d  ionicons.css" %}
+00000640: 223e 0a3c 6c69 6e6b 2072 656c 3d22 7374  ">.<link rel="st
+00000650: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
+00000660: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
+00000670: 6c74 652f 6373 732f 6164 6d69 6e6c 7465  lte/css/adminlte
+00000680: 2e6d 696e 2e63 7373 2220 257d 223e 0a7b  .min.css" %}">.{
+00000690: 2520 656e 6462 6c6f 636b 2025 7d0a 0a7b  % endblock %}..{
+000006a0: 2520 626c 6f63 6b20 7363 7269 7074 2025  % block script %
+000006b0: 7d0a 3c73 6372 6970 7420 7372 633d 227b  }.<script src="{
+000006c0: 2520 7374 6174 6963 2022 6a71 7565 7279  % static "jquery
+000006d0: 2f6a 7175 6572 792e 6a73 2220 257d 223e  /jquery.js" %}">
+000006e0: 3c2f 7363 7269 7074 3e0a 3c73 6372 6970  </script>.<scrip
+000006f0: 7420 7372 633d 227b 2520 7374 6174 6963  t src="{% static
+00000700: 2022 626f 6f74 7374 7261 702f 6a73 2f62   "bootstrap/js/b
+00000710: 6f6f 7473 7472 6170 2e6d 696e 2e6a 7322  ootstrap.min.js"
+00000720: 2025 7d22 3e3c 2f73 6372 6970 743e 0a3c   %}"></script>.<
+00000730: 7363 7269 7074 2073 7263 3d22 7b25 2073  script src="{% s
+00000740: 7461 7469 6320 2261 646d 696e 6c74 652f  tatic "adminlte/
+00000750: 6a73 2f61 646d 696e 6c74 652e 6d69 6e2e  js/adminlte.min.
+00000760: 6a73 2220 257d 223e 3c2f 7363 7269 7074  js" %}"></script
+00000770: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000780: 0a0a 6060 600a 0a23 2320 4162 6f75 7420  ..```..## About 
+00000790: 7265 6c65 6173 6573 0a0a 2d20 5468 6520  releases..- The 
+000007a0: 6669 7273 7420 6e75 6d62 6572 2069 7320  first number is 
+000007b0: 6f75 7220 7265 6c65 6173 6520 6e75 6d62  our release numb
+000007c0: 6572 2e0a 2d20 5468 6520 6f74 6865 7220  er..- The other 
+000007d0: 7468 7265 6520 6e75 6d62 6572 7320 6172  three numbers ar
+000007e0: 6520 7468 6520 7361 6d65 2077 6974 6820  e the same with 
+000007f0: 4144 4d49 4e4c 5445 2773 2072 656c 6561  ADMINLTE's relea
+00000800: 7365 2076 6572 7369 6f6e 2e0a 0a23 2320  se version...## 
+00000810: 5265 6c65 6173 6573 0a0a 2323 2320 322e  Releases..### 2.
+00000820: 342e 330a 0a2d 2046 6972 7374 2072 656c  4.3..- First rel
+00000830: 6561 7365 2e0a 0a23 2323 2032 2e34 2e33  ease...### 2.4.3
+00000840: 2e32 0a0a 2d20 5570 6461 7465 2e0a 0a23  .2..- Update...#
+00000850: 2323 2032 2e34 2e33 2e33 0a0a 2d20 446f  ## 2.4.3.3..- Do
+00000860: 6320 7570 6461 7465 2e0a 0a23 2323 2033  c update...### 3
+00000870: 2e32 2e30 2e31 0a0a 2d20 5570 6772 6164  .2.0.1..- Upgrad
+00000880: 6520 6164 6d69 6e6c 7465 2074 6f20 332e  e adminlte to 3.
+00000890: 322e 302e 0a0a 2323 2320 332e 322e 302e  2.0...### 3.2.0.
+000008a0: 320a 0a2d 2046 6978 2073 7461 7469 6320  2..- Fix static 
+000008b0: 6669 6c65 7320 6d69 7373 696e 6720 7072  files missing pr
+000008c0: 6f62 6c65 6d2e 0a                        oblem..
```

### Comparing `django-static-adminlte-3.2.0.1/setup.py` & `django-static-adminlte-3.2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import os
 from setuptools import setup
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(here, 'README.md'), "r", encoding="utf-8") as fobj:
+with open(os.path.join(here, "README.md"), "r", encoding="utf-8") as fobj:
     long_description = fobj.read()
 
-requires = [
-    "django",
-]
+requires = []
+with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
+    requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-static-adminlte",
-    version="3.2.0.1",
+    version="3.2.0.2",
     description="Django application contain adminlte static files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Quan ZiJia",
-    author_email="quanzijia@zencore.cn",
     maintainer="Quan ZiJia",
-    maintainer_email="quanzijia@zencore.cn",
     license="MIT",
+    license_files=("LICENSE",),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
     ],
-    keywords=['django-static-adminlte'],
+    keywords=["django-static-adminlte"],
     packages=find_packages(".", exclude=[]),
-    requires=requires,
     install_requires=requires,
     zip_safe=False,
     include_package_data=True,
 )
```

