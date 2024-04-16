# Comparing `tmp/django-composed-configuration-0.8.5.tar.gz` & `tmp/django-composed-configuration-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/django-composed-configuration/django-composed-configuration/.tox/release/tmp/tmpyas6uy17/django-composed-conf", last modified: Mon Dec 14 14:31:56 2020, max compression
+gzip compressed data, was "/home/runner/work/django-composed-configuration/django-composed-configuration/.tox/release/tmp/tmplhd2l445/django-composed-conf", last modified: Tue Dec 15 21:37:45 2020, max compression
```

## Comparing `django-composed-configuration-0.8.5.tar` & `django-composed-configuration-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.671893 django-composed-configuration-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.671893 django-composed-configuration-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      530 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (116)      674 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1799 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       54 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1315 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      218 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.675893 django-composed-configuration-0.8.5/composed_configuration/
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_allauth.py
--rw-r--r--   0 runner    (1001) docker     (116)     1439 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_celery.py
--rw-r--r--   0 runner    (1001) docker     (116)     3242 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_cors.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     1271 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_debug.py
--rw-r--r--   0 runner    (1001) docker     (116)     2950 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_django.py
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_email.py
--rw-r--r--   0 runner    (1001) docker     (116)      424 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (116)      376 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_https.py
--rw-r--r--   0 runner    (1001) docker     (116)     2577 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_logging.py
--rw-r--r--   0 runner    (1001) docker     (116)     1299 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_sentry.py
--rw-r--r--   0 runner    (1001) docker     (116)     2752 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_static.py
--rw-r--r--   0 runner    (1001) docker     (116)     2363 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.675893 django-composed-configuration-0.8.5/composed_configuration/authentication/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      272 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/adapter.py
--rw-r--r--   0 runner    (1001) docker     (116)      193 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.671893 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/account_inactive.html
--rw-r--r--   0 runner    (1001) docker     (116)      925 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/base.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/
--rw-r--r--   0 runner    (1001) docker     (116)      342 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/base_message.txt
--rw-r--r--   0 runner    (1001) docker     (116)      484 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/email_confirmation_signup_message.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/email_confirmation_signup_subject.txt
--rw-r--r--   0 runner    (1001) docker     (116)      127 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 runner    (1001) docker     (116)      530 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0 runner    (1001) docker     (116)      114 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email.html
--rw-r--r--   0 runner    (1001) docker     (116)      927 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email_confirm.html
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/login.html
--rw-r--r--   0 runner    (1001) docker     (116)      518 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/logout.html
--rw-r--r--   0 runner    (1001) docker     (116)      436 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_change.html
--rw-r--r--   0 runner    (1001) docker     (116)      805 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset.html
--rw-r--r--   0 runner    (1001) docker     (116)      474 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset_done.html
--rw-r--r--   0 runner    (1001) docker     (116)      942 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset_from_key.html
--rw-r--r--   0 runner    (1001) docker     (116)      251 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset_from_key_done.html
--rw-r--r--   0 runner    (1001) docker     (116)      421 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_set.html
--rw-r--r--   0 runner    (1001) docker     (116)      634 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/signup.html
--rw-r--r--   0 runner    (1001) docker     (116)      264 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/signup_closed.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/snippets/
--rw-r--r--   0 runner    (1001) docker     (116)      204 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/snippets/already_logged_in.html
--rw-r--r--   0 runner    (1001) docker     (116)      437 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/verification_sent.html
--rw-r--r--   0 runner    (1001) docker     (116)      797 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/verified_email_required.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/composed_configuration/sentry/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/composed_configuration/sentry/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1315 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3257 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       48 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-14 14:31:56.000000 django-composed-configuration-0.8.5/django_composed_configuration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)      515 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-14 14:31:56.679893 django-composed-configuration-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1537 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1180 2020-12-14 14:31:36.000000 django-composed-configuration-0.8.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.039937 django-composed-configuration-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.027937 django-composed-configuration-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.031937 django-composed-configuration-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      530 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      674 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1799 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1365 2020-12-15 21:37:45.039937 django-composed-configuration-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.035937 django-composed-configuration-0.9.0/composed_configuration/
+-rw-r--r--   0 runner    (1001) docker     (116)     1607 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2299 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_allauth.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1439 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2171 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_celery.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3242 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1392 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_cors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1746 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_database.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1271 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2950 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_django.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1671 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_email.py
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      644 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_https.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2577 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2723 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2752 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_static.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2363 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.035937 django-composed-configuration-0.9.0/composed_configuration/authentication/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      193 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.027937 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.035937 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/account_inactive.html
+-rw-r--r--   0 runner    (1001) docker     (116)      925 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/base.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.035937 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/
+-rw-r--r--   0 runner    (1001) docker     (116)      342 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/base_message.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      484 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/email_confirmation_signup_message.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/email_confirmation_signup_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      530 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email.html
+-rw-r--r--   0 runner    (1001) docker     (116)      927 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1409 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/login.html
+-rw-r--r--   0 runner    (1001) docker     (116)      518 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/logout.html
+-rw-r--r--   0 runner    (1001) docker     (116)      436 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_change.html
+-rw-r--r--   0 runner    (1001) docker     (116)      805 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset.html
+-rw-r--r--   0 runner    (1001) docker     (116)      474 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset_done.html
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset_from_key.html
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0 runner    (1001) docker     (116)      421 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_set.html
+-rw-r--r--   0 runner    (1001) docker     (116)      634 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/signup.html
+-rw-r--r--   0 runner    (1001) docker     (116)      264 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/signup_closed.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.035937 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/snippets/
+-rw-r--r--   0 runner    (1001) docker     (116)      204 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/snippets/already_logged_in.html
+-rw-r--r--   0 runner    (1001) docker     (116)      437 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/verification_sent.html
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/verified_email_required.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.039937 django-composed-configuration-0.9.0/composed_configuration/sentry/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1252 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/composed_configuration/sentry/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 21:37:45.039937 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1365 2020-12-15 21:37:44.000000 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3205 2020-12-15 21:37:45.000000 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-15 21:37:44.000000 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2020-12-15 21:37:44.000000 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-15 21:37:44.000000 django-composed-configuration-0.9.0/django_composed_configuration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (116)      515 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-15 21:37:45.039937 django-composed-configuration-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1575 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1180 2020-12-15 21:37:25.000000 django-composed-configuration-0.9.0/tox.ini
```

### Comparing `django-composed-configuration-0.8.5/.github/workflows/ci.yml` & `django-composed-configuration-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/.github/workflows/release.yml` & `django-composed-configuration-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/.gitignore` & `django-composed-configuration-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/LICENSE` & `django-composed-configuration-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/PKG-INFO` & `django-composed-configuration-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-composed-configuration
-Version: 0.8.5
+Version: 0.9.0
 Summary: Turnkey Django settings for data management applications
 Home-page: https://github.com/girder/django-composed-configuration
 Author: Kitware, Inc
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/girder/django-composed-configuration/issues
 Project-URL: Source, https://github.com/girder/django-composed-configuration
