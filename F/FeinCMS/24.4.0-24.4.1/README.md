# Comparing `tmp/FeinCMS-24.4.0.tar.gz` & `tmp/feincms-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeinCMS-24.4.0.tar", last modified: Mon Apr  8 14:07:14 2024, max compression
+gzip compressed data, was "feincms-24.4.1.tar", last modified: Tue Apr 16 08:18:00 2024, max compression
```

## Comparing `FeinCMS-24.4.0.tar` & `feincms-24.4.1.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.541496 FeinCMS-24.4.0/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1794 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/AUTHORS
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/CONTRIBUTING.rst
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.541496 FeinCMS-24.4.0/FeinCMS.egg-info/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5263 2024-04-08 14:07:14.000000 FeinCMS-24.4.0/FeinCMS.egg-info/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7930 2024-04-08 14:07:14.000000 FeinCMS-24.4.0/FeinCMS.egg-info/SOURCES.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2024-04-08 14:07:14.000000 FeinCMS-24.4.0/FeinCMS.egg-info/dependency_links.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-08-07 06:21:51.000000 FeinCMS-24.4.0/FeinCMS.egg-info/not-zip-safe
--rw-r--r--   0 matthias  (1000) matthias  (1000)       63 2024-04-08 14:07:14.000000 FeinCMS-24.4.0/FeinCMS.egg-info/requires.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        8 2024-04-08 14:07:14.000000 FeinCMS-24.4.0/FeinCMS.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1557 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      204 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/MANIFEST.in
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5263 2024-04-08 14:07:14.541496 FeinCMS-24.4.0/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3894 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/README.rst
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.527496 FeinCMS-24.4.0/feincms/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      649 2024-04-08 14:06:50.000000 FeinCMS-24.4.0/feincms/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      856 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/_internal.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.527496 FeinCMS-24.4.0/feincms/admin/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      390 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/admin/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3382 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/admin/filters.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9399 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/admin/item_editor.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    20413 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/admin/tree_editor.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      464 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/apps.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.527496 FeinCMS-24.4.0/feincms/content/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.527496 FeinCMS-24.4.0/feincms/content/application/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/application/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15998 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/application/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/contactform/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      172 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/contactform/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2512 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/contactform/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/file/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/file/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      941 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/file/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/filer/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/filer/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3694 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/filer/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/image/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/image/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2988 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/image/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/medialibrary/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/medialibrary/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      167 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/medialibrary/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/raw/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/raw/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      590 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/raw/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/richtext/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/richtext/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1317 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/richtext/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.528496 FeinCMS-24.4.0/feincms/content/section/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/section/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3662 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/section/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.529496 FeinCMS-24.4.0/feincms/content/template/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/template/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1106 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/template/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.529496 FeinCMS-24.4.0/feincms/content/video/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/video/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2255 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/content/video/models.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      245 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contents.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      280 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/context_processors.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.529496 FeinCMS-24.4.0/feincms/contrib/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2805 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/fields.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.529496 FeinCMS-24.4.0/feincms/contrib/preview/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/preview/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      199 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/preview/urls.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1080 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/preview/views.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1012 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/richtext.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4851 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/contrib/tagging.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6164 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/default_settings.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/extensions/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      244 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4401 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/base.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2249 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/changedate.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6284 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/ct_tracker.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5485 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/datepublisher.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      564 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/featured.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1295 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/seo.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12525 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/extensions/translations.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.523496 FeinCMS-24.4.0/feincms/locale/ca/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/locale/ca/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12041 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25383 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.523496 FeinCMS-24.4.0/feincms/locale/cs/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/locale/cs/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12819 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26560 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.523496 FeinCMS-24.4.0/feincms/locale/de/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/locale/de/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    13491 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25408 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.523496 FeinCMS-24.4.0/feincms/locale/en/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/locale/en/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      378 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    20729 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/es/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.530496 FeinCMS-24.4.0/feincms/locale/es/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12216 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25561 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/fr/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.531496 FeinCMS-24.4.0/feincms/locale/fr/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9139 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24456 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/hr/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.531496 FeinCMS-24.4.0/feincms/locale/hr/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12148 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25494 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/it/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.531496 FeinCMS-24.4.0/feincms/locale/it/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8514 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24237 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/nb/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.531496 FeinCMS-24.4.0/feincms/locale/nb/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    11786 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24992 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/nl/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.531496 FeinCMS-24.4.0/feincms/locale/nl/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15507 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    27033 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/pl/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/pl/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9946 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24297 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/pt/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15186 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    27160 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0 matthias  (1000) matthias  (1000)      436 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)      658 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/pt_BR/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    14112 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26764 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/ro/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/ro/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8931 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24475 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/ru/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/ru/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17097 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    30062 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/tr/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.532496 FeinCMS-24.4.0/feincms/locale/tr/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15383 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26900 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.524496 FeinCMS-24.4.0/feincms/locale/zh_CN/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.533496 FeinCMS-24.4.0/feincms/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12710 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25227 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.533496 FeinCMS-24.4.0/feincms/management/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/management/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.533496 FeinCMS-24.4.0/feincms/management/commands/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/management/commands/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      805 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/management/commands/medialibrary_orphans.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2068 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/management/commands/medialibrary_to_filer.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      691 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/management/commands/rebuild_mptt.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    31018 2023-08-07 05:48:30.000000 FeinCMS-24.4.0/feincms/models.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.533496 FeinCMS-24.4.0/feincms/module/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.534496 FeinCMS-24.4.0/feincms/module/extensions/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/changedate.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/ct_tracker.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/datepublisher.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/featured.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/seo.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/extensions/translations.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.534496 FeinCMS-24.4.0/feincms/module/medialibrary/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      371 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      526 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/admin.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2405 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/contents.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3414 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/fields.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3043 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/forms.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8376 2024-04-08 14:04:37.000000 FeinCMS-24.4.0/feincms/module/medialibrary/modeladmins.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9156 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/models.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      608 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/thumbnail.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6833 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/medialibrary/zip.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7885 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/mixins.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.535496 FeinCMS-24.4.0/feincms/module/page/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1070 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/admin.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.535496 FeinCMS-24.4.0/feincms/module/page/extensions/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      704 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/excerpt.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5296 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/navigation.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      979 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/navigationgroups.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      893 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/relatedpages.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      944 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/sites.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1353 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/symlinks.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2115 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/extensions/titles.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8829 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/forms.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9567 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/modeladmins.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12575 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/models.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4511 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/processors.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4807 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/module/page/sitemap.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      417 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/shortcuts.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      709 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/signals.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.525496 FeinCMS-24.4.0/feincms/static/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.536496 FeinCMS-24.4.0/feincms/static/feincms/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.537496 FeinCMS-24.4.0/feincms/static/feincms/img/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      740 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/arrow-move.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24030 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/contenttypes.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      844 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/default-bg.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      313 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/disclosure-down.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      311 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/disclosure-right.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      176 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/icon-no.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      130 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/icon-unknown.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      299 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/icon-yes.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      119 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/icon_addlink.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      181 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/icon_deletelink.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      552 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/img/selector-search.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4871 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/item_editor.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21617 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/item_editor.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    95957 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/jquery-1.11.3.min.js
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)    37489 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/jquery-ui-1.10.3.custom.min.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1681 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/js.cookie.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1346 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/static/feincms/tree_editor.css
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)    13827 2024-04-08 14:04:37.000000 FeinCMS-24.4.0/feincms/static/feincms/tree_editor.js
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.537496 FeinCMS-24.4.0/feincms/templates/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.537496 FeinCMS-24.4.0/feincms/templates/admin/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.525496 FeinCMS-24.4.0/feincms/templates/admin/content/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.537496 FeinCMS-24.4.0/feincms/templates/admin/content/richtext/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1728 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_ckeditor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2906 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_tinymce.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2396 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_tinymce4.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.538496 FeinCMS-24.4.0/feincms/templates/admin/feincms/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1656 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/_content_type_buttons.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      501 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/_messages_js.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1321 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/_regions_js.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1619 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/content_editor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2388 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/content_inline.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      394 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/content_type_selection_widget.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2173 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/item_editor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      438 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/load-jquery.include
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.525496 FeinCMS-24.4.0/feincms/templates/admin/feincms/page/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.538496 FeinCMS-24.4.0/feincms/templates/admin/feincms/page/page/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      996 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/page/page/item_editor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      239 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/page/page/tree_editor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1080 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/recover_form.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1274 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/revision_form.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1057 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/feincms/tree_editor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      894 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/filter.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.538496 FeinCMS-24.4.0/feincms/templates/admin/medialibrary/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      761 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/medialibrary/add_to_category.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.538496 FeinCMS-24.4.0/feincms/templates/admin/medialibrary/mediafile/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1215 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/admin/medialibrary/mediafile/change_list.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      261 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/breadcrumbs.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.525496 FeinCMS-24.4.0/feincms/templates/content/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.538496 FeinCMS-24.4.0/feincms/templates/content/contactform/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       59 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/contactform/email.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)      298 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/contactform/form.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)       82 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/contactform/thanks.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/file/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      188 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/file/default.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/filer/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       69 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/filer/default.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      249 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/filer/download.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      383 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/filer/image.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/image/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      406 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/image/default.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/mediafile/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      234 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/mediafile/default.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      321 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/mediafile/image.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      336 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/mediafile/mp3.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/richtext/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       24 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/richtext/default.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/section/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      171 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/section/default.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      113 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/section/image.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.539496 FeinCMS-24.4.0/feincms/templates/content/video/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      382 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/video/sf.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)       54 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/video/unknown.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      156 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/video/vimeo.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      406 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templates/content/video/youtube.html
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.540496 FeinCMS-24.4.0/feincms/templatetags/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4615 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/applicationcontent_tags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2421 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/feincms_admin_tags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17283 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/feincms_page_tags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3240 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/feincms_tags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7880 2024-04-08 14:04:37.000000 FeinCMS-24.4.0/feincms/templatetags/feincms_thumbnail.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2985 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/templatetags/fragment_tags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    10056 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/translations.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      224 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/urls.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.540496 FeinCMS-24.4.0/feincms/utils/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5531 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/utils/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1997 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/utils/managers.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4315 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/utils/queryset_transform.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2196 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/utils/templatetags.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      706 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/utils/tuple.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-08 14:07:14.541496 FeinCMS-24.4.0/feincms/views/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2637 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/views/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      178 2023-07-21 14:20:15.000000 FeinCMS-24.4.0/feincms/views/decorators.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1469 2024-04-08 14:07:14.541496 FeinCMS-24.4.0/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-05-30 13:57:29.000000 FeinCMS-24.4.0/setup.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.596409 feincms-24.4.1/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1794 2023-07-26 08:48:44.000000 feincms-24.4.1/AUTHORS
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      454 2023-07-26 08:48:44.000000 feincms-24.4.1/CONTRIBUTING.rst
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.595409 feincms-24.4.1/FeinCMS.egg-info/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5263 2024-04-16 08:18:00.000000 feincms-24.4.1/FeinCMS.egg-info/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7930 2024-04-16 08:18:00.000000 feincms-24.4.1/FeinCMS.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2024-04-16 08:18:00.000000 feincms-24.4.1/FeinCMS.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-12-22 13:54:29.000000 feincms-24.4.1/FeinCMS.egg-info/not-zip-safe
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       63 2024-04-16 08:18:00.000000 feincms-24.4.1/FeinCMS.egg-info/requires.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        8 2024-04-16 08:18:00.000000 feincms-24.4.1/FeinCMS.egg-info/top_level.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1557 2023-07-26 08:48:44.000000 feincms-24.4.1/LICENSE
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      204 2023-07-26 08:48:44.000000 feincms-24.4.1/MANIFEST.in
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5263 2024-04-16 08:18:00.595409 feincms-24.4.1/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3894 2023-07-26 08:48:44.000000 feincms-24.4.1/README.rst
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.580409 feincms-24.4.1/feincms/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      649 2024-04-16 08:17:34.000000 feincms-24.4.1/feincms/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      856 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/_internal.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.580409 feincms-24.4.1/feincms/admin/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      390 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/admin/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3382 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/admin/filters.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9399 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/admin/item_editor.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    20413 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/admin/tree_editor.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      464 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/apps.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/application/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/application/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    16622 2024-04-16 08:14:31.000000 feincms-24.4.1/feincms/content/application/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/contactform/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      172 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/contactform/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2512 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/contactform/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/file/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/file/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      941 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/file/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/filer/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/filer/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3694 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/filer/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/image/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/image/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2988 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/image/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.581409 feincms-24.4.1/feincms/content/medialibrary/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/medialibrary/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      167 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/medialibrary/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/content/raw/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/raw/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      590 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/raw/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/content/richtext/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/richtext/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1317 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/richtext/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/content/section/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/section/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3662 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/section/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/content/template/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/template/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1106 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/template/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/content/video/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/video/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2255 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/content/video/models.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      245 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contents.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      280 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/context_processors.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.582409 feincms-24.4.1/feincms/contrib/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2805 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/fields.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.583409 feincms-24.4.1/feincms/contrib/preview/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/preview/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      199 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/preview/urls.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1080 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/preview/views.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1012 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/richtext.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4851 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/contrib/tagging.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6164 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/default_settings.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.583409 feincms-24.4.1/feincms/extensions/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      244 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4401 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/base.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2249 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/changedate.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6284 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/ct_tracker.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5485 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/datepublisher.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      564 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/featured.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1295 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/seo.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12525 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/extensions/translations.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/ca/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.583409 feincms-24.4.1/feincms/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12041 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25383 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/cs/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12819 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26560 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/de/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    13491 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25408 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/en/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/en/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      378 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    20729 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/es/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/es/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12216 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25561 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/fr/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9139 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24456 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/hr/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.584409 feincms-24.4.1/feincms/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12148 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25494 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/it/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.585409 feincms-24.4.1/feincms/locale/it/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8514 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24237 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/nb/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.585409 feincms-24.4.1/feincms/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    11786 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24992 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.576409 feincms-24.4.1/feincms/locale/nl/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.585409 feincms-24.4.1/feincms/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    15507 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    27033 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/pl/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.585409 feincms-24.4.1/feincms/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9946 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24297 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/pt/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    15186 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    27160 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      436 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      658 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/pt_BR/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    14112 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26764 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/ro/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8931 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24475 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/ru/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17097 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    30062 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/tr/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    15383 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26900 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/locale/zh_CN/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12710 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25227 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.586409 feincms-24.4.1/feincms/management/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/management/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.587409 feincms-24.4.1/feincms/management/commands/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/management/commands/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      805 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/management/commands/medialibrary_orphans.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2068 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/management/commands/medialibrary_to_filer.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      691 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/management/commands/rebuild_mptt.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    31018 2023-08-09 12:49:47.000000 feincms-24.4.1/feincms/models.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.587409 feincms-24.4.1/feincms/module/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.587409 feincms-24.4.1/feincms/module/extensions/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/changedate.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/ct_tracker.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/datepublisher.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/featured.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/seo.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      189 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/extensions/translations.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.588409 feincms-24.4.1/feincms/module/medialibrary/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      371 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      526 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/admin.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2405 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/contents.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3414 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/fields.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3043 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/forms.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8376 2023-12-22 13:40:31.000000 feincms-24.4.1/feincms/module/medialibrary/modeladmins.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9161 2024-04-16 08:14:31.000000 feincms-24.4.1/feincms/module/medialibrary/models.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      608 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/thumbnail.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6833 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/medialibrary/zip.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7885 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/mixins.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.589409 feincms-24.4.1/feincms/module/page/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1070 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/admin.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.589409 feincms-24.4.1/feincms/module/page/extensions/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      704 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/excerpt.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5296 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/navigation.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      979 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/navigationgroups.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      893 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/relatedpages.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      944 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/sites.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1353 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/symlinks.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2115 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/extensions/titles.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8829 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/forms.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9567 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/modeladmins.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12575 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/models.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4511 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/processors.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4807 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/module/page/sitemap.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      417 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/shortcuts.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      709 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/signals.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/static/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.590409 feincms-24.4.1/feincms/static/feincms/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.591409 feincms-24.4.1/feincms/static/feincms/img/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      740 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/arrow-move.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24030 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/contenttypes.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      844 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/default-bg.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      313 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/disclosure-down.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      311 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/disclosure-right.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      176 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/icon-no.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      130 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/icon-unknown.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      299 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/icon-yes.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      119 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/icon_addlink.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      181 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/icon_deletelink.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      552 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/img/selector-search.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4871 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/item_editor.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21617 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/item_editor.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    95957 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/jquery-1.11.3.min.js
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)    37489 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/jquery-ui-1.10.3.custom.min.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1681 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/js.cookie.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1346 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/static/feincms/tree_editor.css
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)    13827 2024-04-16 08:14:31.000000 feincms-24.4.1/feincms/static/feincms/tree_editor.js
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.591409 feincms-24.4.1/feincms/templates/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.591409 feincms-24.4.1/feincms/templates/admin/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.577409 feincms-24.4.1/feincms/templates/admin/content/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.591409 feincms-24.4.1/feincms/templates/admin/content/richtext/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1728 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/content/richtext/init_ckeditor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2906 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/content/richtext/init_tinymce.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2396 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/content/richtext/init_tinymce4.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.592409 feincms-24.4.1/feincms/templates/admin/feincms/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1656 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/_content_type_buttons.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      501 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/_messages_js.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1321 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/_regions_js.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1619 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/content_editor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2388 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/content_inline.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      394 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/content_type_selection_widget.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2173 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/item_editor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      438 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/load-jquery.include
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.578409 feincms-24.4.1/feincms/templates/admin/feincms/page/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.592409 feincms-24.4.1/feincms/templates/admin/feincms/page/page/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      996 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/page/page/item_editor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      239 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/page/page/tree_editor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1080 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/recover_form.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1274 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/revision_form.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1057 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/feincms/tree_editor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      894 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/filter.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.592409 feincms-24.4.1/feincms/templates/admin/medialibrary/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      761 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/medialibrary/add_to_category.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.592409 feincms-24.4.1/feincms/templates/admin/medialibrary/mediafile/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1215 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/admin/medialibrary/mediafile/change_list.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      261 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/breadcrumbs.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.578409 feincms-24.4.1/feincms/templates/content/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/contactform/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       59 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/contactform/email.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      298 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/contactform/form.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       82 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/contactform/thanks.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/file/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      188 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/file/default.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/filer/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       69 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/filer/default.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      249 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/filer/download.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      383 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/filer/image.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/image/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      406 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/image/default.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/mediafile/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      234 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/mediafile/default.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      321 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/mediafile/image.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      336 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/mediafile/mp3.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.593409 feincms-24.4.1/feincms/templates/content/richtext/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       24 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/richtext/default.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.594409 feincms-24.4.1/feincms/templates/content/section/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      171 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/section/default.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      113 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/section/image.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.594409 feincms-24.4.1/feincms/templates/content/video/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      382 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/video/sf.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       54 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/video/unknown.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      156 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/video/vimeo.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      406 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templates/content/video/youtube.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.594409 feincms-24.4.1/feincms/templatetags/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4615 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/applicationcontent_tags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2421 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/feincms_admin_tags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17283 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/feincms_page_tags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3240 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/feincms_tags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8297 2024-04-16 08:14:31.000000 feincms-24.4.1/feincms/templatetags/feincms_thumbnail.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2985 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/templatetags/fragment_tags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10056 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/translations.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      224 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/urls.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.595409 feincms-24.4.1/feincms/utils/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5531 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/utils/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1997 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/utils/managers.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4315 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/utils/queryset_transform.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2196 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/utils/templatetags.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      706 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/utils/tuple.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2024-04-16 08:18:00.595409 feincms-24.4.1/feincms/views/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2637 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/views/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      178 2023-07-26 08:48:44.000000 feincms-24.4.1/feincms/views/decorators.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1469 2024-04-16 08:18:00.596409 feincms-24.4.1/setup.cfg
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)       62 2023-07-26 08:48:44.000000 feincms-24.4.1/setup.py
```

### Comparing `FeinCMS-24.4.0/AUTHORS` & `feincms-24.4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/FeinCMS.egg-info/PKG-INFO` & `feincms-24.4.1/FeinCMS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeinCMS
-Version: 24.4.0
+Version: 24.4.1
 Summary: Django-based Page CMS and CMS building toolkit.
 Home-page: http://github.com/feincms/feincms/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FeinCMS-24.4.0/FeinCMS.egg-info/SOURCES.txt` & `feincms-24.4.1/FeinCMS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/LICENSE` & `feincms-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/PKG-INFO` & `feincms-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeinCMS
