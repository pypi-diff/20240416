# Comparing `tmp/djangocms-aldryn-newsblog-3.1.6.tar.gz` & `tmp/djangocms_aldryn_newsblog-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-newsblog-3.1.6.tar", last modified: Thu Nov 16 09:03:33 2023, max compression
+gzip compressed data, was "djangocms_aldryn_newsblog-3.1.7.tar", last modified: Tue Apr 16 08:35:18 2024, max compression
```

## Comparing `djangocms-aldryn-newsblog-3.1.6.tar` & `djangocms_aldryn_newsblog-3.1.7.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.719819 djangocms-aldryn-newsblog-3.1.6/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-08-21 12:26:44.000000 djangocms-aldryn-newsblog-3.1.6/LICENSE.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      249 2023-08-21 12:26:44.000000 djangocms-aldryn-newsblog-3.1.6/MANIFEST.in
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     4569 2023-11-16 09:03:33.719819 djangocms-aldryn-newsblog-3.1.6/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2786 2023-11-16 08:54:29.000000 djangocms-aldryn-newsblog-3.1.6/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       83 2023-11-16 09:00:04.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6789 2023-10-09 06:46:46.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      548 2023-10-09 06:46:46.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5440 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_appconfig.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      585 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1876 2023-11-06 13:50:57.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_menus.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8427 2023-09-07 09:07:09.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4902 2023-11-06 13:50:57.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_toolbars.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3899 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_wizards.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      191 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/compat.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2252 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/feeds.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1989 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/forms.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6109 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13266 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8818 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14268 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6408 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8513 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8824 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14151 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8340 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14655 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9128 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14437 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2326 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11449 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9196 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14443 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9275 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14432 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/__init__.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.711819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/commands/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/commands/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1620 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/commands/rebuild_article_search_data.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4424 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/managers.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    16003 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      448 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0002_newsblogconfig_template_prefix.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      505 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0003_auto_20150422_1921.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      461 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0004_auto_20150622_1606.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      493 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0005_auto_20150807_0207.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      916 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0006_auto_20160105_1013.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3446 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0007_default_newsblog_config.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      793 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0008_auto_20160106_1735.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      448 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0009_auto_20160211_1022.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      861 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0010_auto_20160316_0935.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1808 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0011_auto_20160412_1622.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2988 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0012_auto_20160503_1626.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1488 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0013_auto_20160623_1703.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1039 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0014_auto_20160821_1156.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      470 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0015_auto_20161208_0403.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2376 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0016_auto_20180329_1417.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      520 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0017_newsblogconfig_author_no_photo.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      556 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0018_hide_author.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1929 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0019_serial_episode.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1477 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0020_alter_article_id_alter_articletranslation_id_and_more.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    22430 2023-10-09 06:46:30.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1799 2023-10-09 06:46:46.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/search_indexes.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/sitemaps/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       45 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/sitemaps/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      643 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/sitemaps/sitemap.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.707819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      347 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/admin/serial_episodes_change_form.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1075 2023-08-22 09:28:35.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/article_detail.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      552 2023-08-22 09:28:35.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/article_list.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      200 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/base.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2471 2023-08-22 09:28:35.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/article.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/article_featured_image_in_list.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      720 2023-10-10 12:45:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/author.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1941 2023-11-16 08:58:13.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/pagination.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1364 2023-08-22 09:28:35.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/search_results.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1040 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/archive.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1617 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/article.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      570 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/article_search.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      304 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/authors.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      613 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/categories.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      298 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/featured_articles.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      295 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/latest_articles.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      439 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/related_articles.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      395 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/serial_episodes.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      601 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/tags.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11333 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1533 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2130 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_cms_wizards.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1110 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_commands.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2481 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_feeds.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1671 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_i18n.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      804 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_managers.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8602 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15901 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2088 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_search.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3486 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_sitemaps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2267 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    30651 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2429 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/urls.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.715819 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      163 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2104 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/migration.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6270 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/utilities.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15676 2023-08-21 12:27:37.000000 djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/views.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-11-16 09:03:33.719819 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     4569 2023-11-16 09:03:33.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4928 2023-11-16 09:03:33.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-11-16 09:03:33.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-08-21 12:27:13.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      267 2023-11-16 09:03:33.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       16 2023-11-16 09:03:33.000000 djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       38 2023-11-16 09:03:33.719819 djangocms-aldryn-newsblog-3.1.6/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2068 2023-09-27 08:16:54.000000 djangocms-aldryn-newsblog-3.1.6/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.842564 djangocms_aldryn_newsblog-3.1.7/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-08-21 12:26:44.000000 djangocms_aldryn_newsblog-3.1.7/LICENSE.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      249 2023-08-21 12:26:44.000000 djangocms_aldryn_newsblog-3.1.7/MANIFEST.in
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     4581 2024-04-16 08:35:18.842564 djangocms_aldryn_newsblog-3.1.7/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2786 2023-11-16 08:54:29.000000 djangocms_aldryn_newsblog-3.1.7/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.830564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       83 2024-04-16 08:35:05.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6789 2023-10-09 06:46:46.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      548 2024-04-16 08:34:45.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5440 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_appconfig.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      585 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1876 2023-11-06 13:50:57.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_menus.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8427 2023-09-07 09:07:09.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4902 2023-11-06 13:50:57.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_toolbars.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3899 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_wizards.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      191 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/compat.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2252 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/feeds.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1989 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/forms.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.830564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6109 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13266 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.830564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8818 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14268 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.830564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6408 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8513 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8824 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14151 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8340 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14655 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9128 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14437 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2326 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11449 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9196 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14443 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.826564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9275 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    14432 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/__init__.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/commands/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/commands/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1620 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/commands/rebuild_article_search_data.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4424 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/managers.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    16003 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      448 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0002_newsblogconfig_template_prefix.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      505 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0003_auto_20150422_1921.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      461 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0004_auto_20150622_1606.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      493 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0005_auto_20150807_0207.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      916 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0006_auto_20160105_1013.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3446 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0007_default_newsblog_config.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      793 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0008_auto_20160106_1735.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      448 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0009_auto_20160211_1022.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      861 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0010_auto_20160316_0935.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1808 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0011_auto_20160412_1622.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2988 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0012_auto_20160503_1626.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1488 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0013_auto_20160623_1703.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1039 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0014_auto_20160821_1156.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      470 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0015_auto_20161208_0403.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2376 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0016_auto_20180329_1417.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      520 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0017_newsblogconfig_author_no_photo.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      556 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0018_hide_author.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1929 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0019_serial_episode.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1477 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0020_alter_article_id_alter_articletranslation_id_and_more.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    22430 2023-10-09 06:46:30.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1799 2023-10-09 06:46:46.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/search_indexes.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.834564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/sitemaps/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       45 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/sitemaps/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      643 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/sitemaps/sitemap.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.830564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      347 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/admin/serial_episodes_change_form.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1075 2023-08-22 09:28:35.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/article_detail.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      552 2023-12-07 11:59:51.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/article_list.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      200 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/base.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2471 2023-08-22 09:28:35.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/article.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/article_featured_image_in_list.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      720 2023-10-10 12:45:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/author.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1941 2023-11-16 08:58:13.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/pagination.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1364 2023-08-22 09:28:35.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/search_results.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1040 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/archive.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1617 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/article.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      570 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/article_search.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      304 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/authors.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      613 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/categories.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      298 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/featured_articles.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      295 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/latest_articles.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      439 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/related_articles.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      395 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/serial_episodes.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      601 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/tags.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11333 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1533 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2130 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_cms_wizards.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1110 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_commands.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2481 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_feeds.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1671 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_i18n.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      804 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_managers.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8602 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15901 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2088 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_search.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3486 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_sitemaps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2267 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    30651 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2429 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/urls.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.838564 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      163 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2104 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/migration.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6270 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/utilities.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15676 2023-08-21 12:27:37.000000 djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/views.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-04-16 08:35:18.842564 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     4581 2024-04-16 08:35:18.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4928 2024-04-16 08:35:18.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2024-04-16 08:35:18.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-08-21 12:27:13.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      279 2024-04-16 08:35:18.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       16 2024-04-16 08:35:18.000000 djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       38 2024-04-16 08:35:18.842564 djangocms_aldryn_newsblog-3.1.7/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2080 2024-04-16 08:21:39.000000 djangocms_aldryn_newsblog-3.1.7/setup.py
```

### Comparing `djangocms-aldryn-newsblog-3.1.6/LICENSE.txt` & `djangocms_aldryn_newsblog-3.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/PKG-INFO` & `djangocms_aldryn_newsblog-3.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-newsblog
-Version: 3.1.6
+Version: 3.1.7
 Summary: Adds blogging and newsing capabilities to django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-newsblog
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -35,15 +35,15 @@
 Requires-Dist: djangocms-aldryn-search
 Requires-Dist: djangocms-aldryn-translation-tools
 Requires-Dist: django-haystack
 Requires-Dist: backport-collections
 Requires-Dist: djangocms-text-ckeditor
 Requires-Dist: django-taggit
 Requires-Dist: python-dateutil
