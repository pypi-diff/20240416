# Comparing `tmp/cubicweb-conference-1.0.0.tar.gz` & `tmp/cubicweb-conference-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-conference-1.0.0.tar", last modified: Thu Aug  3 09:51:34 2023, max compression
+gzip compressed data, was "cubicweb-conference-1.0.1.tar", last modified: Tue Apr 16 13:43:43 2024, max compression
```

## Comparing `cubicweb-conference-1.0.0.tar` & `cubicweb-conference-1.0.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     2375 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      615 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.686243 cubicweb-conference-1.0.0/cubicweb_conference/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.690243 cubicweb-conference-1.0.0/cubicweb_conference/data/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/attend.jpeg
--rw-rw-rw-   0 root         (0) root         (0)     2105 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.css
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.js
--rw-rw-rw-   0 root         (0) root         (0)     2889 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/icon_pen.gif
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/noattend.jpeg
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/stat.png
--rw-rw-rw-   0 root         (0) root         (0)     4842 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     9777 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     4749 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.694243 cubicweb-conference-1.0.0/cubicweb_conference/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    12221 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)    12700 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)    12220 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    17790 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.698243 cubicweb-conference-1.0.0/cubicweb_conference/migration/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.10.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.10.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.13.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.2.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.3.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.4.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.5.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.5.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.6.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.7.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.8.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.9.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/0.9.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10014 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/sobjects.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.702243 cubicweb-conference-1.0.0/cubicweb_conference/views/
--rw-rw-rw-   0 root         (0) root         (0)     4211 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     7631 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     9770 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/calendarview.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/components.py
--rw-rw-rw-   0 root         (0) root         (0)     6877 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/conference.py
--rw-rw-rw-   0 root         (0) root         (0)      964 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     3352 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/semantic.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/talk.py
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/track.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/cubicweb_conference/views/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.690243 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/
--rw-r--r--   0 root         (0) root         (0)      615 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2837 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      226 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-03 09:51:34.000000 cubicweb-conference-1.0.0/cubicweb_conference.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.710243 cubicweb-conference-1.0.0/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.710243 cubicweb-conference-1.0.0/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/test/data/acceptance/
--rw-rw-rw-   0 root         (0) root         (0)    14953 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/BBQ_logo_3.jpg
--rw-rw-rw-   0 root         (0) root         (0)    10221 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/ELE_logo_1.jpg
--rw-rw-rw-   0 root         (0) root         (0)    12589 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Pell_logo_3.jpg
--rw-rw-rw-   0 root         (0) root         (0)    98005 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Programme_SemWebPro2010.pdf
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Shell_logo_1.jpg
--rw-rw-rw-   0 root         (0) root         (0)     7541 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/Untel_logo_2.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8210 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/novia_logo_2.jpg
--rw-rw-rw-   0 root         (0) root         (0)     9017 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/acceptance/orange_logo_3.jpg
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)    15382 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/demo_conference.txt
--rw-rw-rw-   0 root         (0) root         (0)     1289 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/review-process.txt
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/test_acceptance.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/test_conference.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4563 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     5465 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_security.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7005 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/unittest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/test/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:51:34.714244 cubicweb-conference-1.0.0/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/wdoc/ChangeLog_en
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-03 09:51:15.000000 cubicweb-conference-1.0.0/wdoc/ChangeLog_fr
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.768563 cubicweb-conference-1.0.1/cubicweb_conference/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.776563 cubicweb-conference-1.0.1/cubicweb_conference/data/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/attend.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/cubes.conference.css
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/cubes.conference.js
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/icon_pen.gif
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/noattend.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/stat.png
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/ticket-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     9777 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/data/ticket-icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4749 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.776563 cubicweb-conference-1.0.1/cubicweb_conference/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    12700 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)    12220 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    17790 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.784563 cubicweb-conference-1.0.1/cubicweb_conference/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.10.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.10.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.13.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      982 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.4.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.5.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.6.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.7.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.8.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.9.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/0.9.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10014 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.788563 cubicweb-conference-1.0.1/cubicweb_conference/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7631 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9770 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/calendarview.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     6877 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/conference.py
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/semantic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/talk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/track.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/cubicweb_conference/views/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      226 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-16 13:43:43.000000 cubicweb-conference-1.0.1/cubicweb_conference.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.792563 cubicweb-conference-1.0.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.796563 cubicweb-conference-1.0.1/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/test/data/acceptance/
+-rw-rw-rw-   0 root         (0) root         (0)    14953 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/BBQ_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    10221 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/ELE_logo_1.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    12589 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/Pell_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    98005 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/Programme_SemWebPro2010.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/Shell_logo_1.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     7541 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/Untel_logo_2.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8210 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/novia_logo_2.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9017 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/acceptance/orange_logo_3.jpg
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    15382 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/demo_conference.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/review-process.txt
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/test_acceptance.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/test_conference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4563 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/unittest_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     5465 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/unittest_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7005 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/unittest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/test/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:43:43.800563 cubicweb-conference-1.0.1/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-16 13:43:21.000000 cubicweb-conference-1.0.1/wdoc/ChangeLog_fr
```

### Comparing `cubicweb-conference-1.0.0/CHANGELOG.md` & `cubicweb-conference-1.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## Version 1.0.1 (2024-04-16)
+### 👷 Bug fixes
+
+- stringify select options' values in vocabulary functions
+
+### 📝 Documentation
+
+- licence: update licence dates
+
 ## Version 1.0.0 (2023-08-03)
 ### 🎉 New features
 
 - run flynt on the code base to convert everything into f-strings
 - upgrade CubicWeb version to 4, and upgrade dependencies
   *BREAKING CHANGE*: upgrade CubicWeb version to 4, and upgrade dependencies
 
