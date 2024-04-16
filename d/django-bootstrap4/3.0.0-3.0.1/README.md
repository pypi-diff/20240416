# Comparing `tmp/django-bootstrap4-3.0.0.tar.gz` & `tmp/django-bootstrap4-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap4-3.0.0.tar", last modified: Fri Apr  9 13:03:08 2021, max compression
+gzip compressed data, was "django-bootstrap4-3.0.1.tar", last modified: Sat May  1 05:04:54 2021, max compression
```

## Comparing `django-bootstrap4-3.0.0.tar` & `django-bootstrap4-3.0.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.834493 django-bootstrap4-3.0.0/
--rw-r--r--   0 dylan      (501) staff       (20)      757 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/AUTHORS
--rw-r--r--   0 dylan      (501) staff       (20)     1533 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.0/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      277 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     4089 2021-04-09 13:03:08.834328 django-bootstrap4-3.0.0/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2336 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.825194 django-bootstrap4-3.0.0/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       25 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/docs/authors.rst
--rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-17 12:32:12.000000 django-bootstrap4-3.0.0/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      914 2020-10-07 05:22:30.000000 django-bootstrap4-3.0.0/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      579 2018-06-14 04:53:49.000000 django-bootstrap4-3.0.0/docs/example_template.rst
--rw-r--r--   0 dylan      (501) staff       (20)      251 2020-06-17 12:32:12.000000 django-bootstrap4-3.0.0/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      578 2017-10-25 10:07:50.000000 django-bootstrap4-3.0.0/docs/installation.rst
--rw-r--r--   0 dylan      (501) staff       (20)      639 2021-03-15 13:31:24.000000 django-bootstrap4-3.0.0/docs/migrate.rst
--rw-r--r--   0 dylan      (501) staff       (20)      658 2020-06-17 12:44:17.000000 django-bootstrap4-3.0.0/docs/quickstart.rst
--rw-r--r--   0 dylan      (501) staff       (20)       50 2021-04-09 13:03:00.000000 django-bootstrap4-3.0.0/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)     3467 2021-03-15 13:31:24.000000 django-bootstrap4-3.0.0/docs/settings.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1308 2017-10-25 10:07:50.000000 django-bootstrap4-3.0.0/docs/templates.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2215 2019-08-07 17:49:18.000000 django-bootstrap4-3.0.0/docs/templatetags.rst
--rw-r--r--   0 dylan      (501) staff       (20)      708 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/docs/widgets.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2019-12-04 08:32:17.000000 django-bootstrap4-3.0.0/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)      646 2021-03-15 06:46:18.000000 django-bootstrap4-3.0.0/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)       38 2021-04-09 13:03:08.834545 django-bootstrap4-3.0.0/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1603 2021-04-09 12:59:52.000000 django-bootstrap4-3.0.0/setup.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.822353 django-bootstrap4-3.0.0/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.826325 django-bootstrap4-3.0.0/src/bootstrap4/
--rw-r--r--   0 dylan      (501) staff       (20)      268 2020-06-01 17:37:42.000000 django-bootstrap4-3.0.0/src/bootstrap4/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     3626 2021-03-15 13:31:24.000000 django-bootstrap4-3.0.0/src/bootstrap4/bootstrap.py
--rw-r--r--   0 dylan      (501) staff       (20)      943 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.0/src/bootstrap4/components.py
--rw-r--r--   0 dylan      (501) staff       (20)      166 2019-08-08 06:04:41.000000 django-bootstrap4-3.0.0/src/bootstrap4/exceptions.py
--rw-r--r--   0 dylan      (501) staff       (20)     4977 2020-10-29 05:40:02.000000 django-bootstrap4-3.0.0/src/bootstrap4/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)       50 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/models.py
--rw-r--r--   0 dylan      (501) staff       (20)    21814 2020-10-29 05:40:02.000000 django-bootstrap4-3.0.0/src/bootstrap4/renderers.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.822137 django-bootstrap4-3.0.0/src/bootstrap4/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.827031 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/
--rw-r--r--   0 dylan      (501) staff       (20)     1130 2019-08-08 09:21:36.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/bootstrap4.html
--rw-r--r--   0 dylan      (501) staff       (20)       95 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/field_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)       97 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/field_help_text.html
--rw-r--r--   0 dylan      (501) staff       (20)      304 2020-08-02 05:36:27.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      316 2019-08-08 09:35:46.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1549 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.827158 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/widgets/
--rw-r--r--   0 dylan      (501) staff       (20)      747 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/widgets/radio_select_button_group.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.827372 django-bootstrap4-3.0.0/src/bootstrap4/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.0/src/bootstrap4/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    23381 2021-03-15 13:31:24.000000 django-bootstrap4-3.0.0/src/bootstrap4/templatetags/bootstrap4.py
--rw-r--r--   0 dylan      (501) staff       (20)      467 2019-11-23 07:37:03.000000 django-bootstrap4-3.0.0/src/bootstrap4/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     4623 2020-10-29 05:40:02.000000 django-bootstrap4-3.0.0/src/bootstrap4/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)      314 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.0/src/bootstrap4/widgets.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.828057 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     4089 2021-04-09 13:03:08.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     3372 2021-04-09 13:03:08.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-04-09 13:03:08.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-03-15 11:14:47.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       82 2021-04-09 13:03:08.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2021-04-09 13:03:08.000000 django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.828820 django-bootstrap4-3.0.0/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2018-07-15 09:39:20.000000 django-bootstrap4-3.0.0/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.832170 django-bootstrap4-3.0.0/tests/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      140 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      144 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.0/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3049 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3053 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3037 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3037 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2286 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2290 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2234 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2334 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     5439 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4786 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4762 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4752 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    30317 2021-04-09 12:44:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    29690 2021-04-09 12:44:53.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    28943 2021-04-09 12:45:26.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    28985 2021-04-09 12:46:12.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      655 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      659 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      671 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      671 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      514 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      518 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      526 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      526 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-39.pyc
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.832605 django-bootstrap4-3.0.0/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.0/tests/app/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-04-09 13:03:08.834102 django-bootstrap4-3.0.0/tests/app/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      144 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      152 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      152 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1544 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1468 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1482 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1454 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      154 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/urls.cpython-36.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      158 2021-03-15 11:16:05.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/urls.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      162 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      162 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.0/tests/app/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1702 2020-10-07 05:22:30.000000 django-bootstrap4-3.0.0/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)       17 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.0/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     2607 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.0/tests/test_components.py
--rw-r--r--   0 dylan      (501) staff       (20)     2426 2021-03-15 09:28:10.000000 django-bootstrap4-3.0.0/tests/test_settings.py
--rw-r--r--   0 dylan      (501) staff       (20)     4810 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.0/tests/test_templates.py
--rw-r--r--   0 dylan      (501) staff       (20)    30477 2021-03-15 13:31:24.000000 django-bootstrap4-3.0.0/tests/test_templatetags.py
--rw-r--r--   0 dylan      (501) staff       (20)      297 2019-12-13 09:01:08.000000 django-bootstrap4-3.0.0/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      341 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.0/tests/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-04-09 12:59:52.000000 django-bootstrap4-3.0.0/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.304121 django-bootstrap4-3.0.1/
+-rw-r--r--   0 dylan      (501) staff       (20)      757 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/AUTHORS
+-rw-r--r--   0 dylan      (501) staff       (20)     1533 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.1/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      277 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     3963 2021-05-01 05:04:54.303930 django-bootstrap4-3.0.1/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2266 2021-04-29 11:10:10.000000 django-bootstrap4-3.0.1/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.287064 django-bootstrap4-3.0.1/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       25 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/docs/authors.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-17 12:32:12.000000 django-bootstrap4-3.0.1/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      914 2020-10-07 05:22:30.000000 django-bootstrap4-3.0.1/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)      579 2018-06-14 04:53:49.000000 django-bootstrap4-3.0.1/docs/example_template.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      251 2020-06-17 12:32:12.000000 django-bootstrap4-3.0.1/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      578 2017-10-25 10:07:50.000000 django-bootstrap4-3.0.1/docs/installation.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      663 2021-05-01 05:03:06.000000 django-bootstrap4-3.0.1/docs/migrate.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      658 2020-06-17 12:44:17.000000 django-bootstrap4-3.0.1/docs/quickstart.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       50 2021-04-29 11:10:10.000000 django-bootstrap4-3.0.1/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     3467 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/docs/settings.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1308 2017-10-25 10:07:50.000000 django-bootstrap4-3.0.1/docs/templates.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2215 2019-08-07 17:49:18.000000 django-bootstrap4-3.0.1/docs/templatetags.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      708 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/docs/widgets.rst
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2019-12-04 08:32:17.000000 django-bootstrap4-3.0.1/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)      646 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2021-05-01 05:04:54.304178 django-bootstrap4-3.0.1/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1603 2021-05-01 05:04:27.000000 django-bootstrap4-3.0.1/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.283214 django-bootstrap4-3.0.1/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.288582 django-bootstrap4-3.0.1/src/bootstrap4/
+-rw-r--r--   0 dylan      (501) staff       (20)      268 2020-06-01 17:37:42.000000 django-bootstrap4-3.0.1/src/bootstrap4/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3633 2021-04-29 11:10:10.000000 django-bootstrap4-3.0.1/src/bootstrap4/bootstrap.py
+-rw-r--r--   0 dylan      (501) staff       (20)      943 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.1/src/bootstrap4/components.py
+-rw-r--r--   0 dylan      (501) staff       (20)      166 2019-08-08 06:04:41.000000 django-bootstrap4-3.0.1/src/bootstrap4/exceptions.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4977 2020-10-29 05:40:02.000000 django-bootstrap4-3.0.1/src/bootstrap4/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)       50 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/models.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21858 2021-04-29 11:11:24.000000 django-bootstrap4-3.0.1/src/bootstrap4/renderers.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.282999 django-bootstrap4-3.0.1/src/bootstrap4/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.289600 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/
+-rw-r--r--   0 dylan      (501) staff       (20)     1130 2019-08-08 09:21:36.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/bootstrap4.html
+-rw-r--r--   0 dylan      (501) staff       (20)       95 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/field_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)       97 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/field_help_text.html
+-rw-r--r--   0 dylan      (501) staff       (20)      304 2020-08-02 05:36:27.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/form_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)      316 2019-08-08 09:35:46.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/messages.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1549 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/pagination.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.289755 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/widgets/
+-rw-r--r--   0 dylan      (501) staff       (20)      747 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/widgets/radio_select_button_group.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.290102 django-bootstrap4-3.0.1/src/bootstrap4/templatetags/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2019-08-07 15:26:14.000000 django-bootstrap4-3.0.1/src/bootstrap4/templatetags/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    23619 2021-04-29 11:10:10.000000 django-bootstrap4-3.0.1/src/bootstrap4/templatetags/bootstrap4.py
+-rw-r--r--   0 dylan      (501) staff       (20)      467 2019-11-23 07:37:03.000000 django-bootstrap4-3.0.1/src/bootstrap4/text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4623 2020-10-29 05:40:02.000000 django-bootstrap4-3.0.1/src/bootstrap4/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)      314 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.1/src/bootstrap4/widgets.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.290973 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     3963 2021-05-01 05:04:54.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     3372 2021-05-01 05:04:54.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2021-05-01 05:04:54.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2021-03-15 11:14:47.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)       82 2021-05-01 05:04:54.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2021-05-01 05:04:54.000000 django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.292540 django-bootstrap4-3.0.1/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2018-07-15 09:39:20.000000 django-bootstrap4-3.0.1/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.300174 django-bootstrap4-3.0.1/tests/__pycache__/
+-rw-r--r--   0 dylan      (501) staff       (20)      140 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      144 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.1/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     3049 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     3053 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     3037 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     3037 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     2286 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     2290 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     2234 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     2334 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     5439 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     4786 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     4762 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     4752 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)    30317 2021-04-09 12:44:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)    29690 2021-04-09 12:44:53.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)    28943 2021-04-09 12:45:26.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)    28985 2021-04-09 12:46:12.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      655 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      659 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      671 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      671 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      514 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      518 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      526 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      526 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-39.pyc
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.300758 django-bootstrap4-3.0.1/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.1/tests/app/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2021-05-01 05:04:54.303582 django-bootstrap4-3.0.1/tests/app/__pycache__/
+-rw-r--r--   0 dylan      (501) staff       (20)      144 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      148 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      152 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      152 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     1544 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     1468 2021-03-15 11:16:04.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     1482 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     1454 2021-03-15 11:17:15.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      154 2021-03-15 11:15:31.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/urls.cpython-36.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      158 2021-03-15 11:16:05.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/urls.cpython-37.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      162 2021-03-15 11:16:36.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)      162 2021-03-15 11:17:16.000000 django-bootstrap4-3.0.1/tests/app/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 dylan      (501) staff       (20)     1702 2020-10-07 05:22:30.000000 django-bootstrap4-3.0.1/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)       17 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.1/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2607 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.1/tests/test_components.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2426 2021-03-15 09:28:10.000000 django-bootstrap4-3.0.1/tests/test_settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4810 2020-06-30 11:49:35.000000 django-bootstrap4-3.0.1/tests/test_templates.py
+-rw-r--r--   0 dylan      (501) staff       (20)    30477 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/tests/test_templatetags.py
+-rw-r--r--   0 dylan      (501) staff       (20)      297 2019-12-13 09:01:08.000000 django-bootstrap4-3.0.1/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)      341 2019-12-09 05:40:27.000000 django-bootstrap4-3.0.1/tests/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-04-29 11:06:34.000000 django-bootstrap4-3.0.1/tox.ini
```

### Comparing `django-bootstrap4-3.0.0/AUTHORS` & `django-bootstrap4-3.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/LICENSE` & `django-bootstrap4-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/PKG-INFO` & `django-bootstrap4-3.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap4
-Version: 3.0.0
+Version: 3.0.1
 Summary: Bootstrap 4 for Django
 Home-page: https://github.com/zostera/django-bootstrap4
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Description: # django-bootstrap 4
         