-Requires-Dist: lxml
+Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytz; extra == "test"
 
 |Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
 
 
 Aldryn News & Blog for django CMS
```

### Comparing `djangocms-aldryn-newsblog-3.1.6/README.rst` & `djangocms_aldryn_newsblog-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/admin.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/apps.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_appconfig.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_appconfig.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_apps.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_menus.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_menus.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_plugins.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_toolbars.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/cms_wizards.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/cms_wizards.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/feeds.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/feeds.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/forms.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/cs/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/de/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/en/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/es/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fa/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/fr/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/it/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/lt/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/LC_MESSAGES/django.mo` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/locale/nl/LC_MESSAGES/django.po` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/management/commands/rebuild_article_search_data.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/management/commands/rebuild_article_search_data.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/managers.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/managers.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0001_initial.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0006_auto_20160105_1013.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0006_auto_20160105_1013.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0007_default_newsblog_config.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0007_default_newsblog_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0008_auto_20160106_1735.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0008_auto_20160106_1735.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0010_auto_20160316_0935.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0010_auto_20160316_0935.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0011_auto_20160412_1622.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0011_auto_20160412_1622.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0012_auto_20160503_1626.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0012_auto_20160503_1626.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0013_auto_20160623_1703.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0013_auto_20160623_1703.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0014_auto_20160821_1156.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0014_auto_20160821_1156.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0016_auto_20180329_1417.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0016_auto_20180329_1417.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0017_newsblogconfig_author_no_photo.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0017_newsblogconfig_author_no_photo.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0018_hide_author.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0018_hide_author.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0019_serial_episode.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0019_serial_episode.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/migrations/0020_alter_article_id_alter_articletranslation_id_and_more.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/migrations/0020_alter_article_id_alter_articletranslation_id_and_more.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/models.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/search_indexes.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/search_indexes.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/sitemaps/sitemap.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/sitemaps/sitemap.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/article_detail.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/article_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/article_list.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/article_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/article.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/article.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/author.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/author.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/pagination.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/includes/search_results.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/includes/search_results.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/archive.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/archive.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/article.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/article.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/article_search.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/article_search.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/categories.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/categories.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/templates/aldryn_newsblog/plugins/tags.html` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/templates/aldryn_newsblog/plugins/tags.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/__init__.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_admin.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_cms_wizards.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_cms_wizards.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_commands.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_feeds.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_i18n.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_managers.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_models.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_plugins.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_search.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_sitemaps.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_sitemaps.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_utils.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/tests/test_views.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/urls.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/migration.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/utils/utilities.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/aldryn_newsblog/views.py` & `djangocms_aldryn_newsblog-3.1.7/aldryn_newsblog/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/PKG-INFO` & `djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-newsblog
-Version: 3.1.6
+Version: 3.1.7
 Summary: Adds blogging and newsing capabilities to django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-newsblog
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -35,15 +35,15 @@
 Requires-Dist: djangocms-aldryn-search
 Requires-Dist: djangocms-aldryn-translation-tools
 Requires-Dist: django-haystack
 Requires-Dist: backport-collections
 Requires-Dist: djangocms-text-ckeditor
 Requires-Dist: django-taggit
 Requires-Dist: python-dateutil
-Requires-Dist: lxml
+Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytz; extra == "test"
 
 |Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
 
 
 Aldryn News & Blog for django CMS
```

### Comparing `djangocms-aldryn-newsblog-3.1.6/djangocms_aldryn_newsblog.egg-info/SOURCES.txt` & `djangocms_aldryn_newsblog-3.1.7/djangocms_aldryn_newsblog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-newsblog-3.1.6/setup.py` & `djangocms_aldryn_newsblog-3.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'djangocms-aldryn-search',
     'djangocms-aldryn-translation-tools',
     'django-haystack',
     'backport-collections',
     'djangocms-text-ckeditor',
     'django-taggit',
     'python-dateutil',
-    'lxml',
+    'lxml[html_clean]',
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
```

