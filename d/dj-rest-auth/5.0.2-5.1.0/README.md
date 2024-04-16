# Comparing `tmp/dj-rest-auth-5.0.2.tar.gz` & `tmp/dj-rest-auth-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-rest-auth-5.0.2.tar", last modified: Wed Nov 15 04:01:38 2023, max compression
+gzip compressed data, was "dj-rest-auth-5.1.0.tar", last modified: Sat Mar 30 20:09:26 2024, max compression
```

## Comparing `dj-rest-auth-5.0.2.tar` & `dj-rest-auth-5.1.0.tar`

### file list

```diff
@@ -1,295 +1,301 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.839289 dj-rest-auth-5.0.2/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.698427 dj-rest-auth-5.0.2/.circleci/
--rw-r--r--   0 michael    (501) staff       (20)     1057 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/.circleci/config.yml
--rw-r--r--   0 michael    (501) staff       (20)       45 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/.coveralls.yml
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.676779 dj-rest-auth-5.0.2/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.699242 dj-rest-auth-5.0.2/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)      352 2020-08-17 05:29:18.000000 dj-rest-auth-5.0.2/.github/workflows/main.yml
--rw-r--r--   0 michael    (501) staff       (20)      923 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/.github/workflows/stale.yml
--rw-r--r--   0 michael    (501) staff       (20)     1330 2020-11-17 22:42:53.000000 dj-rest-auth-5.0.2/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/AUTHORS
--rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-5.0.2/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3591 2023-11-15 04:01:38.838945 dj-rest-auth-5.0.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2808 2023-09-17 14:50:26.000000 dj-rest-auth-5.0.2/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.700064 dj-rest-auth-5.0.2/demo/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.701596 dj-rest-auth-5.0.2/demo/demo/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/demo/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3782 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/demo/settings.py
--rw-r--r--   0 michael    (501) staff       (20)     2313 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/demo/urls.py
--rw-r--r--   0 michael    (501) staff       (20)      385 2020-03-01 05:55:17.000000 dj-rest-auth-5.0.2/demo/demo/wsgi.py
--rwxr-xr-x   0 michael    (501) staff       (20)      247 2021-08-03 03:29:51.000000 dj-rest-auth-5.0.2/demo/manage.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.702969 dj-rest-auth-5.0.2/demo/react-spa/
--rw-r--r--   0 michael    (501) staff       (20)      310 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     2884 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/README.md
--rw-r--r--   0 michael    (501) staff       (20)      797 2023-09-17 14:50:26.000000 dj-rest-auth-5.0.2/demo/react-spa/package.json
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.705790 dj-rest-auth-5.0.2/demo/react-spa/public/
--rw-r--r--   0 michael    (501) staff       (20)     3150 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/favicon.ico
--rw-r--r--   0 michael    (501) staff       (20)     1721 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/index.html
--rw-r--r--   0 michael    (501) staff       (20)     5347 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/logo192.png
--rw-r--r--   0 michael    (501) staff       (20)     9664 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/logo512.png
--rw-r--r--   0 michael    (501) staff       (20)      492 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/manifest.json
--rw-r--r--   0 michael    (501) staff       (20)       67 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/public/robots.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.709307 dj-rest-auth-5.0.2/demo/react-spa/src/
--rw-r--r--   0 michael    (501) staff       (20)      594 2020-03-28 18:49:16.000000 dj-rest-auth-5.0.2/demo/react-spa/src/App.css
--rw-r--r--   0 michael    (501) staff       (20)     1770 2020-03-28 18:50:43.000000 dj-rest-auth-5.0.2/demo/react-spa/src/App.js
--rw-r--r--   0 michael    (501) staff       (20)      280 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/src/App.test.js
--rw-r--r--   0 michael    (501) staff       (20)      821 2020-03-28 18:49:40.000000 dj-rest-auth-5.0.2/demo/react-spa/src/index.css
--rw-r--r--   0 michael    (501) staff       (20)      503 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/src/index.js
--rw-r--r--   0 michael    (501) staff       (20)     2671 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/src/logo.svg
--rw-r--r--   0 michael    (501) staff       (20)     5086 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/src/serviceWorker.js
--rw-r--r--   0 michael    (501) staff       (20)      255 2020-03-28 16:41:44.000000 dj-rest-auth-5.0.2/demo/react-spa/src/setupTests.js
--rw-r--r--   0 michael    (501) staff       (20)      234 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/requirements.pip
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.714015 dj-rest-auth-5.0.2/demo/templates/
--rw-r--r--   0 michael    (501) staff       (20)     4447 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/templates/base.html
--rw-r--r--   0 michael    (501) staff       (20)      188 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/email_verification.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.717768 dj-rest-auth-5.0.2/demo/templates/fragments/
--rw-r--r--   0 michael    (501) staff       (20)      652 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/email_verification_form.html
--rw-r--r--   0 michael    (501) staff       (20)      839 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/login_form.html
--rw-r--r--   0 michael    (501) staff       (20)      668 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/logout_form.html
--rw-r--r--   0 michael    (501) staff       (20)      908 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/password_change_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1489 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/password_reset_confirm_form.html
--rw-r--r--   0 michael    (501) staff       (20)      579 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/password_reset_form.html
--rw-r--r--   0 michael    (501) staff       (20)      578 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/templates/fragments/resend_email_verification_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1365 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/signup_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1344 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/fragments/user_details_form.html
--rw-r--r--   0 michael    (501) staff       (20)      253 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/home.html
--rw-r--r--   0 michael    (501) staff       (20)      161 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/login.html
--rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/logout.html
--rw-r--r--   0 michael    (501) staff       (20)     1161 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/password_change.html
--rw-r--r--   0 michael    (501) staff       (20)      179 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/password_reset.html
--rw-r--r--   0 michael    (501) staff       (20)      724 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/password_reset_confirm.html
--rw-r--r--   0 michael    (501) staff       (20)      202 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/demo/templates/resend_email_verification.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.718174 dj-rest-auth-5.0.2/demo/templates/rest_framework/
--rw-r--r--   0 michael    (501) staff       (20)     1754 2020-06-20 18:56:14.000000 dj-rest-auth-5.0.2/demo/templates/rest_framework/api.html
--rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/signup.html
--rw-r--r--   0 michael    (501) staff       (20)     1915 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/demo/templates/user_details.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.724499 dj-rest-auth-5.0.2/dj_rest_auth/
--rw-r--r--   0 michael    (501) staff       (20)     6148 2023-09-17 14:52:19.000000 dj-rest-auth-5.0.2/dj_rest_auth/.DS_Store
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.0.2/dj_rest_auth/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.741132 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      170 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      167 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     3264 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/app_settings.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     3633 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/forms.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8706 2023-10-27 19:27:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/jwt_auth.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1338 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    19185 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/serializers.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     6644 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/social_serializers.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1828 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1156 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    14962 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      354 2023-11-15 04:01:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-5.0.2/dj_rest_auth/admin.py
--rw-r--r--   0 michael    (501) staff       (20)     3112 2023-11-15 03:59:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/app_settings.py
--rw-r--r--   0 michael    (501) staff       (20)     2785 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/forms.py
--rw-r--r--   0 michael    (501) staff       (20)     6569 2023-11-15 03:59:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/jwt_auth.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.690818 dj-rest-auth-5.0.2/dj_rest_auth/locale/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.679997 dj-rest-auth-5.0.2/dj_rest_auth/locale/ar/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.742031 dj-rest-auth-5.0.2/dj_rest_auth/locale/ar/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3751 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.680367 dj-rest-auth-5.0.2/dj_rest_auth/locale/az/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.742689 dj-rest-auth-5.0.2/dj_rest_auth/locale/az/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2943 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.680732 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.749011 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.681102 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.753032 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.681486 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.757436 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.681890 dj-rest-auth-5.0.2/dj_rest_auth/locale/fa/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.758137 dj-rest-auth-5.0.2/dj_rest_auth/locale/fa/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.682492 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.762039 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3755 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     5257 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.682902 dj-rest-auth-5.0.2/dj_rest_auth/locale/hr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.763195 dj-rest-auth-5.0.2/dj_rest_auth/locale/hr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.683373 dj-rest-auth-5.0.2/dj_rest_auth/locale/id/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.764143 dj-rest-auth-5.0.2/dj_rest_auth/locale/id/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     4954 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.684057 dj-rest-auth-5.0.2/dj_rest_auth/locale/it/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.766034 dj-rest-auth-5.0.2/dj_rest_auth/locale/it/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.684699 dj-rest-auth-5.0.2/dj_rest_auth/locale/ja/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.766835 dj-rest-auth-5.0.2/dj_rest_auth/locale/ja/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.685126 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.770930 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.685664 dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.772382 dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.686430 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.775030 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.687098 dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.775968 dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.687721 dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.776893 dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.688323 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.779102 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.688799 dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.780014 dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.689446 dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.780896 dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2919 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.690023 dj-rest-auth-5.0.2/dj_rest_auth/locale/uk/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.781508 dj-rest-auth-5.0.2/dj_rest_auth/locale/uk/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.690589 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.785306 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.691059 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.789583 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
--rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 michael    (501) staff       (20)      948 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/models.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.793140 dj-rest-auth-5.0.2/dj_rest_auth/registration/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.804272 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      183 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    15442 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/serializers.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1171 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    12679 2023-10-27 19:27:42.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    11066 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     1299 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     7731 2023-09-17 14:50:26.000000 dj-rest-auth-5.0.2/dj_rest_auth/registration/views.py
--rw-r--r--   0 michael    (501) staff       (20)    12700 2023-05-07 05:35:37.000000 dj-rest-auth-5.0.2/dj_rest_auth/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     5034 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/social_serializers.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.813600 dj-rest-auth-5.0.2/dj_rest_auth/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.828384 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      176 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     3094 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/django_urls.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     6897 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     3023 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    64543 2023-10-27 19:27:41.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_api.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    11659 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_serializers.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    19185 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_social.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1012 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_utils.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8348 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2025 2023-10-27 19:27:44.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2420 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/django_urls.py
--rw-r--r--   0 michael    (501) staff       (20)     4012 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/mixins.py
--rw-r--r--   0 michael    (501) staff       (20)      140 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/requirements.pip
--rw-r--r--   0 michael    (501) staff       (20)     2885 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/settings.py
--rw-r--r--   0 michael    (501) staff       (20)    44032 2023-05-07 05:35:37.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/test_api.py
--rw-r--r--   0 michael    (501) staff       (20)     7135 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/test_serializers.py
--rw-r--r--   0 michael    (501) staff       (20)    13998 2023-05-07 05:35:37.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/test_social.py
--rw-r--r--   0 michael    (501) staff       (20)      289 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/test_utils.py
--rw-r--r--   0 michael    (501) staff       (20)     4527 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     1031 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/tests/utils.py
--rw-r--r--   0 michael    (501) staff       (20)     1198 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/urls.py
--rw-r--r--   0 michael    (501) staff       (20)      541 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/dj_rest_auth/utils.py
--rw-r--r--   0 michael    (501) staff       (20)    10760 2023-05-07 05:35:37.000000 dj-rest-auth-5.0.2/dj_rest_auth/views.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.727408 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3591 2023-11-15 04:01:38.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     9461 2023-11-15 04:01:38.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-11-15 04:01:38.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)       86 2023-11-15 04:01:38.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2023-11-15 04:01:38.000000 dj-rest-auth-5.0.2/dj_rest_auth.egg-info/top_level.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-11-15 04:01:38.837133 dj-rest-auth-5.0.2/docs/
--rw-r--r--   0 michael    (501) staff       (20)     6786 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/docs/Makefile
--rw-r--r--   0 michael    (501) staff       (20)     3228 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/docs/api_endpoints.rst
--rw-r--r--   0 michael    (501) staff       (20)     8317 2020-05-09 22:29:21.000000 dj-rest-auth-5.0.2/docs/conf.py
--rw-r--r--   0 michael    (501) staff       (20)     9215 2023-11-15 03:59:42.000000 dj-rest-auth-5.0.2/docs/configuration.rst
--rw-r--r--   0 michael    (501) staff       (20)      758 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/docs/demo.rst
--rw-r--r--   0 michael    (501) staff       (20)      497 2020-05-30 06:34:32.000000 dj-rest-auth-5.0.2/docs/disclosure.rst
--rw-r--r--   0 michael    (501) staff       (20)     3095 2023-03-26 05:23:49.000000 dj-rest-auth-5.0.2/docs/faq.rst
--rw-r--r--   0 michael    (501) staff       (20)      754 2021-03-20 17:51:05.000000 dj-rest-auth-5.0.2/docs/index.rst
--rw-r--r--   0 michael    (501) staff       (20)    11427 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/docs/installation.rst
--rw-r--r--   0 michael    (501) staff       (20)     1301 2020-08-10 01:03:45.000000 dj-rest-auth-5.0.2/docs/introduction.rst
--rw-r--r--   0 michael    (501) staff       (20)     6713 2020-03-01 01:48:46.000000 dj-rest-auth-5.0.2/docs/make.bat
--rw-r--r--   0 michael    (501) staff       (20)      657 2021-03-17 23:58:28.000000 dj-rest-auth-5.0.2/runtests.py
--rw-r--r--   0 michael    (501) staff       (20)      474 2023-11-15 04:01:38.840513 dj-rest-auth-5.0.2/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1543 2023-10-27 19:23:53.000000 dj-rest-auth-5.0.2/setup.py
--rw-r--r--   0 michael    (501) staff       (20)     1062 2023-09-11 14:04:51.000000 dj-rest-auth-5.0.2/tox.ini
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.723272 dj-rest-auth-5.1.0/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.690987 dj-rest-auth-5.1.0/.circleci/
+-rw-r--r--   0 michael    (501) staff       (20)     1057 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/.circleci/config.yml
+-rw-r--r--   0 michael    (501) staff       (20)       45 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/.coveralls.yml
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.686225 dj-rest-auth-5.1.0/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.691492 dj-rest-auth-5.1.0/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)      352 2020-08-17 05:29:18.000000 dj-rest-auth-5.1.0/.github/workflows/main.yml
+-rw-r--r--   0 michael    (501) staff       (20)      923 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/.github/workflows/stale.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1330 2020-11-17 22:42:53.000000 dj-rest-auth-5.1.0/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/AUTHORS
+-rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-5.1.0/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3451 2024-03-30 20:09:26.723344 dj-rest-auth-5.1.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2808 2023-09-17 14:50:26.000000 dj-rest-auth-5.1.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.692028 dj-rest-auth-5.1.0/demo/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.692836 dj-rest-auth-5.1.0/demo/demo/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/demo/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3834 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/demo/demo/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2313 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/demo/demo/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      385 2020-03-01 05:55:17.000000 dj-rest-auth-5.1.0/demo/demo/wsgi.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      247 2021-08-03 03:29:51.000000 dj-rest-auth-5.1.0/demo/manage.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.693402 dj-rest-auth-5.1.0/demo/react-spa/
+-rw-r--r--   0 michael    (501) staff       (20)      310 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     2884 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/README.md
+-rw-r--r--   0 michael    (501) staff       (20)      797 2023-09-17 14:50:26.000000 dj-rest-auth-5.1.0/demo/react-spa/package.json
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.694614 dj-rest-auth-5.1.0/demo/react-spa/public/
+-rw-r--r--   0 michael    (501) staff       (20)     3150 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/favicon.ico
+-rw-r--r--   0 michael    (501) staff       (20)     1721 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/index.html
+-rw-r--r--   0 michael    (501) staff       (20)     5347 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/logo192.png
+-rw-r--r--   0 michael    (501) staff       (20)     9664 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/logo512.png
+-rw-r--r--   0 michael    (501) staff       (20)      492 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/manifest.json
+-rw-r--r--   0 michael    (501) staff       (20)       67 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/public/robots.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.695777 dj-rest-auth-5.1.0/demo/react-spa/src/
+-rw-r--r--   0 michael    (501) staff       (20)      594 2020-03-28 18:49:16.000000 dj-rest-auth-5.1.0/demo/react-spa/src/App.css
+-rw-r--r--   0 michael    (501) staff       (20)     1770 2020-03-28 18:50:43.000000 dj-rest-auth-5.1.0/demo/react-spa/src/App.js
+-rw-r--r--   0 michael    (501) staff       (20)      280 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/src/App.test.js
+-rw-r--r--   0 michael    (501) staff       (20)      821 2020-03-28 18:49:40.000000 dj-rest-auth-5.1.0/demo/react-spa/src/index.css
+-rw-r--r--   0 michael    (501) staff       (20)      503 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/src/index.js
+-rw-r--r--   0 michael    (501) staff       (20)     2671 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/src/logo.svg
+-rw-r--r--   0 michael    (501) staff       (20)     5086 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/src/serviceWorker.js
+-rw-r--r--   0 michael    (501) staff       (20)      255 2020-03-28 16:41:44.000000 dj-rest-auth-5.1.0/demo/react-spa/src/setupTests.js
+-rw-r--r--   0 michael    (501) staff       (20)      234 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/demo/requirements.pip
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.697815 dj-rest-auth-5.1.0/demo/templates/
+-rw-r--r--   0 michael    (501) staff       (20)     4447 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/demo/templates/base.html
+-rw-r--r--   0 michael    (501) staff       (20)      188 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.699404 dj-rest-auth-5.1.0/demo/templates/fragments/
+-rw-r--r--   0 michael    (501) staff       (20)      652 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      839 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/login_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      668 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/logout_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      908 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/password_change_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1489 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/password_reset_confirm_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      579 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/password_reset_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      578 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/demo/templates/fragments/resend_email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1365 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/signup_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1344 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/fragments/user_details_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      253 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/home.html
+-rw-r--r--   0 michael    (501) staff       (20)      161 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/login.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/logout.html
+-rw-r--r--   0 michael    (501) staff       (20)     1161 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/password_change.html
+-rw-r--r--   0 michael    (501) staff       (20)      179 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/password_reset.html
+-rw-r--r--   0 michael    (501) staff       (20)      724 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/password_reset_confirm.html
+-rw-r--r--   0 michael    (501) staff       (20)      202 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/demo/templates/resend_email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.699563 dj-rest-auth-5.1.0/demo/templates/rest_framework/
+-rw-r--r--   0 michael    (501) staff       (20)     1754 2020-06-20 18:56:14.000000 dj-rest-auth-5.1.0/demo/templates/rest_framework/api.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/signup.html
+-rw-r--r--   0 michael    (501) staff       (20)     1915 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/demo/templates/user_details.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.701664 dj-rest-auth-5.1.0/dj_rest_auth/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.1.0/dj_rest_auth/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.705761 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      170 2023-10-27 19:27:41.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      158 2024-03-30 19:52:47.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      167 2023-10-27 19:27:41.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     3293 2024-03-30 20:08:27.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/app_settings.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     3709 2024-03-30 20:08:30.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8985 2024-03-30 20:08:28.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/jwt_auth.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1338 2023-10-27 19:27:41.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    19185 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/serializers.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     6644 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/social_serializers.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1828 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1156 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    15832 2024-03-30 20:08:30.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      354 2024-03-30 19:43:15.000000 dj-rest-auth-5.1.0/dj_rest_auth/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-5.1.0/dj_rest_auth/admin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3112 2023-11-15 03:59:42.000000 dj-rest-auth-5.1.0/dj_rest_auth/app_settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2894 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/forms.py
+-rw-r--r--   0 michael    (501) staff       (20)     6698 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/jwt_auth.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688778 dj-rest-auth-5.1.0/dj_rest_auth/locale/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.686871 dj-rest-auth-5.1.0/dj_rest_auth/locale/ar/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.706102 dj-rest-auth-5.1.0/dj_rest_auth/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3751 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.686948 dj-rest-auth-5.1.0/dj_rest_auth/locale/az/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.706251 dj-rest-auth-5.1.0/dj_rest_auth/locale/az/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2943 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687021 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.707236 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687091 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.707898 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687168 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.708543 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687239 dj-rest-auth-5.1.0/dj_rest_auth/locale/fa/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.708706 dj-rest-auth-5.1.0/dj_rest_auth/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687317 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.709382 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3755 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     5257 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687427 dj-rest-auth-5.1.0/dj_rest_auth/locale/hr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.709503 dj-rest-auth-5.1.0/dj_rest_auth/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687524 dj-rest-auth-5.1.0/dj_rest_auth/locale/id/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.709619 dj-rest-auth-5.1.0/dj_rest_auth/locale/id/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     4954 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687606 dj-rest-auth-5.1.0/dj_rest_auth/locale/it/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.709886 dj-rest-auth-5.1.0/dj_rest_auth/locale/it/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687706 dj-rest-auth-5.1.0/dj_rest_auth/locale/ja/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.710009 dj-rest-auth-5.1.0/dj_rest_auth/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687794 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.710565 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687882 dj-rest-auth-5.1.0/dj_rest_auth/locale/ma/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.710937 dj-rest-auth-5.1.0/dj_rest_auth/locale/ma/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2244 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ma/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3014 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ma/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.687966 dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.711308 dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688062 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.711839 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688168 dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.712082 dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688261 dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.712386 dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688339 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.713090 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688418 dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.713379 dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688497 dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.713660 dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2919 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688603 dj-rest-auth-5.1.0/dj_rest_auth/locale/uk/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.713820 dj-rest-auth-5.1.0/dj_rest_auth/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688727 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.714459 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.688813 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.715105 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 michael    (501) staff       (20)      948 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/models.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.715551 dj-rest-auth-5.1.0/dj_rest_auth/registration/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.716616 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      183 2023-10-27 19:27:41.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    15442 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/serializers.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1171 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    12679 2023-10-27 19:27:42.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    11066 2023-10-27 19:23:53.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     1299 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     7731 2023-09-17 14:50:26.000000 dj-rest-auth-5.1.0/dj_rest_auth/registration/views.py
+-rw-r--r--   0 michael    (501) staff       (20)    12700 2023-05-07 05:35:37.000000 dj-rest-auth-5.1.0/dj_rest_auth/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     5034 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/social_serializers.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.717821 dj-rest-auth-5.1.0/dj_rest_auth/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.720905 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      176 2023-10-27 19:27:41.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      164 2024-03-30 19:52:47.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     3094 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     6897 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     3084 2024-03-30 20:08:27.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     3058 2024-03-30 19:52:47.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/settings.cpython-312.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    66281 2024-03-30 20:08:27.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_api.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    11659 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    19185 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_social.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1012 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_utils.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8348 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2025 2023-10-27 19:27:44.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2420 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/django_urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     4012 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/mixins.py
+-rw-r--r--   0 michael    (501) staff       (20)      157 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/requirements.pip
+-rw-r--r--   0 michael    (501) staff       (20)     3030 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)    45434 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/test_api.py
+-rw-r--r--   0 michael    (501) staff       (20)     7135 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/test_serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)    13998 2023-05-07 05:35:37.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/test_social.py
+-rw-r--r--   0 michael    (501) staff       (20)      289 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/test_utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     4527 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     1031 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/tests/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     1198 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      541 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/dj_rest_auth/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)    11609 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/dj_rest_auth/views.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.702443 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3451 2024-03-30 20:09:26.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     9690 2024-03-30 20:09:26.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-03-30 20:09:26.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/not-zip-safe
+-rw-r--r--   0 michael    (501) staff       (20)       91 2024-03-30 20:09:26.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       13 2024-03-30 20:09:26.000000 dj-rest-auth-5.1.0/dj_rest_auth.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-30 20:09:26.723127 dj-rest-auth-5.1.0/docs/
+-rw-r--r--   0 michael    (501) staff       (20)     6786 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/docs/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)     3228 2023-10-27 19:23:53.000000 dj-rest-auth-5.1.0/docs/api_endpoints.rst
+-rw-r--r--   0 michael    (501) staff       (20)     8317 2020-05-09 22:29:21.000000 dj-rest-auth-5.1.0/docs/conf.py
+-rw-r--r--   0 michael    (501) staff       (20)     9215 2023-11-15 03:59:42.000000 dj-rest-auth-5.1.0/docs/configuration.rst
+-rw-r--r--   0 michael    (501) staff       (20)      758 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/docs/demo.rst
+-rw-r--r--   0 michael    (501) staff       (20)      497 2020-05-30 06:34:32.000000 dj-rest-auth-5.1.0/docs/disclosure.rst
+-rw-r--r--   0 michael    (501) staff       (20)     3095 2023-03-26 05:23:49.000000 dj-rest-auth-5.1.0/docs/faq.rst
+-rw-r--r--   0 michael    (501) staff       (20)      754 2021-03-20 17:51:05.000000 dj-rest-auth-5.1.0/docs/index.rst
+-rw-r--r--   0 michael    (501) staff       (20)    11427 2023-10-27 19:23:53.000000 dj-rest-auth-5.1.0/docs/installation.rst
+-rw-r--r--   0 michael    (501) staff       (20)     1301 2020-08-10 01:03:45.000000 dj-rest-auth-5.1.0/docs/introduction.rst
+-rw-r--r--   0 michael    (501) staff       (20)     6713 2020-03-01 01:48:46.000000 dj-rest-auth-5.1.0/docs/make.bat
+-rw-r--r--   0 michael    (501) staff       (20)      657 2021-03-17 23:58:28.000000 dj-rest-auth-5.1.0/runtests.py
+-rw-r--r--   0 michael    (501) staff       (20)      474 2024-03-30 20:09:26.723623 dj-rest-auth-5.1.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1548 2024-03-24 22:56:31.000000 dj-rest-auth-5.1.0/setup.py
+-rw-r--r--   0 michael    (501) staff       (20)     1062 2023-09-11 14:04:51.000000 dj-rest-auth-5.1.0/tox.ini
```

### Comparing `dj-rest-auth-5.0.2/.circleci/config.yml` & `dj-rest-auth-5.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/.github/workflows/stale.yml` & `dj-rest-auth-5.1.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/.gitignore` & `dj-rest-auth-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/LICENSE` & `dj-rest-auth-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/PKG-INFO` & `dj-rest-auth-5.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: dj-rest-auth
-Version: 5.0.2
+Version: 5.1.0
 Summary: Authentication and Registration in Django Rest Framework
 Home-page: http://github.com/iMerica/dj-rest-auth
 Author: iMerica
 Author-email: imichael@pm.me
 License: MIT
 Keywords: django rest auth registration rest-framework django-registration api
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: with_social
 License-File: LICENSE