@@ -20,10 +20,11 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `django-composed-configuration-0.8.5/composed_configuration/__init__.py` & `django-composed-configuration-0.9.0/composed_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_allauth.py` & `django-composed-configuration-0.9.0/composed_configuration/_allauth.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_base.py` & `django-composed-configuration-0.9.0/composed_configuration/_base.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_celery.py` & `django-composed-configuration-0.9.0/composed_configuration/_celery.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_configuration.py` & `django-composed-configuration-0.9.0/composed_configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_cors.py` & `django-composed-configuration-0.9.0/composed_configuration/_cors.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_database.py` & `django-composed-configuration-0.9.0/composed_configuration/_database.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_debug.py` & `django-composed-configuration-0.9.0/composed_configuration/_debug.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_django.py` & `django-composed-configuration-0.9.0/composed_configuration/_django.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_email.py` & `django-composed-configuration-0.9.0/composed_configuration/_email.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_https.py` & `django-composed-configuration-0.9.0/composed_configuration/_https.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_logging.py` & `django-composed-configuration-0.9.0/composed_configuration/_logging.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_sentry.py` & `django-composed-configuration-0.9.0/composed_configuration/_sentry.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_static.py` & `django-composed-configuration-0.9.0/composed_configuration/_static.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/_storage.py` & `django-composed-configuration-0.9.0/composed_configuration/_storage.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/base.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email/password_reset_key_message.txt` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/email_confirm.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/login.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/logout.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/password_reset_from_key.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/signup.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/authentication/templates/account/verified_email_required.html` & `django-composed-configuration-0.9.0/composed_configuration/authentication/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/composed_configuration/sentry/apps.py` & `django-composed-configuration-0.9.0/composed_configuration/sentry/apps.py`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/django_composed_configuration.egg-info/PKG-INFO` & `django-composed-configuration-0.9.0/django_composed_configuration.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-composed-configuration
-Version: 0.8.5
+Version: 0.9.0
 Summary: Turnkey Django settings for data management applications
 Home-page: https://github.com/girder/django-composed-configuration
 Author: Kitware, Inc
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/girder/django-composed-configuration/issues
 Project-URL: Source, https://github.com/girder/django-composed-configuration
@@ -20,10 +20,11 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `django-composed-configuration-0.8.5/django_composed_configuration.egg-info/SOURCES.txt` & `django-composed-configuration-0.9.0/django_composed_configuration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,10 +54,9 @@
 composed_configuration/authentication/templates/account/email/password_reset_key_subject.txt
 composed_configuration/authentication/templates/account/snippets/already_logged_in.html
 composed_configuration/sentry/__init__.py
 composed_configuration/sentry/apps.py
 django_composed_configuration.egg-info/PKG-INFO
 django_composed_configuration.egg-info/SOURCES.txt
 django_composed_configuration.egg-info/dependency_links.txt
-django_composed_configuration.egg-info/not-zip-safe
 django_composed_configuration.egg-info/requires.txt
 django_composed_configuration.egg-info/top_level.txt
```

### Comparing `django-composed-configuration-0.8.5/pyproject.toml` & `django-composed-configuration-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-composed-configuration-0.8.5/setup.py` & `django-composed-configuration-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,19 @@
         'Framework :: Django :: 3.0',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python',
     ],
     python_requires='>=3.8',
-    install_requires=['django>=3', 'django-configurations[database,email]'],
+    install_requires=[
+        'django>=3',
+        'django-configurations[database,email]',
+        'django-oauth-toolkit==1.3.2',
+    ],
     packages=find_packages(),
     include_package_data=True,
-    # Django templates cannot be streamed from a ZIP
-    zip_safe=False,
 )
```

### Comparing `django-composed-configuration-0.8.5/tox.ini` & `django-composed-configuration-0.9.0/tox.ini`

 * *Files identical despite different names*

