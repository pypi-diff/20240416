# Comparing `tmp/django-glue-0.5.2.2.tar.gz` & `tmp/django_glue-0.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.5.2.2.tar", last modified: Fri Mar 22 15:42:33 2024, max compression
+gzip compressed data, was "django_glue-0.5.2.3.tar", last modified: Tue Apr 16 20:58:45 2024, max compression
```

## Comparing `django-glue-0.5.2.2.tar` & `django_glue-0.5.2.3.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.725470 django-glue-0.5.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-22 15:42:33.725470 django-glue-0.5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.717470 django-glue-0.5.2.2/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.717470 django-glue-0.5.2.2/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.717470 django-glue-0.5.2.2/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.713470 django-glue-0.5.2.2/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.713470 django-glue-0.5.2.2/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_function.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.713470 django-glue-0.5.2.2/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-22 15:42:33.000000 django-glue-0.5.2.2/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-22 15:42:33.725470 django-glue-0.5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:33.721470 django-glue-0.5.2.2/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-22 15:42:26.000000 django-glue-0.5.2.2/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.663000 django_glue-0.5.2.3/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.663000 django_glue-0.5.2.3/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.655000 django_glue-0.5.2.3/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_function.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 20:58:45.671000 django_glue-0.5.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/wsgi.py
```

### Comparing `django-glue-0.5.2.2/CHANGELOG.md` & `django_glue-0.5.2.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog for Django Glue
 
+## 0.5.2.3
+
+### Changes
+- Glue model object returns a null object if we try to find a id that does not exist.
+- Updated html attributes on glue model objects and added attributes to js model objects. 
+
+
 ## 0.5.2.2
 
 ### Changes
 - Render functions on the GlueView object now await the response
 
 ## 0.5.2.1
```

### Comparing `django-glue-0.5.2.2/LICENSE.md` & `django_glue-0.5.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/PKG-INFO` & `django_glue-0.5.2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,45 +22,53 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 License-File: LICENSE.md
 Requires-Dist: django>=3.2
 
 # django-glue
-
 We built Django Glue to help solve the problem of fluid interactions between the front and back ends of a Django application.
 Our end goal is to bring as much front end power to the Django framework as possible while remaining pythonic.
 
 This project is in prototype phase please look at the tests directory of this code base for examples and instructions.
 
 ## Why?
-
 We are active web platform developers that want to provide our clients with the best user experience without having to learn a bunch of different technology stacks.
 Django glue allows us to do fancy javascript like page interactions and updates while remaining in the comfort of our django/python world.
 
 Education is also a big part of what we do and our focus is on teaching our people python, so they can focus on data science and automation and make solid interfaces! 
 
-## Requirements
+## Inspiration
+We are inspired by how quickly django's model structure, ORM and forms (crispy forms) allow you to create functional web applications.
+Can we build on top of 25+ years of development to create a front end tool that uses the power of django.
+
+## Forms
+
 
+## Requirements
 - Django 3.2+ or 4.0+
 - Python 3.8+
 
 ## Dependencies
-
 - Alpine JS
+- Bootstrap 5
 - Axios
 
 ## Documentation
-
 - Installation Guide - [Here](INSTALLATION.md)
 - Usage Guide - [Here](USAGE.md)
 
 ## Roadmap
+### April 2024
+- [ ] Review project architecture for dependency flow and extendability
+- [ ] Includes for Alpine Js & Bootstrap
+- [ ] Basic form field elements
 
-- [x] Prototype (2022-07-12)
-- [x] Alpha (2022-08-31)
-- [ ] Beta (2023-06-31)
 
-## Authors
+### May 2024
+- [ ] Working with form fields that are not glued
+- [ ] Creating your own form elements
 
+## Authors
 - Nathan Johnson
 - Wesley Howery
+- Austin Sauer
```

### Comparing `django-glue-0.5.2.2/README.md` & `django_glue-0.5.2.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # django-glue
-
 We built Django Glue to help solve the problem of fluid interactions between the front and back ends of a Django application.
 Our end goal is to bring as much front end power to the Django framework as possible while remaining pythonic.
 
 This project is in prototype phase please look at the tests directory of this code base for examples and instructions.
 
 ## Why?
-
 We are active web platform developers that want to provide our clients with the best user experience without having to learn a bunch of different technology stacks.
 Django glue allows us to do fancy javascript like page interactions and updates while remaining in the comfort of our django/python world.
 
 Education is also a big part of what we do and our focus is on teaching our people python, so they can focus on data science and automation and make solid interfaces! 
 