-Requires-Dist: Django>=3.2
-Requires-Dist: djangorestframework>=3.13.0
-Provides-Extra: with-social
-Requires-Dist: django-allauth<0.58.0,>=0.56.0; extra == "with-social"
 
 # Dj-Rest-Auth
 [![<iMerica>](https://circleci.com/gh/iMerica/dj-rest-auth.svg?style=svg)](https://app.circleci.com/pipelines/github/iMerica/dj-rest-auth)
 
 
 Drop-in API endpoints for handling authentication securely in Django Rest Framework. Works especially well 
 with SPAs (e.g., React, Vue, Angular), and Mobile applications.
```

### Comparing `dj-rest-auth-5.0.2/README.md` & `dj-rest-auth-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/demo/settings.py` & `dj-rest-auth-5.1.0/demo/demo/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     'corsheaders.middleware.CorsMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    'allauth.account.middleware.AccountMiddleware',
 )
 
 # For backwards compatibility for Django 1.8
 MIDDLEWARE_CLASSES = MIDDLEWARE
 
 ROOT_URLCONF = 'demo.urls'
```

### Comparing `dj-rest-auth-5.0.2/demo/demo/urls.py` & `dj-rest-auth-5.1.0/demo/demo/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/README.md` & `dj-rest-auth-5.1.0/demo/react-spa/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/package.json` & `dj-rest-auth-5.1.0/demo/react-spa/package.json`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/public/favicon.ico` & `dj-rest-auth-5.1.0/demo/react-spa/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/public/index.html` & `dj-rest-auth-5.1.0/demo/react-spa/public/index.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/public/logo192.png` & `dj-rest-auth-5.1.0/demo/react-spa/public/logo192.png`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/public/logo512.png` & `dj-rest-auth-5.1.0/demo/react-spa/public/logo512.png`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/src/App.css` & `dj-rest-auth-5.1.0/demo/react-spa/src/App.css`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/src/App.js` & `dj-rest-auth-5.1.0/demo/react-spa/src/App.js`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/src/index.css` & `dj-rest-auth-5.1.0/demo/react-spa/src/index.css`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/src/logo.svg` & `dj-rest-auth-5.1.0/demo/react-spa/src/logo.svg`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/react-spa/src/serviceWorker.js` & `dj-rest-auth-5.1.0/demo/react-spa/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/base.html` & `dj-rest-auth-5.1.0/demo/templates/base.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/email_verification_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/email_verification_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/login_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/login_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/logout_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/logout_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/password_change_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/password_change_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/password_reset_confirm_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/password_reset_confirm_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/password_reset_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/resend_email_verification_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/resend_email_verification_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/signup_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/signup_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/fragments/user_details_form.html` & `dj-rest-auth-5.1.0/demo/templates/fragments/user_details_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/password_change.html` & `dj-rest-auth-5.1.0/demo/templates/password_change.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/password_reset_confirm.html` & `dj-rest-auth-5.1.0/demo/templates/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/rest_framework/api.html` & `dj-rest-auth-5.1.0/demo/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/demo/templates/user_details.html` & `dj-rest-auth-5.1.0/demo/templates/user_details.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/app_settings.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/app_settings.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,25 +1,25 @@
 magic:    0xa70d0d0a
-moddate:  0xe5d61f64 (Sun Mar 26 05:23:49 2023 UTC)
-files sz: 3075
+moddate:  0x2e425465 (Wed Nov 15 03:59:42 2023 UTC)
+files sz: 3112
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 12
+   stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a040100640064
       036c056d065a07010002006508650164046405a6030000ab030000000000
       0000005a096900640664079301640864099301640a640b9301640c640d93
       01640e640f93016410641193016412641393016414641593016416641793
       01641864199301641a641b9301641c641d9301641e641f93016420642193
       016422642193016423642193016424642593016421640564056426642164
-      25642764216421642164289c0aa5015a0a64295a0b642a5a0c0200470064
-      2b8400642c6507a6030000ab0300000000000000005a0602006506650965
-      0a650ba6030000ab0300000000000000005a0d64055300
+      256427640564216421642164289c0ba5015a0a64295a0b642a5a0c020047
+      00642b8400642c6507a6030000ab0300000000000000005a060200650665
+      09650a650ba6030000ab0300000000000000005a0d64055300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('settings',))
                  6 IMPORT_NAME              0 (django.conf)
                  8 IMPORT_FROM              1 (settings)
                 10 STORE_NAME               1 (settings)
@@ -145,51 +145,53 @@
    
     35         176 LOAD_CONST              33 (False)
    
     36         178 LOAD_CONST              37 (True)
    
     37         180 LOAD_CONST              39 ('Lax')
    
-    38         182 LOAD_CONST              33 (False)
+    38         182 LOAD_CONST               5 (None)
    
     39         184 LOAD_CONST              33 (False)
    
     40         186 LOAD_CONST              33 (False)
    
-     8         188 LOAD_CONST              40 (('USE_JWT', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_RETURN_EXPIRATION', 'JWT_AUTH_COOKIE_USE_CSRF', 'JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED'))
-               190 BUILD_CONST_KEY_MAP     10
-               192 DICT_UPDATE              1
-               194 STORE_NAME              10 (DEFAULTS)
-   
-    44         196 LOAD_CONST              41 (('TOKEN_CREATOR', 'TOKEN_MODEL', 'TOKEN_SERIALIZER', 'JWT_SERIALIZER', 'JWT_SERIALIZER_WITH_EXPIRATION', 'JWT_TOKEN_CLAIMS_SERIALIZER', 'USER_DETAILS_SERIALIZER', 'LOGIN_SERIALIZER', 'PASSWORD_RESET_SERIALIZER', 'PASSWORD_RESET_CONFIRM_SERIALIZER', 'PASSWORD_CHANGE_SERIALIZER', 'REGISTER_SERIALIZER', 'REGISTER_PERMISSION_CLASSES'))
-               198 STORE_NAME              11 (IMPORT_STRINGS)
-   
-    61         200 LOAD_CONST              42 (())
-               202 STORE_NAME              12 (REMOVED_SETTINGS)
-   
-    64         204 PUSH_NULL
-               206 LOAD_BUILD_CLASS
-               208 LOAD_CONST              43 (<code object APISettings, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py", line 64>)
-               210 MAKE_FUNCTION            0
-               212 LOAD_CONST              44 ('APISettings')
-               214 LOAD_NAME                7 (_APISettings)
-               216 PRECALL                  3
-               220 CALL                     3
-               230 STORE_NAME               6 (APISettings)
-   
-    84         232 PUSH_NULL
-               234 LOAD_NAME                6 (APISettings)
-               236 LOAD_NAME                9 (USER_SETTINGS)
-               238 LOAD_NAME               10 (DEFAULTS)
-               240 LOAD_NAME               11 (IMPORT_STRINGS)
-               242 PRECALL                  3
-               246 CALL                     3
-               256 STORE_NAME              13 (api_settings)
-               258 LOAD_CONST               5 (None)
-               260 RETURN_VALUE
+    41         188 LOAD_CONST              33 (False)
+   
+     8         190 LOAD_CONST              40 (('USE_JWT', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_COOKIE_DOMAIN', 'JWT_AUTH_RETURN_EXPIRATION', 'JWT_AUTH_COOKIE_USE_CSRF', 'JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED'))
+               192 BUILD_CONST_KEY_MAP     11
+               194 DICT_UPDATE              1
+               196 STORE_NAME              10 (DEFAULTS)
+   
+    45         198 LOAD_CONST              41 (('TOKEN_CREATOR', 'TOKEN_MODEL', 'TOKEN_SERIALIZER', 'JWT_SERIALIZER', 'JWT_SERIALIZER_WITH_EXPIRATION', 'JWT_TOKEN_CLAIMS_SERIALIZER', 'USER_DETAILS_SERIALIZER', 'LOGIN_SERIALIZER', 'PASSWORD_RESET_SERIALIZER', 'PASSWORD_RESET_CONFIRM_SERIALIZER', 'PASSWORD_CHANGE_SERIALIZER', 'REGISTER_SERIALIZER', 'REGISTER_PERMISSION_CLASSES'))
+               200 STORE_NAME              11 (IMPORT_STRINGS)
+   
+    62         202 LOAD_CONST              42 (())
+               204 STORE_NAME              12 (REMOVED_SETTINGS)
+   
+    65         206 PUSH_NULL
+               208 LOAD_BUILD_CLASS
+               210 LOAD_CONST              43 (<code object APISettings, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py", line 65>)
+               212 MAKE_FUNCTION            0
+               214 LOAD_CONST              44 ('APISettings')
+               216 LOAD_NAME                7 (_APISettings)
+               218 PRECALL                  3
+               222 CALL                     3
+               232 STORE_NAME               6 (APISettings)
+   
+    85         234 PUSH_NULL
+               236 LOAD_NAME                6 (APISettings)
+               238 LOAD_NAME                9 (USER_SETTINGS)
+               240 LOAD_NAME               10 (DEFAULTS)
+               242 LOAD_NAME               11 (IMPORT_STRINGS)
+               244 PRECALL                  3
+               248 CALL                     3
+               258 STORE_NAME              13 (api_settings)
+               260 LOAD_CONST               5 (None)
+               262 RETURN_VALUE
    consts
       0
       ('settings',)
       ('gettext_lazy',)
       ('APISettings',)
       'REST_AUTH'
       None
@@ -223,30 +225,30 @@
       False
       'OLD_PASSWORD_FIELD_ENABLED'
       'LOGOUT_ON_PASSWORD_CHANGE'
       'SESSION_LOGIN'
       True
       '/'
       'Lax'
-      ('USE_JWT', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_RETURN_EXPIRATION', 'JWT_AUTH_COOKIE_USE_CSRF', 'JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED')
+      ('USE_JWT', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_COOKIE_DOMAIN', 'JWT_AUTH_RETURN_EXPIRATION', 'JWT_AUTH_COOKIE_USE_CSRF', 'JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED')
       ('TOKEN_CREATOR', 'TOKEN_MODEL', 'TOKEN_SERIALIZER', 'JWT_SERIALIZER', 'JWT_SERIALIZER_WITH_EXPIRATION', 'JWT_TOKEN_CLAIMS_SERIALIZER', 'USER_DETAILS_SERIALIZER', 'LOGIN_SERIALIZER', 'PASSWORD_RESET_SERIALIZER', 'PASSWORD_RESET_CONFIRM_SERIALIZER', 'PASSWORD_CHANGE_SERIALIZER', 'REGISTER_SERIALIZER', 'REGISTER_PERMISSION_CLASSES')
       ()
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          64           0 RESUME                   0
+          65           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('APISettings')
                        8 STORE_NAME               2 (__qualname__)
          
-          65          10 LOAD_CONST               1 (<code object __check_user_settings, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py", line 65>)
+          66          10 LOAD_CONST               1 (<code object __check_user_settings, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py", line 66>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_APISettings__check_user_settings)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'APISettings'
             code
@@ -256,94 +258,94 @@
                flags     : 3
                code
                   0x9700640164026c006d017d02010064037d037404000000000000000000
                   0044005d2d7d047c047c017600722774070000000000000000000002007c
                   027409000000000000000000006404a6010000ab0100000000000000007c
                   047c03a6030000ab030000000000000000a6010000ab0100000000000000
                   0082018c2e7c015300
-                65           0 RESUME                   0
+                66           0 RESUME                   0
                
-                66           2 LOAD_CONST               1 (1)
+                67           2 LOAD_CONST               1 (1)
                              4 LOAD_CONST               2 (('format_lazy',))
                              6 IMPORT_NAME              0 (utils)
                              8 IMPORT_FROM              1 (format_lazy)
                             10 STORE_FAST               2 (format_lazy)
                             12 POP_TOP
                
-                67          14 LOAD_CONST               3 ('https://dj-rest-auth.readthedocs.io/en/latest/configuration.html')
+                68          14 LOAD_CONST               3 ('https://dj-rest-auth.readthedocs.io/en/latest/configuration.html')
                             16 STORE_FAST               3 (SETTINGS_DOC)
                
-                69          18 LOAD_GLOBAL              4 (REMOVED_SETTINGS)
+                70          18 LOAD_GLOBAL              4 (REMOVED_SETTINGS)
                             30 GET_ITER
                        >>   32 FOR_ITER                45 (to 124)
                             34 STORE_FAST               4 (setting)
                
-                70          36 LOAD_FAST                4 (setting)
+                71          36 LOAD_FAST                4 (setting)
                             38 LOAD_FAST                1 (user_settings)
                             40 CONTAINS_OP              0
                             42 POP_JUMP_FORWARD_IF_FALSE    39 (to 122)
                
-                71          44 LOAD_GLOBAL              7 (NULL + RuntimeError)
+                72          44 LOAD_GLOBAL              7 (NULL + RuntimeError)
                
-                72          56 PUSH_NULL
+                73          56 PUSH_NULL
                             58 LOAD_FAST                2 (format_lazy)
                
-                73          60 LOAD_GLOBAL              9 (NULL + _)
+                74          60 LOAD_GLOBAL              9 (NULL + _)
                
-                74          72 LOAD_CONST               4 ("The '{}' setting has been removed. Please refer to '{}' for available settings.")
+                75          72 LOAD_CONST               4 ("The '{}' setting has been removed. Please refer to '{}' for available settings.")
                
-                73          74 PRECALL                  1
+                74          74 PRECALL                  1
                             78 CALL                     1
                
-                76          88 LOAD_FAST                4 (setting)
+                77          88 LOAD_FAST                4 (setting)
                
-                77          90 LOAD_FAST                3 (SETTINGS_DOC)
+                78          90 LOAD_FAST                3 (SETTINGS_DOC)
                
-                72          92 PRECALL                  3
+                73          92 PRECALL                  3
                             96 CALL                     3
                
-                71         106 PRECALL                  1
+                72         106 PRECALL                  1
                            110 CALL                     1
                            120 RAISE_VARARGS            1
                
-                70     >>  122 JUMP_BACKWARD           46 (to 32)
+                71     >>  122 JUMP_BACKWARD           46 (to 32)
                
-                81     >>  124 LOAD_FAST                1 (user_settings)
+                82     >>  124 LOAD_FAST                1 (user_settings)
                            126 RETURN_VALUE
                consts
                   None
                   1
                   ('format_lazy',)
                   'https://dj-rest-auth.readthedocs.io/en/latest/configuration.html'
                   "The '{}' setting has been removed. Please refer to '{}' for available settings."
                names      ('utils', 'format_lazy', 'REMOVED_SETTINGS', 'RuntimeError', '_')
                varnames   ('self', 'user_settings', 'format_lazy', 'SETTINGS_DOC', 'setting')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py'
                name       '__check_user_settings'
-               firstlineno 65
+               firstlineno 66
                lnotab
                   0x02010c010402120108010c0104010c0102ff0e03020102fb0eff10ff02
                   0b
             None
          names      ('__name__', '__module__', '__qualname__', '_APISettings__check_user_settings')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py'
          name       'APISettings'
-         firstlineno 64
+         firstlineno 65
          lnotab 0x0a01
       'APISettings'
    names      ('django.conf', 'settings', 'django.utils.translation', 'gettext_lazy', '_', 'rest_framework.settings', 'APISettings', '_APISettings', 'getattr', 'USER_SETTINGS', 'DEFAULTS', 'IMPORT_STRINGS', 'REMOVED_SETTINGS', 'api_settings')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/app_settings.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c010c031a02020104ff020204fe020304fd020404fc02
       0504fb020604fa020704f9020804f8020904f7020b04f5020d04f3020f04
       f1021004f0021204ee021304ed021404ec021504eb021602020201020102
-      010201020102010201020102e00824041104031c14
+      0102010201020102010201020102df0825041104031c14
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/forms.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/forms.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe5d61f64 (Sun Mar 26 05:23:49 2023 UTC)
-files sz: 2785
+moddate:  0x9faf0066 (Sun Mar 24 22:56:31 2024 UTC)
+files sz: 2894
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -276,34 +276,35 @@
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/forms.py'
                name       'clean_email'
                firstlineno 39
                lnotab 0x02051a0142012c01
             code
                argcount  : 2
-               nlocals   : 11
-               stacksize : 6
+               nlocals   : 12
+               stacksize : 8
                flags     : 11
                code
                   0x97007401000000000000000000007c01a6010000ab0100000000000000
                   007d037c006a0100000000000000006401190000000000000000007d047c
                   02a002000000000000000000000000000000000000000064027406000000
                   00000000000000a6020000ab0200000000000000007d057c006a04000000
-                  000000000044005d9b7d067c05a005000000000000000000000000000000
+                  000000000044005dac7d067c05a005000000000000000000000000000000
                   00000000007c06a6010000ab0100000000000000007d077c02a002000000
                   00000000000000000000000000000000006403740c000000000000000000
                   00a6020000ab0200000000000000007d0802007c087c017c067c07a60300
-                  00ab0300000000000000007d097c037c067c097c0164049c047d0a740e00
-                  0000000000000000006a080000000000000000740e000000000000000000
-                  006a0900000000000000006a0a00000000000000006b0300000000721274
-                  17000000000000000000007c06a6010000ab0100000000000000007c0a64
-                  053c0000007419000000000000000000007c01a6010000ab010000000000
-                  000000a00d000000000000000000000000000000000000000064067c047c
-                  0aa6030000ab03000000000000000001008c9c7c006a0100000000000000
-                  006401190000000000000000005300
+                  00ab0300000000000000007d09740f000000000000000000007c06a60100
+                  00ab0100000000000000007d0a7c037c067c097c017c077c0a64049c067d
+                  0b7410000000000000000000006a09000000000000000074100000000000
+                  00000000006a0a00000000000000006a0b00000000000000006b03000000
+                  0072127419000000000000000000007c06a6010000ab0100000000000000
+                  007c0b64053c000000741b000000000000000000007c01a6010000ab0100
+                  00000000000000a00e000000000000000000000000000000000000000064
+                  067c047c0ba6030000ab03000000000000000001008cad7c006a01000000
+                  00000000006401190000000000000000005300
                 49           0 RESUME                   0
                
                 50           2 LOAD_GLOBAL              1 (NULL + get_current_site)
                             14 LOAD_FAST                1 (request)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (current_site)
@@ -321,15 +322,15 @@
                             96 PRECALL                  2
                            100 CALL                     2
                            110 STORE_FAST               5 (token_generator)
                
                 54         112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                4 (users)
                            124 GET_ITER
-                       >>  126 FOR_ITER               155 (to 438)
+                       >>  126 FOR_ITER               172 (to 472)
                            128 STORE_FAST               6 (user)
                
                 56         130 LOAD_FAST                5 (token_generator)
                            132 LOAD_METHOD              5 (make_token)
                            154 LOAD_FAST                6 (user)
                            156 PRECALL                  1
                            160 CALL                     1
@@ -348,82 +349,92 @@
                            230 LOAD_FAST                1 (request)
                            232 LOAD_FAST                6 (user)
                            234 LOAD_FAST                7 (temp_key)
                            236 PRECALL                  3
                            240 CALL                     3
                            250 STORE_FAST               9 (url)
                
-                67         252 LOAD_FAST                3 (current_site)
-               
-                68         254 LOAD_FAST                6 (user)
-               
-                69         256 LOAD_FAST                9 (url)
-               
-                70         258 LOAD_FAST                1 (request)
-               
-                66         260 LOAD_CONST               4 (('current_site', 'user', 'password_reset_url', 'request'))
-                           262 BUILD_CONST_KEY_MAP      4
-                           264 STORE_FAST              10 (context)
-               
-                73         266 LOAD_GLOBAL             14 (allauth_account_settings)
-                           278 LOAD_ATTR                8 (AUTHENTICATION_METHOD)
-               
-                74         288 LOAD_GLOBAL             14 (allauth_account_settings)
-                           300 LOAD_ATTR                9 (AuthenticationMethod)
-                           310 LOAD_ATTR               10 (EMAIL)
-               
-                73         320 COMPARE_OP               3 (!=)
-                           326 POP_JUMP_FORWARD_IF_FALSE    18 (to 364)
-               
-                76         328 LOAD_GLOBAL             23 (NULL + user_username)
-                           340 LOAD_FAST                6 (user)
-                           342 PRECALL                  1
-                           346 CALL                     1
-                           356 LOAD_FAST               10 (context)
-                           358 LOAD_CONST               5 ('username')
-                           360 STORE_SUBSCR
-               
-                77     >>  364 LOAD_GLOBAL             25 (NULL + get_adapter)
-                           376 LOAD_FAST                1 (request)
-                           378 PRECALL                  1
-                           382 CALL                     1
-                           392 LOAD_METHOD             13 (send_mail)
-               
-                78         414 LOAD_CONST               6 ('account/email/password_reset_key')
-                           416 LOAD_FAST                4 (email)
-                           418 LOAD_FAST               10 (context)
-               
-                77         420 PRECALL                  3
-                           424 CALL                     3
-                           434 POP_TOP
-                           436 JUMP_BACKWARD          156 (to 126)
-               
-                80     >>  438 LOAD_FAST                0 (self)
-                           440 LOAD_ATTR                1 (cleaned_data)
-                           450 LOAD_CONST               1 ('email')
-                           452 BINARY_SUBSCR
-                           462 RETURN_VALUE
+                65         252 LOAD_GLOBAL             15 (NULL + user_pk_to_url_str)
+                           264 LOAD_FAST                6 (user)
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 STORE_FAST              10 (uid)
+               
+                68         282 LOAD_FAST                3 (current_site)
+               
+                69         284 LOAD_FAST                6 (user)
+               
+                70         286 LOAD_FAST                9 (url)
+               
+                71         288 LOAD_FAST                1 (request)
+               
+                72         290 LOAD_FAST                7 (temp_key)
+               
+                73         292 LOAD_FAST               10 (uid)
+               
+                67         294 LOAD_CONST               4 (('current_site', 'user', 'password_reset_url', 'request', 'token', 'uid'))
+                           296 BUILD_CONST_KEY_MAP      6
+                           298 STORE_FAST              11 (context)
+               
+                76         300 LOAD_GLOBAL             16 (allauth_account_settings)
+                           312 LOAD_ATTR                9 (AUTHENTICATION_METHOD)
+               
+                77         322 LOAD_GLOBAL             16 (allauth_account_settings)
+                           334 LOAD_ATTR               10 (AuthenticationMethod)
+                           344 LOAD_ATTR               11 (EMAIL)
+               
+                76         354 COMPARE_OP               3 (!=)
+                           360 POP_JUMP_FORWARD_IF_FALSE    18 (to 398)
+               
+                79         362 LOAD_GLOBAL             25 (NULL + user_username)
+                           374 LOAD_FAST                6 (user)
+                           376 PRECALL                  1
+                           380 CALL                     1
+                           390 LOAD_FAST               11 (context)
+                           392 LOAD_CONST               5 ('username')
+                           394 STORE_SUBSCR
+               
+                80     >>  398 LOAD_GLOBAL             27 (NULL + get_adapter)
+                           410 LOAD_FAST                1 (request)
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 LOAD_METHOD             14 (send_mail)
+               
+                81         448 LOAD_CONST               6 ('account/email/password_reset_key')
+                           450 LOAD_FAST                4 (email)
+                           452 LOAD_FAST               11 (context)
+               
+                80         454 PRECALL                  3
+                           458 CALL                     3
+                           468 POP_TOP
+                           470 JUMP_BACKWARD          173 (to 126)
+               
+                83     >>  472 LOAD_FAST                0 (self)
+                           474 LOAD_ATTR                1 (cleaned_data)
+                           484 LOAD_CONST               1 ('email')
+                           486 BINARY_SUBSCR
+                           496 RETURN_VALUE
                consts
                   None
                   'email'
                   'token_generator'
                   'url_generator'
-                  ('current_site', 'user', 'password_reset_url', 'request')
+                  ('current_site', 'user', 'password_reset_url', 'request', 'token', 'uid')
                   'username'
                   'account/email/password_reset_key'
-               names      ('get_current_site', 'cleaned_data', 'get', 'default_token_generator', 'users', 'make_token', 'default_url_generator', 'allauth_account_settings', 'AUTHENTICATION_METHOD', 'AuthenticationMethod', 'EMAIL', 'user_username', 'get_adapter', 'send_mail')
-               varnames   ('self', 'request', 'kwargs', 'current_site', 'email', 'token_generator', 'user', 'temp_key', 'url_generator', 'url', 'context')
+               names      ('get_current_site', 'cleaned_data', 'get', 'default_token_generator', 'users', 'make_token', 'default_url_generator', 'user_pk_to_url_str', 'allauth_account_settings', 'AUTHENTICATION_METHOD', 'AuthenticationMethod', 'EMAIL', 'user_username', 'get_adapter', 'send_mail')
+               varnames   ('self', 'request', 'kwargs', 'current_site', 'email', 'token_generator', 'user', 'temp_key', 'url_generator', 'url', 'uid', 'context')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/forms.py'
                name       'save'
                firstlineno 49
                lnotab
-                  0x02011e011a01360212022a0736011a0302010201020102fc0607160120
-                  ff08032401320106ff1203
+                  0x02011e011a01360212022a0736011a011e030201020102010201020102
+                  fa0609160120ff08032401320106ff1203
             None
          names      ('__name__', '__module__', '__qualname__', 'clean_email', 'save')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/forms.py'
          name       'AllAuthPasswordResetForm'
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/forms.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/jwt_auth.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/jwt_auth.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa9385764 (Sun May  7 05:35:37 2023 UTC)
-files sz: 6282
+moddate:  0x9faf0066 (Sun Mar 24 22:56:31 2024 UTC)
+files sz: 6698
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a040100640064
@@ -74,43 +74,43 @@
                 98 STORE_NAME              16 (api_settings)
                100 POP_TOP
    
     12         102 LOAD_CONST              10 (<code object set_jwt_access_cookie, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 12>)
                104 MAKE_FUNCTION            0
                106 STORE_NAME              17 (set_jwt_access_cookie)
    
-    31         108 LOAD_CONST              11 (<code object set_jwt_refresh_cookie, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 31>)
+    34         108 LOAD_CONST              11 (<code object set_jwt_refresh_cookie, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 34>)
                110 MAKE_FUNCTION            0
                112 STORE_NAME              18 (set_jwt_refresh_cookie)
    
-    52         114 LOAD_CONST              12 (<code object set_jwt_cookies, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 52>)
+    57         114 LOAD_CONST              12 (<code object set_jwt_cookies, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 57>)
                116 MAKE_FUNCTION            0
                118 STORE_NAME              19 (set_jwt_cookies)
    
-    57         120 LOAD_CONST              13 (<code object unset_jwt_cookies, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 57>)
+    62         120 LOAD_CONST              13 (<code object unset_jwt_cookies, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 62>)
                122 MAKE_FUNCTION            0
                124 STORE_NAME              20 (unset_jwt_cookies)
    
-    69         126 PUSH_NULL
+    75         126 PUSH_NULL
                128 LOAD_BUILD_CLASS
-               130 LOAD_CONST              14 (<code object CookieTokenRefreshSerializer, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 69>)
+               130 LOAD_CONST              14 (<code object CookieTokenRefreshSerializer, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 75>)
                132 MAKE_FUNCTION            0
                134 LOAD_CONST              15 ('CookieTokenRefreshSerializer')
                136 LOAD_NAME               14 (TokenRefreshSerializer)
                138 PRECALL                  3
                142 CALL                     3
                152 STORE_NAME              21 (CookieTokenRefreshSerializer)
    
-    88         154 LOAD_CONST              16 (<code object get_refresh_view, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 88>)
+    94         154 LOAD_CONST              16 (<code object get_refresh_view, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 94>)
                156 MAKE_FUNCTION            0
                158 STORE_NAME              22 (get_refresh_view)
    
-   107         160 PUSH_NULL
+   116         160 PUSH_NULL
                162 LOAD_BUILD_CLASS
-               164 LOAD_CONST              17 (<code object JWTCookieAuthentication, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 107>)
+               164 LOAD_CONST              17 (<code object JWTCookieAuthentication, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 116>)
                166 MAKE_FUNCTION            0
                168 LOAD_CONST              18 ('JWTCookieAuthentication')
                170 LOAD_NAME               12 (JWTAuthentication)
                172 PRECALL                  3
                176 CALL                     3
                186 STORE_NAME              23 (JWTCookieAuthentication)
                188 LOAD_CONST              19 (None)
@@ -124,26 +124,27 @@
       ('CSRFCheck',)
       ('JWTAuthentication',)
       ('TokenRefreshSerializer',)
       1
       ('api_settings',)
       code
          argcount  : 2
-         nlocals   : 8
-         stacksize : 8
+         nlocals   : 9
+         stacksize : 9
          flags     : 3
          code
             0x9700640164026c006d017d0201007402000000000000000000006a0200
             000000000000007d037407000000000000000000006a0400000000000000
             00a6000000ab0000000000000000007c026a0500000000000000007a0000
             007d047402000000000000000000006a0600000000000000007d05740200
             0000000000000000006a0700000000000000007d06740200000000000000
-            0000006a0800000000000000007d077c03721d7c00a00900000000000000
-            000000000000000000000000007c037c017c047c057c067c07ac03a60600
-            00ab06000000000000000001006400530064005300
+            0000006a0800000000000000007d077402000000000000000000006a0900
+            000000000000007d087c03721e7c00a00a00000000000000000000000000
+            000000000000007c037c017c047c057c067c077c08ac03a6070000ab0700
+            0000000000000001006400530064005300
           12           0 RESUME                   0
          
           13           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('api_settings',))
                        6 IMPORT_NAME              0 (rest_framework_simplejwt.settings)
                        8 IMPORT_FROM              1 (api_settings)
                       10 STORE_FAST               2 (jwt_settings)
@@ -170,172 +171,185 @@
                      128 LOAD_ATTR                7 (JWT_AUTH_HTTPONLY)
                      138 STORE_FAST               6 (cookie_httponly)
          
           18         140 LOAD_GLOBAL              2 (api_settings)
                      152 LOAD_ATTR                8 (JWT_AUTH_SAMESITE)
                      162 STORE_FAST               7 (cookie_samesite)
          
-          20         164 LOAD_FAST                3 (cookie_name)
-                     166 POP_JUMP_FORWARD_IF_FALSE    29 (to 226)
+          19         164 LOAD_GLOBAL              2 (api_settings)
+                     176 LOAD_ATTR                9 (JWT_AUTH_COOKIE_DOMAIN)
+                     186 STORE_FAST               8 (cookie_domain)
+         
+          22         188 LOAD_FAST                3 (cookie_name)
+                     190 POP_JUMP_FORWARD_IF_FALSE    30 (to 252)
          
-          21         168 LOAD_FAST                0 (response)
-                     170 LOAD_METHOD              9 (set_cookie)
+          23         192 LOAD_FAST                0 (response)
+                     194 LOAD_METHOD             10 (set_cookie)
          
-          22         192 LOAD_FAST                3 (cookie_name)
+          24         216 LOAD_FAST                3 (cookie_name)
          
-          23         194 LOAD_FAST                1 (access_token)
+          25         218 LOAD_FAST                1 (access_token)
          
-          24         196 LOAD_FAST                4 (access_token_expiration)
+          26         220 LOAD_FAST                4 (access_token_expiration)
          
-          25         198 LOAD_FAST                5 (cookie_secure)
+          27         222 LOAD_FAST                5 (cookie_secure)
          
-          26         200 LOAD_FAST                6 (cookie_httponly)
+          28         224 LOAD_FAST                6 (cookie_httponly)
          
-          27         202 LOAD_FAST                7 (cookie_samesite)
+          29         226 LOAD_FAST                7 (cookie_samesite)
          
-          21         204 KW_NAMES                 3
-                     206 PRECALL                  6
-                     210 CALL                     6
-                     220 POP_TOP
-                     222 LOAD_CONST               0 (None)
-                     224 RETURN_VALUE
+          30         228 LOAD_FAST                8 (cookie_domain)
          
-          20     >>  226 LOAD_CONST               0 (None)
-                     228 RETURN_VALUE
+          23         230 KW_NAMES                 3
+                     232 PRECALL                  7
+                     236 CALL                     7
+                     246 POP_TOP
+                     248 LOAD_CONST               0 (None)
+                     250 RETURN_VALUE
+         
+          22     >>  252 LOAD_CONST               0 (None)
+                     254 RETURN_VALUE
          consts
             None
             0
             ('api_settings',)
-            ('expires', 'secure', 'httponly', 'samesite')
-         names      ('rest_framework_simplejwt.settings', 'api_settings', 'JWT_AUTH_COOKIE', 'timezone', 'now', 'ACCESS_TOKEN_LIFETIME', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'set_cookie')
-         varnames   ('response', 'access_token', 'jwt_settings', 'cookie_name', 'access_token_expiration', 'cookie_secure', 'cookie_httponly', 'cookie_samesite')
+            ('expires', 'secure', 'httponly', 'samesite', 'domain')
+         names      ('rest_framework_simplejwt.settings', 'api_settings', 'JWT_AUTH_COOKIE', 'timezone', 'now', 'ACCESS_TOKEN_LIFETIME', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_COOKIE_DOMAIN', 'set_cookie')
+         varnames   ('response', 'access_token', 'jwt_settings', 'cookie_name', 'access_token_expiration', 'cookie_secure', 'cookie_httponly', 'cookie_samesite', 'cookie_domain')
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'set_jwt_access_cookie'
          firstlineno 12
          lnotab
-            0x02010c0118013601180118011802040118010201020102010201020102
-            fa16ff
+            0x02010c0118013601180118011801180304011801020102010201020102
+            01020102f916ff
       code
          argcount  : 2
-         nlocals   : 9
-         stacksize : 9
+         nlocals   : 10
+         stacksize : 10
          flags     : 3
          code
             0x9700640164026c006d017d0201007405000000000000000000006a0300
             00000000000000a6000000ab0000000000000000007c026a040000000000
             0000007a0000007d037402000000000000000000006a0500000000000000
             007d047402000000000000000000006a0600000000000000007d05740200
             0000000000000000006a0700000000000000007d06740200000000000000
             0000006a0800000000000000007d077402000000000000000000006a0900
-            000000000000007d087c04721e7c00a00a00000000000000000000000000
-            000000000000007c047c017c037c067c077c087c05ac03a6070000ab0700
-            0000000000000001006400530064005300
-          31           0 RESUME                   0
+            000000000000007d087402000000000000000000006a0a00000000000000
+            007d097c04721f7c00a00b00000000000000000000000000000000000000
+            007c047c017c037c067c077c087c057c09ac03a6080000ab080000000000
+            00000001006400530064005300
+          34           0 RESUME                   0
          
-          32           2 LOAD_CONST               1 (0)
+          35           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('api_settings',))
                        6 IMPORT_NAME              0 (rest_framework_simplejwt.settings)
                        8 IMPORT_FROM              1 (api_settings)
                       10 STORE_FAST               2 (jwt_settings)
                       12 POP_TOP
          
-          33          14 LOAD_GLOBAL              5 (NULL + timezone)
+          36          14 LOAD_GLOBAL              5 (NULL + timezone)
                       26 LOAD_ATTR                3 (now)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_FAST                2 (jwt_settings)
                       52 LOAD_ATTR                4 (REFRESH_TOKEN_LIFETIME)
                       62 BINARY_OP                0 (+)
                       66 STORE_FAST               3 (refresh_token_expiration)
          
-          34          68 LOAD_GLOBAL              2 (api_settings)
+          37          68 LOAD_GLOBAL              2 (api_settings)
                       80 LOAD_ATTR                5 (JWT_AUTH_REFRESH_COOKIE)
                       90 STORE_FAST               4 (refresh_cookie_name)
          
-          35          92 LOAD_GLOBAL              2 (api_settings)
+          38          92 LOAD_GLOBAL              2 (api_settings)
                      104 LOAD_ATTR                6 (JWT_AUTH_REFRESH_COOKIE_PATH)
                      114 STORE_FAST               5 (refresh_cookie_path)
          
-          36         116 LOAD_GLOBAL              2 (api_settings)
+          39         116 LOAD_GLOBAL              2 (api_settings)
                      128 LOAD_ATTR                7 (JWT_AUTH_SECURE)
                      138 STORE_FAST               6 (cookie_secure)
          
-          37         140 LOAD_GLOBAL              2 (api_settings)
+          40         140 LOAD_GLOBAL              2 (api_settings)
                      152 LOAD_ATTR                8 (JWT_AUTH_HTTPONLY)
                      162 STORE_FAST               7 (cookie_httponly)
          
-          38         164 LOAD_GLOBAL              2 (api_settings)
+          41         164 LOAD_GLOBAL              2 (api_settings)
                      176 LOAD_ATTR                9 (JWT_AUTH_SAMESITE)
                      186 STORE_FAST               8 (cookie_samesite)
          
-          40         188 LOAD_FAST                4 (refresh_cookie_name)
-                     190 POP_JUMP_FORWARD_IF_FALSE    30 (to 252)
+          42         188 LOAD_GLOBAL              2 (api_settings)
+                     200 LOAD_ATTR               10 (JWT_AUTH_COOKIE_DOMAIN)
+                     210 STORE_FAST               9 (cookie_domain)
          
-          41         192 LOAD_FAST                0 (response)
-                     194 LOAD_METHOD             10 (set_cookie)
+          44         212 LOAD_FAST                4 (refresh_cookie_name)
+                     214 POP_JUMP_FORWARD_IF_FALSE    31 (to 278)
          
-          42         216 LOAD_FAST                4 (refresh_cookie_name)
+          45         216 LOAD_FAST                0 (response)
+                     218 LOAD_METHOD             11 (set_cookie)
          
-          43         218 LOAD_FAST                1 (refresh_token)
+          46         240 LOAD_FAST                4 (refresh_cookie_name)
          
-          44         220 LOAD_FAST                3 (refresh_token_expiration)
+          47         242 LOAD_FAST                1 (refresh_token)
          
-          45         222 LOAD_FAST                6 (cookie_secure)
+          48         244 LOAD_FAST                3 (refresh_token_expiration)
          
-          46         224 LOAD_FAST                7 (cookie_httponly)
+          49         246 LOAD_FAST                6 (cookie_secure)
          
-          47         226 LOAD_FAST                8 (cookie_samesite)
+          50         248 LOAD_FAST                7 (cookie_httponly)
          
-          48         228 LOAD_FAST                5 (refresh_cookie_path)
+          51         250 LOAD_FAST                8 (cookie_samesite)
          
-          41         230 KW_NAMES                 3
-                     232 PRECALL                  7
-                     236 CALL                     7
-                     246 POP_TOP
-                     248 LOAD_CONST               0 (None)
-                     250 RETURN_VALUE
+          52         252 LOAD_FAST                5 (refresh_cookie_path)
          
-          40     >>  252 LOAD_CONST               0 (None)
-                     254 RETURN_VALUE
+          53         254 LOAD_FAST                9 (cookie_domain)
+         
+          45         256 KW_NAMES                 3
+                     258 PRECALL                  8
+                     262 CALL                     8
+                     272 POP_TOP
+                     274 LOAD_CONST               0 (None)
+                     276 RETURN_VALUE
+         
+          44     >>  278 LOAD_CONST               0 (None)
+                     280 RETURN_VALUE
          consts
             None
             0
             ('api_settings',)
-            ('expires', 'secure', 'httponly', 'samesite', 'path')
-         names      ('rest_framework_simplejwt.settings', 'api_settings', 'timezone', 'now', 'REFRESH_TOKEN_LIFETIME', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'set_cookie')
-         varnames   ('response', 'refresh_token', 'jwt_settings', 'refresh_token_expiration', 'refresh_cookie_name', 'refresh_cookie_path', 'cookie_secure', 'cookie_httponly', 'cookie_samesite')
+            ('expires', 'secure', 'httponly', 'samesite', 'path', 'domain')
+         names      ('rest_framework_simplejwt.settings', 'api_settings', 'timezone', 'now', 'REFRESH_TOKEN_LIFETIME', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SECURE', 'JWT_AUTH_HTTPONLY', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_COOKIE_DOMAIN', 'set_cookie')
+         varnames   ('response', 'refresh_token', 'jwt_settings', 'refresh_token_expiration', 'refresh_cookie_name', 'refresh_cookie_path', 'cookie_secure', 'cookie_httponly', 'cookie_samesite', 'cookie_domain')
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'set_jwt_refresh_cookie'
-         firstlineno 31
+         firstlineno 34
          lnotab
-            0x02010c0136011801180118011801180204011801020102010201020102
-            01020102f916ff
+            0x02010c0136011801180118011801180118020401180102010201020102
+            0102010201020102f816ff
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01a6020000ab020000000000
             00000001007403000000000000000000007c007c02a6020000ab02000000
             0000000000010064005300
-          52           0 RESUME                   0
+          57           0 RESUME                   0
          
-          53           2 LOAD_GLOBAL              1 (NULL + set_jwt_access_cookie)
+          58           2 LOAD_GLOBAL              1 (NULL + set_jwt_access_cookie)
                       14 LOAD_FAST                0 (response)
                       16 LOAD_FAST                1 (access_token)
                       18 PRECALL                  2
                       22 CALL                     2
                       32 POP_TOP
          
-          54          34 LOAD_GLOBAL              3 (NULL + set_jwt_refresh_cookie)
+          59          34 LOAD_GLOBAL              3 (NULL + set_jwt_refresh_cookie)
                       46 LOAD_FAST                0 (response)
                       48 LOAD_FAST                2 (refresh_token)
                       50 PRECALL                  2
                       54 CALL                     2
                       64 POP_TOP
                       66 LOAD_CONST               0 (None)
                       68 RETURN_VALUE
@@ -343,127 +357,134 @@
             None
          names      ('set_jwt_access_cookie', 'set_jwt_refresh_cookie')
          varnames   ('response', 'access_token', 'refresh_token')
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'set_jwt_cookies'
-         firstlineno 52
+         firstlineno 57
          lnotab 0x02012001
       code
          argcount  : 1
-         nlocals   : 5
-         stacksize : 5
+         nlocals   : 6
+         stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a0100000000000000007d01740000
             0000000000000000006a0200000000000000007d02740000000000000000
             0000006a0300000000000000007d037400000000000000000000006a0400
-            000000000000007d047c0172177c00a00500000000000000000000000000
-            000000000000007c017c04ac01a6020000ab02000000000000000001007c
-            02721a7c00a00500000000000000000000000000000000000000007c027c
-            037c04ac02a6030000ab03000000000000000001006400530064005300
-          57           0 RESUME                   0
+            000000000000007d047400000000000000000000006a0500000000000000
+            007d057c0172187c00a00600000000000000000000000000000000000000
+            007c017c047c05ac01a6030000ab03000000000000000001007c02721b7c
+            00a00600000000000000000000000000000000000000007c027c037c047c
+            05ac02a6040000ab04000000000000000001006400530064005300
+          62           0 RESUME                   0
          
-          58           2 LOAD_GLOBAL              0 (api_settings)
+          63           2 LOAD_GLOBAL              0 (api_settings)
                       14 LOAD_ATTR                1 (JWT_AUTH_COOKIE)
                       24 STORE_FAST               1 (cookie_name)
          
-          59          26 LOAD_GLOBAL              0 (api_settings)
+          64          26 LOAD_GLOBAL              0 (api_settings)
                       38 LOAD_ATTR                2 (JWT_AUTH_REFRESH_COOKIE)
                       48 STORE_FAST               2 (refresh_cookie_name)
          
-          60          50 LOAD_GLOBAL              0 (api_settings)
+          65          50 LOAD_GLOBAL              0 (api_settings)
                       62 LOAD_ATTR                3 (JWT_AUTH_REFRESH_COOKIE_PATH)
                       72 STORE_FAST               3 (refresh_cookie_path)
          
-          61          74 LOAD_GLOBAL              0 (api_settings)
+          66          74 LOAD_GLOBAL              0 (api_settings)
                       86 LOAD_ATTR                4 (JWT_AUTH_SAMESITE)
                       96 STORE_FAST               4 (cookie_samesite)
          
-          63          98 LOAD_FAST                1 (cookie_name)
-                     100 POP_JUMP_FORWARD_IF_FALSE    23 (to 148)
+          67          98 LOAD_GLOBAL              0 (api_settings)
+                     110 LOAD_ATTR                5 (JWT_AUTH_COOKIE_DOMAIN)
+                     120 STORE_FAST               5 (cookie_domain)
+         
+          69         122 LOAD_FAST                1 (cookie_name)
+                     124 POP_JUMP_FORWARD_IF_FALSE    24 (to 174)
+         
+          70         126 LOAD_FAST                0 (response)
+                     128 LOAD_METHOD              6 (delete_cookie)
+                     150 LOAD_FAST                1 (cookie_name)
+                     152 LOAD_FAST                4 (cookie_samesite)
+                     154 LOAD_FAST                5 (cookie_domain)
+                     156 KW_NAMES                 1
+                     158 PRECALL                  3
+                     162 CALL                     3
+                     172 POP_TOP
+         
+          71     >>  174 LOAD_FAST                2 (refresh_cookie_name)
+                     176 POP_JUMP_FORWARD_IF_FALSE    27 (to 232)
+         
+          72         178 LOAD_FAST                0 (response)
+                     180 LOAD_METHOD              6 (delete_cookie)
+                     202 LOAD_FAST                2 (refresh_cookie_name)
+                     204 LOAD_FAST                3 (refresh_cookie_path)
+                     206 LOAD_FAST                4 (cookie_samesite)
+                     208 LOAD_FAST                5 (cookie_domain)
+                     210 KW_NAMES                 2
+                     212 PRECALL                  4
+                     216 CALL                     4
+                     226 POP_TOP
+                     228 LOAD_CONST               0 (None)
+                     230 RETURN_VALUE
          
-          64         102 LOAD_FAST                0 (response)
-                     104 LOAD_METHOD              5 (delete_cookie)
-                     126 LOAD_FAST                1 (cookie_name)
-                     128 LOAD_FAST                4 (cookie_samesite)
-                     130 KW_NAMES                 1
-                     132 PRECALL                  2
-                     136 CALL                     2
-                     146 POP_TOP
-         
-          65     >>  148 LOAD_FAST                2 (refresh_cookie_name)
-                     150 POP_JUMP_FORWARD_IF_FALSE    26 (to 204)
-         
-          66         152 LOAD_FAST                0 (response)
-                     154 LOAD_METHOD              5 (delete_cookie)
-                     176 LOAD_FAST                2 (refresh_cookie_name)
-                     178 LOAD_FAST                3 (refresh_cookie_path)
-                     180 LOAD_FAST                4 (cookie_samesite)
-                     182 KW_NAMES                 2
-                     184 PRECALL                  3
-                     188 CALL                     3
-                     198 POP_TOP
-                     200 LOAD_CONST               0 (None)
-                     202 RETURN_VALUE
-         
-          65     >>  204 LOAD_CONST               0 (None)
-                     206 RETURN_VALUE
+          71     >>  232 LOAD_CONST               0 (None)
+                     234 RETURN_VALUE
          consts
             None
-            ('samesite',)
-            ('path', 'samesite')
-         names      ('api_settings', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SAMESITE', 'delete_cookie')
-         varnames   ('response', 'cookie_name', 'refresh_cookie_name', 'refresh_cookie_path', 'cookie_samesite')
+            ('samesite', 'domain')
+            ('path', 'samesite', 'domain')
+         names      ('api_settings', 'JWT_AUTH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE', 'JWT_AUTH_REFRESH_COOKIE_PATH', 'JWT_AUTH_SAMESITE', 'JWT_AUTH_COOKIE_DOMAIN', 'delete_cookie')
+         varnames   ('response', 'cookie_name', 'refresh_cookie_name', 'refresh_cookie_path', 'cookie_samesite', 'cookie_domain')
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'unset_jwt_cookies'
-         firstlineno 57
-         lnotab 0x0201180118011801180204012e01040134ff
+         firstlineno 62
+         lnotab 0x02011801180118011801180204013001040136ff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x8700970065005a0164005a02020065036a040000000000000000640102
             0065056402a6010000ab010000000000000000ac03a6020000ab02000000
             00000000005a06640484005a0788006601640584085a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-          69           2 RESUME                   0
+          75           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CookieTokenRefreshSerializer')
                       10 STORE_NAME               2 (__qualname__)
          
-          70          12 PUSH_NULL
+          76          12 PUSH_NULL
                       14 LOAD_NAME                3 (serializers)
                       16 LOAD_ATTR                4 (CharField)
                       26 LOAD_CONST               1 (False)
                       28 PUSH_NULL
                       30 LOAD_NAME                5 (_)
                       32 LOAD_CONST               2 ('WIll override cookie.')
                       34 PRECALL                  1
                       38 CALL                     1
                       48 KW_NAMES                 3
                       50 PRECALL                  2
                       54 CALL                     2
                       64 STORE_NAME               6 (refresh)
          
-          72          66 LOAD_CONST               4 (<code object extract_refresh_token, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 72>)
+          78          66 LOAD_CONST               4 (<code object extract_refresh_token, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 78>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME               7 (extract_refresh_token)
          
-          83          72 LOAD_CLOSURE             0 (__class__)
+          89          72 LOAD_CLOSURE             0 (__class__)
                       74 BUILD_TUPLE              1
-                      76 LOAD_CONST               5 (<code object validate, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 83>)
+                      76 LOAD_CONST               5 (<code object validate, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 89>)
                       78 MAKE_FUNCTION            8 (closure)
                       80 STORE_NAME               8 (validate)
                       82 LOAD_CLOSURE             0 (__class__)
                       84 COPY                     1
                       86 STORE_NAME               9 (__classcell__)
                       88 RETURN_VALUE
          consts
@@ -482,69 +503,69 @@
                   021900000000000000000064036b0300000000720d7c016a010000000000
                   00000064021900000000000000000053007404000000000000000000006a
                   0300000000000000007d027c0272237c027c016a04000000000000000076
                   00721a7c016a040000000000000000a00500000000000000000000000000
                   000000000000007c02a6010000ab0100000000000000005300640464056c
                   066d077d03010002007c037411000000000000000000006406a6010000ab
                   010000000000000000a6010000ab0100000000000000008201
-                72           0 RESUME                   0
+                78           0 RESUME                   0
                
-                73           2 LOAD_FAST                0 (self)
+                79           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (context)
                             14 LOAD_CONST               1 ('request')
                             16 BINARY_SUBSCR
                             26 STORE_FAST               1 (request)
                
-                74          28 LOAD_CONST               2 ('refresh')
+                80          28 LOAD_CONST               2 ('refresh')
                             30 LOAD_FAST                1 (request)
                             32 LOAD_ATTR                1 (data)
                             42 CONTAINS_OP              0
                             44 POP_JUMP_FORWARD_IF_FALSE    30 (to 106)
                             46 LOAD_FAST                1 (request)
                             48 LOAD_ATTR                1 (data)
                             58 LOAD_CONST               2 ('refresh')
                             60 BINARY_SUBSCR
                             70 LOAD_CONST               3 ('')
                             72 COMPARE_OP               3 (!=)
                             78 POP_JUMP_FORWARD_IF_FALSE    13 (to 106)
                
-                75          80 LOAD_FAST                1 (request)
+                81          80 LOAD_FAST                1 (request)
                             82 LOAD_ATTR                1 (data)
                             92 LOAD_CONST               2 ('refresh')
                             94 BINARY_SUBSCR
                            104 RETURN_VALUE
                
-                76     >>  106 LOAD_GLOBAL              4 (api_settings)
+                82     >>  106 LOAD_GLOBAL              4 (api_settings)
                            118 LOAD_ATTR                3 (JWT_AUTH_REFRESH_COOKIE)
                            128 STORE_FAST               2 (cookie_name)
                
-                77         130 LOAD_FAST                2 (cookie_name)
+                83         130 LOAD_FAST                2 (cookie_name)
                            132 POP_JUMP_FORWARD_IF_FALSE    35 (to 204)
                            134 LOAD_FAST                2 (cookie_name)
                            136 LOAD_FAST                1 (request)
                            138 LOAD_ATTR                4 (COOKIES)
                            148 CONTAINS_OP              0
                            150 POP_JUMP_FORWARD_IF_FALSE    26 (to 204)
                
-                78         152 LOAD_FAST                1 (request)
+                84         152 LOAD_FAST                1 (request)
                            154 LOAD_ATTR                4 (COOKIES)
                            164 LOAD_METHOD              5 (get)
                            186 LOAD_FAST                2 (cookie_name)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 RETURN_VALUE
                
-                80     >>  204 LOAD_CONST               4 (0)
+                86     >>  204 LOAD_CONST               4 (0)
                            206 LOAD_CONST               5 (('InvalidToken',))
                            208 IMPORT_NAME              6 (rest_framework_simplejwt.exceptions)
                            210 IMPORT_FROM              7 (InvalidToken)
                            212 STORE_FAST               3 (InvalidToken)
                            214 POP_TOP
                
-                81         216 PUSH_NULL
+                87         216 PUSH_NULL
                            218 LOAD_FAST                3 (InvalidToken)
                            220 LOAD_GLOBAL             17 (NULL + _)
                            232 LOAD_CONST               6 ('No valid refresh token found.')
                            234 PRECALL                  1
                            238 CALL                     1
                            248 PRECALL                  1
                            252 CALL                     1
@@ -559,39 +580,39 @@
                   'No valid refresh token found.'
                names      ('context', 'data', 'api_settings', 'JWT_AUTH_REFRESH_COOKIE', 'COOKIES', 'get', 'rest_framework_simplejwt.exceptions', 'InvalidToken', '_')
                varnames   ('self', 'request', 'cookie_name', 'InvalidToken')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                name       'extract_refresh_token'
-               firstlineno 72
+               firstlineno 78
                lnotab 0x02011a0134011a011801160134020c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x950197007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007c0164013c000000740300000000000000
                   000000a6000000ab000000000000000000a0020000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-                83           2 RESUME                   0
+                89           2 RESUME                   0
                
-                84           4 LOAD_FAST                0 (self)
+                90           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (extract_refresh_token)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 LOAD_FAST                1 (attrs)
                             44 LOAD_CONST               1 ('refresh')
                             46 STORE_SUBSCR
                
-                85          50 LOAD_GLOBAL              3 (NULL + super)
+                91          50 LOAD_GLOBAL              3 (NULL + super)
                             62 PRECALL                  0
                             66 CALL                     0
                             76 LOAD_METHOD              2 (validate)
                             98 LOAD_FAST                1 (attrs)
                            100 PRECALL                  1
                            104 CALL                     1
                            114 RETURN_VALUE
@@ -600,65 +621,65 @@
                   'refresh'
                names      ('extract_refresh_token', 'super', 'validate')
                varnames   ('self', 'attrs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                name       'validate'
-               firstlineno 83
+               firstlineno 89
                lnotab 0x04012e01
          names      ('__name__', '__module__', '__qualname__', 'serializers', 'CharField', '_', 'refresh', 'extract_refresh_token', 'validate', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'CookieTokenRefreshSerializer'
-         firstlineno 69
+         firstlineno 75
          lnotab 0x0c013602060b
       'CookieTokenRefreshSerializer'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x87029700640164026c006d018a020100640164036c026d037d00010002
             004700880266016404840864057c00a6030000ab0300000000000000007d
             017c015300
                        0 MAKE_CELL                2 (jwt_settings)
          
-          88           2 RESUME                   0
+          94           2 RESUME                   0
          
-          90           4 LOAD_CONST               1 (0)
+          96           4 LOAD_CONST               1 (0)
                        6 LOAD_CONST               2 (('api_settings',))
                        8 IMPORT_NAME              0 (rest_framework_simplejwt.settings)
                       10 IMPORT_FROM              1 (api_settings)
                       12 STORE_DEREF              2 (jwt_settings)
                       14 POP_TOP
          
-          91          16 LOAD_CONST               1 (0)
+          97          16 LOAD_CONST               1 (0)
                       18 LOAD_CONST               3 (('TokenRefreshView',))
                       20 IMPORT_NAME              2 (rest_framework_simplejwt.views)
                       22 IMPORT_FROM              3 (TokenRefreshView)
                       24 STORE_FAST               0 (TokenRefreshView)
                       26 POP_TOP
          
-          93          28 PUSH_NULL
+          99          28 PUSH_NULL
                       30 LOAD_BUILD_CLASS
                       32 LOAD_CLOSURE             2 (jwt_settings)
                       34 BUILD_TUPLE              1
-                      36 LOAD_CONST               4 (<code object RefreshViewWithCookieSupport, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 93>)
+                      36 LOAD_CONST               4 (<code object RefreshViewWithCookieSupport, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 99>)
                       38 MAKE_FUNCTION            8 (closure)
                       40 LOAD_CONST               5 ('RefreshViewWithCookieSupport')
                       42 LOAD_FAST                0 (TokenRefreshView)
                       44 PRECALL                  3
                       48 CALL                     3
                       58 STORE_FAST               1 (RefreshViewWithCookieSupport)
          
-         104          60 LOAD_FAST                1 (RefreshViewWithCookieSupport)
+         113          60 LOAD_FAST                1 (RefreshViewWithCookieSupport)
                       62 RETURN_VALUE
          consts
             ' Returns a Token Refresh CBV without a circular import '
             0
             ('api_settings',)
             ('TokenRefreshView',)
             code
@@ -668,27 +689,27 @@
                flags     : 0
                code
                   0x95018700970065005a0164005a0265035a04880088016602640184085a
                   05880078015a065300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (__class__)
                
-                93           4 RESUME                   0
+                99           4 RESUME                   0
                              6 LOAD_NAME                0 (__name__)
                              8 STORE_NAME               1 (__module__)
                             10 LOAD_CONST               0 ('get_refresh_view.<locals>.RefreshViewWithCookieSupport')
                             12 STORE_NAME               2 (__qualname__)
                
-                94          14 LOAD_NAME                3 (CookieTokenRefreshSerializer)
+               100          14 LOAD_NAME                3 (CookieTokenRefreshSerializer)
                             16 STORE_NAME               4 (serializer_class)
                
-                96          18 LOAD_CLOSURE             0 (__class__)
+               102          18 LOAD_CLOSURE             0 (__class__)
                             20 LOAD_CLOSURE             1 (jwt_settings)
                             22 BUILD_TUPLE              2
-                            24 LOAD_CONST               1 (<code object finalize_response, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 96>)
+                            24 LOAD_CONST               1 (<code object finalize_response, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 102>)
                             26 MAKE_FUNCTION            8 (closure)
                             28 STORE_NAME               5 (finalize_response)
                             30 LOAD_CLOSURE             0 (__class__)
                             32 COPY                     1
                             34 STORE_NAME               6 (__classcell__)
                             36 RETURN_VALUE
                consts
@@ -702,163 +723,174 @@
                         0x950297007c026a0000000000000000007402000000000000000000006a
                         0200000000000000006b0200000000724764017c026a0300000000000000
                         007600723e7409000000000000000000007c027c026a0300000000000000
                         00640119000000000000000000a6020000ab020000000000000000010074
                         0b000000000000000000006a060000000000000000a6000000ab00000000
                         000000000089066a0700000000000000007a0000007c026a030000000000
                         00000064023c0000007c026a000000000000000000740200000000000000
-                        0000006a0200000000000000006b0200000000724764037c026a03000000
-                        00000000007600723e7411000000000000000000007c027c026a03000000
+                        0000006a0200000000000000006b0200000000725c64037c026a03000000
+                        0000000000760072537411000000000000000000007c027c026a03000000
                         0000000000640319000000000000000000a6020000ab0200000000000000
-                        000100740b000000000000000000006a060000000000000000a6000000ab
-                        00000000000000000089066a0900000000000000007a0000007c026a0300
-                        0000000000000064043c0000000200741500000000000000000000a60000
-                        00ab0000000000000000006a0b00000000000000007c017c0267027c03a2
-                        01520069007c04a4018e015300
+                        0001007412000000000000000000006a0a000000000000000072097c026a
+                        03000000000000000064033d006e23740b000000000000000000006a0600
+                        00000000000000a6000000ab00000000000000000089066a0b0000000000
+                        0000007a0000007c026a03000000000000000064043c0000000200741900
+                        000000000000000000a6000000ab0000000000000000006a0d0000000000
+                        0000007c017c0267027c03a201520069007c04a4018e015300
                                    0 COPY_FREE_VARS           2
                      
-                      96           2 RESUME                   0
+                     102           2 RESUME                   0
                      
-                      97           4 LOAD_FAST                2 (response)
+                     103           4 LOAD_FAST                2 (response)
                                    6 LOAD_ATTR                0 (status_code)
                                   16 LOAD_GLOBAL              2 (status)
                                   28 LOAD_ATTR                2 (HTTP_200_OK)
                                   38 COMPARE_OP               2 (==)
                                   44 POP_JUMP_FORWARD_IF_FALSE    71 (to 188)
                                   46 LOAD_CONST               1 ('access')
                                   48 LOAD_FAST                2 (response)
                                   50 LOAD_ATTR                3 (data)
                                   60 CONTAINS_OP              0
                                   62 POP_JUMP_FORWARD_IF_FALSE    62 (to 188)
                      
-                      98          64 LOAD_GLOBAL              9 (NULL + set_jwt_access_cookie)
+                     104          64 LOAD_GLOBAL              9 (NULL + set_jwt_access_cookie)
                                   76 LOAD_FAST                2 (response)
                                   78 LOAD_FAST                2 (response)
                                   80 LOAD_ATTR                3 (data)
                                   90 LOAD_CONST               1 ('access')
                                   92 BINARY_SUBSCR
                                  102 PRECALL                  2
                                  106 CALL                     2
                                  116 POP_TOP
                      
-                      99         118 LOAD_GLOBAL             11 (NULL + timezone)
+                     105         118 LOAD_GLOBAL             11 (NULL + timezone)
                                  130 LOAD_ATTR                6 (now)
                                  140 PRECALL                  0
                                  144 CALL                     0
                                  154 LOAD_DEREF               6 (jwt_settings)
                                  156 LOAD_ATTR                7 (ACCESS_TOKEN_LIFETIME)
                                  166 BINARY_OP                0 (+)
                                  170 LOAD_FAST                2 (response)
                                  172 LOAD_ATTR                3 (data)
                                  182 LOAD_CONST               2 ('access_expiration')
                                  184 STORE_SUBSCR
                      
-                     100     >>  188 LOAD_FAST                2 (response)
+                     106     >>  188 LOAD_FAST                2 (response)
                                  190 LOAD_ATTR                0 (status_code)
                                  200 LOAD_GLOBAL              2 (status)
                                  212 LOAD_ATTR                2 (HTTP_200_OK)
                                  222 COMPARE_OP               2 (==)
-                                 228 POP_JUMP_FORWARD_IF_FALSE    71 (to 372)
+                                 228 POP_JUMP_FORWARD_IF_FALSE    92 (to 414)
                                  230 LOAD_CONST               3 ('refresh')
                                  232 LOAD_FAST                2 (response)
                                  234 LOAD_ATTR                3 (data)
                                  244 CONTAINS_OP              0
-                                 246 POP_JUMP_FORWARD_IF_FALSE    62 (to 372)
+                                 246 POP_JUMP_FORWARD_IF_FALSE    83 (to 414)
                      
-                     101         248 LOAD_GLOBAL             17 (NULL + set_jwt_refresh_cookie)
+                     107         248 LOAD_GLOBAL             17 (NULL + set_jwt_refresh_cookie)
                                  260 LOAD_FAST                2 (response)
                                  262 LOAD_FAST                2 (response)
                                  264 LOAD_ATTR                3 (data)
                                  274 LOAD_CONST               3 ('refresh')
                                  276 BINARY_SUBSCR
                                  286 PRECALL                  2
                                  290 CALL                     2
                                  300 POP_TOP
                      
-                     102         302 LOAD_GLOBAL             11 (NULL + timezone)
-                                 314 LOAD_ATTR                6 (now)
-                                 324 PRECALL                  0
-                                 328 CALL                     0
-                                 338 LOAD_DEREF               6 (jwt_settings)
-                                 340 LOAD_ATTR                9 (REFRESH_TOKEN_LIFETIME)
-                                 350 BINARY_OP                0 (+)
-                                 354 LOAD_FAST                2 (response)
-                                 356 LOAD_ATTR                3 (data)
-                                 366 LOAD_CONST               4 ('refresh_expiration')
-                                 368 STORE_SUBSCR
+                     108         302 LOAD_GLOBAL             18 (api_settings)
+                                 314 LOAD_ATTR               10 (JWT_AUTH_HTTPONLY)
+                                 324 POP_JUMP_FORWARD_IF_FALSE     9 (to 344)
+                     
+                     109         326 LOAD_FAST                2 (response)
+                                 328 LOAD_ATTR                3 (data)
+                                 338 LOAD_CONST               3 ('refresh')
+                                 340 DELETE_SUBSCR
+                                 342 JUMP_FORWARD            35 (to 414)
+                     
+                     111     >>  344 LOAD_GLOBAL             11 (NULL + timezone)
+                                 356 LOAD_ATTR                6 (now)
+                                 366 PRECALL                  0
+                                 370 CALL                     0
+                                 380 LOAD_DEREF               6 (jwt_settings)
+                                 382 LOAD_ATTR               11 (REFRESH_TOKEN_LIFETIME)
+                                 392 BINARY_OP                0 (+)
+                                 396 LOAD_FAST                2 (response)
+                                 398 LOAD_ATTR                3 (data)
+                                 408 LOAD_CONST               4 ('refresh_expiration')
+                                 410 STORE_SUBSCR
                      
-                     103     >>  372 PUSH_NULL
-                                 374 LOAD_GLOBAL             21 (NULL + super)
-                                 386 PRECALL                  0
-                                 390 CALL                     0
-                                 400 LOAD_ATTR               11 (finalize_response)
-                                 410 LOAD_FAST                1 (request)
-                                 412 LOAD_FAST                2 (response)
-                                 414 BUILD_LIST               2
-                                 416 LOAD_FAST                3 (args)
-                                 418 LIST_EXTEND              1
-                                 420 LIST_TO_TUPLE
-                                 422 BUILD_MAP                0
-                                 424 LOAD_FAST                4 (kwargs)
-                                 426 DICT_MERGE               1
-                                 428 CALL_FUNCTION_EX         1
-                                 430 RETURN_VALUE
+                     112     >>  414 PUSH_NULL
+                                 416 LOAD_GLOBAL             25 (NULL + super)
+                                 428 PRECALL                  0
+                                 432 CALL                     0
+                                 442 LOAD_ATTR               13 (finalize_response)
+                                 452 LOAD_FAST                1 (request)
+                                 454 LOAD_FAST                2 (response)
+                                 456 BUILD_LIST               2
+                                 458 LOAD_FAST                3 (args)
+                                 460 LIST_EXTEND              1
+                                 462 LIST_TO_TUPLE
+                                 464 BUILD_MAP                0
+                                 466 LOAD_FAST                4 (kwargs)
+                                 468 DICT_MERGE               1
+                                 470 CALL_FUNCTION_EX         1
+                                 472 RETURN_VALUE
                      consts
                         None
                         'access'
                         'access_expiration'
                         'refresh'
                         'refresh_expiration'
-                     names      ('status_code', 'status', 'HTTP_200_OK', 'data', 'set_jwt_access_cookie', 'timezone', 'now', 'ACCESS_TOKEN_LIFETIME', 'set_jwt_refresh_cookie', 'REFRESH_TOKEN_LIFETIME', 'super', 'finalize_response')
+                     names      ('status_code', 'status', 'HTTP_200_OK', 'data', 'set_jwt_access_cookie', 'timezone', 'now', 'ACCESS_TOKEN_LIFETIME', 'set_jwt_refresh_cookie', 'api_settings', 'JWT_AUTH_HTTPONLY', 'REFRESH_TOKEN_LIFETIME', 'super', 'finalize_response')
                      varnames   ('self', 'request', 'response', 'args', 'kwargs')
                      freevars   ('__class__', 'jwt_settings')
                      cellvars   ()
                      filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                      name       'finalize_response'
-                     firstlineno 96
-                     lnotab 0x04013c01360146013c0136014601
+                     firstlineno 102
+                     lnotab 0x04013c01360146013c013601180112024601
                names      ('__name__', '__module__', '__qualname__', 'CookieTokenRefreshSerializer', 'serializer_class', 'finalize_response', '__classcell__')
                varnames   ()
                freevars   ('jwt_settings',)
                cellvars   ('__class__',)
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                name       'RefreshViewWithCookieSupport'
-               firstlineno 93
+               firstlineno 99
                lnotab 0x0e010402
             'RefreshViewWithCookieSupport'
          names      ('rest_framework_simplejwt.settings', 'api_settings', 'rest_framework_simplejwt.views', 'TokenRefreshView')
          varnames   ('TokenRefreshView', 'RefreshViewWithCookieSupport')
          freevars   ()
          cellvars   ('jwt_settings',)
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'get_refresh_view'
-         firstlineno 88
-         lnotab 0x04020c010c02200b
+         firstlineno 94
+         lnotab 0x04020c010c02200e
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a03640284005a04640384005a05640453
             00
-         107           0 RESUME                   0
+         116           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('JWTCookieAuthentication')
                        8 STORE_NAME               2 (__qualname__)
          
-         108          10 LOAD_CONST               1 ('\n    An authentication plugin that hopefully authenticates requests through a JSON web\n    token provided in a request cookie (and through the header as normal, with a\n    preference to the header).\n    ')
+         117          10 LOAD_CONST               1 ('\n    An authentication plugin that hopefully authenticates requests through a JSON web\n    token provided in a request cookie (and through the header as normal, with a\n    preference to the header).\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         113          14 LOAD_CONST               2 (<code object enforce_csrf, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 113>)
+         122          14 LOAD_CONST               2 (<code object enforce_csrf, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 122>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (enforce_csrf)
          
-         127          20 LOAD_CONST               3 (<code object authenticate, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 127>)
+         136          20 LOAD_CONST               3 (<code object authenticate, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 136>)
                       22 MAKE_FUNCTION            0
                       24 STORE_NAME               5 (authenticate)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'JWTCookieAuthentication'
             '\n    An authentication plugin that hopefully authenticates requests through a JSON web\n    token provided in a request cookie (and through the header as normal, with a\n    preference to the header).\n    '
@@ -871,90 +903,90 @@
                   0x9700640184007d027401000000000000000000007c02a6010000ab0100
                   000000000000007d037c03a0010000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001007c03a0020000000000
                   0000000000000000000000000000007c01640264036900a6040000ab0400
                   000000000000007d047c0472177407000000000000000000006a04000000
                   000000000064047c049b009d02a6010000ab010000000000000000820164
                   025300
-               113           0 RESUME                   0
+               122           0 RESUME                   0
                
-               117           2 LOAD_CONST               1 (<code object dummy_get_response, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 117>)
+               126           2 LOAD_CONST               1 (<code object dummy_get_response, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py", line 126>)
                              4 MAKE_FUNCTION            0
                              6 STORE_FAST               2 (dummy_get_response)
                
-               119           8 LOAD_GLOBAL              1 (NULL + CSRFCheck)
+               128           8 LOAD_GLOBAL              1 (NULL + CSRFCheck)
                             20 LOAD_FAST                2 (dummy_get_response)
                             22 PRECALL                  1
                             26 CALL                     1
                             36 STORE_FAST               3 (check)
                
-               121          38 LOAD_FAST                3 (check)
+               130          38 LOAD_FAST                3 (check)
                             40 LOAD_METHOD              1 (process_request)
                             62 LOAD_FAST                1 (request)
                             64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                
-               122          80 LOAD_FAST                3 (check)
+               131          80 LOAD_FAST                3 (check)
                             82 LOAD_METHOD              2 (process_view)
                            104 LOAD_FAST                1 (request)
                            106 LOAD_CONST               2 (None)
                            108 LOAD_CONST               3 (())
                            110 BUILD_MAP                0
                            112 PRECALL                  4
                            116 CALL                     4
                            126 STORE_FAST               4 (reason)
                
-               123         128 LOAD_FAST                4 (reason)
+               132         128 LOAD_FAST                4 (reason)
                            130 POP_JUMP_FORWARD_IF_FALSE    23 (to 178)
                
-               125         132 LOAD_GLOBAL              7 (NULL + exceptions)
+               134         132 LOAD_GLOBAL              7 (NULL + exceptions)
                            144 LOAD_ATTR                4 (PermissionDenied)
                            154 LOAD_CONST               4 ('CSRF Failed: ')
                            156 LOAD_FAST                4 (reason)
                            158 FORMAT_VALUE             0
                            160 BUILD_STRING             2
                            162 PRECALL                  1
                            166 CALL                     1
                            176 RAISE_VARARGS            1
                
-               123     >>  178 LOAD_CONST               2 (None)
+               132     >>  178 LOAD_CONST               2 (None)
                            180 RETURN_VALUE
                consts
                   '\n        Enforce CSRF validation for session based authentication.\n        '
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 1
                      flags     : 19
                      code 0x970064005300
-                     117           0 RESUME                   0
+                     126           0 RESUME                   0
                      
-                     118           2 LOAD_CONST               0 (None)
+                     127           2 LOAD_CONST               0 (None)
                                    4 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('request',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                      name       'dummy_get_response'
-                     firstlineno 117
+                     firstlineno 126
                      lnotab 0x0201
                   None
                   ()
                   'CSRF Failed: '
                names      ('CSRFCheck', 'process_request', 'process_view', 'exceptions', 'PermissionDenied')
                varnames   ('self', 'request', 'dummy_get_response', 'check', 'reason')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                name       'enforce_csrf'
-               firstlineno 113
+               firstlineno 122
                lnotab 0x020406021e022a01300104022efe
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 3
                flags     : 3
                code
@@ -968,91 +1000,91 @@
                   0000006a07000000000000000072157c00a0060000000000000000000000
                   0000000000000000007c01a6010000ab01000000000000000001006e1764
                   0053007c00a00800000000000000000000000000000000000000007c03a6
                   010000ab0100000000000000007d047c048002640053007c00a009000000
                   00000000000000000000000000000000007c04a6010000ab010000000000
                   0000007d057c00a00a00000000000000000000000000000000000000007c
                   05a6010000ab0100000000000000007c0566025300
-               127           0 RESUME                   0
+               136           0 RESUME                   0
                
-               128           2 LOAD_GLOBAL              0 (api_settings)
+               137           2 LOAD_GLOBAL              0 (api_settings)
                             14 LOAD_ATTR                1 (JWT_AUTH_COOKIE)
                             24 STORE_FAST               2 (cookie_name)
                
-               129          26 LOAD_FAST                0 (self)
+               138          26 LOAD_FAST                0 (self)
                             28 LOAD_METHOD              2 (get_header)
                             50 LOAD_FAST                1 (request)
                             52 PRECALL                  1
                             56 CALL                     1
                             66 STORE_FAST               3 (header)
                
-               130          68 LOAD_FAST                3 (header)
+               139          68 LOAD_FAST                3 (header)
                             70 POP_JUMP_FORWARD_IF_NOT_NONE   100 (to 272)
                
-               131          72 LOAD_FAST                2 (cookie_name)
+               140          72 LOAD_FAST                2 (cookie_name)
                             74 POP_JUMP_FORWARD_IF_FALSE    96 (to 268)
                
-               132          76 LOAD_FAST                1 (request)
+               141          76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                3 (COOKIES)
                             88 LOAD_METHOD              4 (get)
                            110 LOAD_FAST                2 (cookie_name)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               4 (raw_token)
                
-               133         128 LOAD_GLOBAL              0 (api_settings)
+               142         128 LOAD_GLOBAL              0 (api_settings)
                            140 LOAD_ATTR                5 (JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED)
                            150 POP_JUMP_FORWARD_IF_FALSE    22 (to 196)
                
-               134         152 LOAD_FAST                0 (self)
+               143         152 LOAD_FAST                0 (self)
                            154 LOAD_METHOD              6 (enforce_csrf)
                            176 LOAD_FAST                1 (request)
                            178 PRECALL                  1
                            182 CALL                     1
                            192 POP_TOP
                            194 JUMP_FORWARD            59 (to 314)
                
-               135     >>  196 LOAD_FAST                4 (raw_token)
+               144     >>  196 LOAD_FAST                4 (raw_token)
                            198 POP_JUMP_FORWARD_IF_NONE    33 (to 266)
                            200 LOAD_GLOBAL              0 (api_settings)
                            212 LOAD_ATTR                7 (JWT_AUTH_COOKIE_USE_CSRF)
                            222 POP_JUMP_FORWARD_IF_FALSE    21 (to 266)
                
-               136         224 LOAD_FAST                0 (self)
+               145         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              6 (enforce_csrf)
                            248 LOAD_FAST                1 (request)
                            250 PRECALL                  1
                            254 CALL                     1
                            264 POP_TOP
                        >>  266 JUMP_FORWARD            23 (to 314)
                
-               138     >>  268 LOAD_CONST               0 (None)
+               147     >>  268 LOAD_CONST               0 (None)
                            270 RETURN_VALUE
                
-               140     >>  272 LOAD_FAST                0 (self)
+               149     >>  272 LOAD_FAST                0 (self)
                            274 LOAD_METHOD              8 (get_raw_token)
                            296 LOAD_FAST                3 (header)
                            298 PRECALL                  1
                            302 CALL                     1
                            312 STORE_FAST               4 (raw_token)
                
-               142     >>  314 LOAD_FAST                4 (raw_token)
+               151     >>  314 LOAD_FAST                4 (raw_token)
                            316 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 322)
                
-               143         318 LOAD_CONST               0 (None)
+               152         318 LOAD_CONST               0 (None)
                            320 RETURN_VALUE
                
-               145     >>  322 LOAD_FAST                0 (self)
+               154     >>  322 LOAD_FAST                0 (self)
                            324 LOAD_METHOD              9 (get_validated_token)
                            346 LOAD_FAST                4 (raw_token)
                            348 PRECALL                  1
                            352 CALL                     1
                            362 STORE_FAST               5 (validated_token)
                
-               146         364 LOAD_FAST                0 (self)
+               155         364 LOAD_FAST                0 (self)
                            366 LOAD_METHOD             10 (get_user)
                            388 LOAD_FAST                5 (validated_token)
                            390 PRECALL                  1
                            394 CALL                     1
                            404 LOAD_FAST                5 (validated_token)
                            406 BUILD_TUPLE              2
                            408 RETURN_VALUE
@@ -1060,32 +1092,32 @@
                   None
                names      ('api_settings', 'JWT_AUTH_COOKIE', 'get_header', 'COOKIES', 'get', 'JWT_AUTH_COOKIE_ENFORCE_CSRF_ON_UNAUTHENTICATED', 'enforce_csrf', 'JWT_AUTH_COOKIE_USE_CSRF', 'get_raw_token', 'get_validated_token', 'get_user')
                varnames   ('self', 'request', 'cookie_name', 'header', 'raw_token', 'validated_token')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
                name       'authenticate'
-               firstlineno 127
+               firstlineno 136
                lnotab
                   0x020118012a0104010401340118012c011c012c0204022a02040104022a
                   01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'enforce_csrf', 'authenticate')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
          name       'JWTCookieAuthentication'
-         firstlineno 107
+         firstlineno 116
          lnotab 0x0a010405060e
       'JWTCookieAuthentication'
       None
    names      ('django.utils', 'timezone', 'django.utils.translation', 'gettext_lazy', '_', 'rest_framework', 'status', 'exceptions', 'serializers', 'rest_framework.authentication', 'CSRFCheck', 'rest_framework_simplejwt.authentication', 'JWTAuthentication', 'rest_framework_simplejwt.serializers', 'TokenRefreshSerializer', 'app_settings', 'api_settings', 'set_jwt_access_cookie', 'set_jwt_refresh_cookie', 'set_jwt_cookies', 'unset_jwt_cookies', 'CookieTokenRefreshSerializer', 'get_refresh_view', 'JWTCookieAuthentication')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/jwt_auth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c010c0110010c010c010c020c03061306150605060c1c
-      130613
+      0x00ff02010c010c010c0110010c010c010c020c03061606170605060d1c
+      130616
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/models.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/models.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/serializers.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/serializers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/social_serializers.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/social_serializers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/urls.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/utils.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/utils.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/views.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/views.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa9385764 (Sun May  7 05:35:37 2023 UTC)
-files sz: 10760
+moddate:  0x9faf0066 (Sun Mar 24 22:56:31 2024 UTC)
+files sz: 11609
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -181,47 +181,47 @@
                294 MAKE_FUNCTION            0
                296 LOAD_CONST              26 ('LogoutView')
                298 LOAD_NAME               30 (APIView)
                300 PRECALL                  3
                304 CALL                     3
                314 STORE_NAME              39 (LogoutView)
    
-   209         316 PUSH_NULL
+   224         316 PUSH_NULL
                318 LOAD_BUILD_CLASS
-               320 LOAD_CONST              27 (<code object UserDetailsView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 209>)
+               320 LOAD_CONST              27 (<code object UserDetailsView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 224>)
                322 MAKE_FUNCTION            0
                324 LOAD_CONST              28 ('UserDetailsView')
                326 LOAD_NAME               23 (RetrieveUpdateAPIView)
                328 PRECALL                  3
                332 CALL                     3
                342 STORE_NAME              40 (UserDetailsView)
    
-   234         344 PUSH_NULL
+   249         344 PUSH_NULL
                346 LOAD_BUILD_CLASS
-               348 LOAD_CONST              29 (<code object PasswordResetView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 234>)
+               348 LOAD_CONST              29 (<code object PasswordResetView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 249>)
                350 MAKE_FUNCTION            0
                352 LOAD_CONST              30 ('PasswordResetView')
                354 LOAD_NAME               22 (GenericAPIView)
                356 PRECALL                  3
                360 CALL                     3
                370 STORE_NAME              41 (PasswordResetView)
    
-   258         372 PUSH_NULL
+   273         372 PUSH_NULL
                374 LOAD_BUILD_CLASS
-               376 LOAD_CONST              31 (<code object PasswordResetConfirmView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 258>)
+               376 LOAD_CONST              31 (<code object PasswordResetConfirmView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 273>)
                378 MAKE_FUNCTION            0
                380 LOAD_CONST              32 ('PasswordResetConfirmView')
                382 LOAD_NAME               22 (GenericAPIView)
                384 PRECALL                  3
                388 CALL                     3
                398 STORE_NAME              42 (PasswordResetConfirmView)
    
-   284         400 PUSH_NULL
+   299         400 PUSH_NULL
                402 LOAD_BUILD_CLASS
-               404 LOAD_CONST              33 (<code object PasswordChangeView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 284>)
+               404 LOAD_CONST              33 (<code object PasswordChangeView, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 299>)
                406 MAKE_FUNCTION            0
                408 LOAD_CONST              34 ('PasswordChangeView')
                410 LOAD_NAME               22 (GenericAPIView)
                412 PRECALL                  3
                416 CALL                     3
                426 STORE_NAME              43 (PasswordChangeView)
                428 LOAD_CONST              35 (None)
@@ -958,340 +958,454 @@
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 10
                stacksize : 6
                flags     : 3
                code
-                  0x970009007c016a0000000000000000006a010000000000000000a00200
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  00000001006e172300740600000000000000000000740800000000000000
-                  000000660224007203010059006e047700780359007701740a0000000000
-                  00000000006a060000000000000000720f740f000000000000000000007c
-                  01a6010000ab010000000000000000010074110000000000000000000064
-                  017413000000000000000000006402a6010000ab01000000000000000069
-                  017414000000000000000000006a0b0000000000000000ac03a6020000ab
-                  0200000000000000007d02740a000000000000000000006a0c0000000000
-                  00000090017285640464056c0d6d0e7d030100640464066c0f6d107d0401
-                  00640764086c116d127d050100740a000000000000000000006a13000000
-                  00000000007d0602007c057c02a6010000ab010000000000000000010064
-                  097428000000000000000000006a15000000000000000076009001722209
-                  0002007c047c016a160000000000000000640a19000000000000000000a6
-                  010000ab0100000000000000007d077c07a0170000000000000000000000
-                  000000000000000000a6000000ab000000000000000000010090016e2023
-                  007430000000000000000000002400722a01006401741300000000000000
-                  000000640ba6010000ab01000000000000000069017c025f160000000000
-                  0000007414000000000000000000006a1900000000000000007c025f1a00
-                  0000000000000059006eed7c037406000000000000000000007436000000
-                  000000000000006603240072ae7d087439000000000000000000007c0864
-                  0ca6020000ab020000000000000000726d640d7c086a1d00000000000000
-                  0076007309640e7c086a1d00000000000000007600723364017413000000
-                  000000000000007c086a1d00000000000000006404190000000000000000
-                  00a6010000ab01000000000000000069017c025f16000000000000000074
-                  14000000000000000000006a1900000000000000007c025f1a0000000000
-                  0000006e4f6401741300000000000000000000640fa6010000ab01000000
-                  000000000069017c025f1600000000000000007414000000000000000000
-                  006a1e00000000000000007c025f1a00000000000000006e276401741300
-                  000000000000000000640fa6010000ab01000000000000000069017c025f
-                  1600000000000000007414000000000000000000006a1e00000000000000
-                  007c025f1a0000000000000000590064007d087e086e3364007d087e0877
-                  0177007803590077017c0673297413000000000000000000006410a60100
-                  00ab0100000000000000007d0964017c0969017c025f1600000000000000
-                  007414000000000000000000006a0b00000000000000007c025f1a000000
-                  00000000007c025300
+                  0x97007c016a00000000000000000073427402000000000000000000006a
+                  02000000000000000073367402000000000000000000006a030000000000
+                  000000732a7409000000000000000000006401740b000000000000000000
+                  006402a6010000ab0100000000000000006901740c000000000000000000
+                  006a070000000000000000ac03a6020000ab020000000000000000530009
+                  007c016a0800000000000000006a090000000000000000a00a0000000000
+                  000000000000000000000000000000a6000000ab00000000000000000001
+                  006e17230074160000000000000000000074180000000000000000000066
+                  0224007203010059006e0477007803590077017402000000000000000000
+                  006a030000000000000000720f741b000000000000000000007c01a60100
+                  00ab01000000000000000001007409000000000000000000006401740b00
+                  0000000000000000006404a6010000ab0100000000000000006901740c00
+                  0000000000000000006a0e0000000000000000ac03a6020000ab02000000
+                  00000000007d027402000000000000000000006a02000000000000000090
+                  0172fb640564066c0f6d107d030100640564076c116d127d040100640864
+                  096c136d147d0501007402000000000000000000006a1500000000000000
+                  007d0602007c057c02a6010000ab0100000000000000000100640a742c00
+                  0000000000000000006a170000000000000000760090017298090002007c
+                  046400a6010000ab0100000000000000007d077402000000000000000000
+                  006a1800000000000000007259090002007c047c016a1900000000000000
+                  007402000000000000000000006a1a000000000000000019000000000000
+                  000000a6010000ab0100000000000000007d076e86230074360000000000
+                  00000000002400722a01006401740b00000000000000000000640ba60100
+                  00ab01000000000000000069017c025f1c0000000000000000740c000000
+                  000000000000006a1d00000000000000007c025f1e000000000000000059
+                  006e537700780359007701090002007c047c016a1c000000000000000064
+                  0c19000000000000000000a6010000ab0100000000000000007d076e3723
+                  007436000000000000000000002400722a01006401740b00000000000000
+                  000000640da6010000ab01000000000000000069017c025f1c0000000000
+                  000000740c000000000000000000006a1d00000000000000007c025f1e00
+                  0000000000000059006e0477007803590077017c07a01f00000000000000
+                  00000000000000000000000000a6000000ab00000000000000000001006e
+                  ee23007c0374160000000000000000000074400000000000000000000066
+                  03240072ae7d087443000000000000000000007c08640ea6020000ab0200
+                  00000000000000726d640f7c086a2200000000000000007600730964107c
+                  086a220000000000000000760072336401740b000000000000000000007c
+                  086a220000000000000000640519000000000000000000a6010000ab0100
+                  0000000000000069017c025f1c0000000000000000740c00000000000000
+                  0000006a1d00000000000000007c025f1e00000000000000006e4f640174
+                  0b000000000000000000006411a6010000ab01000000000000000069017c
+                  025f1c0000000000000000740c000000000000000000006a230000000000
+                  0000007c025f1e00000000000000006e276401740b000000000000000000
+                  006411a6010000ab01000000000000000069017c025f1c00000000000000
+                  00740c000000000000000000006a2300000000000000007c025f1e000000
+                  0000000000590064007d087e086e3364007d087e08770177007803590077
+                  017c067329740b000000000000000000006412a6010000ab010000000000
+                  0000007d0964017c0969017c025f1c0000000000000000740c0000000000
+                  00000000006a0e00000000000000007c025f1e00000000000000007c0253
+                  00
                152           0 RESUME                   0
                
-               153           2 NOP
-               
-               154           4 LOAD_FAST                1 (request)
-                             6 LOAD_ATTR                0 (user)
-                            16 LOAD_ATTR                1 (auth_token)
-                            26 LOAD_METHOD              2 (delete)
-                            48 PRECALL                  0
-                            52 CALL                     0
-                            62 POP_TOP
-                            64 JUMP_FORWARD            23 (to 112)
-                       >>   66 PUSH_EXC_INFO
-               
-               155          68 LOAD_GLOBAL              6 (AttributeError)
-                            80 LOAD_GLOBAL              8 (ObjectDoesNotExist)
-                            92 BUILD_TUPLE              2
-                            94 CHECK_EXC_MATCH
-                            96 POP_JUMP_FORWARD_IF_FALSE     3 (to 104)
-                            98 POP_TOP
+               153           2 LOAD_FAST                1 (request)
+                             4 LOAD_ATTR                0 (auth)
+                            14 POP_JUMP_FORWARD_IF_TRUE    66 (to 148)
+                            16 LOAD_GLOBAL              2 (api_settings)
+                            28 LOAD_ATTR                2 (USE_JWT)
+                            38 POP_JUMP_FORWARD_IF_TRUE    54 (to 148)
+                            40 LOAD_GLOBAL              2 (api_settings)
+                            52 LOAD_ATTR                3 (SESSION_LOGIN)
+                            62 POP_JUMP_FORWARD_IF_TRUE    42 (to 148)
+               
+               154          64 LOAD_GLOBAL              9 (NULL + Response)
+               
+               155          76 LOAD_CONST               1 ('detail')
+                            78 LOAD_GLOBAL             11 (NULL + _)
+                            90 LOAD_CONST               2 ('You should be logged in to logout. Check whether the token is passed.')
+                            92 PRECALL                  1
+                            96 CALL                     1
+                           106 BUILD_MAP                1
+               
+               156         108 LOAD_GLOBAL             12 (status)
+                           120 LOAD_ATTR                7 (HTTP_400_BAD_REQUEST)
+               
+               154         130 KW_NAMES                 3
+                           132 PRECALL                  2
+                           136 CALL                     2
+                           146 RETURN_VALUE
+               
+               158     >>  148 NOP
+               
+               159         150 LOAD_FAST                1 (request)
+                           152 LOAD_ATTR                8 (user)
+                           162 LOAD_ATTR                9 (auth_token)
+                           172 LOAD_METHOD             10 (delete)
+                           194 PRECALL                  0
+                           198 CALL                     0
+                           208 POP_TOP
+                           210 JUMP_FORWARD            23 (to 258)
+                       >>  212 PUSH_EXC_INFO
+               
+               160         214 LOAD_GLOBAL             22 (AttributeError)
+                           226 LOAD_GLOBAL             24 (ObjectDoesNotExist)
+                           238 BUILD_TUPLE              2
+                           240 CHECK_EXC_MATCH
+                           242 POP_JUMP_FORWARD_IF_FALSE     3 (to 250)
+                           244 POP_TOP
+               
+               161         246 POP_EXCEPT
+                           248 JUMP_FORWARD             4 (to 258)
+               
+               160     >>  250 RERAISE                  0
+                       >>  252 COPY                     3
+                           254 POP_EXCEPT
+                           256 RERAISE                  1
+               
+               163     >>  258 LOAD_GLOBAL              2 (api_settings)
+                           270 LOAD_ATTR                3 (SESSION_LOGIN)
+                           280 POP_JUMP_FORWARD_IF_FALSE    15 (to 312)
+               
+               164         282 LOAD_GLOBAL             27 (NULL + django_logout)
+                           294 LOAD_FAST                1 (request)
+                           296 PRECALL                  1
+                           300 CALL                     1
+                           310 POP_TOP
                
-               156         100 POP_EXCEPT
-                           102 JUMP_FORWARD             4 (to 112)
+               166     >>  312 LOAD_GLOBAL              9 (NULL + Response)
                
-               155     >>  104 RERAISE                  0
-                       >>  106 COPY                     3
-                           108 POP_EXCEPT
-                           110 RERAISE                  1
-               
-               158     >>  112 LOAD_GLOBAL             10 (api_settings)
-                           124 LOAD_ATTR                6 (SESSION_LOGIN)
-                           134 POP_JUMP_FORWARD_IF_FALSE    15 (to 166)
-               
-               159         136 LOAD_GLOBAL             15 (NULL + django_logout)
-                           148 LOAD_FAST                1 (request)
-                           150 PRECALL                  1
-                           154 CALL                     1
-                           164 POP_TOP
-               
-               161     >>  166 LOAD_GLOBAL             17 (NULL + Response)
-               
-               162         178 LOAD_CONST               1 ('detail')
-                           180 LOAD_GLOBAL             19 (NULL + _)
-                           192 LOAD_CONST               2 ('Successfully logged out.')
-                           194 PRECALL                  1
-                           198 CALL                     1
-                           208 BUILD_MAP                1
-               
-               163         210 LOAD_GLOBAL             20 (status)
-                           222 LOAD_ATTR               11 (HTTP_200_OK)
-               
-               161         232 KW_NAMES                 3
-                           234 PRECALL                  2
-                           238 CALL                     2
-                           248 STORE_FAST               2 (response)
-               
-               166         250 LOAD_GLOBAL             10 (api_settings)
-                           262 LOAD_ATTR               12 (USE_JWT)
-                           272 EXTENDED_ARG             1
-                           274 POP_JUMP_FORWARD_IF_FALSE   389 (to 1054)
-               
-               170         276 LOAD_CONST               4 (0)
-                           278 LOAD_CONST               5 (('TokenError',))
-                           280 IMPORT_NAME             13 (rest_framework_simplejwt.exceptions)
-                           282 IMPORT_FROM             14 (TokenError)
-                           284 STORE_FAST               3 (TokenError)
-                           286 POP_TOP
-               
-               171         288 LOAD_CONST               4 (0)
-                           290 LOAD_CONST               6 (('RefreshToken',))
-                           292 IMPORT_NAME             15 (rest_framework_simplejwt.tokens)
-                           294 IMPORT_FROM             16 (RefreshToken)
-                           296 STORE_FAST               4 (RefreshToken)
-                           298 POP_TOP
-               
-               173         300 LOAD_CONST               7 (1)
-                           302 LOAD_CONST               8 (('unset_jwt_cookies',))
-                           304 IMPORT_NAME             17 (jwt_auth)
-                           306 IMPORT_FROM             18 (unset_jwt_cookies)
-                           308 STORE_FAST               5 (unset_jwt_cookies)
-                           310 POP_TOP
+               167         324 LOAD_CONST               1 ('detail')
+                           326 LOAD_GLOBAL             11 (NULL + _)
+                           338 LOAD_CONST               4 ('Successfully logged out.')
+                           340 PRECALL                  1
+                           344 CALL                     1
+                           354 BUILD_MAP                1
+               
+               168         356 LOAD_GLOBAL             12 (status)
+                           368 LOAD_ATTR               14 (HTTP_200_OK)
+               
+               166         378 KW_NAMES                 3
+                           380 PRECALL                  2
+                           384 CALL                     2
+                           394 STORE_FAST               2 (response)
+               
+               171         396 LOAD_GLOBAL              2 (api_settings)
+                           408 LOAD_ATTR                2 (USE_JWT)
+                           418 EXTENDED_ARG             1
+                           420 POP_JUMP_FORWARD_IF_FALSE   507 (to 1436)
+               
+               175         422 LOAD_CONST               5 (0)
+                           424 LOAD_CONST               6 (('TokenError',))
+                           426 IMPORT_NAME             15 (rest_framework_simplejwt.exceptions)
+                           428 IMPORT_FROM             16 (TokenError)
+                           430 STORE_FAST               3 (TokenError)
+                           432 POP_TOP
+               
+               176         434 LOAD_CONST               5 (0)
+                           436 LOAD_CONST               7 (('RefreshToken',))
+                           438 IMPORT_NAME             17 (rest_framework_simplejwt.tokens)
+                           440 IMPORT_FROM             18 (RefreshToken)
+                           442 STORE_FAST               4 (RefreshToken)
+                           444 POP_TOP
+               
+               178         446 LOAD_CONST               8 (1)
+                           448 LOAD_CONST               9 (('unset_jwt_cookies',))
+                           450 IMPORT_NAME             19 (jwt_auth)
+                           452 IMPORT_FROM             20 (unset_jwt_cookies)
+                           454 STORE_FAST               5 (unset_jwt_cookies)
+                           456 POP_TOP
+               
+               179         458 LOAD_GLOBAL              2 (api_settings)
+                           470 LOAD_ATTR               21 (JWT_AUTH_COOKIE)
+                           480 STORE_FAST               6 (cookie_name)
+               
+               181         482 PUSH_NULL
+                           484 LOAD_FAST                5 (unset_jwt_cookies)
+                           486 LOAD_FAST                2 (response)
+                           488 PRECALL                  1
+                           492 CALL                     1
+                           502 POP_TOP
+               
+               183         504 LOAD_CONST              10 ('rest_framework_simplejwt.token_blacklist')
+                           506 LOAD_GLOBAL             44 (settings)
+                           518 LOAD_ATTR               23 (INSTALLED_APPS)
+                           528 CONTAINS_OP              0
+                           530 EXTENDED_ARG             1
+                           532 POP_JUMP_FORWARD_IF_FALSE   408 (to 1350)
+               
+               185         534 NOP
+               
+               186         536 PUSH_NULL
+                           538 LOAD_FAST                4 (RefreshToken)
+                           540 LOAD_CONST               0 (None)
+                           542 PRECALL                  1
+                           546 CALL                     1
+                           556 STORE_FAST               7 (token)
+               
+               187         558 LOAD_GLOBAL              2 (api_settings)
+                           570 LOAD_ATTR               24 (JWT_AUTH_HTTPONLY)
+                           580 POP_JUMP_FORWARD_IF_FALSE    89 (to 760)
+               
+               188         582 NOP
+               
+               189         584 PUSH_NULL
+                           586 LOAD_FAST                4 (RefreshToken)
+                           588 LOAD_FAST                1 (request)
+                           590 LOAD_ATTR               25 (COOKIES)
+                           600 LOAD_GLOBAL              2 (api_settings)
+                           612 LOAD_ATTR               26 (JWT_AUTH_REFRESH_COOKIE)
+                           622 BINARY_SUBSCR
+                           632 PRECALL                  1
+                           636 CALL                     1
+                           646 STORE_FAST               7 (token)
+                           648 JUMP_FORWARD           134 (to 918)
+                       >>  650 PUSH_EXC_INFO
+               
+               190         652 LOAD_GLOBAL             54 (KeyError)
+                           664 CHECK_EXC_MATCH
+                           666 POP_JUMP_FORWARD_IF_FALSE    42 (to 752)
+                           668 POP_TOP
+               
+               191         670 LOAD_CONST               1 ('detail')
+                           672 LOAD_GLOBAL             11 (NULL + _)
+                           684 LOAD_CONST              11 ('Refresh token was not included in cookie data.')
+                           686 PRECALL                  1
+                           690 CALL                     1
+                           700 BUILD_MAP                1
+                           702 LOAD_FAST                2 (response)
+                           704 STORE_ATTR              28 (data)
                
-               174         312 LOAD_GLOBAL             10 (api_settings)
-                           324 LOAD_ATTR               19 (JWT_AUTH_COOKIE)
-                           334 STORE_FAST               6 (cookie_name)
-               
-               176         336 PUSH_NULL
-                           338 LOAD_FAST                5 (unset_jwt_cookies)
-                           340 LOAD_FAST                2 (response)
-                           342 PRECALL                  1
-                           346 CALL                     1
-                           356 POP_TOP
-               
-               178         358 LOAD_CONST               9 ('rest_framework_simplejwt.token_blacklist')
-                           360 LOAD_GLOBAL             40 (settings)
-                           372 LOAD_ATTR               21 (INSTALLED_APPS)
-                           382 CONTAINS_OP              0
-                           384 EXTENDED_ARG             1
-                           386 POP_JUMP_FORWARD_IF_FALSE   290 (to 968)
-               
-               180         388 NOP
-               
-               181         390 PUSH_NULL
-                           392 LOAD_FAST                4 (RefreshToken)
-                           394 LOAD_FAST                1 (request)
-                           396 LOAD_ATTR               22 (data)
-                           406 LOAD_CONST              10 ('refresh')
-                           408 BINARY_SUBSCR
-                           418 PRECALL                  1
-                           422 CALL                     1
-                           432 STORE_FAST               7 (token)
-               
-               182         434 LOAD_FAST                7 (token)
-                           436 LOAD_METHOD             23 (blacklist)
-                           458 PRECALL                  0
-                           462 CALL                     0
-                           472 POP_TOP
-                           474 EXTENDED_ARG             1
-                           476 JUMP_FORWARD           288 (to 1054)
-                       >>  478 PUSH_EXC_INFO
-               
-               183         480 LOAD_GLOBAL             48 (KeyError)
-                           492 CHECK_EXC_MATCH
-                           494 POP_JUMP_FORWARD_IF_FALSE    42 (to 580)
-                           496 POP_TOP
-               
-               184         498 LOAD_CONST               1 ('detail')
-                           500 LOAD_GLOBAL             19 (NULL + _)
-                           512 LOAD_CONST              11 ('Refresh token was not included in request data.')
-                           514 PRECALL                  1
-                           518 CALL                     1
-                           528 BUILD_MAP                1
-                           530 LOAD_FAST                2 (response)
-                           532 STORE_ATTR              22 (data)
-               
-               185         542 LOAD_GLOBAL             20 (status)
-                           554 LOAD_ATTR               25 (HTTP_401_UNAUTHORIZED)
-                           564 LOAD_FAST                2 (response)
-                           566 STORE_ATTR              26 (status_code)
-                           576 POP_EXCEPT
-                           578 JUMP_FORWARD           237 (to 1054)
-               
-               186     >>  580 LOAD_FAST                3 (TokenError)
-                           582 LOAD_GLOBAL              6 (AttributeError)
-                           594 LOAD_GLOBAL             54 (TypeError)
-                           606 BUILD_TUPLE              3
-                           608 CHECK_EXC_MATCH
-                           610 POP_JUMP_FORWARD_IF_FALSE   174 (to 960)
-                           612 STORE_FAST               8 (error)
-               
-               187         614 LOAD_GLOBAL             57 (NULL + hasattr)
-                           626 LOAD_FAST                8 (error)
-                           628 LOAD_CONST              12 ('args')
-                           630 PRECALL                  2
-                           634 CALL                     2
-                           644 POP_JUMP_FORWARD_IF_FALSE   109 (to 864)
-               
-               188         646 LOAD_CONST              13 ('Token is blacklisted')
-                           648 LOAD_FAST                8 (error)
-                           650 LOAD_ATTR               29 (args)
-                           660 CONTAINS_OP              0
-                           662 POP_JUMP_FORWARD_IF_TRUE     9 (to 682)
-                           664 LOAD_CONST              14 ('Token is invalid or expired')
-                           666 LOAD_FAST                8 (error)
-                           668 LOAD_ATTR               29 (args)
-                           678 CONTAINS_OP              0
-                           680 POP_JUMP_FORWARD_IF_FALSE    51 (to 784)
-               
-               189     >>  682 LOAD_CONST               1 ('detail')
-                           684 LOAD_GLOBAL             19 (NULL + _)
-                           696 LOAD_FAST                8 (error)
-                           698 LOAD_ATTR               29 (args)
-                           708 LOAD_CONST               4 (0)
-                           710 BINARY_SUBSCR
-                           720 PRECALL                  1
-                           724 CALL                     1
-                           734 BUILD_MAP                1
+               192         714 LOAD_GLOBAL             12 (status)
+                           726 LOAD_ATTR               29 (HTTP_401_UNAUTHORIZED)
                            736 LOAD_FAST                2 (response)
-                           738 STORE_ATTR              22 (data)
-               
-               190         748 LOAD_GLOBAL             20 (status)
-                           760 LOAD_ATTR               25 (HTTP_401_UNAUTHORIZED)
-                           770 LOAD_FAST                2 (response)
-                           772 STORE_ATTR              26 (status_code)
-                           782 JUMP_FORWARD            79 (to 942)
-               
-               192     >>  784 LOAD_CONST               1 ('detail')
-                           786 LOAD_GLOBAL             19 (NULL + _)
-                           798 LOAD_CONST              15 ('An error has occurred.')
-                           800 PRECALL                  1
-                           804 CALL                     1
-                           814 BUILD_MAP                1
-                           816 LOAD_FAST                2 (response)
-                           818 STORE_ATTR              22 (data)
-               
-               193         828 LOAD_GLOBAL             20 (status)
-                           840 LOAD_ATTR               30 (HTTP_500_INTERNAL_SERVER_ERROR)
-                           850 LOAD_FAST                2 (response)
-                           852 STORE_ATTR              26 (status_code)
-                           862 JUMP_FORWARD            39 (to 942)
-               
-               196     >>  864 LOAD_CONST               1 ('detail')
-                           866 LOAD_GLOBAL             19 (NULL + _)
-                           878 LOAD_CONST              15 ('An error has occurred.')
-                           880 PRECALL                  1
-                           884 CALL                     1
-                           894 BUILD_MAP                1
-                           896 LOAD_FAST                2 (response)
-                           898 STORE_ATTR              22 (data)
-               
-               197         908 LOAD_GLOBAL             20 (status)
-                           920 LOAD_ATTR               30 (HTTP_500_INTERNAL_SERVER_ERROR)
-                           930 LOAD_FAST                2 (response)
-                           932 STORE_ATTR              26 (status_code)
-                       >>  942 POP_EXCEPT
-                           944 LOAD_CONST               0 (None)
-                           946 STORE_FAST               8 (error)
-                           948 DELETE_FAST              8 (error)
-                           950 JUMP_FORWARD            51 (to 1054)
-                       >>  952 LOAD_CONST               0 (None)
-                           954 STORE_FAST               8 (error)
-                           956 DELETE_FAST              8 (error)
-                           958 RERAISE                  1
-               
-               186     >>  960 RERAISE                  0
-                       >>  962 COPY                     3
-                           964 POP_EXCEPT
-                           966 RERAISE                  1
-               
-               199     >>  968 LOAD_FAST                6 (cookie_name)
-                           970 POP_JUMP_FORWARD_IF_TRUE    41 (to 1054)
-               
-               200         972 LOAD_GLOBAL             19 (NULL + _)
-               
-               201         984 LOAD_CONST              16 ('Neither cookies or blacklist are enabled, so the token has not been deleted server side. Please make sure the token is deleted client side.')
-               
-               200         986 PRECALL                  1
-                           990 CALL                     1
-                          1000 STORE_FAST               9 (message)
-               
-               204        1002 LOAD_CONST               1 ('detail')
-                          1004 LOAD_FAST                9 (message)
-                          1006 BUILD_MAP                1
-                          1008 LOAD_FAST                2 (response)
-                          1010 STORE_ATTR              22 (data)
-               
-               205        1020 LOAD_GLOBAL             20 (status)
-                          1032 LOAD_ATTR               11 (HTTP_200_OK)
-                          1042 LOAD_FAST                2 (response)
-                          1044 STORE_ATTR              26 (status_code)
+                           738 STORE_ATTR              30 (status_code)
+                           748 POP_EXCEPT
+                           750 JUMP_FORWARD            83 (to 918)
+               
+               190     >>  752 RERAISE                  0
+                       >>  754 COPY                     3
+                           756 POP_EXCEPT
+                           758 RERAISE                  1
+               
+               194     >>  760 NOP
+               
+               195         762 PUSH_NULL
+                           764 LOAD_FAST                4 (RefreshToken)
+                           766 LOAD_FAST                1 (request)
+                           768 LOAD_ATTR               28 (data)
+                           778 LOAD_CONST              12 ('refresh')
+                           780 BINARY_SUBSCR
+                           790 PRECALL                  1
+                           794 CALL                     1
+                           804 STORE_FAST               7 (token)
+                           806 JUMP_FORWARD            55 (to 918)
+                       >>  808 PUSH_EXC_INFO
+               
+               196         810 LOAD_GLOBAL             54 (KeyError)
+                           822 CHECK_EXC_MATCH
+                           824 POP_JUMP_FORWARD_IF_FALSE    42 (to 910)
+                           826 POP_TOP
+               
+               197         828 LOAD_CONST               1 ('detail')
+                           830 LOAD_GLOBAL             11 (NULL + _)
+                           842 LOAD_CONST              13 ('Refresh token was not included in request data.')
+                           844 PRECALL                  1
+                           848 CALL                     1
+                           858 BUILD_MAP                1
+                           860 LOAD_FAST                2 (response)
+                           862 STORE_ATTR              28 (data)
+               
+               198         872 LOAD_GLOBAL             12 (status)
+                           884 LOAD_ATTR               29 (HTTP_401_UNAUTHORIZED)
+                           894 LOAD_FAST                2 (response)
+                           896 STORE_ATTR              30 (status_code)
+                           906 POP_EXCEPT
+                           908 JUMP_FORWARD             4 (to 918)
+               
+               196     >>  910 RERAISE                  0
+                       >>  912 COPY                     3
+                           914 POP_EXCEPT
+                           916 RERAISE                  1
+               
+               200     >>  918 LOAD_FAST                7 (token)
+                           920 LOAD_METHOD             31 (blacklist)
+                           942 PRECALL                  0
+                           946 CALL                     0
+                           956 POP_TOP
+                           958 JUMP_FORWARD           238 (to 1436)
+                       >>  960 PUSH_EXC_INFO
+               
+               201         962 LOAD_FAST                3 (TokenError)
+                           964 LOAD_GLOBAL             22 (AttributeError)
+                           976 LOAD_GLOBAL             64 (TypeError)
+                           988 BUILD_TUPLE              3
+                           990 CHECK_EXC_MATCH
+                           992 POP_JUMP_FORWARD_IF_FALSE   174 (to 1342)
+                           994 STORE_FAST               8 (error)
+               
+               202         996 LOAD_GLOBAL             67 (NULL + hasattr)
+                          1008 LOAD_FAST                8 (error)
+                          1010 LOAD_CONST              14 ('args')
+                          1012 PRECALL                  2
+                          1016 CALL                     2
+                          1026 POP_JUMP_FORWARD_IF_FALSE   109 (to 1246)
+               
+               203        1028 LOAD_CONST              15 ('Token is blacklisted')
+                          1030 LOAD_FAST                8 (error)
+                          1032 LOAD_ATTR               34 (args)
+                          1042 CONTAINS_OP              0
+                          1044 POP_JUMP_FORWARD_IF_TRUE     9 (to 1064)
+                          1046 LOAD_CONST              16 ('Token is invalid or expired')
+                          1048 LOAD_FAST                8 (error)
+                          1050 LOAD_ATTR               34 (args)
+                          1060 CONTAINS_OP              0
+                          1062 POP_JUMP_FORWARD_IF_FALSE    51 (to 1166)
+               
+               204     >> 1064 LOAD_CONST               1 ('detail')
+                          1066 LOAD_GLOBAL             11 (NULL + _)
+                          1078 LOAD_FAST                8 (error)
+                          1080 LOAD_ATTR               34 (args)
+                          1090 LOAD_CONST               5 (0)
+                          1092 BINARY_SUBSCR
+                          1102 PRECALL                  1
+                          1106 CALL                     1
+                          1116 BUILD_MAP                1
+                          1118 LOAD_FAST                2 (response)
+                          1120 STORE_ATTR              28 (data)
+               
+               205        1130 LOAD_GLOBAL             12 (status)
+                          1142 LOAD_ATTR               29 (HTTP_401_UNAUTHORIZED)
+                          1152 LOAD_FAST                2 (response)
+                          1154 STORE_ATTR              30 (status_code)
+                          1164 JUMP_FORWARD            79 (to 1324)
+               
+               207     >> 1166 LOAD_CONST               1 ('detail')
+                          1168 LOAD_GLOBAL             11 (NULL + _)
+                          1180 LOAD_CONST              17 ('An error has occurred.')
+                          1182 PRECALL                  1
+                          1186 CALL                     1
+                          1196 BUILD_MAP                1
+                          1198 LOAD_FAST                2 (response)
+                          1200 STORE_ATTR              28 (data)
+               
+               208        1210 LOAD_GLOBAL             12 (status)
+                          1222 LOAD_ATTR               35 (HTTP_500_INTERNAL_SERVER_ERROR)
+                          1232 LOAD_FAST                2 (response)
+                          1234 STORE_ATTR              30 (status_code)
+                          1244 JUMP_FORWARD            39 (to 1324)
+               
+               211     >> 1246 LOAD_CONST               1 ('detail')
+                          1248 LOAD_GLOBAL             11 (NULL + _)
+                          1260 LOAD_CONST              17 ('An error has occurred.')
+                          1262 PRECALL                  1
+                          1266 CALL                     1
+                          1276 BUILD_MAP                1
+                          1278 LOAD_FAST                2 (response)
+                          1280 STORE_ATTR              28 (data)
+               
+               212        1290 LOAD_GLOBAL             12 (status)
+                          1302 LOAD_ATTR               35 (HTTP_500_INTERNAL_SERVER_ERROR)
+                          1312 LOAD_FAST                2 (response)
+                          1314 STORE_ATTR              30 (status_code)
+                       >> 1324 POP_EXCEPT
+                          1326 LOAD_CONST               0 (None)
+                          1328 STORE_FAST               8 (error)
+                          1330 DELETE_FAST              8 (error)
+                          1332 JUMP_FORWARD            51 (to 1436)
+                       >> 1334 LOAD_CONST               0 (None)
+                          1336 STORE_FAST               8 (error)
+                          1338 DELETE_FAST              8 (error)
+                          1340 RERAISE                  1
+               
+               201     >> 1342 RERAISE                  0
+                       >> 1344 COPY                     3
+                          1346 POP_EXCEPT
+                          1348 RERAISE                  1
+               
+               214     >> 1350 LOAD_FAST                6 (cookie_name)
+                          1352 POP_JUMP_FORWARD_IF_TRUE    41 (to 1436)
+               
+               215        1354 LOAD_GLOBAL             11 (NULL + _)
+               
+               216        1366 LOAD_CONST              18 ('Neither cookies or blacklist are enabled, so the token has not been deleted server side. Please make sure the token is deleted client side.')
+               
+               215        1368 PRECALL                  1
+                          1372 CALL                     1
+                          1382 STORE_FAST               9 (message)
+               
+               219        1384 LOAD_CONST               1 ('detail')
+                          1386 LOAD_FAST                9 (message)
+                          1388 BUILD_MAP                1
+                          1390 LOAD_FAST                2 (response)
+                          1392 STORE_ATTR              28 (data)
+               
+               220        1402 LOAD_GLOBAL             12 (status)
+                          1414 LOAD_ATTR               14 (HTTP_200_OK)
+                          1424 LOAD_FAST                2 (response)
+                          1426 STORE_ATTR              30 (status_code)
                
-               206     >> 1054 LOAD_FAST                2 (response)
-                          1056 RETURN_VALUE
+               221     >> 1436 LOAD_FAST                2 (response)
+                          1438 RETURN_VALUE
                ExceptionTable:
-                 4 to 62 -> 66 [0]
-                 66 to 98 -> 106 [1] lasti
-                 104 to 104 -> 106 [1] lasti
-                 390 to 472 -> 478 [0]
-                 478 to 574 -> 962 [1] lasti
-                 580 to 612 -> 962 [1] lasti
-                 614 to 940 -> 952 [1] lasti
-                 952 to 960 -> 962 [1] lasti
+                 150 to 208 -> 212 [0]
+                 212 to 244 -> 252 [1] lasti
+                 250 to 250 -> 252 [1] lasti
+                 536 to 580 -> 960 [0]
+                 584 to 646 -> 650 [0]
+                 648 to 648 -> 960 [0]
+                 650 to 746 -> 754 [1] lasti
+                 748 to 750 -> 960 [0]
+                 752 to 752 -> 754 [1] lasti
+                 754 to 758 -> 960 [0]
+                 762 to 804 -> 808 [0]
+                 806 to 806 -> 960 [0]
+                 808 to 904 -> 912 [1] lasti
+                 906 to 908 -> 960 [0]
+                 910 to 910 -> 912 [1] lasti
+                 912 to 956 -> 960 [0]
+                 960 to 994 -> 1344 [1] lasti
+                 996 to 1322 -> 1334 [1] lasti
+                 1334 to 1342 -> 1344 [1] lasti
                consts
                   None
                   'detail'
-                  'Successfully logged out.'
+                  'You should be logged in to logout. Check whether the token is passed.'
                   ('status',)
+                  'Successfully logged out.'
                   0
                   ('TokenError',)
                   ('RefreshToken',)
                   1
                   ('unset_jwt_cookies',)
                   'rest_framework_simplejwt.token_blacklist'
+                  'Refresh token was not included in cookie data.'
                   'refresh'
                   'Refresh token was not included in request data.'
                   'args'
                   'Token is blacklisted'
                   'Token is invalid or expired'
                   'An error has occurred.'
                   'Neither cookies or blacklist are enabled, so the token has not been deleted server side. Please make sure the token is deleted client side.'
-               names      ('user', 'auth_token', 'delete', 'AttributeError', 'ObjectDoesNotExist', 'api_settings', 'SESSION_LOGIN', 'django_logout', 'Response', '_', 'status', 'HTTP_200_OK', 'USE_JWT', 'rest_framework_simplejwt.exceptions', 'TokenError', 'rest_framework_simplejwt.tokens', 'RefreshToken', 'jwt_auth', 'unset_jwt_cookies', 'JWT_AUTH_COOKIE', 'settings', 'INSTALLED_APPS', 'data', 'blacklist', 'KeyError', 'HTTP_401_UNAUTHORIZED', 'status_code', 'TypeError', 'hasattr', 'args', 'HTTP_500_INTERNAL_SERVER_ERROR')
+               names      ('auth', 'api_settings', 'USE_JWT', 'SESSION_LOGIN', 'Response', '_', 'status', 'HTTP_400_BAD_REQUEST', 'user', 'auth_token', 'delete', 'AttributeError', 'ObjectDoesNotExist', 'django_logout', 'HTTP_200_OK', 'rest_framework_simplejwt.exceptions', 'TokenError', 'rest_framework_simplejwt.tokens', 'RefreshToken', 'jwt_auth', 'unset_jwt_cookies', 'JWT_AUTH_COOKIE', 'settings', 'INSTALLED_APPS', 'JWT_AUTH_HTTPONLY', 'COOKIES', 'JWT_AUTH_REFRESH_COOKIE', 'KeyError', 'data', 'HTTP_401_UNAUTHORIZED', 'status_code', 'blacklist', 'TypeError', 'hasattr', 'args', 'HTTP_500_INTERNAL_SERVER_ERROR')
                varnames   ('self', 'request', 'response', 'TokenError', 'RefreshToken', 'unset_jwt_cookies', 'cookie_name', 'token', 'error', 'message')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'logout'
                firstlineno 152
                lnotab
-                  0x020102014001200104ff080318011e020c01200116fe12051a040c010c
-                  020c01180216021e0202012c012e0112012c012601220120012401420124
+                  0x02013e010c01200116fe120402014001200104ff080318011e020c0120
+                  0116fe12051a040c010c020c01180216021e020201160118010201440112
+                  012c0126fe08040201300112012c0126fe08042c01220120012401420124
                   022c0124032c0134f5080d04010c0102ff100412012201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'AllowAny', 'permission_classes', 'throttle_scope', 'get', 'post', 'logout')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
@@ -1303,77 +1417,77 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0365046a0500000000000000005a0665
             0766015a08640284005a09640384005a0a64045300
-         209           0 RESUME                   0
+         224           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserDetailsView')
                        8 STORE_NAME               2 (__qualname__)
          
-         210          10 LOAD_CONST               1 ('\n    Reads and updates UserModel fields\n    Accepts GET, PUT, PATCH methods.\n\n    Default accepted fields: username, first_name, last_name\n    Default display fields: pk, username, email, first_name, last_name\n    Read-only fields: pk, email\n\n    Returns UserModel fields.\n    ')
+         225          10 LOAD_CONST               1 ('\n    Reads and updates UserModel fields\n    Accepts GET, PUT, PATCH methods.\n\n    Default accepted fields: username, first_name, last_name\n    Default display fields: pk, username, email, first_name, last_name\n    Read-only fields: pk, email\n\n    Returns UserModel fields.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         220          14 LOAD_NAME                4 (api_settings)
+         235          14 LOAD_NAME                4 (api_settings)
                       16 LOAD_ATTR                5 (USER_DETAILS_SERIALIZER)
                       26 STORE_NAME               6 (serializer_class)
          
-         221          28 LOAD_NAME                7 (IsAuthenticated)
+         236          28 LOAD_NAME                7 (IsAuthenticated)
                       30 BUILD_TUPLE              1
                       32 STORE_NAME               8 (permission_classes)
          
-         223          34 LOAD_CONST               2 (<code object get_object, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 223>)
+         238          34 LOAD_CONST               2 (<code object get_object, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 238>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               9 (get_object)
          
-         226          40 LOAD_CONST               3 (<code object get_queryset, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 226>)
+         241          40 LOAD_CONST               3 (<code object get_queryset, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 241>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME              10 (get_queryset)
                       46 LOAD_CONST               4 (None)
                       48 RETURN_VALUE
          consts
             'UserDetailsView'
             '\n    Reads and updates UserModel fields\n    Accepts GET, PUT, PATCH methods.\n\n    Default accepted fields: username, first_name, last_name\n    Default display fields: pk, username, email, first_name, last_name\n    Read-only fields: pk, email\n\n    Returns UserModel fields.\n    '
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-               223           0 RESUME                   0
+               238           0 RESUME                   0
                
-               224           2 LOAD_FAST                0 (self)
+               239           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (request)
                             14 LOAD_ATTR                1 (user)
                             24 RETURN_VALUE
                consts
                   None
                names      ('request', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'get_object'
-               firstlineno 223
+               firstlineno 238
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000006a
                   010000000000000000a00200000000000000000000000000000000000000
                   00a6000000ab0000000000000000005300
-               226           0 RESUME                   0
+               241           0 RESUME                   0
                
-               231           2 LOAD_GLOBAL              1 (NULL + get_user_model)
+               246           2 LOAD_GLOBAL              1 (NULL + get_user_model)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_ATTR                1 (objects)
                             38 LOAD_METHOD              2 (none)
                             60 PRECALL                  0
                             64 CALL                     0
                             74 RETURN_VALUE
@@ -1381,55 +1495,55 @@
                   '\n        Adding this method since it is sometimes called when using\n        django-rest-swagger\n        '
                names      ('get_user_model', 'objects', 'none')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'get_queryset'
-               firstlineno 226
+               firstlineno 241
                lnotab 0x0205
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'api_settings', 'USER_DETAILS_SERIALIZER', 'serializer_class', 'IsAuthenticated', 'permission_classes', 'get_object', 'get_queryset')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
          name       'UserDetailsView'
-         firstlineno 209
+         firstlineno 224
          lnotab 0x0a01040a0e0106020603
       'UserDetailsView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0365046a0500000000000000005a0665
             0766015a0864025a09640384005a0a64045300
-         234           0 RESUME                   0
+         249           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PasswordResetView')
                        8 STORE_NAME               2 (__qualname__)
          
-         235          10 LOAD_CONST               1 ('\n    Calls Django Auth PasswordResetForm save method.\n\n    Accepts the following POST parameters: email\n    Returns the success/fail message.\n    ')
+         250          10 LOAD_CONST               1 ('\n    Calls Django Auth PasswordResetForm save method.\n\n    Accepts the following POST parameters: email\n    Returns the success/fail message.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         241          14 LOAD_NAME                4 (api_settings)
+         256          14 LOAD_NAME                4 (api_settings)
                       16 LOAD_ATTR                5 (PASSWORD_RESET_SERIALIZER)
                       26 STORE_NAME               6 (serializer_class)
          
-         242          28 LOAD_NAME                7 (AllowAny)
+         257          28 LOAD_NAME                7 (AllowAny)
                       30 BUILD_TUPLE              1
                       32 STORE_NAME               8 (permission_classes)
          
-         243          34 LOAD_CONST               2 ('dj_rest_auth')
+         258          34 LOAD_CONST               2 ('dj_rest_auth')
                       36 STORE_NAME               9 (throttle_scope)
          
-         245          38 LOAD_CONST               3 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 245>)
+         260          38 LOAD_CONST               3 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 260>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME              10 (post)
                       44 LOAD_CONST               4 (None)
                       46 RETURN_VALUE
          consts
             'PasswordResetView'
             '\n    Calls Django Auth PasswordResetForm save method.\n\n    Accepts the following POST parameters: email\n    Returns the success/fail message.\n    '
@@ -1444,52 +1558,52 @@
                   010000000000000000ac01a6010000ab0100000000000000007d047c04a0
                   0200000000000000000000000000000000000000006402ac03a6010000ab
                   01000000000000000001007c04a003000000000000000000000000000000
                   0000000000a6000000ab0000000000000000000100740900000000000000
                   0000006404740b000000000000000000006405a6010000ab010000000000
                   0000006901740c000000000000000000006a070000000000000000ac06a6
                   020000ab0200000000000000005300
-               245           0 RESUME                   0
+               260           0 RESUME                   0
                
-               247           2 LOAD_FAST                0 (self)
+               262           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_serializer)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_ATTR                1 (data)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               4 (serializer)
                
-               248          56 LOAD_FAST                4 (serializer)
+               263          56 LOAD_FAST                4 (serializer)
                             58 LOAD_METHOD              2 (is_valid)
                             80 LOAD_CONST               2 (True)
                             82 KW_NAMES                 3
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_TOP
                
-               250         100 LOAD_FAST                4 (serializer)
+               265         100 LOAD_FAST                4 (serializer)
                            102 LOAD_METHOD              3 (save)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 POP_TOP
                
-               252         140 LOAD_GLOBAL              9 (NULL + Response)
+               267         140 LOAD_GLOBAL              9 (NULL + Response)
                
-               253         152 LOAD_CONST               4 ('detail')
+               268         152 LOAD_CONST               4 ('detail')
                            154 LOAD_GLOBAL             11 (NULL + _)
                            166 LOAD_CONST               5 ('Password reset e-mail has been sent.')
                            168 PRECALL                  1
                            172 CALL                     1
                            182 BUILD_MAP                1
                
-               254         184 LOAD_GLOBAL             12 (status)
+               269         184 LOAD_GLOBAL             12 (status)
                            196 LOAD_ATTR                7 (HTTP_200_OK)
                
-               252         206 KW_NAMES                 6
+               267         206 KW_NAMES                 6
                            208 PRECALL                  2
                            212 CALL                     2
                            222 RETURN_VALUE
                consts
                   None
                   ('data',)
                   True
@@ -1499,70 +1613,70 @@
                   ('status',)
                names      ('get_serializer', 'data', 'is_valid', 'save', 'Response', '_', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'args', 'kwargs', 'serializer')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'post'
-               firstlineno 245
+               firstlineno 260
                lnotab 0x020236012c0228020c01200116fe
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'api_settings', 'PASSWORD_RESET_SERIALIZER', 'serializer_class', 'AllowAny', 'permission_classes', 'throttle_scope', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
          name       'PasswordResetView'
-         firstlineno 234
+         firstlineno 249
          lnotab 0x0a0104060e0106010402
       'PasswordResetView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0365046a0500000000000000005a
             06650766015a0864025a09650a8800660164038408a6000000ab00000000
             00000000005a0b640484005a0c880078015a0d5300
                        0 MAKE_CELL                0 (__class__)
          
-         258           2 RESUME                   0
+         273           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('PasswordResetConfirmView')
                       10 STORE_NAME               2 (__qualname__)
          
-         259          12 LOAD_CONST               1 ("\n    Password reset e-mail link is confirmed, therefore\n    this resets the user's password.\n\n    Accepts the following POST parameters: token, uid,\n        new_password1, new_password2\n    Returns the success/fail message.\n    ")
+         274          12 LOAD_CONST               1 ("\n    Password reset e-mail link is confirmed, therefore\n    this resets the user's password.\n\n    Accepts the following POST parameters: token, uid,\n        new_password1, new_password2\n    Returns the success/fail message.\n    ")
                       14 STORE_NAME               3 (__doc__)
          
-         267          16 LOAD_NAME                4 (api_settings)
+         282          16 LOAD_NAME                4 (api_settings)
                       18 LOAD_ATTR                5 (PASSWORD_RESET_CONFIRM_SERIALIZER)
                       28 STORE_NAME               6 (serializer_class)
          
-         268          30 LOAD_NAME                7 (AllowAny)
+         283          30 LOAD_NAME                7 (AllowAny)
                       32 BUILD_TUPLE              1
                       34 STORE_NAME               8 (permission_classes)
          
-         269          36 LOAD_CONST               2 ('dj_rest_auth')
+         284          36 LOAD_CONST               2 ('dj_rest_auth')
                       38 STORE_NAME               9 (throttle_scope)
          
-         271          40 LOAD_NAME               10 (sensitive_post_parameters_m)
+         286          40 LOAD_NAME               10 (sensitive_post_parameters_m)
          
-         272          42 LOAD_CLOSURE             0 (__class__)
+         287          42 LOAD_CLOSURE             0 (__class__)
                       44 BUILD_TUPLE              1
-                      46 LOAD_CONST               3 (<code object dispatch, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 271>)
+                      46 LOAD_CONST               3 (<code object dispatch, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 286>)
                       48 MAKE_FUNCTION            8 (closure)
          
-         271          50 PRECALL                  0
+         286          50 PRECALL                  0
                       54 CALL                     0
          
-         272          64 STORE_NAME              11 (dispatch)
+         287          64 STORE_NAME              11 (dispatch)
          
-         275          66 LOAD_CONST               4 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 275>)
+         290          66 LOAD_CONST               4 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 290>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              12 (post)
                       72 LOAD_CLOSURE             0 (__class__)
                       74 COPY                     1
                       76 STORE_NAME              13 (__classcell__)
                       78 RETURN_VALUE
          consts
@@ -1575,17 +1689,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e015300
                              0 COPY_FREE_VARS           1
                
-               271           2 RESUME                   0
+               286           2 RESUME                   0
                
-               273           4 PUSH_NULL
+               288           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (dispatch)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1596,64 +1710,64 @@
                   None
                names      ('super', 'dispatch')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'dispatch'
-               firstlineno 271
+               firstlineno 286
                lnotab 0x0402
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 6
                flags     : 15
                code
                   0x97007c00a00000000000000000000000000000000000000000007c016a
                   010000000000000000ac01a6010000ab0100000000000000007d047c04a0
                   0200000000000000000000000000000000000000006402ac03a6010000ab
                   01000000000000000001007c04a003000000000000000000000000000000
                   0000000000a6000000ab0000000000000000000100740900000000000000
                   0000006404740b000000000000000000006405a6010000ab010000000000
                   0000006901a6010000ab0100000000000000005300
-               275           0 RESUME                   0
+               290           0 RESUME                   0
                
-               276           2 LOAD_FAST                0 (self)
+               291           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_serializer)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_ATTR                1 (data)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               4 (serializer)
                
-               277          56 LOAD_FAST                4 (serializer)
+               292          56 LOAD_FAST                4 (serializer)
                             58 LOAD_METHOD              2 (is_valid)
                             80 LOAD_CONST               2 (True)
                             82 KW_NAMES                 3
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_TOP
                
-               278         100 LOAD_FAST                4 (serializer)
+               293         100 LOAD_FAST                4 (serializer)
                            102 LOAD_METHOD              3 (save)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 POP_TOP
                
-               279         140 LOAD_GLOBAL              9 (NULL + Response)
+               294         140 LOAD_GLOBAL              9 (NULL + Response)
                
-               280         152 LOAD_CONST               4 ('detail')
+               295         152 LOAD_CONST               4 ('detail')
                            154 LOAD_GLOBAL             11 (NULL + _)
                            166 LOAD_CONST               5 ('Password has been reset with the new password.')
                            168 PRECALL                  1
                            172 CALL                     1
                            182 BUILD_MAP                1
                
-               279         184 PRECALL                  1
+               294         184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                consts
                   None
                   ('data',)
                   True
                   ('raise_exception',)
@@ -1661,69 +1775,69 @@
                   'Password has been reset with the new password.'
                names      ('get_serializer', 'data', 'is_valid', 'save', 'Response', '_')
                varnames   ('self', 'request', 'args', 'kwargs', 'serializer')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'post'
-               firstlineno 275
+               firstlineno 290
                lnotab 0x020136012c0128010c0120ff
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'api_settings', 'PASSWORD_RESET_CONFIRM_SERIALIZER', 'serializer_class', 'AllowAny', 'permission_classes', 'throttle_scope', 'sensitive_post_parameters_m', 'dispatch', 'post', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
          name       'PasswordResetConfirmView'
-         firstlineno 258
+         firstlineno 273
          lnotab 0x0c0104080e0106010402020108ff0e010203
       'PasswordResetConfirmView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0365046a0500000000000000005a
             06650766015a0864025a09650a8800660164038408a6000000ab00000000
             00000000005a0b640484005a0c880078015a0d5300
                        0 MAKE_CELL                0 (__class__)
          
-         284           2 RESUME                   0
+         299           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('PasswordChangeView')
                       10 STORE_NAME               2 (__qualname__)
          
-         285          12 LOAD_CONST               1 ('\n    Calls Django Auth SetPasswordForm save method.\n\n    Accepts the following POST parameters: new_password1, new_password2\n    Returns the success/fail message.\n    ')
+         300          12 LOAD_CONST               1 ('\n    Calls Django Auth SetPasswordForm save method.\n\n    Accepts the following POST parameters: new_password1, new_password2\n    Returns the success/fail message.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         291          16 LOAD_NAME                4 (api_settings)
+         306          16 LOAD_NAME                4 (api_settings)
                       18 LOAD_ATTR                5 (PASSWORD_CHANGE_SERIALIZER)
                       28 STORE_NAME               6 (serializer_class)
          
-         292          30 LOAD_NAME                7 (IsAuthenticated)
+         307          30 LOAD_NAME                7 (IsAuthenticated)
                       32 BUILD_TUPLE              1
                       34 STORE_NAME               8 (permission_classes)
          
-         293          36 LOAD_CONST               2 ('dj_rest_auth')
+         308          36 LOAD_CONST               2 ('dj_rest_auth')
                       38 STORE_NAME               9 (throttle_scope)
          
-         295          40 LOAD_NAME               10 (sensitive_post_parameters_m)
+         310          40 LOAD_NAME               10 (sensitive_post_parameters_m)
          
-         296          42 LOAD_CLOSURE             0 (__class__)
+         311          42 LOAD_CLOSURE             0 (__class__)
                       44 BUILD_TUPLE              1
-                      46 LOAD_CONST               3 (<code object dispatch, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 295>)
+                      46 LOAD_CONST               3 (<code object dispatch, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 310>)
                       48 MAKE_FUNCTION            8 (closure)
          
-         295          50 PRECALL                  0
+         310          50 PRECALL                  0
                       54 CALL                     0
          
-         296          64 STORE_NAME              11 (dispatch)
+         311          64 STORE_NAME              11 (dispatch)
          
-         299          66 LOAD_CONST               4 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 299>)
+         314          66 LOAD_CONST               4 (<code object post, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py", line 314>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              12 (post)
                       72 LOAD_CLOSURE             0 (__class__)
                       74 COPY                     1
                       76 STORE_NAME              13 (__classcell__)
                       78 RETURN_VALUE
          consts
@@ -1736,17 +1850,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e015300
                              0 COPY_FREE_VARS           1
                
-               295           2 RESUME                   0
+               310           2 RESUME                   0
                
-               297           4 PUSH_NULL
+               312           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (dispatch)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1757,55 +1871,55 @@
                   None
                names      ('super', 'dispatch')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'dispatch'
-               firstlineno 295
+               firstlineno 310
                lnotab 0x0402
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 6
                flags     : 15
                code
                   0x97007c00a00000000000000000000000000000000000000000007c016a
                   010000000000000000ac01a6010000ab0100000000000000007d047c04a0
                   0200000000000000000000000000000000000000006402ac03a6010000ab
                   01000000000000000001007c04a003000000000000000000000000000000
                   0000000000a6000000ab0000000000000000000100740900000000000000
                   0000006404740b000000000000000000006405a6010000ab010000000000
                   0000006901a6010000ab0100000000000000005300
-               299           0 RESUME                   0
+               314           0 RESUME                   0
                
-               300           2 LOAD_FAST                0 (self)
+               315           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_serializer)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_ATTR                1 (data)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               4 (serializer)
                
-               301          56 LOAD_FAST                4 (serializer)
+               316          56 LOAD_FAST                4 (serializer)
                             58 LOAD_METHOD              2 (is_valid)
                             80 LOAD_CONST               2 (True)
                             82 KW_NAMES                 3
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_TOP
                
-               302         100 LOAD_FAST                4 (serializer)
+               317         100 LOAD_FAST                4 (serializer)
                            102 LOAD_METHOD              3 (save)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 POP_TOP
                
-               303         140 LOAD_GLOBAL              9 (NULL + Response)
+               318         140 LOAD_GLOBAL              9 (NULL + Response)
                            152 LOAD_CONST               4 ('detail')
                            154 LOAD_GLOBAL             11 (NULL + _)
                            166 LOAD_CONST               5 ('New password has been saved.')
                            168 PRECALL                  1
                            172 CALL                     1
                            182 BUILD_MAP                1
                            184 PRECALL                  1
@@ -1820,29 +1934,29 @@
                   'New password has been saved.'
                names      ('get_serializer', 'data', 'is_valid', 'save', 'Response', '_')
                varnames   ('self', 'request', 'args', 'kwargs', 'serializer')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
                name       'post'
-               firstlineno 299
+               firstlineno 314
                lnotab 0x020136012c012801
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'api_settings', 'PASSWORD_CHANGE_SERIALIZER', 'serializer_class', 'IsAuthenticated', 'permission_classes', 'throttle_scope', 'sensitive_post_parameters_m', 'dispatch', 'post', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
          name       'PasswordChangeView'
-         firstlineno 284
+         firstlineno 299
          lnotab 0x0c0104060e0106010402020108ff0e010203
       'PasswordChangeView'
       None
    names      ('django.conf', 'settings', 'django.contrib.auth', 'get_user_model', 'login', 'django_login', 'logout', 'django_logout', 'django.core.exceptions', 'ObjectDoesNotExist', 'django.utils', 'timezone', 'django.utils.decorators', 'method_decorator', 'django.utils.translation', 'gettext_lazy', '_', 'django.views.decorators.debug', 'sensitive_post_parameters', 'rest_framework', 'status', 'rest_framework.generics', 'GenericAPIView', 'RetrieveUpdateAPIView', 'rest_framework.permissions', 'AllowAny', 'IsAuthenticated', 'rest_framework.response', 'Response', 'rest_framework.views', 'APIView', 'app_settings', 'api_settings', 'models', 'get_token_model', 'utils', 'jwt_encode', 'sensitive_post_parameters_m', 'LoginView', 'LogoutView', 'UserDetailsView', 'PasswordResetView', 'PasswordResetConfirmView', 'PasswordChangeView')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c010c010c010c010c010c010c010c010c01100110010c
-      010c020c010c010c030401040108ff0eff10071c671c4e1c191c181c1a
+      010c020c010c010c030401040108ff0eff10071c671c5d1c191c181c1a
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/app_settings.py` & `dj-rest-auth-5.1.0/dj_rest_auth/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/forms.py` & `dj-rest-auth-5.1.0/dj_rest_auth/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,20 +58,23 @@
             # save it to the password reset model
             # password_reset = PasswordReset(user=user, temp_key=temp_key)
             # password_reset.save()
 
             # send the password reset email
             url_generator = kwargs.get('url_generator', default_url_generator)
             url = url_generator(request, user, temp_key)
+            uid = user_pk_to_url_str(user)
 
             context = {
                 'current_site': current_site,
                 'user': user,
                 'password_reset_url': url,
                 'request': request,
+                'token': temp_key,
+                'uid': uid,
             }
             if (
                 allauth_account_settings.AUTHENTICATION_METHOD
                 != allauth_account_settings.AuthenticationMethod.EMAIL
             ):
                 context['username'] = user_username(user)
             get_adapter(request).send_mail(
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/jwt_auth.py` & `dj-rest-auth-5.1.0/dj_rest_auth/jwt_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,18 @@
 
         def finalize_response(self, request, response, *args, **kwargs):
             if response.status_code == status.HTTP_200_OK and 'access' in response.data:
                 set_jwt_access_cookie(response, response.data['access'])
                 response.data['access_expiration'] = (timezone.now() + jwt_settings.ACCESS_TOKEN_LIFETIME)
             if response.status_code == status.HTTP_200_OK and 'refresh' in response.data:
                 set_jwt_refresh_cookie(response, response.data['refresh'])
-                response.data['refresh_expiration'] = (timezone.now() + jwt_settings.REFRESH_TOKEN_LIFETIME)
+                if api_settings.JWT_AUTH_HTTPONLY:
+                    del response.data['refresh']
+                else:
+                    response.data['refresh_expiration'] = (timezone.now() + jwt_settings.REFRESH_TOKEN_LIFETIME)
             return super().finalize_response(request, response, *args, **kwargs)
     return RefreshViewWithCookieSupport
 
 
 class JWTCookieAuthentication(JWTAuthentication):
     """
     An authentication plugin that hopefully authenticates requests through a JSON web
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ar/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/az/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/cs/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/de/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/es/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/fa/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/fr/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/hr/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/id/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/it/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/it/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ja/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ko/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/nl/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/pl/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ro/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/ru/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/sv/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/tr/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/uk/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po` & `dj-rest-auth-5.1.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/models.py` & `dj-rest-auth-5.1.0/dj_rest_auth/models.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/serializers.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/serializers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/urls.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/views.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/views.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/serializers.py` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/urls.py` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/registration/views.py` & `dj-rest-auth-5.1.0/dj_rest_auth/registration/views.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/serializers.py` & `dj-rest-auth-5.1.0/dj_rest_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/social_serializers.py` & `dj-rest-auth-5.1.0/dj_rest_auth/social_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/django_urls.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/mixins.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/settings.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/settings.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x490e3c65 (Fri Oct 27 19:23:53 2023 UTC)
-files sz: 2885
+moddate:  0x9faf0066 (Sun Mar 24 22:56:31 2024 UTC)
+files sz: 3030
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a0265016a
@@ -19,15 +19,15 @@
       0266015a0d64075a0e6408650e9b0064089d035a0f65016a030000000000
       000000a01000000000000000000000000000000000000000006507650e9b
       00a6020000ab0200000000000000005a1164095a1264095a1364095a1464
       0a65026a15000000000000000076007008640b65026a1500000000000000
       0076005a16640c640d640e640f9c0269015a1767006410a2015a1865185a
       196411641267025a1a6413670064146415651a690164169c0467015a1b64
       17641869015a1c64195a1d641a5a1e6700641ba2015a1f641c5a20641d5a
-      21641d5a22641e5a2369005a2464015300
+      21641e640169015a22641d5a23641f5a2469005a2564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -197,24 +197,30 @@
    
     99         472 LOAD_CONST              28 ('38dh*skf8sjfhs287dh&^hd8&3hdg*j2&sd')
                474 STORE_NAME              32 (SECRET_KEY)
    
    100         476 LOAD_CONST              29 (1)
                478 STORE_NAME              33 (ACCOUNT_ACTIVATION_DAYS)
    
-   101         480 LOAD_CONST              29 (1)
-               482 STORE_NAME              34 (SITE_ID)
+   103         480 LOAD_CONST              30 ('confirm_email')
+               482 LOAD_CONST               1 (None)
    
-   103         484 LOAD_CONST              30 (('django.contrib.auth.backends.ModelBackend', 'allauth.account.auth_backends.AuthenticationBackend'))
-               486 STORE_NAME              35 (AUTHENTICATION_BACKENDS)
+   102         484 BUILD_MAP                1
+               486 STORE_NAME              34 (ACCOUNT_RATE_LIMITS)
    
-   110         488 BUILD_MAP                0
-               490 STORE_NAME              36 (REST_AUTH)
-               492 LOAD_CONST               1 (None)
-               494 RETURN_VALUE
+   105         488 LOAD_CONST              29 (1)
+               490 STORE_NAME              35 (SITE_ID)
+   
+   107         492 LOAD_CONST              31 (('django.contrib.auth.backends.ModelBackend', 'allauth.account.auth_backends.AuthenticationBackend'))
+               494 STORE_NAME              36 (AUTHENTICATION_BACKENDS)
+   
+   114         496 BUILD_MAP                0
+               498 STORE_NAME              37 (REST_AUTH)
+               500 LOAD_CONST               1 (None)
+               502 RETURN_VALUE
    consts
       0
       None
       'urls'
       '/static/'
       '/staticserve'
       'global'
@@ -238,20 +244,21 @@
       'DEFAULT_AUTHENTICATION_CLASSES'
       ('rest_framework.authentication.SessionAuthentication', 'dj_rest_auth.jwt_auth.JWTCookieAuthentication')
       'xmlrunner.extra.djangotestrunner.XMLTestRunner'
       'test-results'
       ('django.contrib.messages', 'django.contrib.admin', 'django.contrib.auth', 'django.contrib.humanize', 'django.contrib.contenttypes', 'django.contrib.sessions', 'django.contrib.sites', 'django.contrib.sitemaps', 'django.contrib.staticfiles', 'allauth', 'allauth.account', 'allauth.socialaccount', 'allauth.socialaccount.providers.facebook', 'allauth.socialaccount.providers.twitter', 'rest_framework', 'rest_framework.authtoken', 'dj_rest_auth', 'dj_rest_auth.registration', 'rest_framework_simplejwt.token_blacklist')
       '38dh*skf8sjfhs287dh&^hd8&3hdg*j2&sd'
       1
+      'confirm_email'
       ('django.contrib.auth.backends.ModelBackend', 'allauth.account.auth_backends.AuthenticationBackend')
-   names      ('logging', 'os', 'sys', 'path', 'abspath', 'split', '__file__', 'PROJECT_ROOT', 'disable', 'CRITICAL', 'ROOT_URLCONF', 'STATIC_URL', 'STATIC_ROOT', 'STATICFILES_DIRS', 'UPLOADS_DIR_NAME', 'MEDIA_URL', 'join', 'MEDIA_ROOT', 'IS_DEV', 'IS_STAGING', 'IS_PROD', 'argv', 'IS_TEST', 'DATABASES', 'MIDDLEWARE', 'MIDDLEWARE_CLASSES', 'TEMPLATE_CONTEXT_PROCESSORS', 'TEMPLATES', 'REST_FRAMEWORK', 'TEST_RUNNER', 'TEST_OUTPUT_DIR', 'INSTALLED_APPS', 'SECRET_KEY', 'ACCOUNT_ACTIVATION_DAYS', 'SITE_ID', 'AUTHENTICATION_BACKENDS', 'REST_AUTH')
+   names      ('logging', 'os', 'sys', 'path', 'abspath', 'split', '__file__', 'PROJECT_ROOT', 'disable', 'CRITICAL', 'ROOT_URLCONF', 'STATIC_URL', 'STATIC_ROOT', 'STATICFILES_DIRS', 'UPLOADS_DIR_NAME', 'MEDIA_URL', 'join', 'MEDIA_ROOT', 'IS_DEV', 'IS_STAGING', 'IS_PROD', 'argv', 'IS_TEST', 'DATABASES', 'MIDDLEWARE', 'MIDDLEWARE_CLASSES', 'TEMPLATE_CONTEXT_PROCESSORS', 'TEMPLATES', 'REST_FRAMEWORK', 'TEST_RUNNER', 'TEST_OUTPUT_DIR', 'INSTALLED_APPS', 'SECRET_KEY', 'ACCOUNT_ACTIVATION_DAYS', 'ACCOUNT_RATE_LIMITS', 'SITE_ID', 'AUTHENTICATION_BACKENDS', 'REST_AUTH')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/settings.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010803ac032a01040104010a020cff040304010c0138
       0204010401040124030201020102fe04ff0407080a0403020102fe040802
-      010203020204ff02fa04ff040e04ff040704010402081a04010401040204
-      07
+      010203020204ff02fa04ff040e04ff040704010402081a0401040304ff04
+      0304020407
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_api.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_api.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa9385764 (Sun May  7 05:35:37 2023 UTC)
-files sz: 44032
+moddate:  0x9faf0066 (Sun Mar 24 22:56:31 2024 UTC)
+files sz: 45434
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a030100640064036c046d
@@ -459,22 +459,28 @@
             000000ab000000000000000000a6000000ab0000000000000000005a4102
             006519640bac5ba6010000ab01000000000000000002006519640bac15a6
             010000ab01000000000000000002006519645dac41a6010000ab01000000
             000000000002006519645eac45a6010000ab010000000000000000020065
             19642bac4da6010000ab01000000000000000064628400a6000000ab0000
             00000000000000a6000000ab000000000000000000a6000000ab00000000
             0000000000a6000000ab000000000000000000a6000000ab000000000000
-            0000005a4202006519640bac15a6010000ab010000000000000000020065
-            19642bac4da6010000ab01000000000000000064638400a6000000ab0000
-            00000000000000a6000000ab0000000000000000005a43020065196435ac
-            36a6010000ab0100000000000000000200651b6417646467016901ac1aa6
-            010000ab01000000000000000064658400a6000000ab0000000000000000
-            00a6000000ab0000000000000000005a44646684005a450200651b641764
-            6467016901ac1aa6010000ab01000000000000000064678400a6000000ab
-            0000000000000000005a4664355300
+            0000005a4202006519640bac5ba6010000ab010000000000000000020065
+            19640bac15a6010000ab01000000000000000002006519645dac41a60100
+            00ab01000000000000000002006519645eac45a6010000ab010000000000
+            00000002006519640bac4da6010000ab01000000000000000064638400a6
+            000000ab000000000000000000a6000000ab000000000000000000a60000
+            00ab000000000000000000a6000000ab000000000000000000a6000000ab
+            0000000000000000005a4302006519640bac15a6010000ab010000000000
+            00000002006519642bac4da6010000ab01000000000000000064648400a6
+            000000ab000000000000000000a6000000ab0000000000000000005a4402
+            0065196435ac36a6010000ab0100000000000000000200651b6417646567
+            016901ac1aa6010000ab01000000000000000064668400a6000000ab0000
+            00000000000000a6000000ab0000000000000000005a45646784005a4602
+            00651b6417646567016901ac1aa6010000ab010000000000000000646884
+            00a6000000ab0000000000000000005a4764355300
            38           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('APIBasicTests')
                         8 STORE_NAME               2 (__qualname__)
          
            40          10 LOAD_CONST               1 ('\n    Case #1:\n    - user profile: defined\n    - custom registration: backend defined\n    ')
@@ -1800,87 +1806,142 @@
                      4012 CALL                     0
          
          1048        4022 STORE_NAME              66 (test_custom_token_refresh_view)
          
          1068        4024 PUSH_NULL
                      4026 LOAD_NAME               25 (override_api_settings)
                      4028 LOAD_CONST              11 (True)
-                     4030 KW_NAMES                21
+                     4030 KW_NAMES                91
                      4032 PRECALL                  1
                      4036 CALL                     1
          
          1069        4046 PUSH_NULL
                      4048 LOAD_NAME               25 (override_api_settings)
-                     4050 LOAD_CONST              43 (False)
-                     4052 KW_NAMES                77
+                     4050 LOAD_CONST              11 (True)
+                     4052 KW_NAMES                21
                      4054 PRECALL                  1
                      4058 CALL                     1
          
-         1070        4068 LOAD_CONST              99 (<code object test_rotate_token_refresh_view, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1068>)
-                     4070 MAKE_FUNCTION            0
-         
-         1069        4072 PRECALL                  0
-                     4076 CALL                     0
-         
-         1068        4086 PRECALL                  0
-                     4090 CALL                     0
-         
-         1070        4100 STORE_NAME              67 (test_rotate_token_refresh_view)
-         
-         1093        4102 PUSH_NULL
-                     4104 LOAD_NAME               25 (override_api_settings)
-                     4106 LOAD_CONST              53 (None)
-                     4108 KW_NAMES                54
-                     4110 PRECALL                  1
-                     4114 CALL                     1
-         
-         1094        4124 PUSH_NULL
-                     4126 LOAD_NAME               27 (modify_settings)
-                     4128 LOAD_CONST              23 ('remove')
-                     4130 LOAD_CONST             100 ('rest_framework.authtoken')
-                     4132 BUILD_LIST               1
-                     4134 BUILD_MAP                1
-                     4136 KW_NAMES                26
-                     4138 PRECALL                  1
-                     4142 CALL                     1
-         
-         1095        4152 LOAD_CONST             101 (<code object test_login_with_no_token_model, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1093>)
-                     4154 MAKE_FUNCTION            0
-         
-         1094        4156 PRECALL                  0
-                     4160 CALL                     0
-         
-         1093        4170 PRECALL                  0
-                     4174 CALL                     0
-         
-         1095        4184 STORE_NAME              68 (test_login_with_no_token_model)
-         
-         1105        4186 LOAD_CONST             102 (<code object test_rest_session_login_sets_session_cookie, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1105>)
-                     4188 MAKE_FUNCTION            0
-                     4190 STORE_NAME              69 (test_rest_session_login_sets_session_cookie)
-         
-         1117        4192 PUSH_NULL
-                     4194 LOAD_NAME               27 (modify_settings)
-                     4196 LOAD_CONST              23 ('remove')
-                     4198 LOAD_CONST             100 ('rest_framework.authtoken')
-                     4200 BUILD_LIST               1
-                     4202 BUILD_MAP                1
-                     4204 KW_NAMES                26
-                     4206 PRECALL                  1
-                     4210 CALL                     1
-         
-         1118        4220 LOAD_CONST             103 (<code object test_misconfigured_token_model, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1117>)
-                     4222 MAKE_FUNCTION            0
-         
-         1117        4224 PRECALL                  0
-                     4228 CALL                     0
-         
-         1118        4238 STORE_NAME              70 (test_misconfigured_token_model)
-                     4240 LOAD_CONST              53 (None)
-                     4242 RETURN_VALUE
+         1070        4068 PUSH_NULL
+                     4070 LOAD_NAME               25 (override_api_settings)
+                     4072 LOAD_CONST              93 ('xxx')
+                     4074 KW_NAMES                65
+                     4076 PRECALL                  1
+                     4080 CALL                     1
+         
+         1071        4090 PUSH_NULL
+                     4092 LOAD_NAME               25 (override_api_settings)
+                     4094 LOAD_CONST              94 ('refresh-xxx')
+                     4096 KW_NAMES                69
+                     4098 PRECALL                  1
+                     4102 CALL                     1
+         
+         1072        4112 PUSH_NULL
+                     4114 LOAD_NAME               25 (override_api_settings)
+                     4116 LOAD_CONST              11 (True)
+                     4118 KW_NAMES                77
+                     4120 PRECALL                  1
+                     4124 CALL                     1
+         
+         1073        4134 LOAD_CONST              99 (<code object test_custom_token_refresh_view_with_http_only_cookie_and_refresh_token_rotation, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1068>)
+                     4136 MAKE_FUNCTION            0
+         
+         1072        4138 PRECALL                  0
+                     4142 CALL                     0
+         
+         1071        4152 PRECALL                  0
+                     4156 CALL                     0
+         
+         1070        4166 PRECALL                  0
+                     4170 CALL                     0
+         
+         1069        4180 PRECALL                  0
+                     4184 CALL                     0
+         
+         1068        4194 PRECALL                  0
+                     4198 CALL                     0
+         
+         1073        4208 STORE_NAME              67 (test_custom_token_refresh_view_with_http_only_cookie_and_refresh_token_rotation)
+         
+         1099        4210 PUSH_NULL
+                     4212 LOAD_NAME               25 (override_api_settings)
+                     4214 LOAD_CONST              11 (True)
+                     4216 KW_NAMES                21
+                     4218 PRECALL                  1
+                     4222 CALL                     1
+         
+         1100        4232 PUSH_NULL
+                     4234 LOAD_NAME               25 (override_api_settings)
+                     4236 LOAD_CONST              43 (False)
+                     4238 KW_NAMES                77
+                     4240 PRECALL                  1
+                     4244 CALL                     1
+         
+         1101        4254 LOAD_CONST             100 (<code object test_rotate_token_refresh_view, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1099>)
+                     4256 MAKE_FUNCTION            0
+         
+         1100        4258 PRECALL                  0
+                     4262 CALL                     0
+         
+         1099        4272 PRECALL                  0
+                     4276 CALL                     0
+         
+         1101        4286 STORE_NAME              68 (test_rotate_token_refresh_view)
+         
+         1124        4288 PUSH_NULL
+                     4290 LOAD_NAME               25 (override_api_settings)
+                     4292 LOAD_CONST              53 (None)
+                     4294 KW_NAMES                54
+                     4296 PRECALL                  1
+                     4300 CALL                     1
+         
+         1125        4310 PUSH_NULL
+                     4312 LOAD_NAME               27 (modify_settings)
+                     4314 LOAD_CONST              23 ('remove')
+                     4316 LOAD_CONST             101 ('rest_framework.authtoken')
+                     4318 BUILD_LIST               1
+                     4320 BUILD_MAP                1
+                     4322 KW_NAMES                26
+                     4324 PRECALL                  1
+                     4328 CALL                     1
+         
+         1126        4338 LOAD_CONST             102 (<code object test_login_with_no_token_model, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1124>)
+                     4340 MAKE_FUNCTION            0
+         
+         1125        4342 PRECALL                  0
+                     4346 CALL                     0
+         
+         1124        4356 PRECALL                  0
+                     4360 CALL                     0
+         
+         1126        4370 STORE_NAME              69 (test_login_with_no_token_model)
+         
+         1136        4372 LOAD_CONST             103 (<code object test_rest_session_login_sets_session_cookie, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1136>)
+                     4374 MAKE_FUNCTION            0
+                     4376 STORE_NAME              70 (test_rest_session_login_sets_session_cookie)
+         
+         1148        4378 PUSH_NULL
+                     4380 LOAD_NAME               27 (modify_settings)
+                     4382 LOAD_CONST              23 ('remove')
+                     4384 LOAD_CONST             101 ('rest_framework.authtoken')
+                     4386 BUILD_LIST               1
+                     4388 BUILD_MAP                1
+                     4390 KW_NAMES                26
+                     4392 PRECALL                  1
+                     4396 CALL                     1
+         
+         1149        4406 LOAD_CONST             104 (<code object test_misconfigured_token_model, file "/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py", line 1148>)
+                     4408 MAKE_FUNCTION            0
+         
+         1148        4410 PRECALL                  0
+                     4414 CALL                     0
+         
+         1149        4424 STORE_NAME              71 (test_misconfigured_token_model)
+                     4426 LOAD_CONST              53 (None)
+                     4428 RETURN_VALUE
          consts
             'APIBasicTests'
             '\n    Case #1:\n    - user profile: defined\n    - custom registration: backend defined\n    '
             'person'
             'person1@world.com'
             'new-test-pass'
             'rest_auth.runtests.RegistrationView'
@@ -8117,14 +8178,194 @@
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
                name       'test_custom_token_refresh_view'
                firstlineno 1043
                lnotab 0x02070c010cfe060564013a01340118011c011e0102fd120536033601
             code
                argcount  : 1
+               nlocals   : 7
+               stacksize : 6
+               flags     : 3
+               code
+                  0x9700640164026c006d017d01010064037c015f0200000000000000007c
+                  006a0300000000000000007c006a04000000000000000064049c027d0264
+                  057d03740b00000000000000000000a6000000ab0000000000000000006a
+                  060000000000000000a00700000000000000000000000000000000000000
+                  007c006a03000000000000000064067c006a040000000000000000a60300
+                  00ab03000000000000000001007c00a00800000000000000000000000000
+                  000000000000007c006a0900000000000000007c026407ac08a6030000ab
+                  0300000000000000007d047c046a0a00000000000000007c031900000000
+                  00000000006a0b00000000000000007d057c00a008000000000000000000
+                  00000000000000000000007419000000000000000000006409a6010000ab
+                  010000000000000000741b000000000000000000007c05ac0aa6010000ab
+                  0100000000000000006407ac08a6030000ab0300000000000000007d067c
+                  00a00e0000000000000000000000000000000000000000640b7c066a0a00
+                  00000000000000a6020000ab02000000000000000001007c00a00e000000
+                  0000000000000000000000000000000000640c7c066a0f00000000000000
+                  00a6020000ab02000000000000000001007c00a00e000000000000000000
+                  0000000000000000000000640d7c066a0f0000000000000000a6020000ab
+                  02000000000000000001007c00a010000000000000000000000000000000
+                  0000000000640e7c066a0f0000000000000000a6020000ab020000000000
+                  00000001007c00a010000000000000000000000000000000000000000064
+                  0f7c066a0f0000000000000000a6020000ab020000000000000000010064
+                  005300
+               1068           0 RESUME                   0
+               
+               1074           2 LOAD_CONST               1 (0)
+                              4 LOAD_CONST               2 (('api_settings',))
+                              6 IMPORT_NAME              0 (rest_framework_simplejwt.settings)
+                              8 IMPORT_FROM              1 (api_settings)
+                             10 STORE_FAST               1 (jwt_settings)
+                             12 POP_TOP
+               
+               1075          14 LOAD_CONST               3 (True)
+                             16 LOAD_FAST                1 (jwt_settings)
+                             18 STORE_ATTR               2 (ROTATE_REFRESH_TOKENS)
+               
+               1077          28 LOAD_FAST                0 (self)
+                             30 LOAD_ATTR                3 (USERNAME)
+               
+               1078          40 LOAD_FAST                0 (self)
+                             42 LOAD_ATTR                4 (PASS)
+               
+               1076          52 LOAD_CONST               4 (('username', 'password'))
+                             54 BUILD_CONST_KEY_MAP      2
+                             56 STORE_FAST               2 (payload)
+               
+               1080          58 LOAD_CONST               5 ('refresh-xxx')
+                             60 STORE_FAST               3 (refresh_cookie_name)
+               
+               1082          62 LOAD_GLOBAL             11 (NULL + get_user_model)
+                             74 PRECALL                  0
+                             78 CALL                     0
+                             88 LOAD_ATTR                6 (objects)
+                             98 LOAD_METHOD              7 (create_user)
+                            120 LOAD_FAST                0 (self)
+                            122 LOAD_ATTR                3 (USERNAME)
+                            132 LOAD_CONST               6 ('')
+                            134 LOAD_FAST                0 (self)
+                            136 LOAD_ATTR                4 (PASS)
+                            146 PRECALL                  3
+                            150 CALL                     3
+                            160 POP_TOP
+               
+               1083         162 LOAD_FAST                0 (self)
+                            164 LOAD_METHOD              8 (post)
+                            186 LOAD_FAST                0 (self)
+                            188 LOAD_ATTR                9 (login_url)
+                            198 LOAD_FAST                2 (payload)
+                            200 LOAD_CONST               7 (200)
+                            202 KW_NAMES                 8
+                            204 PRECALL                  3
+                            208 CALL                     3
+                            218 STORE_FAST               4 (resp)
+               
+               1084         220 LOAD_FAST                4 (resp)
+                            222 LOAD_ATTR               10 (cookies)
+                            232 LOAD_FAST                3 (refresh_cookie_name)
+                            234 BINARY_SUBSCR
+                            244 LOAD_ATTR               11 (value)
+                            254 STORE_FAST               5 (refresh)
+               
+               1085         256 LOAD_FAST                0 (self)
+                            258 LOAD_METHOD              8 (post)
+               
+               1086         280 LOAD_GLOBAL             25 (NULL + reverse)
+                            292 LOAD_CONST               9 ('token_refresh')
+                            294 PRECALL                  1
+                            298 CALL                     1
+               
+               1087         308 LOAD_GLOBAL             27 (NULL + dict)
+                            320 LOAD_FAST                5 (refresh)
+                            322 KW_NAMES                10
+                            324 PRECALL                  1
+                            328 CALL                     1
+               
+               1088         338 LOAD_CONST               7 (200)
+               
+               1085         340 KW_NAMES                 8
+                            342 PRECALL                  3
+                            346 CALL                     3
+                            356 STORE_FAST               6 (refresh_resp)
+               
+               1090         358 LOAD_FAST                0 (self)
+                            360 LOAD_METHOD             14 (assertIn)
+                            382 LOAD_CONST              11 ('xxx')
+                            384 LOAD_FAST                6 (refresh_resp)
+                            386 LOAD_ATTR               10 (cookies)
+                            396 PRECALL                  2
+                            400 CALL                     2
+                            410 POP_TOP
+               
+               1093         412 LOAD_FAST                0 (self)
+                            414 LOAD_METHOD             14 (assertIn)
+                            436 LOAD_CONST              12 ('access')
+                            438 LOAD_FAST                6 (refresh_resp)
+                            440 LOAD_ATTR               15 (data)
+                            450 PRECALL                  2
+                            454 CALL                     2
+                            464 POP_TOP
+               
+               1094         466 LOAD_FAST                0 (self)
+                            468 LOAD_METHOD             14 (assertIn)
+                            490 LOAD_CONST              13 ('access_expiration')
+                            492 LOAD_FAST                6 (refresh_resp)
+                            494 LOAD_ATTR               15 (data)
+                            504 PRECALL                  2
+                            508 CALL                     2
+                            518 POP_TOP
+               
+               1096         520 LOAD_FAST                0 (self)
+                            522 LOAD_METHOD             16 (assertNotIn)
+                            544 LOAD_CONST              14 ('refresh')
+                            546 LOAD_FAST                6 (refresh_resp)
+                            548 LOAD_ATTR               15 (data)
+                            558 PRECALL                  2
+                            562 CALL                     2
+                            572 POP_TOP
+               
+               1097         574 LOAD_FAST                0 (self)
+                            576 LOAD_METHOD             16 (assertNotIn)
+                            598 LOAD_CONST              15 ('refresh_expiration')
+                            600 LOAD_FAST                6 (refresh_resp)
+                            602 LOAD_ATTR               15 (data)
+                            612 PRECALL                  2
+                            616 CALL                     2
+                            626 POP_TOP
+                            628 LOAD_CONST               0 (None)
+                            630 RETURN_VALUE
+               consts
+                  None
+                  0
+                  ('api_settings',)
+                  True
+                  ('username', 'password')
+                  'refresh-xxx'
+                  ''
+                  200
+                  ('data', 'status_code')
+                  'token_refresh'
+                  ('refresh',)
+                  'xxx'
+                  'access'
+                  'access_expiration'
+                  'refresh'
+                  'refresh_expiration'
+               names      ('rest_framework_simplejwt.settings', 'api_settings', 'ROTATE_REFRESH_TOKENS', 'USERNAME', 'PASS', 'get_user_model', 'objects', 'create_user', 'post', 'login_url', 'cookies', 'value', 'reverse', 'dict', 'assertIn', 'data', 'assertNotIn')
+               varnames   ('self', 'jwt_settings', 'payload', 'refresh_cookie_name', 'resp', 'refresh', 'refresh_resp')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
+               name       'test_custom_token_refresh_view_with_http_only_cookie_and_refresh_token_rotation'
+               firstlineno 1068
+               lnotab
+                  0x02060c010e020c010cfe0604040264013a01240118011c011e0102fd12
+                  053603360136023601
+            code
+               argcount  : 1
                nlocals   : 5
                stacksize : 6
                flags     : 3
                code
                   0x9700640164026c006d017d01010064037c015f0200000000000000007c
                   006a0300000000000000007c006a04000000000000000064049c027d0274
                   0b00000000000000000000a6000000ab0000000000000000006a06000000
@@ -8142,119 +8383,119 @@
                   0000000000ac06a6020000ab0200000000000000007d037c00a00a000000
                   00000000000000000000000000000000007c036a0b000000000000000074
                   18000000000000000000006a0d0000000000000000a6020000ab02000000
                   000000000001007c00a01200000000000000000000000000000000000000
                   0064077c036a0e0000000000000000a6020000ab02000000000000000001
                   007c00a0120000000000000000000000000000000000000000640a7c036a
                   0e0000000000000000a6020000ab020000000000000000010064005300
-               1068           0 RESUME                   0
+               1099           0 RESUME                   0
                
-               1071           2 LOAD_CONST               1 (0)
+               1102           2 LOAD_CONST               1 (0)
                               4 LOAD_CONST               2 (('api_settings',))
                               6 IMPORT_NAME              0 (rest_framework_simplejwt.settings)
                               8 IMPORT_FROM              1 (api_settings)
                              10 STORE_FAST               1 (jwt_settings)
                              12 POP_TOP
                
-               1072          14 LOAD_CONST               3 (True)
+               1103          14 LOAD_CONST               3 (True)
                              16 LOAD_FAST                1 (jwt_settings)
                              18 STORE_ATTR               2 (ROTATE_REFRESH_TOKENS)
                
-               1074          28 LOAD_FAST                0 (self)
+               1105          28 LOAD_FAST                0 (self)
                              30 LOAD_ATTR                3 (USERNAME)
                
-               1075          40 LOAD_FAST                0 (self)
+               1106          40 LOAD_FAST                0 (self)
                              42 LOAD_ATTR                4 (PASS)
                
-               1073          52 LOAD_CONST               4 (('username', 'password'))
+               1104          52 LOAD_CONST               4 (('username', 'password'))
                              54 BUILD_CONST_KEY_MAP      2
                              56 STORE_FAST               2 (payload)
                
-               1078          58 LOAD_GLOBAL             11 (NULL + get_user_model)
+               1109          58 LOAD_GLOBAL             11 (NULL + get_user_model)
                              70 PRECALL                  0
                              74 CALL                     0
                              84 LOAD_ATTR                6 (objects)
                              94 LOAD_METHOD              7 (create_user)
                             116 LOAD_FAST                0 (self)
                             118 LOAD_ATTR                3 (USERNAME)
                             128 LOAD_CONST               5 ('')
                             130 LOAD_FAST                0 (self)
                             132 LOAD_ATTR                4 (PASS)
                             142 PRECALL                  3
                             146 CALL                     3
                             156 POP_TOP
                
-               1079         158 LOAD_FAST                0 (self)
+               1110         158 LOAD_FAST                0 (self)
                             160 LOAD_METHOD              8 (post)
                             182 LOAD_FAST                0 (self)
                             184 LOAD_ATTR                9 (login_url)
                             194 LOAD_FAST                2 (payload)
                             196 KW_NAMES                 6
                             198 PRECALL                  2
                             202 CALL                     2
                             212 STORE_FAST               3 (resp)
                
-               1080         214 LOAD_FAST                0 (self)
+               1111         214 LOAD_FAST                0 (self)
                             216 LOAD_METHOD             10 (assertEqual)
                             238 LOAD_FAST                3 (resp)
                             240 LOAD_ATTR               11 (status_code)
                             250 LOAD_GLOBAL             24 (status)
                             262 LOAD_ATTR               13 (HTTP_200_OK)
                             272 PRECALL                  2
                             276 CALL                     2
                             286 POP_TOP
                
-               1082         288 LOAD_FAST                3 (resp)
+               1113         288 LOAD_FAST                3 (resp)
                             290 LOAD_ATTR               14 (data)
                             300 LOAD_METHOD             15 (get)
                             322 LOAD_CONST               7 ('refresh')
                             324 LOAD_CONST               0 (None)
                             326 PRECALL                  2
                             330 CALL                     2
                             340 STORE_FAST               4 (refresh)
                
-               1083         342 LOAD_FAST                0 (self)
+               1114         342 LOAD_FAST                0 (self)
                             344 LOAD_METHOD              8 (post)
                
-               1084         366 LOAD_GLOBAL             33 (NULL + reverse)
+               1115         366 LOAD_GLOBAL             33 (NULL + reverse)
                             378 LOAD_CONST               8 ('token_refresh')
                             380 PRECALL                  1
                             384 CALL                     1
                
-               1085         394 LOAD_GLOBAL             35 (NULL + dict)
+               1116         394 LOAD_GLOBAL             35 (NULL + dict)
                             406 LOAD_FAST                4 (refresh)
                             408 KW_NAMES                 9
                             410 PRECALL                  1
                             414 CALL                     1
                
-               1083         424 KW_NAMES                 6
+               1114         424 KW_NAMES                 6
                             426 PRECALL                  2
                             430 CALL                     2
                             440 STORE_FAST               3 (resp)
                
-               1087         442 LOAD_FAST                0 (self)
+               1118         442 LOAD_FAST                0 (self)
                             444 LOAD_METHOD             10 (assertEqual)
                             466 LOAD_FAST                3 (resp)
                             468 LOAD_ATTR               11 (status_code)
                             478 LOAD_GLOBAL             24 (status)
                             490 LOAD_ATTR               13 (HTTP_200_OK)
                             500 PRECALL                  2
                             504 CALL                     2
                             514 POP_TOP
                
-               1090         516 LOAD_FAST                0 (self)
+               1121         516 LOAD_FAST                0 (self)
                             518 LOAD_METHOD             18 (assertIn)
                             540 LOAD_CONST               7 ('refresh')
                             542 LOAD_FAST                3 (resp)
                             544 LOAD_ATTR               14 (data)
                             554 PRECALL                  2
                             558 CALL                     2
                             568 POP_TOP
                
-               1091         570 LOAD_FAST                0 (self)
+               1122         570 LOAD_FAST                0 (self)
                             572 LOAD_METHOD             18 (assertIn)
                             594 LOAD_CONST              10 ('refresh_expiration')
                             596 LOAD_FAST                3 (resp)
                             598 LOAD_ATTR               14 (data)
                             608 PRECALL                  2
                             612 CALL                     2
                             622 POP_TOP
@@ -8274,15 +8515,15 @@
                   'refresh_expiration'
                names      ('rest_framework_simplejwt.settings', 'api_settings', 'ROTATE_REFRESH_TOKENS', 'USERNAME', 'PASS', 'get_user_model', 'objects', 'create_user', 'post', 'login_url', 'assertEqual', 'status_code', 'status', 'HTTP_200_OK', 'data', 'get', 'reverse', 'dict', 'assertIn')
                varnames   ('self', 'jwt_settings', 'payload', 'resp', 'refresh')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
                name       'test_rotate_token_refresh_view'
-               firstlineno 1068
+               firstlineno 1099
                lnotab
                   0x02030c010e020c010cfe0605640138014a02360118011c011efe12044a
                   033601
             'rest_framework.authtoken'
             code
                argcount  : 1
                nlocals   : 3
@@ -8297,63 +8538,63 @@
                   000000000000000000000000000000000000007c006a0000000000000000
                   0064037c006a010000000000000000a6030000ab03000000000000000001
                   007c00a00200000000000000000000000000000000000000007c006a0300
                   000000000000007c017408000000000000000000006a0900000000000000
                   00ac02a6030000ab0300000000000000007d027c00a00a00000000000000
                   000000000000000000000000007c026a0b00000000000000006404a60200
                   00ab020000000000000000010064005300
-               1093           0 RESUME                   0
+               1124           0 RESUME                   0
                
-               1096           2 LOAD_FAST                0 (self)
+               1127           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (USERNAME)
                              14 LOAD_FAST                0 (self)
                              16 LOAD_ATTR                1 (PASS)
                              26 LOAD_CONST               1 (('username', 'password'))
                              28 BUILD_CONST_KEY_MAP      2
                              30 STORE_FAST               1 (payload)
                
-               1098          32 LOAD_FAST                0 (self)
+               1129          32 LOAD_FAST                0 (self)
                              34 LOAD_METHOD              2 (post)
                              56 LOAD_FAST                0 (self)
                              58 LOAD_ATTR                3 (login_url)
                              68 LOAD_FAST                1 (payload)
                              70 LOAD_GLOBAL              8 (status)
                              82 LOAD_ATTR                5 (HTTP_400_BAD_REQUEST)
                              92 KW_NAMES                 2
                              94 PRECALL                  3
                              98 CALL                     3
                             108 STORE_FAST               2 (resp)
                
-               1100         110 LOAD_GLOBAL             13 (NULL + get_user_model)
+               1131         110 LOAD_GLOBAL             13 (NULL + get_user_model)
                             122 PRECALL                  0
                             126 CALL                     0
                             136 LOAD_ATTR                7 (objects)
                             146 LOAD_METHOD              8 (create_user)
                             168 LOAD_FAST                0 (self)
                             170 LOAD_ATTR                0 (USERNAME)
                             180 LOAD_CONST               3 ('')
                             182 LOAD_FAST                0 (self)
                             184 LOAD_ATTR                1 (PASS)
                             194 PRECALL                  3
                             198 CALL                     3
                             208 POP_TOP
                
-               1101         210 LOAD_FAST                0 (self)
+               1132         210 LOAD_FAST                0 (self)
                             212 LOAD_METHOD              2 (post)
                             234 LOAD_FAST                0 (self)
                             236 LOAD_ATTR                3 (login_url)
                             246 LOAD_FAST                1 (payload)
                             248 LOAD_GLOBAL              8 (status)
                             260 LOAD_ATTR                9 (HTTP_204_NO_CONTENT)
                             270 KW_NAMES                 2
                             272 PRECALL                  3
                             276 CALL                     3
                             286 STORE_FAST               2 (resp)
                
-               1103         288 LOAD_FAST                0 (self)
+               1134         288 LOAD_FAST                0 (self)
                             290 LOAD_METHOD             10 (assertEqual)
                             312 LOAD_FAST                2 (resp)
                             314 LOAD_ATTR               11 (content)
                             324 LOAD_CONST               4 (b'')
                             326 PRECALL                  2
                             330 CALL                     2
                             340 POP_TOP
@@ -8367,15 +8608,15 @@
                   b''
                names      ('USERNAME', 'PASS', 'post', 'login_url', 'status', 'HTTP_400_BAD_REQUEST', 'get_user_model', 'objects', 'create_user', 'HTTP_204_NO_CONTENT', 'assertEqual', 'content')
                varnames   ('self', 'payload', 'resp')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
                name       'test_login_with_no_token_model'
-               firstlineno 1093
+               firstlineno 1124
                lnotab 0x02031e024e0264014e02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -8397,72 +8638,72 @@
                   0000007c016405ac06a6030000ab0300000000000000007d027c00a00d00
                   000000000000000000000000000000000000007412000000000000000000
                   006a0a00000000000000007c026a0b0000000000000000a00c0000000000
                   000000000000000000000000000000a6000000ab00000000000000000076
                   00a6010000ab0100000000000000000100640064006400a6020000ab0200
                   000000000000000100640053002300310073047702780359007701010059
                   000100010064005300
-               1105           0 RESUME                   0
+               1136           0 RESUME                   0
                
-               1106           2 LOAD_GLOBAL              1 (NULL + get_user_model)
+               1137           2 LOAD_GLOBAL              1 (NULL + get_user_model)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_ATTR                1 (objects)
                              38 LOAD_METHOD              2 (create_user)
                              60 LOAD_FAST                0 (self)
                              62 LOAD_ATTR                3 (USERNAME)
                              72 LOAD_CONST               1 ('')
                              74 LOAD_FAST                0 (self)
                              76 LOAD_ATTR                4 (PASS)
                              86 PRECALL                  3
                              90 CALL                     3
                             100 POP_TOP
                
-               1107         102 LOAD_FAST                0 (self)
+               1138         102 LOAD_FAST                0 (self)
                             104 LOAD_ATTR                3 (USERNAME)
                             114 LOAD_FAST                0 (self)
                             116 LOAD_ATTR                4 (PASS)
                             126 LOAD_CONST               2 (('username', 'password'))
                             128 BUILD_CONST_KEY_MAP      2
                             130 STORE_FAST               1 (payload)
                
-               1109         132 LOAD_GLOBAL             11 (NULL + override_api_settings)
+               1140         132 LOAD_GLOBAL             11 (NULL + override_api_settings)
                             144 LOAD_CONST               3 (False)
                             146 KW_NAMES                 4
                             148 PRECALL                  1
                             152 CALL                     1
                             162 BEFORE_WITH
                             164 POP_TOP
                
-               1110         166 LOAD_FAST                0 (self)
+               1141         166 LOAD_FAST                0 (self)
                             168 LOAD_METHOD              6 (post)
                             190 LOAD_FAST                0 (self)
                             192 LOAD_ATTR                7 (login_url)
                             202 LOAD_FAST                1 (payload)
                             204 LOAD_CONST               5 (200)
                             206 KW_NAMES                 6
                             208 PRECALL                  3
                             212 CALL                     3
                             222 STORE_FAST               2 (resp)
                
-               1111         224 LOAD_FAST                0 (self)
+               1142         224 LOAD_FAST                0 (self)
                             226 LOAD_METHOD              8 (assertFalse)
                             248 LOAD_GLOBAL             18 (settings)
                             260 LOAD_ATTR               10 (SESSION_COOKIE_NAME)
                             270 LOAD_FAST                2 (resp)
                             272 LOAD_ATTR               11 (cookies)
                             282 LOAD_METHOD             12 (keys)
                             304 PRECALL                  0
                             308 CALL                     0
                             318 CONTAINS_OP              0
                             320 PRECALL                  1
                             324 CALL                     1
                             334 POP_TOP
                
-               1109         336 LOAD_CONST               0 (None)
+               1140         336 LOAD_CONST               0 (None)
                             338 LOAD_CONST               0 (None)
                             340 LOAD_CONST               0 (None)
                             342 PRECALL                  2
                             346 CALL                     2
                             356 POP_TOP
                             358 JUMP_FORWARD            11 (to 382)
                         >>  360 PUSH_EXC_INFO
@@ -8473,48 +8714,48 @@
                             370 POP_EXCEPT
                             372 RERAISE                  1
                         >>  374 POP_TOP
                             376 POP_EXCEPT
                             378 POP_TOP
                             380 POP_TOP
                
-               1113     >>  382 LOAD_GLOBAL             11 (NULL + override_api_settings)
+               1144     >>  382 LOAD_GLOBAL             11 (NULL + override_api_settings)
                             394 LOAD_CONST               7 (True)
                             396 KW_NAMES                 4
                             398 PRECALL                  1
                             402 CALL                     1
                             412 BEFORE_WITH
                             414 POP_TOP
                
-               1114         416 LOAD_FAST                0 (self)
+               1145         416 LOAD_FAST                0 (self)
                             418 LOAD_METHOD              6 (post)
                             440 LOAD_FAST                0 (self)
                             442 LOAD_ATTR                7 (login_url)
                             452 LOAD_FAST                1 (payload)
                             454 LOAD_CONST               5 (200)
                             456 KW_NAMES                 6
                             458 PRECALL                  3
                             462 CALL                     3
                             472 STORE_FAST               2 (resp)
                
-               1115         474 LOAD_FAST                0 (self)
+               1146         474 LOAD_FAST                0 (self)
                             476 LOAD_METHOD             13 (assertTrue)
                             498 LOAD_GLOBAL             18 (settings)
                             510 LOAD_ATTR               10 (SESSION_COOKIE_NAME)
                             520 LOAD_FAST                2 (resp)
                             522 LOAD_ATTR               11 (cookies)
                             532 LOAD_METHOD             12 (keys)
                             554 PRECALL                  0
                             558 CALL                     0
                             568 CONTAINS_OP              0
                             570 PRECALL                  1
                             574 CALL                     1
                             584 POP_TOP
                
-               1113         586 LOAD_CONST               0 (None)
+               1144         586 LOAD_CONST               0 (None)
                             588 LOAD_CONST               0 (None)
                             590 LOAD_CONST               0 (None)
                             592 PRECALL                  2
                             596 CALL                     2
                             606 POP_TOP
                             608 LOAD_CONST               0 (None)
                             610 RETURN_VALUE
@@ -8549,15 +8790,15 @@
                   True
                names      ('get_user_model', 'objects', 'create_user', 'USERNAME', 'PASS', 'override_api_settings', 'post', 'login_url', 'assertFalse', 'settings', 'SESSION_COOKIE_NAME', 'cookies', 'keys', 'assertTrue')
                varnames   ('self', 'payload', 'resp')
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
                name       'test_rest_session_login_sets_session_cookie'
-               firstlineno 1105
+               firstlineno 1136
                lnotab 0x020164011e0222013a0170fe2e0422013a0170fe
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
@@ -8577,30 +8818,30 @@
                   000000a6000000ab0000000000000000006401750073024a008201090064
                   0064006400a6020000ab02000000000000000001006e0b23003100730477
                   027803590077010100590001000100740700000000000000000000640164
                   036401ac02a6030000ab0300000000000000003500010074050000000000
                   0000000000a6000000ab0000000000000000006401750073024a00820109
                   00640064006400a6020000ab020000000000000000010064005300230031
                   0073047702780359007701010059000100010064005300
-               1117           0 RESUME                   0
+               1148           0 RESUME                   0
                
-               1120           2 LOAD_FAST                0 (self)
+               1151           2 LOAD_FAST                0 (self)
                               4 LOAD_METHOD              0 (assertRaises)
                              26 LOAD_GLOBAL              2 (ImproperlyConfigured)
                              38 PRECALL                  1
                              42 CALL                     1
                              52 BEFORE_WITH
                              54 POP_TOP
                
-               1121          56 LOAD_GLOBAL              5 (NULL + get_token_model)
+               1152          56 LOAD_GLOBAL              5 (NULL + get_token_model)
                              68 PRECALL                  0
                              72 CALL                     0
                              82 POP_TOP
                
-               1120          84 LOAD_CONST               0 (None)
+               1151          84 LOAD_CONST               0 (None)
                              86 LOAD_CONST               0 (None)
                              88 LOAD_CONST               0 (None)
                              90 PRECALL                  2
                              94 CALL                     2
                             104 POP_TOP
                             106 JUMP_FORWARD            11 (to 130)
                         >>  108 PUSH_EXC_INFO
@@ -8611,41 +8852,41 @@
                             118 POP_EXCEPT
                             120 RERAISE                  1
                         >>  122 POP_TOP
                             124 POP_EXCEPT
                             126 POP_TOP
                             128 POP_TOP
                
-               1124     >>  130 LOAD_GLOBAL              7 (NULL + override_api_settings)
+               1155     >>  130 LOAD_GLOBAL              7 (NULL + override_api_settings)
                             142 LOAD_CONST               1 (False)
                
-               1125         144 LOAD_CONST               1 (False)
+               1156         144 LOAD_CONST               1 (False)
                
-               1126         146 LOAD_CONST               1 (False)
+               1157         146 LOAD_CONST               1 (False)
                
-               1124         148 KW_NAMES                 2
+               1155         148 KW_NAMES                 2
                             150 PRECALL                  3
                             154 CALL                     3
                             164 BEFORE_WITH
                             166 POP_TOP
                
-               1127         168 LOAD_FAST                0 (self)
+               1158         168 LOAD_FAST                0 (self)
                             170 LOAD_METHOD              0 (assertRaises)
                             192 LOAD_GLOBAL              2 (ImproperlyConfigured)
                             204 PRECALL                  1
                             208 CALL                     1
                             218 BEFORE_WITH
                             220 POP_TOP
                
-               1128         222 LOAD_GLOBAL              5 (NULL + get_token_model)
+               1159         222 LOAD_GLOBAL              5 (NULL + get_token_model)
                             234 PRECALL                  0
                             238 CALL                     0
                             248 POP_TOP
                
-               1127         250 LOAD_CONST               0 (None)
+               1158         250 LOAD_CONST               0 (None)
                             252 LOAD_CONST               0 (None)
                             254 LOAD_CONST               0 (None)
                             256 PRECALL                  2
                             260 CALL                     2
                             270 POP_TOP
                             272 JUMP_FORWARD            11 (to 296)
                         >>  274 PUSH_EXC_INFO
@@ -8656,15 +8897,15 @@
                             284 POP_EXCEPT
                             286 RERAISE                  1
                         >>  288 POP_TOP
                             290 POP_EXCEPT
                             292 POP_TOP
                             294 POP_TOP
                
-               1124     >>  296 LOAD_CONST               0 (None)
+               1155     >>  296 LOAD_CONST               0 (None)
                             298 LOAD_CONST               0 (None)
                             300 LOAD_CONST               0 (None)
                             302 PRECALL                  2
                             306 CALL                     2
                             316 POP_TOP
                             318 JUMP_FORWARD            11 (to 342)
                         >>  320 PUSH_EXC_INFO
@@ -8675,38 +8916,38 @@
                             330 POP_EXCEPT
                             332 RERAISE                  1
                         >>  334 POP_TOP
                             336 POP_EXCEPT
                             338 POP_TOP
                             340 POP_TOP
                
-               1131     >>  342 LOAD_GLOBAL              7 (NULL + override_api_settings)
+               1162     >>  342 LOAD_GLOBAL              7 (NULL + override_api_settings)
                             354 LOAD_CONST               3 (True)
                
-               1132         356 LOAD_CONST               1 (False)
+               1163         356 LOAD_CONST               1 (False)
                
-               1133         358 LOAD_CONST               1 (False)
+               1164         358 LOAD_CONST               1 (False)
                
-               1131         360 KW_NAMES                 2
+               1162         360 KW_NAMES                 2
                             362 PRECALL                  3
                             366 CALL                     3
                             376 BEFORE_WITH
                             378 POP_TOP
                
-               1134         380 LOAD_GLOBAL              5 (NULL + get_token_model)
+               1165         380 LOAD_GLOBAL              5 (NULL + get_token_model)
                             392 PRECALL                  0
                             396 CALL                     0
                             406 LOAD_CONST               1 (False)
                             408 IS_OP                    0
                             410 POP_JUMP_FORWARD_IF_TRUE     2 (to 416)
                             412 LOAD_ASSERTION_ERROR
                             414 RAISE_VARARGS            1
                         >>  416 NOP
                
-               1131         418 LOAD_CONST               0 (None)
+               1162         418 LOAD_CONST               0 (None)
                             420 LOAD_CONST               0 (None)
                             422 LOAD_CONST               0 (None)
                             424 PRECALL                  2
                             428 CALL                     2
                             438 POP_TOP
                             440 JUMP_FORWARD            11 (to 464)
                         >>  442 PUSH_EXC_INFO
@@ -8717,38 +8958,38 @@
                             452 POP_EXCEPT
                             454 RERAISE                  1
                         >>  456 POP_TOP
                             458 POP_EXCEPT
                             460 POP_TOP
                             462 POP_TOP
                
-               1137     >>  464 LOAD_GLOBAL              7 (NULL + override_api_settings)
+               1168     >>  464 LOAD_GLOBAL              7 (NULL + override_api_settings)
                             476 LOAD_CONST               1 (False)
                
-               1138         478 LOAD_CONST               3 (True)
+               1169         478 LOAD_CONST               3 (True)
                
-               1139         480 LOAD_CONST               1 (False)
+               1170         480 LOAD_CONST               1 (False)
                
-               1137         482 KW_NAMES                 2
+               1168         482 KW_NAMES                 2
                             484 PRECALL                  3
                             488 CALL                     3
                             498 BEFORE_WITH
                             500 POP_TOP
                
-               1140         502 LOAD_GLOBAL              5 (NULL + get_token_model)
+               1171         502 LOAD_GLOBAL              5 (NULL + get_token_model)
                             514 PRECALL                  0
                             518 CALL                     0
                             528 LOAD_CONST               1 (False)
                             530 IS_OP                    0
                             532 POP_JUMP_FORWARD_IF_TRUE     2 (to 538)
                             534 LOAD_ASSERTION_ERROR
                             536 RAISE_VARARGS            1
                         >>  538 NOP
                
-               1137         540 LOAD_CONST               0 (None)
+               1168         540 LOAD_CONST               0 (None)
                             542 LOAD_CONST               0 (None)
                             544 LOAD_CONST               0 (None)
                             546 PRECALL                  2
                             550 CALL                     2
                             560 POP_TOP
                             562 LOAD_CONST               0 (None)
                             564 RETURN_VALUE
@@ -8791,19 +9032,19 @@
                   True
                names      ('assertRaises', 'ImproperlyConfigured', 'get_token_model', 'override_api_settings')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
                name       'test_misconfigured_token_model'
-               firstlineno 1117
+               firstlineno 1148
                lnotab
                   0x020336011cff2e040e01020102fe140336011cff2efd2e070e01020102
                   fe140326fd2e060e01020102fe140326fd
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'USERNAME', 'PASS', 'EMAIL', 'NEW_PASS', 'REGISTRATION_VIEW', 'REGISTRATION_DATA', 'copy', 'REGISTRATION_DATA_WITH_EMAIL', 'BASIC_USER_DATA', 'USER_DATA', 'setUp', '_generate_uid_and_token', 'override_settings', 'allauth_account_settings', 'AuthenticationMethod', 'test_login_failed_email_validation', 'test_login_failed_username_validation', 'USERNAME_EMAIL', 'test_login_failed_username_email_validation', 'test_allauth_login_with_username', 'test_allauth_login_with_email', 'override_api_settings', 'test_login_jwt', 'modify_settings', 'test_login_by_email', 'test_password_change', 'test_password_change_honors_password_validators', 'test_password_change_with_old_password', '_password_reset', 'test_password_reset_allauth', 'test_password_reset_no_allauth', 'test_password_reset_with_email_in_different_case', 'test_password_reset_with_invalid_email', 'test_password_reset_honors_password_validators', 'test_user_details', 'test_user_details_using_jwt', 'test_registration', 'test_registration_honors_password_validators', 'test_registration_with_custom_permission_class', 'test_registration_allowed_with_custom_no_password_serializer', 'test_registration_with_jwt', 'test_registration_with_session', 'test_registration_with_invalid_password', 'test_registration_with_email_verification', 'test_should_not_resend_email_verification_for_nonexistent_email', 'test_logout_on_get', 'test_logout_on_post_only', 'test_login_jwt_sets_cookie', 'test_logout_jwt_deletes_cookie', 'test_logout_jwt_deletes_cookie_refresh', 'dict', 'test_cookie_authentication', 'test_blacklisting_not_installed', 'test_blacklisting', 'test_custom_jwt_claims', 'test_custom_jwt_claims_cookie_w_authentication', 'test_wo_csrf_enforcement', 'test_csrf_wo_login_csrf_enforcement', 'test_csrf_w_login_csrf_enforcement', 'test_csrf_w_login_csrf_enforcement_2', 'test_return_expiration', 'test_refresh_cookie_name', 'test_custom_token_refresh_view', 'test_rotate_token_refresh_view', 'test_login_with_no_token_model', 'test_rest_session_login_sets_session_cookie', 'test_misconfigured_token_model')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'USERNAME', 'PASS', 'EMAIL', 'NEW_PASS', 'REGISTRATION_VIEW', 'REGISTRATION_DATA', 'copy', 'REGISTRATION_DATA_WITH_EMAIL', 'BASIC_USER_DATA', 'USER_DATA', 'setUp', '_generate_uid_and_token', 'override_settings', 'allauth_account_settings', 'AuthenticationMethod', 'test_login_failed_email_validation', 'test_login_failed_username_validation', 'USERNAME_EMAIL', 'test_login_failed_username_email_validation', 'test_allauth_login_with_username', 'test_allauth_login_with_email', 'override_api_settings', 'test_login_jwt', 'modify_settings', 'test_login_by_email', 'test_password_change', 'test_password_change_honors_password_validators', 'test_password_change_with_old_password', '_password_reset', 'test_password_reset_allauth', 'test_password_reset_no_allauth', 'test_password_reset_with_email_in_different_case', 'test_password_reset_with_invalid_email', 'test_password_reset_honors_password_validators', 'test_user_details', 'test_user_details_using_jwt', 'test_registration', 'test_registration_honors_password_validators', 'test_registration_with_custom_permission_class', 'test_registration_allowed_with_custom_no_password_serializer', 'test_registration_with_jwt', 'test_registration_with_session', 'test_registration_with_invalid_password', 'test_registration_with_email_verification', 'test_should_not_resend_email_verification_for_nonexistent_email', 'test_logout_on_get', 'test_logout_on_post_only', 'test_login_jwt_sets_cookie', 'test_logout_jwt_deletes_cookie', 'test_logout_jwt_deletes_cookie_refresh', 'dict', 'test_cookie_authentication', 'test_blacklisting_not_installed', 'test_blacklisting', 'test_custom_jwt_claims', 'test_custom_jwt_claims_cookie_w_authentication', 'test_wo_csrf_enforcement', 'test_csrf_wo_login_csrf_enforcement', 'test_csrf_w_login_csrf_enforcement', 'test_csrf_w_login_csrf_enforcement_2', 'test_return_expiration', 'test_refresh_cookie_name', 'test_custom_token_refresh_view', 'test_custom_token_refresh_view_with_http_only_cookie_and_refresh_token_rotation', 'test_rotate_token_refresh_view', 'test_login_with_no_token_model', 'test_rest_session_login_sets_session_cookie', 'test_misconfigured_token_model')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
          name       'APIBasicTests'
          firstlineno 38
          lnotab
@@ -8825,16 +9066,17 @@
             ff0eff0eff0ef90eff0eff0eff0eff0e0e021c1601160116011601040104
             0202ff02ff10ff100716011601160104ff0eff0eff0ef90eff0eff0eff0e
             ff0e0e022816011601160116010401040202ff02ff10ff10071601160116
             0104ff0eff0eff0ef90eff0eff0eff0eff0e0e0223160116011601160104
             01040202ff02ff10ff100716011601160104ff0eff0eff0ef90eff0eff0e
             ff0eff0e0e022316011601160104ff0eff0eff0e03020d16011601160116
             011601160104ff0eff0eff0eff0eff0eff0e06020e160116011601160116
-            0104ff0eff0eff0eff0eff0e0502141601160104ff0eff0e02021716011c
-            0104ff0eff0e02020a060c1c0104ff0e01
+            0104ff0eff0eff0eff0eff0e0502141601160116011601160104ff0eff0e
+            ff0eff0eff0e05021a1601160104ff0eff0e02021716011c0104ff0eff0e
+            02020a060c1c0104ff0e01
       'APIBasicTests'
    names      ('json', 'allauth.account', 'app_settings', 'allauth_account_settings', 'django.conf', 'settings', 'django.contrib.auth', 'get_user_model', 'django.core', 'mail', 'django.core.exceptions', 'ImproperlyConfigured', 'django.test', 'TestCase', 'modify_settings', 'override_settings', 'django.utils.encoding', 'force_str', 'rest_framework', 'status', 'rest_framework.test', 'APIRequestFactory', 'dj_rest_auth.app_settings', 'api_settings', 'dj_rest_auth.registration.views', 'RegisterView', 'dj_rest_auth.models', 'get_token_model', 'mixins', 'TestsMixin', 'utils', 'override_api_settings', 'django.urls', 'reverse', 'ImportError', 'django.core.urlresolvers', 'jwt', 'decode', 'decode_jwt', 'rest_framework_simplejwt.serializers', 'TokenObtainPairSerializer', 'TESTTokenObtainPairSerializer', 'APIBasicTests')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/michael/Projects/dj-rest-auth/dj_rest_auth/tests/test_api.py'
    name       '<module>'
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_serializers.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_social.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_social.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/test_utils.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/test_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/urls.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/__pycache__/utils.cpython-311.pyc` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/django_urls.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/django_urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/mixins.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/settings.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,17 +94,21 @@
     'dj_rest_auth.registration',
 
     'rest_framework_simplejwt.token_blacklist',
 ]
 
 SECRET_KEY = '38dh*skf8sjfhs287dh&^hd8&3hdg*j2&sd'
 ACCOUNT_ACTIVATION_DAYS = 1