-Version: 24.4.0
+Version: 24.4.1
 Summary: Django-based Page CMS and CMS building toolkit.
 Home-page: http://github.com/feincms/feincms/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FeinCMS-24.4.0/README.rst` & `feincms-24.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/__init__.py` & `feincms-24.4.1/feincms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = (24, 4, 0)
+VERSION = (24, 4, 1)
 __version__ = ".".join(map(str, VERSION))
 
 
 class LazySettings:
     def _load_settings(self):
         from django.conf import settings as django_settings
```

### Comparing `FeinCMS-24.4.0/feincms/_internal.py` & `feincms-24.4.1/feincms/_internal.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/admin/filters.py` & `feincms-24.4.1/feincms/admin/filters.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/admin/item_editor.py` & `feincms-24.4.1/feincms/admin/item_editor.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/admin/tree_editor.py` & `feincms-24.4.1/feincms/admin/tree_editor.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/application/models.py` & `feincms-24.4.1/feincms/content/application/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,14 +350,18 @@
                 self.rendered_headers = {}
 
                 # Copy relevant headers for later perusal
                 for h in ("Cache-Control", "Last-Modified", "Expires"):
                     if h in output:
                         self.rendered_headers.setdefault(h, []).append(output[h])
 
+                application_cookies = output.cookies
+                if application_cookies:
+                    self.rendered_headers['X-Feincms-Cookie'] = application_cookies
+
         elif isinstance(output, tuple) and "view" in kw:
             kw["view"].template_name = output[0]
             kw["view"].request._feincms_extra_context.update(output[1])
 
         else:
             self.rendered_result = mark_safe(output)
 