-## Requirements
+## Inspiration
+We are inspired by how quickly django's model structure, ORM and forms (crispy forms) allow you to create functional web applications.
+Can we build on top of 25+ years of development to create a front end tool that uses the power of django.
+
+## Forms
+
 
+## Requirements
 - Django 3.2+ or 4.0+
 - Python 3.8+
 
 ## Dependencies
-
 - Alpine JS
+- Bootstrap 5
 - Axios
 
 ## Documentation
-
 - Installation Guide - [Here](INSTALLATION.md)
 - Usage Guide - [Here](USAGE.md)
 
 ## Roadmap
+### April 2024
+- [ ] Review project architecture for dependency flow and extendability
+- [ ] Includes for Alpine Js & Bootstrap
+- [ ] Basic form field elements
 
-- [x] Prototype (2022-07-12)
-- [x] Alpha (2022-08-31)
-- [ ] Beta (2023-06-31)
 
-## Authors
+### May 2024
+- [ ] Working with form fields that are not glued
+- [ ] Creating your own form elements
 
+## Authors
 - Nathan Johnson
-- Wesley Howery
+- Wesley Howery
+- Austin Sauer
```

### Comparing `django-glue-0.5.2.2/django_glue/context_processors.py` & `django_glue-0.5.2.3/django_glue/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/core/decorators.py` & `django_glue-0.5.2.3/django_glue/core/decorators.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/data_classes.py` & `django_glue-0.5.2.3/django_glue/data_classes.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/enums.py` & `django_glue-0.5.2.3/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/glue.py` & `django_glue-0.5.2.3/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/handlers.py` & `django_glue-0.5.2.3/django_glue/handlers.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/middleware.py` & `django_glue-0.5.2.3/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/responses.py` & `django_glue-0.5.2.3/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/services/functions.py` & `django_glue-0.5.2.3/django_glue/services/functions.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/services/model_objects.py` & `django_glue-0.5.2.3/django_glue/services/model_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     def __init__(self, meta_data: GlueMetaData) -> None:
         self.meta_data = meta_data
         self.model_class = None
         self.object: Optional[Model] = None
 
     def load_object(self):
         self.load_model_class()
-        self.object = self.model_class.objects.get(pk=self.meta_data.object_pk)
+        try:
+            self.object = self.model_class.objects.get(pk=self.meta_data.object_pk)
+        except self.model_class.DoesNotExist:
+            self.object = self.model_class()
 
     def load_model_class(self):
         self.model_class = ContentType.objects.get_by_natural_key(
             self.meta_data.app_label,
             self.meta_data.model
         ).model_class()
 
@@ -32,14 +35,16 @@
 
         json_data.simple_fields = generate_simple_field_dict(
             self.object,
             self.meta_data.fields,
             self.meta_data.exclude,
         )
 
+        json_data.fields = generate_field_dict(self.object, self.meta_data.fields, self.meta_data.exclude)
+
         return generate_json_200_response_data(
             'THE GET ACTION',
             'this is a response from an model object get action!!! stay tuned!',
             json_data,
         )
 
     def process_update_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
```

### Comparing `django-glue-0.5.2.2/django_glue/services/query_sets.py` & `django_glue-0.5.2.3/django_glue/services/query_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,23 @@
             for model_object in self.query_set.filter(**body_data['data']['filter_params']):
                 data.append(GlueJsonData(simple_fields=generate_simple_field_dict(
                         model_object, self.meta_data.fields, self.meta_data.exclude)))
 
         elif 'all' in body_data['data']:
             data = []
             for model_object in self.query_set.all():
-                data.append(GlueJsonData(simple_fields=generate_simple_field_dict(
-                        model_object, self.meta_data.fields, self.meta_data.exclude)))
+                data.append(GlueJsonData(
+                    simple_fields=generate_simple_field_dict(model_object, self.meta_data.fields, self.meta_data.exclude)
+                ))
 
         else:
             model_object = self.query_set.get(id=body_data['data']['id'])
-            data = GlueJsonData(simple_fields=generate_simple_field_dict(
-                model_object, self.meta_data.fields, self.meta_data.exclude))
+            data = GlueJsonData(
+                simple_fields=generate_simple_field_dict(model_object, self.meta_data.fields, self.meta_data.exclude)
+            )
 
         return generate_json_200_response_data(
             'THE QUERY GET ACTION',
             'this is a response from an query set get action',
             data
         )