@@ -95,8 +104,8 @@
 
 ### 🤷 Various changes
 
 - Add a .hgignore
 - Indicate that Python 2.7 is now the minimum version
 - Fix typo in purl dc URI
 - Fix typo in RDFS URI
-- pkg: 0.14.0
+- pkg: 0.14.0
```

### Comparing `cubicweb-conference-1.0.0/MANIFEST.in` & `cubicweb-conference-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/__pkginfo__.py` & `cubicweb-conference-1.0.1/cubicweb_conference/__pkginfo__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import listdir as _listdir
 from os.path import join, isdir
 from glob import glob
 
 modname = "conference"
 distname = f"cubicweb-{modname}"
 
-numversion = (1, 0, 0)
+numversion = (1, 0, 1)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 description = "conference component for the CubicWeb framework"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
```

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/attend.jpeg` & `cubicweb-conference-1.0.1/cubicweb_conference/data/attend.jpeg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.css` & `cubicweb-conference-1.0.1/cubicweb_conference/data/cubes.conference.css`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/cubes.conference.js` & `cubicweb-conference-1.0.1/cubicweb_conference/data/cubes.conference.js`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/icon_pen.gif` & `cubicweb-conference-1.0.1/cubicweb_conference/data/icon_pen.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/noattend.jpeg` & `cubicweb-conference-1.0.1/cubicweb_conference/data/noattend.jpeg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/stat.png` & `cubicweb-conference-1.0.1/cubicweb_conference/data/stat.png`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.png` & `cubicweb-conference-1.0.1/cubicweb_conference/data/ticket-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/data/ticket-icon.svg` & `cubicweb-conference-1.0.1/cubicweb_conference/data/ticket-icon.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/entities.py` & `cubicweb-conference-1.0.1/cubicweb_conference/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/i18n/de.po` & `cubicweb-conference-1.0.1/cubicweb_conference/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/i18n/en.po` & `cubicweb-conference-1.0.1/cubicweb_conference/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/i18n/es.po` & `cubicweb-conference-1.0.1/cubicweb_conference/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/i18n/fr.po` & `cubicweb-conference-1.0.1/cubicweb_conference/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.10.3_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.10.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.3.0_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.3.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.4.0_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.4.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.6.0_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.6.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.7.0_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.7.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/0.8.0_Any.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/0.8.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/migration/postcreate.py` & `cubicweb-conference-1.0.1/cubicweb_conference/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/schema.py` & `cubicweb-conference-1.0.1/cubicweb_conference/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/site_cubicweb.py` & `cubicweb-conference-1.0.1/cubicweb_conference/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/sobjects.py` & `cubicweb-conference-1.0.1/cubicweb_conference/sobjects.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/__init__.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/actions.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/boxes.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/calendarview.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/calendarview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/components.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/components.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/conference.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/conference.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/facets.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/facets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/forms.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,74 +6,74 @@
 
 def reviewers_vocabulary(form, field):
     entity = form.edited_entity
     rset = form._cw.execute(
         "Any U WHERE U is_reviewer_at C, X in_conf C, " "X is Talk, X eid %(x)s",
         {"x": entity.eid},
     )
-    return [(item.dc_long_title(), item.eid) for item in rset.entities()]
+    return [(item.dc_long_title(), str(item.eid)) for item in rset.entities()]
 
 
 def subject_call_open_conf_vocabulary(form, field):
     options = []
     edited_entity = form.edited_entity
     if edited_entity.has_eid() and edited_entity.in_conf:
         conf = edited_entity.in_conf[0]