@@ -416,14 +420,23 @@
             response["Last-Modified"] = http_date(mktime(max(lm_list)))
 
         # Check all Expires headers, choose the earliest one
         lm_list = [parsedate(x) for x in headers.get("Expires", ())]
         if len(lm_list) > 0:
             response["Expires"] = http_date(mktime(min(lm_list)))
 
+        # Add all cookies
+        cookies = headers.get('X-Feincms-Cookie', None)
+        if cookies:
+            for kookie, val in cookies.items():
+                response.set_cookie(kookie, value=val.value,
+                        max_age=val['max-age'], expires=val['expires'], path=val['path'],
+                        domain=val['domain'], secure=val['secure'], httponly=val['httponly'],
+                        samesite=val['samesite'])
+
     @classmethod
     def app_reverse_cache_key(self, urlconf_path, **kwargs):
         return "FEINCMS:{}:APPCONTENT:{}:{}".format(
             getattr(settings, "SITE_ID", 0),
             get_language(),
             urlconf_path,
         )
```

### Comparing `FeinCMS-24.4.0/feincms/content/contactform/models.py` & `feincms-24.4.1/feincms/content/contactform/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/file/models.py` & `feincms-24.4.1/feincms/content/file/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/filer/models.py` & `feincms-24.4.1/feincms/content/filer/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/image/models.py` & `feincms-24.4.1/feincms/content/image/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/raw/models.py` & `feincms-24.4.1/feincms/content/raw/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/richtext/models.py` & `feincms-24.4.1/feincms/content/richtext/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/section/models.py` & `feincms-24.4.1/feincms/content/section/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/template/models.py` & `feincms-24.4.1/feincms/content/template/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/content/video/models.py` & `feincms-24.4.1/feincms/content/video/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/contrib/fields.py` & `feincms-24.4.1/feincms/contrib/fields.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/contrib/preview/views.py` & `feincms-24.4.1/feincms/contrib/preview/views.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/contrib/richtext.py` & `feincms-24.4.1/feincms/contrib/richtext.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/contrib/tagging.py` & `feincms-24.4.1/feincms/contrib/tagging.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/default_settings.py` & `feincms-24.4.1/feincms/default_settings.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/base.py` & `feincms-24.4.1/feincms/extensions/base.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/changedate.py` & `feincms-24.4.1/feincms/extensions/changedate.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/ct_tracker.py` & `feincms-24.4.1/feincms/extensions/ct_tracker.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/datepublisher.py` & `feincms-24.4.1/feincms/extensions/datepublisher.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/featured.py` & `feincms-24.4.1/feincms/extensions/featured.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/seo.py` & `feincms-24.4.1/feincms/extensions/seo.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/extensions/translations.py` & `feincms-24.4.1/feincms/extensions/translations.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ca/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ca/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/cs/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/cs/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/de/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/de/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/en/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/es/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/es/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/fr/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/fr/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/hr/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/hr/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/it/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/it/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/nb/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/nb/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/nl/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/nl/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pl/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pl/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pt/LC_MESSAGES/djangojs.po` & `feincms-24.4.1/feincms/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pt_BR/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/pt_BR/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ro/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ro/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ru/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/ru/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/tr/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/tr/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/zh_CN/LC_MESSAGES/django.mo` & `feincms-24.4.1/feincms/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/locale/zh_CN/LC_MESSAGES/django.po` & `feincms-24.4.1/feincms/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/management/commands/medialibrary_orphans.py` & `feincms-24.4.1/feincms/management/commands/medialibrary_orphans.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/management/commands/medialibrary_to_filer.py` & `feincms-24.4.1/feincms/management/commands/medialibrary_to_filer.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/management/commands/rebuild_mptt.py` & `feincms-24.4.1/feincms/management/commands/rebuild_mptt.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/models.py` & `feincms-24.4.1/feincms/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/admin.py` & `feincms-24.4.1/feincms/module/medialibrary/admin.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/contents.py` & `feincms-24.4.1/feincms/module/medialibrary/contents.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/fields.py` & `feincms-24.4.1/feincms/module/medialibrary/fields.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/forms.py` & `feincms-24.4.1/feincms/module/medialibrary/forms.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/modeladmins.py` & `feincms-24.4.1/feincms/module/medialibrary/modeladmins.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/models.py` & `feincms-24.4.1/feincms/module/medialibrary/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 # ------------------------------------------------------------------------
 MediaFileBase.register_filetypes(
     # Should we be using imghdr.what instead of extension guessing?
     (
         "image",
         _("Image"),
         lambda f: re.compile(
-            r"\.(bmp|jpe?g|jp2|jxr|gif|png|tiff?)$", re.IGNORECASE
+            r"\.(bmp|jpe?g|jp2|jxr|gif|png|tiff?|webp)$", re.IGNORECASE
         ).search(f),
     ),
     (
         "video",
         _("Video"),
         lambda f: re.compile(
             r"\.(mov|m[14]v|mp4|avi|mpe?g|qt|ogv|wmv|flv)$", re.IGNORECASE
```

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/thumbnail.py` & `feincms-24.4.1/feincms/module/medialibrary/thumbnail.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/medialibrary/zip.py` & `feincms-24.4.1/feincms/module/medialibrary/zip.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/mixins.py` & `feincms-24.4.1/feincms/module/mixins.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/admin.py` & `feincms-24.4.1/feincms/module/page/admin.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/excerpt.py` & `feincms-24.4.1/feincms/module/page/extensions/excerpt.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/navigation.py` & `feincms-24.4.1/feincms/module/page/extensions/navigation.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/navigationgroups.py` & `feincms-24.4.1/feincms/module/page/extensions/navigationgroups.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/relatedpages.py` & `feincms-24.4.1/feincms/module/page/extensions/relatedpages.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/sites.py` & `feincms-24.4.1/feincms/module/page/extensions/sites.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/symlinks.py` & `feincms-24.4.1/feincms/module/page/extensions/symlinks.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/extensions/titles.py` & `feincms-24.4.1/feincms/module/page/extensions/titles.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/forms.py` & `feincms-24.4.1/feincms/module/page/forms.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/modeladmins.py` & `feincms-24.4.1/feincms/module/page/modeladmins.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/models.py` & `feincms-24.4.1/feincms/module/page/models.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/processors.py` & `feincms-24.4.1/feincms/module/page/processors.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/module/page/sitemap.py` & `feincms-24.4.1/feincms/module/page/sitemap.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/signals.py` & `feincms-24.4.1/feincms/signals.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/img/arrow-move.png` & `feincms-24.4.1/feincms/static/feincms/img/arrow-move.png`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/img/contenttypes.png` & `feincms-24.4.1/feincms/static/feincms/img/contenttypes.png`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/img/default-bg.gif` & `feincms-24.4.1/feincms/static/feincms/img/default-bg.gif`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/img/selector-search.gif` & `feincms-24.4.1/feincms/static/feincms/img/selector-search.gif`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/item_editor.css` & `feincms-24.4.1/feincms/static/feincms/item_editor.css`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/item_editor.js` & `feincms-24.4.1/feincms/static/feincms/item_editor.js`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/jquery-1.11.3.min.js` & `feincms-24.4.1/feincms/static/feincms/jquery-1.11.3.min.js`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/jquery-ui-1.10.3.custom.min.js` & `feincms-24.4.1/feincms/static/feincms/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/js.cookie.js` & `feincms-24.4.1/feincms/static/feincms/js.cookie.js`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/tree_editor.css` & `feincms-24.4.1/feincms/static/feincms/tree_editor.css`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/static/feincms/tree_editor.js` & `feincms-24.4.1/feincms/static/feincms/tree_editor.js`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_ckeditor.html` & `feincms-24.4.1/feincms/templates/admin/content/richtext/init_ckeditor.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_tinymce.html` & `feincms-24.4.1/feincms/templates/admin/content/richtext/init_tinymce.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/content/richtext/init_tinymce4.html` & `feincms-24.4.1/feincms/templates/admin/content/richtext/init_tinymce4.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/_content_type_buttons.html` & `feincms-24.4.1/feincms/templates/admin/feincms/_content_type_buttons.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/_regions_js.html` & `feincms-24.4.1/feincms/templates/admin/feincms/_regions_js.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/content_editor.html` & `feincms-24.4.1/feincms/templates/admin/feincms/content_editor.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/content_inline.html` & `feincms-24.4.1/feincms/templates/admin/feincms/content_inline.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/item_editor.html` & `feincms-24.4.1/feincms/templates/admin/feincms/item_editor.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/page/page/item_editor.html` & `feincms-24.4.1/feincms/templates/admin/feincms/page/page/item_editor.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/recover_form.html` & `feincms-24.4.1/feincms/templates/admin/feincms/recover_form.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/revision_form.html` & `feincms-24.4.1/feincms/templates/admin/feincms/revision_form.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/feincms/tree_editor.html` & `feincms-24.4.1/feincms/templates/admin/feincms/tree_editor.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/filter.html` & `feincms-24.4.1/feincms/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/medialibrary/add_to_category.html` & `feincms-24.4.1/feincms/templates/admin/medialibrary/add_to_category.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templates/admin/medialibrary/mediafile/change_list.html` & `feincms-24.4.1/feincms/templates/admin/medialibrary/mediafile/change_list.html`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templatetags/applicationcontent_tags.py` & `feincms-24.4.1/feincms/templatetags/applicationcontent_tags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templatetags/feincms_admin_tags.py` & `feincms-24.4.1/feincms/templatetags/feincms_admin_tags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templatetags/feincms_page_tags.py` & `feincms-24.4.1/feincms/templatetags/feincms_page_tags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templatetags/feincms_tags.py` & `feincms-24.4.1/feincms/templatetags/feincms_tags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/templatetags/feincms_thumbnail.py` & `feincms-24.4.1/feincms/templatetags/feincms_thumbnail.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 logger = logging.getLogger("feincms.templatetags.thumbnail")
 register = template.Library()
 
 
 class Thumbnailer:
     THUMBNAIL_SIZE_RE = re.compile(r"^(?P<w>\d+)x(?P<h>\d+)$")
     MARKER = "_thumb_"
+    BROWSER_SUPPORTED_FORMATS = ("jpg", "jpeg", "png", "webp")  # browser supported image formats
+    TRANSPARENCY_SUPPORTING_FORMATS = ('png', 'webp')  # formats with alpha channel
 
     def __init__(self, filename, size="200x200"):
         self.filename = filename
         self.size = size
 
     @property
     def url(self):
@@ -81,15 +83,15 @@
                 generate = storage.modified_time(miniature) < storage.modified_time(
                     filename
                 )
             except (NotImplementedError, AttributeError):
                 # storage does NOT support modified_time
                 generate = False
             except OSError:
-                # Someone might have delete the file
+                # Someone might have deleted the file
                 return ""
 
         if generate:
             try:
                 self.generate(
                     storage=storage,
                     original=filename,
@@ -112,21 +114,22 @@
         with storage.open(original) as original_handle:
             with BytesIO(original_handle.read()) as original_bytes:
                 image = Image.open(original_bytes)
 
                 # defining the size
                 w, h = int(size["w"]), int(size["h"])
 
-                format = image.format  # Save format for the save() call later
+                assert image.format is not None
+                format = image.format.lower()  # Save format for the save() call later
                 image.thumbnail([w, h], Image.Resampling.LANCZOS)
                 buf = BytesIO()
-                if format.lower() not in ("jpg", "jpeg", "png"):
+                if format not in self.BROWSER_SUPPORTED_FORMATS:  # browser supported image formats
                     format = "jpeg"
                 if image.mode not in ("RGBA", "RGB", "L"):
-                    if format == "png":
+                    if format in self.TRANSPARENCY_SUPPORTING_FORMATS:  # handles transparency?
                         image = image.convert("RGBA")
                     else:
                         image = image.convert("RGB")
                 image.save(buf, format, quality=90)
                 raw_data = buf.getvalue()
                 buf.close()
 
@@ -164,30 +167,31 @@
                     y_offset = 0
                 else:
                     crop_width = src_width
                     crop_height = crop_width / dst_ratio
                     x_offset = 0
                     y_offset = int(float(src_height - crop_height) * y / 100)
 
-                format = image.format  # Save format for the save() call later
+                assert image.format is not None
+                format = image.format.lower()  # Save format for the save() call later
                 image = image.crop(
                     (
                         x_offset,
                         y_offset,
                         x_offset + int(crop_width),
                         y_offset + int(crop_height),
                     )
                 )
                 image = image.resize((dst_width, dst_height), Image.Resampling.LANCZOS)
 
                 buf = BytesIO()
-                if format.lower() not in ("jpg", "jpeg", "png"):
+                if format not in self.BROWSER_SUPPORTED_FORMATS:
                     format = "jpeg"
                 if image.mode not in ("RGBA", "RGB", "L"):
-                    if format == "png":
+                    if format in self.TRANSPARENCY_SUPPORTING_FORMATS:
                         image = image.convert("RGBA")
                     else:
                         image = image.convert("RGB")
                 image.save(buf, format, quality=90)
                 raw_data = buf.getvalue()
                 buf.close()
```

### Comparing `FeinCMS-24.4.0/feincms/templatetags/fragment_tags.py` & `feincms-24.4.1/feincms/templatetags/fragment_tags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/translations.py` & `feincms-24.4.1/feincms/translations.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/utils/__init__.py` & `feincms-24.4.1/feincms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/utils/managers.py` & `feincms-24.4.1/feincms/utils/managers.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/utils/queryset_transform.py` & `feincms-24.4.1/feincms/utils/queryset_transform.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/utils/templatetags.py` & `feincms-24.4.1/feincms/utils/templatetags.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/utils/tuple.py` & `feincms-24.4.1/feincms/utils/tuple.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/feincms/views/__init__.py` & `feincms-24.4.1/feincms/views/__init__.py`

 * *Files identical despite different names*

### Comparing `FeinCMS-24.4.0/setup.cfg` & `feincms-24.4.1/setup.cfg`

 * *Files identical despite different names*