+# With the default rate limits of allauth only one email confirmation per 180s is supported
+ACCOUNT_RATE_LIMITS = {
+    'confirm_email': None
+}
 SITE_ID = 1
 
 AUTHENTICATION_BACKENDS = (
     # Needed to login by username in Django admin, regardless of `allauth`
     'django.contrib.auth.backends.ModelBackend',
     # `allauth` specific authentication methods, such as login by e-mail
     'allauth.account.auth_backends.AuthenticationBackend',
 )
 
-REST_AUTH = {}
+REST_AUTH = {}
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/test_api.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1060,14 +1060,45 @@
             status_code=200,
         )
         self.assertIn('xxx', refresh_resp.cookies)
 
         # Ensure access keys are provided in response
         self.assertIn('access', refresh_resp.data)
         self.assertIn('access_expiration', refresh_resp.data)
+    
+    @override_api_settings(JWT_AUTH_RETURN_EXPIRATION=True)
+    @override_api_settings(USE_JWT=True)
+    @override_api_settings(JWT_AUTH_COOKIE='xxx')
+    @override_api_settings(JWT_AUTH_REFRESH_COOKIE='refresh-xxx')
+    @override_api_settings(JWT_AUTH_HTTPONLY=True)
+    def test_custom_token_refresh_view_with_http_only_cookie_and_refresh_token_rotation(self):
+        from rest_framework_simplejwt.settings import api_settings as jwt_settings
+        jwt_settings.ROTATE_REFRESH_TOKENS = True
+        payload = {
+            'username': self.USERNAME,
+            'password': self.PASS,
+        }
+        refresh_cookie_name = 'refresh-xxx'
+
+        get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
+        resp = self.post(self.login_url, data=payload, status_code=200)
+        refresh = resp.cookies[refresh_cookie_name].value
+        refresh_resp = self.post(
+            reverse('token_refresh'),
+            data=dict(refresh=refresh),
+            status_code=200,
+        )
+        self.assertIn('xxx', refresh_resp.cookies)
+
+        # Ensure access keys are provided in response
+        self.assertIn('access', refresh_resp.data)
+        self.assertIn('access_expiration', refresh_resp.data)
+        # ensure refresh token is removed from response
+        self.assertNotIn('refresh', refresh_resp.data)
+        self.assertNotIn('refresh_expiration', refresh_resp.data)
 
     @override_api_settings(USE_JWT=True)
     @override_api_settings(JWT_AUTH_HTTPONLY=False)
     def test_rotate_token_refresh_view(self):
         from rest_framework_simplejwt.settings import api_settings as jwt_settings
         jwt_settings.ROTATE_REFRESH_TOKENS = True
         payload = {
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/test_serializers.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/test_social.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/urls.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/tests/utils.py` & `dj-rest-auth-5.1.0/dj_rest_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/urls.py` & `dj-rest-auth-5.1.0/dj_rest_auth/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/utils.py` & `dj-rest-auth-5.1.0/dj_rest_auth/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth/views.py` & `dj-rest-auth-5.1.0/dj_rest_auth/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,19 @@
 
         return self.finalize_response(request, response, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         return self.logout(request)
 
     def logout(self, request):
+        if not (request.auth or api_settings.USE_JWT or api_settings.SESSION_LOGIN):
+            return Response(
+                {'detail': _('You should be logged in to logout. Check whether the token is passed.')},
+                status=status.HTTP_400_BAD_REQUEST,
+            )
         try:
             request.user.auth_token.delete()
         except (AttributeError, ObjectDoesNotExist):
             pass
 
         if api_settings.SESSION_LOGIN:
             django_logout(request)
@@ -174,19 +179,29 @@
             cookie_name = api_settings.JWT_AUTH_COOKIE
 
             unset_jwt_cookies(response)
 
             if 'rest_framework_simplejwt.token_blacklist' in settings.INSTALLED_APPS:
                 # add refresh token to blacklist
                 try:
-                    token = RefreshToken(request.data['refresh'])
+                    token: RefreshToken = RefreshToken(None)
+                    if api_settings.JWT_AUTH_HTTPONLY:
+                        try:
+                            token = RefreshToken(request.COOKIES[api_settings.JWT_AUTH_REFRESH_COOKIE])
+                        except KeyError:
+                            response.data = {'detail': _('Refresh token was not included in cookie data.')}
+                            response.status_code =status.HTTP_401_UNAUTHORIZED
+                    else:
+                        try:
+                            token = RefreshToken(request.data['refresh'])
+                        except KeyError:
+                            response.data = {'detail': _('Refresh token was not included in request data.')}
+                            response.status_code =status.HTTP_401_UNAUTHORIZED
+
                     token.blacklist()
-                except KeyError:
-                    response.data = {'detail': _('Refresh token was not included in request data.')}
-                    response.status_code =status.HTTP_401_UNAUTHORIZED
                 except (TokenError, AttributeError, TypeError) as error:
                     if hasattr(error, 'args'):
                         if 'Token is blacklisted' in error.args or 'Token is invalid or expired' in error.args:
                             response.data = {'detail': _(error.args[0])}
                             response.status_code = status.HTTP_401_UNAUTHORIZED
                         else:
                             response.data = {'detail': _('An error has occurred.')}
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth.egg-info/PKG-INFO` & `dj-rest-auth-5.1.0/dj_rest_auth.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: dj-rest-auth
-Version: 5.0.2
+Version: 5.1.0
 Summary: Authentication and Registration in Django Rest Framework
 Home-page: http://github.com/iMerica/dj-rest-auth
 Author: iMerica
 Author-email: imichael@pm.me
 License: MIT
 Keywords: django rest auth registration rest-framework django-registration api
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: with_social
 License-File: LICENSE
-Requires-Dist: Django>=3.2
-Requires-Dist: djangorestframework>=3.13.0
-Provides-Extra: with-social
-Requires-Dist: django-allauth<0.58.0,>=0.56.0; extra == "with-social"
 
 # Dj-Rest-Auth
 [![<iMerica>](https://circleci.com/gh/iMerica/dj-rest-auth.svg?style=svg)](https://app.circleci.com/pipelines/github/iMerica/dj-rest-auth)
 
 
 Drop-in API endpoints for handling authentication securely in Django Rest Framework. Works especially well 
 with SPAs (e.g., React, Vue, Angular), and Mobile applications.
```

### Comparing `dj-rest-auth-5.0.2/dj_rest_auth.egg-info/SOURCES.txt` & `dj-rest-auth-5.1.0/dj_rest_auth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 demo/templates/fragments/password_change_form.html
 demo/templates/fragments/password_reset_confirm_form.html
 demo/templates/fragments/password_reset_form.html
 demo/templates/fragments/resend_email_verification_form.html
 demo/templates/fragments/signup_form.html
 demo/templates/fragments/user_details_form.html
 demo/templates/rest_framework/api.html
-dj_rest_auth/.DS_Store
 dj_rest_auth/__init__.py
 dj_rest_auth/__version__.py
 dj_rest_auth/admin.py
 dj_rest_auth/app_settings.py
 dj_rest_auth/forms.py
 dj_rest_auth/jwt_auth.py
 dj_rest_auth/models.py
@@ -71,14 +70,15 @@
 dj_rest_auth.egg-info/PKG-INFO
 dj_rest_auth.egg-info/SOURCES.txt
 dj_rest_auth.egg-info/dependency_links.txt
 dj_rest_auth.egg-info/not-zip-safe
 dj_rest_auth.egg-info/requires.txt
 dj_rest_auth.egg-info/top_level.txt
 dj_rest_auth/__pycache__/__init__.cpython-311.pyc
+dj_rest_auth/__pycache__/__init__.cpython-312.pyc
 dj_rest_auth/__pycache__/__init__.cpython-38.pyc
 dj_rest_auth/__pycache__/admin.cpython-311.pyc
 dj_rest_auth/__pycache__/admin.cpython-38.pyc
 dj_rest_auth/__pycache__/app_settings.cpython-311.pyc
 dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
 dj_rest_auth/__pycache__/forms.cpython-311.pyc
 dj_rest_auth/__pycache__/forms.cpython-38.pyc
@@ -135,14 +135,16 @@
 dj_rest_auth/locale/ja/LC_MESSAGES/django.po
 dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
 dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
 dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
 dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
 dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
 dj_rest_auth/locale/ko/LC_MESSAGES/django.po
+dj_rest_auth/locale/ma/LC_MESSAGES/django.mo
+dj_rest_auth/locale/ma/LC_MESSAGES/django.po
 dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
 dj_rest_auth/locale/nl/LC_MESSAGES/django.po
 dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
 dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
 dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
 dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
 dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
@@ -195,20 +197,22 @@
 dj_rest_auth/tests/test_api.py
 dj_rest_auth/tests/test_serializers.py
 dj_rest_auth/tests/test_social.py
 dj_rest_auth/tests/test_utils.py
 dj_rest_auth/tests/urls.py
 dj_rest_auth/tests/utils.py
 dj_rest_auth/tests/__pycache__/__init__.cpython-311.pyc
+dj_rest_auth/tests/__pycache__/__init__.cpython-312.pyc
 dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/django_urls.cpython-311.pyc
 dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/mixins.cpython-311.pyc
 dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/settings.cpython-311.pyc
+dj_rest_auth/tests/__pycache__/settings.cpython-312.pyc
 dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/test_api.cpython-311.pyc
 dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/test_serializers.cpython-311.pyc
 dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
 dj_rest_auth/tests/__pycache__/test_social.cpython-311.pyc
 dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
```

### Comparing `dj-rest-auth-5.0.2/docs/Makefile` & `dj-rest-auth-5.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/api_endpoints.rst` & `dj-rest-auth-5.1.0/docs/api_endpoints.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/conf.py` & `dj-rest-auth-5.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/configuration.rst` & `dj-rest-auth-5.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/demo.rst` & `dj-rest-auth-5.1.0/docs/demo.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/faq.rst` & `dj-rest-auth-5.1.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/index.rst` & `dj-rest-auth-5.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/installation.rst` & `dj-rest-auth-5.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/introduction.rst` & `dj-rest-auth-5.1.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/docs/make.bat` & `dj-rest-auth-5.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/runtests.py` & `dj-rest-auth-5.1.0/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-5.0.2/setup.py` & `dj-rest-auth-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     license='MIT',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='django rest auth registration rest-framework django-registration api',
     zip_safe=False,
     install_requires=[
-        'Django>=3.2',
+        'Django>=3.2,<5.0',
         'djangorestframework>=3.13.0',
     ],
     extras_require={
-        'with_social': ['django-allauth>=0.56.0,<0.58.0'],
+        'with_social': ['django-allauth>=0.56.0,<0.62.0'],
     },
     tests_require=[
         'coveralls>=1.11.1',
         'django-allauth>=0.57.0',
         'djangorestframework-simplejwt==4.6.0',
         'responses==0.12.1',
         'unittest-xml-reporting==3.0.4',
```

### Comparing `dj-rest-auth-5.0.2/tox.ini` & `dj-rest-auth-5.1.0/tox.ini`

 * *Files identical despite different names*