-        options = [(conf.dc_title(), conf.eid)]
+        options = [(conf.dc_title(), str(conf.eid))]
     if form._cw.user.matching_groups("managers"):
         rset = form._cw.execute("Any C WHERE C is Conference")
     else:
         rset = form._cw.execute(
             "Any C WHERE C is Conference, C call_open True, "
             'C in_state S, S name "scheduled"'
         )
     for entity in rset.entities():
         if edited_entity.has_eid() and conf.eid == entity.eid:
             continue
-        options.append((entity.dc_title(), entity.eid))
+        options.append((entity.dc_title(), str(entity.eid)))
     return options
 
 
 def subject_reg_open_conf_vocabulary(form, field):
     options = []
     edited_entity = form.edited_entity
     if edited_entity.has_eid() and edited_entity.book_conf:
         conf = edited_entity.book_conf[0]
-        options = [(conf.dc_title(), conf.eid)]
+        options = [(conf.dc_title(), str(conf.eid))]
     if form._cw.user.matching_groups("managers"):
         rset = form._cw.execute("Any C WHERE C is Conference")
     else:
         rset = form._cw.execute(
             "Any C WHERE C is Conference, C reg_open True, "
             'C in_state S, S name "scheduled"'
         )
     for entity in rset.entities():
         if edited_entity.has_eid() and conf.eid == entity.eid:
             continue
-        options.append((entity.dc_title(), entity.eid))
+        options.append((entity.dc_title(), str(entity.eid)))
     return options
 
 
 def subject_in_track_vocabulary(form, field):
     options = []
     edited_entity = form.edited_entity
     if edited_entity.has_eid() and edited_entity.in_track:
         track = edited_entity.in_track[0]
-        options = [(track.dc_title(), track.eid)]
+        options = [(track.dc_title(), str(track.eid))]
     if form._cw.user.matching_groups("managers"):
         rset = form._cw.execute("Any T WHERE T is Track")
     else:
         rset = form._cw.execute(
             "DISTINCT Any T WHERE T is Track, T in_conf C, "
             'C call_open True, C in_state S, S name "scheduled"'
         )
     for entity in rset.entities():
         if edited_entity.has_eid() and track.eid == entity.eid:
             continue
-        options.append((entity.dc_title(), entity.eid))
+        options.append((entity.dc_title(), str(entity.eid)))
     return options
 
 
 class TalkAutoForm(autoform.AutomaticEntityForm):
     __select__ = (
         autoform.AutomaticEntityForm.__select__
         & is_instance("Talk")
```

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/semantic.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/semantic.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/startup.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/startup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/talk.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/talk.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/track.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/track.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference/views/workflow.py` & `cubicweb-conference-1.0.1/cubicweb_conference/views/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/cubicweb_conference.egg-info/SOURCES.txt` & `cubicweb-conference-1.0.1/cubicweb_conference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/setup.py` & `cubicweb-conference-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # pylint: disable=W0404,W0622,W0704,W0613
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 
 from os.path import join, dirname
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
```

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/BBQ_logo_3.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/BBQ_logo_3.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/ELE_logo_1.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/ELE_logo_1.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/Pell_logo_3.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/Pell_logo_3.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/Programme_SemWebPro2010.pdf` & `cubicweb-conference-1.0.1/test/data/acceptance/Programme_SemWebPro2010.pdf`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/Shell_logo_1.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/Shell_logo_1.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/Untel_logo_2.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/Untel_logo_2.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/novia_logo_2.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/novia_logo_2.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/data/acceptance/orange_logo_3.jpg` & `cubicweb-conference-1.0.1/test/data/acceptance/orange_logo_3.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/demo_conference.txt` & `cubicweb-conference-1.0.1/test/demo_conference.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/pytestconf.py` & `cubicweb-conference-1.0.1/test/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/review-process.txt` & `cubicweb-conference-1.0.1/test/review-process.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/test_acceptance.py` & `cubicweb-conference-1.0.1/test/test_acceptance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 
 :organization: Logilab
 :copyright: 2001-2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL v2.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
+
 from os.path import dirname, join
 
 from logilab.common.testlib import unittest_main
 
 from cubicweb_web.devtools.testlib import WebCWTC
```

### Comparing `cubicweb-conference-1.0.0/test/unittest_hooks.py` & `cubicweb-conference-1.0.1/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/unittest_notifications.py` & `cubicweb-conference-1.0.1/test/unittest_notifications.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/unittest_security.py` & `cubicweb-conference-1.0.1/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/test/unittest_views.py` & `cubicweb-conference-1.0.1/test/unittest_views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-conference-1.0.0/tox.ini` & `cubicweb-conference-1.0.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 addopts = -r fEs
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
   flake8 >= 3.6
-commands = flake8
+commands = flake8 --show-source
 
 [flake8]
 basepython = python3
 ignore = W503, E203, E731, E231
 max-line-length = 100
 exclude = cubicweb_conference/migration/*,test/data/*,.tox/*,cubicweb_conference/uiprops.py
```