@@ -27,70 +27,63 @@
         
         The full documentation is at https://django-bootstrap4.readthedocs.io/
         
         ## Installation
         
         1. Install using pip:
         
-            ```shell script
-            pip install django-bootstrap4
-            ```
+        ```bash
+        pip install django-bootstrap4
+        ```
            
            Alternatively, you can install download or clone this repo and call ``pip install -e .``.
         
         2. Add to `INSTALLED_APPS` in your `settings.py`:
         
-           ```python
-           INSTALLED_APPS = (
-               # ...
-               "bootstrap4",
-               # ...
-           )
-           ````
+        ```python
+        INSTALLED_APPS = (
+          # ...
+          "bootstrap4",
+          # ...
+        )
+        ```
         
-        3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags:
+        3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags. See example below.
         
         ## Example template
         
-        ```djangotemplate
+        ```jinja
         {% load bootstrap4 %}
         
         {# Display a form #}
         
         <form action="/url/to/submit/" method="post" class="form">
             {% csrf_token %}
             {% bootstrap_form form %}
             {% buttons %}
                 <button type="submit" class="btn btn-primary">Submit</button>
             {% endbuttons %}
         </form>
         ```
         
-        Demo
-        ----
+        ## Demo
         
         A demo app is provided in `demo`. You can run it from your virtualenv with `python manage.py runserver`.
         