```

### Comparing `django-glue-0.5.2.2/django_glue/services/services.py` & `django_glue-0.5.2.3/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/services/templates.py` & `django_glue-0.5.2.3/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/sessions.py` & `django_glue-0.5.2.3/django_glue/sessions.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_ajax.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_event.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_event.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_function.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_function.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_model_object.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 class GlueModelObject {
     constructor(glue_unique_name) {
         // Needs to be named glue_unique_name to avoid overriding the unique_name property
         this.glue_unique_name = encodeUniqueName(glue_unique_name)
-
+        this['fields'] = {}
         for (let key in window.glue_session_data['context'][this.glue_unique_name].fields) {
             this[key] = window.glue_session_data['context'][this.glue_unique_name].fields[key].value
+            this['fields'][key] = window.glue_session_data['context'][this.glue_unique_name].fields[key]
         }
-
         window.glue_keep_live.add_unique_name(this.glue_unique_name)
     }
 
     delete() {
         glue_ajax_request(
             this.glue_unique_name,
             'delete'
```

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_query_set.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,13 @@
 class GlueQuerySet {
     constructor(glue_unique_name) {
         this.glue_unique_name = encodeUniqueName(glue_unique_name)
 
         // We need this value on query to build GlueModelObjects
         this.decoded_unique_name = glue_unique_name
-
         for (let key in window.glue_session_data['context'][this.glue_unique_name].fields) {
             this[key] = window.glue_session_data['context'][this.glue_unique_name].fields[key].value
         }
 
         window.glue_keep_live.add_unique_name(this.glue_unique_name)
     }
 
@@ -22,15 +21,14 @@
                 console.log(response)
                 glue_dispatch_response_event(response)
                 for (let object in response.data) {
                     let model_object = new GlueModelObject(this.decoded_unique_name);
                     model_object.set_properties(response.data[object].simple_fields)
                     model_object_list.push(model_object)
                 }
-
                 return model_object_list
             });
     }
 
     async bulk_create(query_model_object_list) {
 
     }
```

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_template.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/static/django_glue/js/django_glue_view.js` & `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/templates/django_glue/django_glue.html` & `django_glue-0.5.2.3/django_glue/templates/django_glue/django_glue.html`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/templatetags/django_glue.py` & `django_glue-0.5.2.3/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue/utils.py` & `django_glue-0.5.2.3/django_glue/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
-import logging, pickle, base64, json
+import pickle, base64, json
 import urllib.parse
 from typing import Optional, Callable, Union
 
-from django.core import exceptions
 from django.db.models import Model
+from django.core.serializers.json import DjangoJSONEncoder
 
 from django_glue.core.utils import serialize_object_to_json
 from django_glue.data_classes import GlueModelFieldData
 
 
 def decode_query_set_from_str(query_set_string):
     query = pickle.loads(base64.b64decode(query_set_string))
@@ -27,33 +27,49 @@
         if name in fields or fields[0] == '__all__':
             included = True
 
     return included
 
 
 def generate_field_attr_dict(field):
-    form_field = field.formfield()
-    return form_field.widget_attrs(form_field.widget)
+    return {
+        'name': field.name,
+        'label': ''.join(word.capitalize() for word in field.name.split('_')),
+        'id': f'id_{field.name}',
+        'help_text': field.help_text,
+        'required': not field.null,
+        'disabled': not field.editable,
+        'hidden': field.hidden,
+        'choices': field.choices,
+        'maxlength': field.max_length,
+    }
+    # form_field = field.formfield()
+    # return form_field.widget_attrs(form_field.widget)
 
 
 def generate_field_dict(model_object: Model, fields: [list, tuple], exclude: Union[list, tuple]):
-    fields_dict = dict()
+    # Creates a detailed dictionary of model fields
+    fields_dict = {}
 
     model = type(model_object)
-    json_model = json.loads(serialize_object_to_json(model_object))[0]
+    # print(model_dict)
+    # json_model = json.loads(serialize_object_to_json(model_object))[0]
+    # print(json_model)
 
     for field in model._meta.fields:
         try:
             if field_name_included(field.name, fields, exclude):
                 if hasattr(field, 'get_internal_type'):
                     if field.name == 'id':
-                        field_value = json_model['pk']
+                        # field_value = json_model['pk']
+                        field_value = model_object.pk
                         field_attr = ''
                     else:
-                        field_value = json_model['fields'][field.name]
+                        field_value = getattr(model_object, field.name)
+                        # field_value = json_model['fields'][field.name]
                         field_attr = generate_field_attr_dict(field)
 
                     # Todo: Field name logic is duplicated
                     if field.many_to_one or field.one_to_one:
                         field_name = field.name + '_id'
                     else:
                         field_name = field.name
@@ -63,15 +79,19 @@
                         value=field_value,
                         html_attr=field_attr,
                     ).to_dict()
 
         except:
             raise f'Field "{field.name}" is invalid field or exclude for model type "{model.__class__.__name__}"'
 
-    return fields_dict
+    # for key, val in fields_dict.items():
+    #     print(val)
+    #
+    # return fields_dict
+    return json.loads(json.dumps(fields_dict, cls=DjangoJSONEncoder))
 
 
 def generate_method_list(model_object, methods: tuple) -> list:
     methods_list = list()
 
     model = type(model_object)
```

### Comparing `django-glue-0.5.2.2/django_glue/views.py` & `django_glue-0.5.2.3/django_glue/views.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/django_glue.egg-info/PKG-INFO` & `django_glue-0.5.2.3/django_glue.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,45 +22,53 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 License-File: LICENSE.md
 Requires-Dist: django>=3.2
 
 # django-glue
-
 We built Django Glue to help solve the problem of fluid interactions between the front and back ends of a Django application.
 Our end goal is to bring as much front end power to the Django framework as possible while remaining pythonic.
 
 This project is in prototype phase please look at the tests directory of this code base for examples and instructions.
 
 ## Why?
-
 We are active web platform developers that want to provide our clients with the best user experience without having to learn a bunch of different technology stacks.
 Django glue allows us to do fancy javascript like page interactions and updates while remaining in the comfort of our django/python world.
 
 Education is also a big part of what we do and our focus is on teaching our people python, so they can focus on data science and automation and make solid interfaces! 
 
-## Requirements
+## Inspiration
+We are inspired by how quickly django's model structure, ORM and forms (crispy forms) allow you to create functional web applications.
+Can we build on top of 25+ years of development to create a front end tool that uses the power of django.
+
+## Forms
+
 
+## Requirements
 - Django 3.2+ or 4.0+
 - Python 3.8+
 
 ## Dependencies
-
 - Alpine JS
+- Bootstrap 5
 - Axios
 
 ## Documentation
-
 - Installation Guide - [Here](INSTALLATION.md)
 - Usage Guide - [Here](USAGE.md)
 
 ## Roadmap
+### April 2024
+- [ ] Review project architecture for dependency flow and extendability
+- [ ] Includes for Alpine Js & Bootstrap
+- [ ] Basic form field elements
 
-- [x] Prototype (2022-07-12)
-- [x] Alpha (2022-08-31)
-- [ ] Beta (2023-06-31)
 
-## Authors
+### May 2024
+- [ ] Working with form fields that are not glued
+- [ ] Creating your own form elements
 
+## Authors
 - Nathan Johnson
 - Wesley Howery
+- Austin Sauer
```

### Comparing `django-glue-0.5.2.2/django_glue.egg-info/SOURCES.txt` & `django_glue-0.5.2.3/django_glue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 tests/admin.py
 tests/forms.py
 tests/manage.py
 tests/models.py
 tests/processors.py
 tests/settings.py
 tests/test_core.py
+tests/test_functions.py
+tests/test_views.py
 tests/urls.py
 tests/utils.py
 tests/validators.py
 tests/views.py
 tests/wsgi.py
 tests/migrations/0001_initial.py
 tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
```

### Comparing `django-glue-0.5.2.2/setup.py` & `django_glue-0.5.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/forms.py` & `django_glue-0.5.2.3/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/manage.py` & `django_glue-0.5.2.3/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/migrations/0001_initial.py` & `django_glue-0.5.2.3/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py` & `django_glue-0.5.2.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/models.py` & `django_glue-0.5.2.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/settings.py` & `django_glue-0.5.2.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/urls.py` & `django_glue-0.5.2.3/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/utils.py` & `django_glue-0.5.2.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.5.2.2/tests/views.py` & `django_glue-0.5.2.3/tests/views.py`

 * *Files identical despite different names*