-        
-        Bugs and suggestions
-        --------------------
+        ## Bugs and suggestions
         
         If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.
         
         https://github.com/zostera/django-bootstrap4/issues
         
-        
-        License
-        -------
+        ## License
         
         You can use this under BSD-3-Clause. See [LICENSE](LICENSE) file for details.
         
-        
-        Author
-        ------
+        ## Author
         
         Developed and maintained by [Zostera](https://zostera.nl).
         
         Original author: [Dylan Verheul](https://github.com/dyve).
         
         Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.
```

### Comparing `django-bootstrap4-3.0.0/README.md` & `django-bootstrap4-3.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -19,70 +19,63 @@
 
 The full documentation is at https://django-bootstrap4.readthedocs.io/
 
 ## Installation
 
 1. Install using pip:
 
-    ```shell script
-    pip install django-bootstrap4
-    ```
+```bash
+pip install django-bootstrap4
+```
    
    Alternatively, you can install download or clone this repo and call ``pip install -e .``.
 
 2. Add to `INSTALLED_APPS` in your `settings.py`:
 
-   ```python
-   INSTALLED_APPS = (
-       # ...
-       "bootstrap4",
-       # ...
-   )
-   ````
+```python
+INSTALLED_APPS = (
+  # ...
+  "bootstrap4",
+  # ...
+)
+```
 
-3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags:
+3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags. See example below.
 
 ## Example template
 
-```djangotemplate
+```jinja
 {% load bootstrap4 %}
 
 {# Display a form #}
 
 <form action="/url/to/submit/" method="post" class="form">
     {% csrf_token %}
     {% bootstrap_form form %}
     {% buttons %}
         <button type="submit" class="btn btn-primary">Submit</button>
     {% endbuttons %}
 </form>
 ```
 
-Demo
-----
+## Demo
 
 A demo app is provided in `demo`. You can run it from your virtualenv with `python manage.py runserver`.
 
-
-Bugs and suggestions
---------------------
+## Bugs and suggestions
 
 If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.
 
 https://github.com/zostera/django-bootstrap4/issues
 
-
-License
--------
+## License
 
 You can use this under BSD-3-Clause. See [LICENSE](LICENSE) file for details.
 
-
-Author
-------
+## Author
 
 Developed and maintained by [Zostera](https://zostera.nl).
 
 Original author: [Dylan Verheul](https://github.com/dyve).
 
 Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.
```

### Comparing `django-bootstrap4-3.0.0/docs/conf.py` & `django-bootstrap4-3.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/example_template.rst` & `django-bootstrap4-3.0.1/docs/example_template.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/installation.rst` & `django-bootstrap4-3.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/migrate.rst` & `django-bootstrap4-3.0.1/docs/migrate.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 =========
 Migration
 =========
 
-Below is a list of caveats when migrating from Bootstrap3/django-bootstrap3 to Bootstrap4/django-bootstrap4.
+Below is a list of warnings when migrating from Bootstrap 3/django-bootstrap3 to Bootstrap 4/django-bootstrap4.
 
 This document only considers the differences between django-bootstrap3 and django-bootstrap4. For the migration
 guide from Bootstrap 3 to 4, please look at the Bootstrap docs, especially the `Migration section <https://getbootstrap.com/docs/4.6/migration/>`_.
 
 Icons
 -----
 
-Bootstrap 4 does not ship with an icon set, so everything regarding to icons has been removed.
+Bootstrap 4 does not ship with an icon set, so everything regarding icons has been removed.
 
-If you need easy access to icons that are compatible with Bootstrap 4, please consider
-https://github.com/zostera/django-icons.
+If you need easy access to icons that are compatible with Bootstrap 4, please consider using `django-icons <https://github.com/zostera/django-icons>`_.
```

### Comparing `django-bootstrap4-3.0.0/docs/quickstart.rst` & `django-bootstrap4-3.0.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/settings.rst` & `django-bootstrap4-3.0.1/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/templates.rst` & `django-bootstrap4-3.0.1/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/templatetags.rst` & `django-bootstrap4-3.0.1/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/docs/widgets.rst` & `django-bootstrap4-3.0.1/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/pyproject.toml` & `django-bootstrap4-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/setup.py` & `django-bootstrap4-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 
 # This call to setup() does all the work
 setup(
     name="django-bootstrap4",
     zip_safe=False,
-    version="3.0.0",
+    version="3.0.1",
     description="Bootstrap 4 for Django",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/zostera/django-bootstrap4",
     author="Dylan Verheul",
     author_email="dylan@dyve.net",
     license="BSD-3-Clause",
```

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/bootstrap.py` & `django-bootstrap4-3.0.1/src/bootstrap4/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 BOOTSTRAP4_DEFAULTS = {
     "css_url": {
         "href": "https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.min.css",
         "integrity": "sha384-B0vP5xmATw1+K9KRQjQERJvTumQW0nPEzvF6L/Z6nronJ3oUOFUFpCjEUQouq2+l",
         "crossorigin": "anonymous",
     },
     "javascript_url": {
-        "url": "https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.min.js",
-        "integrity": "sha384-+YQ4JLhjyBLPDQt//I+STsc9iw4uQqACwlvpslubQzn4u2UU2UFM80nGisd026JF",
+        "url": "https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.bundle.min.js",
+        "integrity": "sha384-Piv4xVNRyMGpqkS2by6br4gNJ7DXjqk09RmUpJ8jgGtD7zP9yug3goQfGII0yAns",
         "crossorigin": "anonymous",
     },
     "theme_url": None,
     "jquery_url": {
         "url": "https://code.jquery.com/jquery-3.5.1.min.js",
         "integrity": "sha384-ZvpUoO/+PpLXR1lu4jmpXWu80pZlYUAfxl5NsBMWOEPSjUn/6Z/hRTt8+pR6L4N2",
         "crossorigin": "anonymous",
```

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/components.py` & `django-bootstrap4-3.0.1/src/bootstrap4/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/forms.py` & `django-bootstrap4-3.0.1/src/bootstrap4/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/renderers.py` & `django-bootstrap4-3.0.1/src/bootstrap4/renderers.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,16 @@
         div1 = '<div class="col-4">'
         div2 = "</div>"
         html = html.replace("<select", div1 + "<select")
         html = html.replace("</select>", "</select>" + div2)
         return '<div class="row bootstrap4-multi-input">{html}</div>'.format(html=html)
 
     def fix_file_input_label(self, html):
-        html = "<br>" + html
+        if self.layout != "horizontal":
+            html = "<br>" + html
         return html
 
     def post_widget_render(self, html):
         if isinstance(self.widget, RadioSelect):
             html = self.list_to_class(html, "radio radio-success")
         elif isinstance(self.widget, CheckboxSelectMultiple):
             html = self.list_to_class(html, "checkbox")
```

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/bootstrap4.html` & `django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/pagination.html` & `django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/templates/bootstrap4/widgets/radio_select_button_group.html` & `django-bootstrap4-3.0.1/src/bootstrap4/templates/bootstrap4/widgets/radio_select_button_group.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/templatetags/bootstrap4.py` & `django-bootstrap4-3.0.1/src/bootstrap4/templatetags/bootstrap4.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,14 +870,21 @@
     **Usage**::
 
         {% bootstrap_pagination page %}
 
     **Example**::
 
         {% bootstrap_pagination lines url="/pagination?page=1" size="large" %}
+
+    **Tip**::
+
+      If you want to repeat the query string arguments in subsequent pagination links,
+      use the "extra" parameter with "request.GET.urlencode":
+
+        {% bootstrap_pagination page_obj extra=request.GET.urlencode %}
     """
     pagination_kwargs = kwargs.copy()
     pagination_kwargs["page"] = page
     return get_pagination_context(**pagination_kwargs)
 
 
 @register.simple_tag
```

### Comparing `django-bootstrap4-3.0.0/src/bootstrap4/utils.py` & `django-bootstrap4-3.0.1/src/bootstrap4/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/PKG-INFO` & `django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap4
-Version: 3.0.0
+Version: 3.0.1
 Summary: Bootstrap 4 for Django
 Home-page: https://github.com/zostera/django-bootstrap4
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Description: # django-bootstrap 4
         
@@ -27,70 +27,63 @@
         
         The full documentation is at https://django-bootstrap4.readthedocs.io/
         
         ## Installation
         
         1. Install using pip:
         
-            ```shell script
-            pip install django-bootstrap4
-            ```
+        ```bash
+        pip install django-bootstrap4
+        ```
            
            Alternatively, you can install download or clone this repo and call ``pip install -e .``.
         
         2. Add to `INSTALLED_APPS` in your `settings.py`:
         
-           ```python
-           INSTALLED_APPS = (
-               # ...
-               "bootstrap4",
-               # ...
-           )
-           ````
+        ```python
+        INSTALLED_APPS = (
+          # ...
+          "bootstrap4",
+          # ...
+        )
+        ```
         
-        3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags:
+        3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags. See example below.
         
         ## Example template
         
-        ```djangotemplate
+        ```jinja
         {% load bootstrap4 %}
         
         {# Display a form #}
         
         <form action="/url/to/submit/" method="post" class="form">
             {% csrf_token %}
             {% bootstrap_form form %}
             {% buttons %}
                 <button type="submit" class="btn btn-primary">Submit</button>
             {% endbuttons %}
         </form>
         ```
         
-        Demo
-        ----
+        ## Demo
         
         A demo app is provided in `demo`. You can run it from your virtualenv with `python manage.py runserver`.
         
-        
-        Bugs and suggestions
-        --------------------
+        ## Bugs and suggestions
         
         If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.
         
         https://github.com/zostera/django-bootstrap4/issues
         
-        
-        License
-        -------
+        ## License
         
         You can use this under BSD-3-Clause. See [LICENSE](LICENSE) file for details.
         
-        
-        Author
-        ------
+        ## Author
         
         Developed and maintained by [Zostera](https://zostera.nl).
         
         Original author: [Dylan Verheul](https://github.com/dyve).
         
         Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.
```

### Comparing `django-bootstrap4-3.0.0/src/django_bootstrap4.egg-info/SOURCES.txt` & `django-bootstrap4-3.0.1/src/django_bootstrap4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_components.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_settings.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templates.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_templatetags.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_templatetags.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/test_version.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/test_version.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/__pycache__/utils.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-36.pyc` & `django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-37.pyc` & `django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-38.pyc` & `django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/app/__pycache__/settings.cpython-39.pyc` & `django-bootstrap4-3.0.1/tests/app/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/app/settings.py` & `django-bootstrap4-3.0.1/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/test_components.py` & `django-bootstrap4-3.0.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/test_settings.py` & `django-bootstrap4-3.0.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/test_templates.py` & `django-bootstrap4-3.0.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tests/test_templatetags.py` & `django-bootstrap4-3.0.1/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap4-3.0.0/tox.ini` & `django-bootstrap4-3.0.1/tox.ini`

 * *Files identical despite different names*

