# Comparing `tmp/plone.app.event-5.1.1.tar.gz` & `tmp/plone.app.event-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.event-5.1.1.tar", last modified: Fri Oct  6 22:07:57 2023, max compression
+gzip compressed data, was "plone.app.event-5.1.2.tar", last modified: Tue Apr 16 19:33:06 2024, max compression
```

## Comparing `plone.app.event-5.1.1.tar` & `plone.app.event-5.1.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.863910 plone.app.event-5.1.1/
--rw-r--r--   0 maurits    (501) staff       (20)    58306 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18099 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      202 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    63963 2023-10-06 22:07:57.863252 plone.app.event-5.1.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      587 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.812133 plone.app.event-5.1.1/docs/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.813926 plone.app.event-5.1.1/docs/api/
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/base.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.816218 plone.app.event-5.1.1/docs/api/browser/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/browser/event_listing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/browser/event_summary.rst
--rw-r--r--   0 maurits    (501) staff       (20)      136 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/browser/event_view.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/browser/formatted_date.rst
--rw-r--r--   0 maurits    (501) staff       (20)      158 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/browser/leadimage_viewlet.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.817565 plone.app.event-5.1.1/docs/api/dx/
--rw-r--r--   0 maurits    (501) staff       (20)      118 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/dx/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/dx/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      119 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/dx/traverser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.818467 plone.app.event-5.1.1/docs/api/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/ical/exporter.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/ical/importer.rst
--rw-r--r--   0 maurits    (501) staff       (20)      403 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      112 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      113 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/api/recurrence.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5633 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/architectural-overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3464 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/designchoices.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10346 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/development.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1590 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2839 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/installation.rst
--rw-r--r--   0 maurits    (501) staff       (20)      884 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/docs/tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.818898 plone.app.event-5.1.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.823141 plone.app.event-5.1.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.827944 plone.app.event-5.1.1/plone/app/event/
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    33259 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.833564 plone.app.event-5.1.1/plone/app/event/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5435 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15434 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     9719 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2965 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      605 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/formatted_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1001 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/formatted_date.py
--rw-r--r--   0 maurits    (501) staff       (20)      726 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/formatted_start_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)      550 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/leadimage_viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.834488 plone.app.event-5.1.1/plone/app/event/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      349 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/resources/calendar.svg
--rw-r--r--   0 maurits    (501) staff       (20)     3726 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/browser/resources/event.js
--rw-r--r--   0 maurits    (501) staff       (20)     2121 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.837218 plone.app.event-5.1.1/plone/app/event/dx/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    14257 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1981 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      585 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/ical.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/dx/traverser.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.839065 plone.app.event-5.1.1/plone/app/event/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      430 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/ical/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3135 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/ical/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    14653 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/ical/exporter.py
--rw-r--r--   0 maurits    (501) staff       (20)    14459 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/ical/importer.py
--rw-r--r--   0 maurits    (501) staff       (20)      350 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      171 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.841946 plone.app.event-5.1.1/plone/app/event/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      836 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/portlet_calendar.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11194 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     3357 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/portlet_events.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9912 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/portlets/portlet_events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.803759 plone.app.event-5.1.1/plone/app/event/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.846263 plone.app.event-5.1.1/plone/app/event/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     2651 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      357 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      321 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/plone.app.event-default.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      479 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      328 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.847712 plone.app.event-5.1.1/plone/app/event/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)      355 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.848682 plone.app.event-5.1.1/plone/app/event/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      181 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.849173 plone.app.event-5.1.1/plone/app/event/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2850 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     6714 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      567 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/recurrence.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     3694 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.857342 plone.app.event-5.1.1/plone/app/event/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      898 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/INACTIVE_test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5753 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/base_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/icaltest.ics
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/icaltest2.ics
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.858329 plone.app.event-5.1.1/plone/app/event/tests/javascripts/
--rw-r--r--   0 maurits    (501) staff       (20)    23860 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/javascripts/test_event.html
--rw-r--r--   0 maurits    (501) staff       (20)      715 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/javascripts/test_event.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.859251 plone.app.event-5.1.1/plone/app/event/tests/qunit/
--rw-r--r--   0 maurits    (501) staff       (20)     3952 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/qunit/qunit.css
--rw-r--r--   0 maurits    (501) staff       (20)    37060 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/qunit/qunit.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.860334 plone.app.event-5.1.1/plone/app/event/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     6114 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/robot/test_event_roundtrip.robot
--rw-r--r--   0 maurits    (501) staff       (20)      633 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)    35328 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_base_module.py
--rw-r--r--   0 maurits    (501) staff       (20)      773 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    22380 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_dx_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     6395 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     4982 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     2075 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3583 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_ical_import.py
--rw-r--r--   0 maurits    (501) staff       (20)    19302 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_icalendar.py
--rw-r--r--   0 maurits    (501) staff       (20)    10307 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     8861 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_portlet_events.py
--rw-r--r--   0 maurits    (501) staff       (20)    13916 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      544 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/tests/test_search.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.861635 plone.app.event-5.1.1/plone/app/event/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      969 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3415 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/upgrades/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     1261 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/plone/app/event/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:07:57.822683 plone.app.event-5.1.1/plone.app.event.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    63963 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4236 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      705 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:07:57.000000 plone.app.event-5.1.1/plone.app.event.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3930 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-10-06 22:07:57.864036 plone.app.event-5.1.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2593 2023-10-06 22:07:56.000000 plone.app.event-5.1.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.222715 plone.app.event-5.1.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    58418 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18099 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    64112 2024-04-16 19:33:06.222303 plone.app.event-5.1.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      587 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.187437 plone.app.event-5.1.2/docs/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.188774 plone.app.event-5.1.2/docs/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/base.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.190353 plone.app.event-5.1.2/docs/api/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_listing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_summary.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_view.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/formatted_date.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/leadimage_viewlet.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.191279 plone.app.event-5.1.2/docs/api/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)      118 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      119 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/traverser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.191889 plone.app.event-5.1.2/docs/api/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/ical/exporter.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/ical/importer.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      113 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/recurrence.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5633 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/architectural-overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3464 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/designchoices.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10346 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/development.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1589 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2839 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/installation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      884 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.192173 plone.app.event-5.1.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.194783 plone.app.event-5.1.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.197856 plone.app.event-5.1.2/plone/app/event/
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    33259 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.202027 plone.app.event-5.1.2/plone/app/event/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3398 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5435 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15434 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9719 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      605 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3228 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1001 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_date.py
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_start_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/leadimage_viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.202585 plone.app.event-5.1.2/plone/app/event/browser/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/resources/calendar.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     3726 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/resources/event.js
+-rw-r--r--   0 maurits    (501) staff       (20)     2121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.204358 plone.app.event-5.1.2/plone/app/event/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14485 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1981 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/ical.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/traverser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.205649 plone.app.event-5.1.2/plone/app/event/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      430 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3135 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    14653 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/exporter.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14459 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/importer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      350 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      171 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.207483 plone.app.event-5.1.2/plone/app/event/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      836 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11194 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3357 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9912 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.180886 plone.app.event-5.1.2/plone/app/event/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.210110 plone.app.event-5.1.2/plone/app/event/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     2651 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/plone.app.event-default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      479 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      328 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.211363 plone.app.event-5.1.2/plone/app/event/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      355 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.211947 plone.app.event-5.1.2/plone/app/event/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.212284 plone.app.event-5.1.2/plone/app/event/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2850 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     6714 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      567 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/recurrence.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2462 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3694 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.217607 plone.app.event-5.1.2/plone/app/event/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      898 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/INACTIVE_test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5841 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/base_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2201 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/icaltest.ics
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/icaltest2.ics
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.218341 plone.app.event-5.1.2/plone/app/event/tests/javascripts/
+-rw-r--r--   0 maurits    (501) staff       (20)    23860 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.html
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.218957 plone.app.event-5.1.2/plone/app/event/tests/qunit/
+-rw-r--r--   0 maurits    (501) staff       (20)     3952 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.css
+-rw-r--r--   0 maurits    (501) staff       (20)    37060 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.219853 plone.app.event-5.1.2/plone/app/event/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     6114 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/robot/test_event_roundtrip.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      633 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35328 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_base_module.py
+-rw-r--r--   0 maurits    (501) staff       (20)      773 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22404 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_dx_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6395 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4982 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2075 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3585 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_ical_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19302 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_icalendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10307 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11112 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_portlet_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13916 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      544 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_search.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.220781 plone.app.event-5.1.2/plone/app/event/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3415 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1261 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.221154 plone.app.event-5.1.2/plone.app.event.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    64112 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4236 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4300 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:33:06.222792 plone.app.event-5.1.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2613 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/setup.py
```

### Comparing `plone.app.event-5.1.1/CHANGES.rst` & `plone.app.event-5.1.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Fix calculation of eventaccessor urls @1letter (#387)
+
+
 5.1.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Require setuptools 68.2 or higher for building the package.
@@ -881,15 +890,15 @@
 - Remove ``data_postprocessing`` logic, which was handling ``open_end`` and
   ``whole_day`` events and was manipulating the object on form submission.
   Instead, just adapt start/end dates on indexing and when accessing them via
   ``IEventAccessor``.
   [thet]
 
 - Remove the ``plone.app.event.EventTypes`` vocabulary, which relied on
-  temporaily creating types. It's used for importing ical files. It should be
+  temporarily creating types. It's used for importing ical files. It should be
   possible to figure out, which types might suitable for creating events from
   ical VEVENT entries.
   [thet]
 
 - No need to return DateTime objects for the indexer.
   Products.DateRecurringIndex works with Python datetime objects.
   [thet]
@@ -1168,15 +1177,15 @@
 
 - Allow query parameters for timezone vocabularies for filtering. Create the
   "Timezones" vocabulary from SimpleTerm objects with a value and title set
   for better support with plone.app.widgets AjaxSelectWidget.
   [thet]
 
 - Remove "ploneintegration" from setuptools extra section and GenericSetup
-  profile. PLEASE UPDATE YOUR INSTALLTIONS, to use Archetypes or Dexterity
+  profile. PLEASE UPDATE YOUR INSTALLATIONS, to use Archetypes or Dexterity
   instead and to use plone.app.portlets 2.5a1! This change makes it easier for
   Plone to integrate plone.app.event.
   [thet]
 
 
 1.0.5 (2014-02-11)
 ------------------
```

### Comparing `plone.app.event-5.1.1/LICENSE.GPL` & `plone.app.event-5.1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/LICENSE.rst` & `plone.app.event-5.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/PKG-INFO` & `plone.app.event-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.1.1
+Version: 5.1.2
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,14 +56,15 @@
 Requires-Dist: z3c.form>=3.2.1
 Requires-Dist: Zope
 Provides-Extra: test
 Requires-Dist: plone.app.robotframework; extra == "test"
 Requires-Dist: plone.app.testing[robot]; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: robotsuite; extra == "test"
+Requires-Dist: lxml; extra == "test"
 
 plone.app.event
 ===============
 
 ``plone.app.event`` is the calendaring framework for Plone. 
 
 It provides 
@@ -154,14 +155,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Fix calculation of eventaccessor urls @1letter (#387)
+
+
 5.1.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Require setuptools 68.2 or higher for building the package.
@@ -1031,15 +1041,15 @@
 - Remove ``data_postprocessing`` logic, which was handling ``open_end`` and
   ``whole_day`` events and was manipulating the object on form submission.
   Instead, just adapt start/end dates on indexing and when accessing them via
   ``IEventAccessor``.
   [thet]
 
 - Remove the ``plone.app.event.EventTypes`` vocabulary, which relied on
-  temporaily creating types. It's used for importing ical files. It should be
+  temporarily creating types. It's used for importing ical files. It should be
   possible to figure out, which types might suitable for creating events from
   ical VEVENT entries.
   [thet]
 
 - No need to return DateTime objects for the indexer.
   Products.DateRecurringIndex works with Python datetime objects.
   [thet]
@@ -1318,15 +1328,15 @@
 
 - Allow query parameters for timezone vocabularies for filtering. Create the
   "Timezones" vocabulary from SimpleTerm objects with a value and title set
   for better support with plone.app.widgets AjaxSelectWidget.
   [thet]
 
 - Remove "ploneintegration" from setuptools extra section and GenericSetup
-  profile. PLEASE UPDATE YOUR INSTALLTIONS, to use Archetypes or Dexterity
+  profile. PLEASE UPDATE YOUR INSTALLATIONS, to use Archetypes or Dexterity
   instead and to use plone.app.portlets 2.5a1! This change makes it easier for
   Plone to integrate plone.app.event.
   [thet]
 
 
 1.0.5 (2014-02-11)
 ------------------
```

### Comparing `plone.app.event-5.1.1/README.rst` & `plone.app.event-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/docs/architectural-overview.rst` & `plone.app.event-5.1.2/docs/architectural-overview.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/docs/designchoices.rst` & `plone.app.event-5.1.2/docs/designchoices.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/docs/development.rst` & `plone.app.event-5.1.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/docs/index.rst` & `plone.app.event-5.1.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - Icalendar import,
     - Better calendar and events portlets,
     - An event listing and event detail view.
 
 
     It was developed with these goals in mind:
 
-    - Encapsulation and independence: All event related code should reside in a single package. Relevant, re-usable functionality is split to separate packages.  Plone's dependencies on calendar related code should be reduced to a minimum. plone.app.event should be able to be deinstalled from Plone.
+    - Encapsulation and independence: All event related code should reside in a single package. Relevant, reusable functionality is split to separate packages.  Plone's dependencies on calendar related code should be reduced to a minimum. plone.app.event should be able to be deinstalled from Plone.
 
     - Dexterity and Archetypes support: plone.app.event should provide Dexterity behaviors, which can be used in Dexterity types and an ATEvent content type (factored out from ATContentTypes). For a Dexterity event type, use plone.app.contenttypes 1.1 or newer.
 
     - Standards compliance: We support the icalendar standard (`RFC5545 <http://tools.ietf.org/html/rfc5545>`_) including recurrence.
 
     - Recurring events based on the RFC5545 standard.
```

### Comparing `plone.app.event-5.1.1/docs/installation.rst` & `plone.app.event-5.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/docs/tests.rst` & `plone.app.event-5.1.2/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/base.py` & `plone.app.event-5.1.2/plone/app/event/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_listing.pt` & `plone.app.event-5.1.2/plone/app/event/browser/event_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_listing.py` & `plone.app.event-5.1.2/plone/app/event/browser/event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_summary.pt` & `plone.app.event-5.1.2/plone/app/event/browser/event_summary.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_summary.py` & `plone.app.event-5.1.2/plone/app/event/browser/event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_view.pt` & `plone.app.event-5.1.2/plone/app/event/browser/event_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/event_view.py` & `plone.app.event-5.1.2/plone/app/event/browser/event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/formatted_date.pt` & `plone.app.event-5.1.2/plone/app/event/browser/formatted_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/formatted_date.py` & `plone.app.event-5.1.2/plone/app/event/browser/formatted_date.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/formatted_start_date.pt` & `plone.app.event-5.1.2/plone/app/event/browser/formatted_start_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/leadimage_viewlet.py` & `plone.app.event-5.1.2/plone/app/event/browser/leadimage_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/browser/resources/event.js` & `plone.app.event-5.1.2/plone/app/event/browser/resources/event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/dx/behaviors.py` & `plone.app.event-5.1.2/plone/app/event/dx/behaviors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Behaviors to enable calendarish event extension to dexterity content types.
 """
+
 from plone.app.dexterity.behaviors.metadata import ICategorization
 from plone.app.event import _
 from plone.app.event.base import default_end as default_end_dt
 from plone.app.event.base import default_start as default_start_dt
 from plone.app.event.base import default_timezone
 from plone.app.event.base import DT
 from plone.app.event.base import dt_end_of_day
@@ -57,15 +58,14 @@
 @provider(IContextAwareDefaultFactory)
 def default_end(context):
     """Provide default end for the form."""
     return default_end_dt(context)
 
 
 class IEventBasic(model.Schema, IDXEvent):
-
     """Basic event schema."""
 
     start = schema.Datetime(
         title=_("label_event_start", default="Event Starts"),
         description=_(
             "help_event_start", default="Date and Time, when the event begins."
         ),
@@ -125,15 +125,14 @@
                     "error_end_must_be_after_start_date",
                     default="End date must be after start date.",
                 )
             )
 
 
 class IEventRecurrence(model.Schema, IDXEventRecurrence):
-
     """Recurring Event Schema."""
 
     recurrence = schema.Text(
         title=_("label_event_recurrence", default="Recurrence"),
         description=_(
             "help_event_recurrence", default="Define the event recurrence rule."
         ),
@@ -147,43 +146,40 @@
         first_day=first_weekday_sun0,
         show_repeat_forever=False,
         klass="event_recurrence",
     )
 
 
 class IEventLocation(model.Schema):
-
     """Event Location Schema."""
 
     location = schema.TextLine(
         title=_("label_event_location", default="Location"),
         description=_("help_event_location", default="Location of the event."),
         required=False,
         default=None,
     )
     directives.widget("location", TextFieldWidget, klass="event_location")
 
 
 class IEventAttendees(model.Schema):
-
     """Event Attendees Schema."""
 
     attendees = schema.Tuple(
         title=_("label_event_attendees", default="Attendees"),
         description=_("help_event_attendees", default="List of attendees."),
         value_type=schema.TextLine(),
         required=False,
         missing_value=(),
         default=(),
     )
     directives.widget("attendees", TextLinesFieldWidget, klass="event_attendees")
 
 
 class IEventContact(model.Schema):
-
     """Event Contact Schema."""
 
     contact_name = schema.TextLine(
         title=_("label_event_contact_name", default="Contact Name"),
         description=_(
             "help_event_contact_name",
             default="Name of a person to contact about this event.",
@@ -278,15 +274,14 @@
 
 # Object adapters
 
 
 @adapter(IDXEvent)
 @implementer(IEventAccessor)
 class EventAccessor:
-
     """Generic event accessor adapter implementation for Dexterity content
     objects.
     """
 
     def __init__(self, context):
         object.__setattr__(self, "context", context)
 
@@ -340,15 +335,20 @@
 
     @property
     def uid(self):
         return IUUID(self.context, None)
 
     @property
     def url(self):
-        return safe_text(self.context.absolute_url())
+        """need to lookup globalrequest in order to calculate
+        correct URL during cached lookup (eg. in event portlet renderer)
+        """
+        request = getRequest()
+        absolute_url = request.physicalPathToURL(self.context.getPhysicalPath())
+        return absolute_url
 
     @property
     def created(self):
         return utc(self.context.creation_date)
 
     @property
     def duration(self):
```

### Comparing `plone.app.event-5.1.1/plone/app/event/dx/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/dx/ical.zcml` & `plone.app.event-5.1.2/plone/app/event/dx/ical.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/dx/traverser.py` & `plone.app.event-5.1.2/plone/app/event/dx/traverser.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/ical/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/ical/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/ical/exporter.py` & `plone.app.event-5.1.2/plone/app/event/ical/exporter.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/ical/importer.py` & `plone.app.event-5.1.2/plone/app/event/ical/importer.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/__init__.py` & `plone.app.event-5.1.2/plone/app/event/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/portlet_calendar.pt` & `plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/portlet_calendar.py` & `plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/portlet_events.pt` & `plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/portlets/portlet_events.py` & `plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/profiles/default/actions.xml` & `plone.app.event-5.1.2/plone/app/event/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/profiles/default/portlets.xml` & `plone.app.event-5.1.2/plone/app/event/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml` & `plone.app.event-5.1.2/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/recurrence.py` & `plone.app.event-5.1.2/plone/app/event/recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/recurrence.zcml` & `plone.app.event-5.1.2/plone/app/event/recurrence.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/setuphandlers.py` & `plone.app.event-5.1.2/plone/app/event/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/testing.py` & `plone.app.event-5.1.2/plone/app/event/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/INACTIVE_test_robot.py` & `plone.app.event-5.1.2/plone/app/event/tests/INACTIVE_test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/base_setup.py` & `plone.app.event-5.1.2/plone/app/event/tests/base_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
     def make_dates(self):
         tz = pytz.timezone(TEST_TIMEZONE)
         now = self.now = patched_now()
         self.tomorrow = tz.normalize(now + timedelta(days=1))
         past = self.past = tz.normalize(now - timedelta(days=10))
         future = self.future = tz.normalize(now + timedelta(days=10))
         far = self.far = tz.normalize(now + timedelta(days=30))
+        scifi = self.scifi = tz.normalize(now + 50 * timedelta(days=365))
         duration = self.duration = timedelta(hours=1)
-        return (now, past, future, far, duration)
+        return (now, past, future, far, duration, scifi)
 
     def setUp(self):
         """Construct sample contents.
 
         These are all events:
 
         'Long Event: 2013-04-25T10:00:00+02:00 - 2013-06-04T10:00:00+02:00'
@@ -68,15 +69,15 @@
         """
         self.portal = self.layer["portal"]
         self.app = self.layer["app"]
         self.request = self.layer["request"]
         set_browserlayer(self.request)
         set_timezone(TEST_TIMEZONE)
 
-        now, past, future, far, duration = self.make_dates()
+        now, past, future, far, duration, scifi = self.make_dates()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         workflow = getToolByName(self.portal, "portal_workflow")
         workflow.setDefaultChain("simple_publication_workflow")
 
         factory = self.event_factory
         self.past_event = factory(
             container=self.portal,
```

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/icaltest.ics` & `plone.app.event-5.1.2/plone/app/event/tests/icaltest.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/icaltest2.ics` & `plone.app.event-5.1.2/plone/app/event/tests/icaltest2.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/javascripts/test_event.html` & `plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.html`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/javascripts/test_event.js` & `plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/qunit/qunit.css` & `plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/qunit/qunit.js` & `plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/robot/test_event_roundtrip.robot` & `plone.app.event-5.1.2/plone/app/event/tests/robot/test_event_roundtrip.robot`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/robot/variables.py` & `plone.app.event-5.1.2/plone/app/event/tests/robot/variables.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_base_module.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_base_module.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_catalog.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_dx_behaviors.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_dx_behaviors.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,25 +97,25 @@
 
         self.browser.open(
             "{}/{}".format(
                 self.portal.absolute_url(), "++add++plone.app.event.dx.event"
             )
         )
 
-        self.browser.getControl(
-            name="form.widgets.IDublinCore.title"
-        ).value = "TestEvent"
+        self.browser.getControl(name="form.widgets.IDublinCore.title").value = (
+            "TestEvent"
+        )
 
         # TODO: these values are simply not set in the pat-pickadate pattern.
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.start"
-        ).value = "2014-03-30"
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.end"
-        ).value = "2014-03-31"
+        self.browser.getControl(name="form.widgets.IEventBasic.start").value = (
+            "2014-03-30"
+        )
+        self.browser.getControl(name="form.widgets.IEventBasic.end").value = (
+            "2014-03-31"
+        )
 
         self.browser.getControl("Save").click()
 
         # CHECK VALUES
         #
         # TODO: fix all defaults
         event = self.portal["testevent"]
@@ -161,25 +161,25 @@
         """
 
         #
         # ADD
         #
         self.browser.open(self.portal.absolute_url())
         self.browser.getLink("plone.app.event.dx.event").click()
-        self.browser.getControl(
-            name="form.widgets.IDublinCore.title"
-        ).value = "TestEvent"
+        self.browser.getControl(name="form.widgets.IDublinCore.title").value = (
+            "TestEvent"
+        )
 
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.start"
-        ).value = "2014-03-30T03:51"
+        self.browser.getControl(name="form.widgets.IEventBasic.start").value = (
+            "2014-03-30T03:51"
+        )
 
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.end"
-        ).value = "2014-03-30T04:51"
+        self.browser.getControl(name="form.widgets.IEventBasic.end").value = (
+            "2014-03-30T04:51"
+        )
 
         self.browser.getControl("Save").click()
 
         # CHECK VALUES
         #
         self.assertTrue(self.browser.url.endswith("testevent/view"))
         self.assertTrue("TestEvent" in self.browser.contents)
@@ -187,21 +187,21 @@
 
         #
         # EDIT
         #
         testevent = self.portal.testevent
         self.browser.open("%s/@@edit" % testevent.absolute_url())
 
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.start"
-        ).value = "2014-03-31T03:51"
+        self.browser.getControl(name="form.widgets.IEventBasic.start").value = (
+            "2014-03-31T03:51"
+        )
 
-        self.browser.getControl(
-            name="form.widgets.IEventBasic.end"
-        ).value = "2014-03-31T04:51"
+        self.browser.getControl(name="form.widgets.IEventBasic.end").value = (
+            "2014-03-31T04:51"
+        )
 
         self.browser.getControl("Save").click()
 
         #
         # EDIT AGAIN
         #
         testevent = self.portal.testevent
@@ -570,23 +570,23 @@
             end=tz.localize(datetime(2011, 11, 11, 12, 0)),
         )
 
         # Fill the field values into the annotation storage
         ann = IAnnotations(e1)
         ann["plone.app.event.dx.behaviors.IEventLocation.location"] = self.location
         ann["plone.app.event.dx.behaviors.IEventAttendees.attendees"] = self.attendees
-        ann[
-            "plone.app.event.dx.behaviors.IEventContact.contact_email"
-        ] = self.contact_email
-        ann[
-            "plone.app.event.dx.behaviors.IEventContact.contact_name"
-        ] = self.contact_name
-        ann[
-            "plone.app.event.dx.behaviors.IEventContact.contact_phone"
-        ] = self.contact_phone
+        ann["plone.app.event.dx.behaviors.IEventContact.contact_email"] = (
+            self.contact_email
+        )
+        ann["plone.app.event.dx.behaviors.IEventContact.contact_name"] = (
+            self.contact_name
+        )
+        ann["plone.app.event.dx.behaviors.IEventContact.contact_phone"] = (
+            self.contact_phone
+        )
         ann["plone.app.event.dx.behaviors.IEventContact.event_url"] = self.event_url
         ann["plone.app.event.dx.behaviors.IEventSummary.text"] = RichTextValue(
             raw=self.text
         )
 
         # All behavior-related fields are not set yet
         self.assertEqual(e1.location, None)
@@ -620,17 +620,17 @@
         )
 
         # Fill the field values into the annotation storage
         ann = IAnnotations(e1)
         ann["plone.app.event.dx.behaviors.IEventLocation.location"] = (
             self.location + "X"
         )
-        ann[
-            "plone.app.event.dx.behaviors.IEventAttendees.attendees"
-        ] = self.attendees + ("Paula",)
+        ann["plone.app.event.dx.behaviors.IEventAttendees.attendees"] = (
+            self.attendees + ("Paula",)
+        )
         ann["plone.app.event.dx.behaviors.IEventContact.contact_email"] = (
             self.contact_email + "X"
         )
         ann["plone.app.event.dx.behaviors.IEventContact.contact_name"] = (
             self.contact_name + "X"
         )
         ann["plone.app.event.dx.behaviors.IEventContact.contact_phone"] = (
```

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_event_listing.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_event_summary.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_event_view.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_ical_import.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_ical_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,12 +81,12 @@
         self.browser.getControl("Confirm action").click()
 
         # Set it to a file url.
         self.browser.open(f1_url + "/ical_import_settings")
         self.assertIn(
             "URL to an external icalendar resource file", self.browser.contents
         )
-        self.browser.getControl(
-            name="form.widgets.ical_url"
-        ).value = "file:///tmp/test.ical"
+        self.browser.getControl(name="form.widgets.ical_url").value = (
+            "file:///tmp/test.ical"
+        )
         self.browser.getControl(name="form.buttons.save").click()
         self.assertIn("URLs with file: are not allowed.", self.browser.contents)
```

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_icalendar.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_icalendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_portlet_calendar.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_portlet_events.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_portlet_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from datetime import timedelta
 from plone.app.event.base import localized_now
 from plone.app.event.portlets import portlet_events
 from plone.app.event.testing import PAEvent_INTEGRATION_TESTING
+from plone.app.event.testing import PAEventDX_FUNCTIONAL_TESTING
 from plone.app.event.testing import PAEventDX_INTEGRATION_TESTING
 from plone.app.event.testing import set_env_timezone
 from plone.app.event.testing import set_timezone
+from plone.app.event.tests.base_setup import AbstractSampleDataEvents
 from plone.app.portlets.storage import PortletAssignmentMapping
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.z3cform.interfaces import IPloneFormLayer
 from plone.dexterity.utils import createContentInContainer
 from plone.portlets.interfaces import IPortletAssignment
 from plone.portlets.interfaces import IPortletDataProvider
 from plone.portlets.interfaces import IPortletManager
 from plone.portlets.interfaces import IPortletRenderer
 from plone.portlets.interfaces import IPortletType
+from plone.testing.zope import Browser
 from Products.CMFCore.utils import getToolByName
 from Products.GenericSetup.utils import _getDottedName
 from zExceptions import Unauthorized
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component.hooks import setHooks
 from zope.component.hooks import setSite
@@ -244,7 +247,69 @@
 
     def test_portlet_event_renderer__listing_link(self):
         r = self.renderer(assignment=portlet_events.Assignment(count=5))
         r.update()
         rd = r.render()
         self.assertTrue("?mode=future" in rd)
         self.assertTrue("?mode=past" in rd)
+
+
+class FunctionalTestCachedPortletEvents(AbstractSampleDataEvents):
+    layer = PAEventDX_FUNCTIONAL_TESTING
+
+    def setUp(self):
+        super().setUp()
+
+        # a event in the future is needed, show in the portlet
+
+        self.scifi_event = self.event_factory(
+            container=self.portal.sub,
+            id="scifi_event",
+            title="Long Event in the future",
+            start=self.scifi,
+            location="My Home",
+        )
+        workflow = getToolByName(self.portal, "portal_workflow")
+        workflow.setDefaultChain("simple_publication_workflow")
+        workflow.doActionFor(self.scifi_event, "publish")
+        self.scifi_event.reindexObject()
+
+    def anonymous_browser(self):
+        """Browser of anonymous user"""
+        import transaction
+
+        transaction.commit()
+        browser = Browser(self.layer["app"])
+        browser.handleErrors = False
+        return browser
+
+    def test_event_portlet_links(self):
+        from io import StringIO
+        from lxml import etree
+
+        # first request, events not in ram cache
+        browser = self.anonymous_browser()
+        browser.open(f"{self.portal.absolute_url()}")
+        tree = etree.parse(StringIO(browser.contents), etree.HTMLParser())
+        result = tree.xpath("//li[contains(@class,'portletItem even')]/a/@href")
+
+        self.assertEqual(
+            result[0],
+            "http://nohost/plone/sub/scifi_event",
+            "URL of Event is wrong",
+        )
+
+        # second request, events are in ram cache
+        browser = self.anonymous_browser()
+        browser.open(f"{self.portal.absolute_url()}")
+        tree = etree.parse(StringIO(browser.contents), etree.HTMLParser())
+        result = tree.xpath("//li[contains(@class,'portletItem even')]/a/@href")
+
+        self.assertEqual(
+            result[0],
+            "http://nohost/plone/sub/scifi_event",
+            "URL of Event, calculate from ram cache, is wrong",
+        )
+
+    def tearDown(self):
+        if "scifi_event" in self.portal.sub.keys():
+            del self.portal.sub["scifi_event"]
```

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_recurrence.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/tests/test_search.py` & `plone.app.event-5.1.2/plone/app/event/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/upgrades/configure.zcml` & `plone.app.event-5.1.2/plone/app/event/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/upgrades/upgrades.py` & `plone.app.event-5.1.2/plone/app/event/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone/app/event/vocabularies.py` & `plone.app.event-5.1.2/plone/app/event/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone.app.event.egg-info/PKG-INFO` & `plone.app.event-5.1.2/plone.app.event.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.1.1
+Version: 5.1.2
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,14 +56,15 @@
 Requires-Dist: z3c.form>=3.2.1
 Requires-Dist: Zope
 Provides-Extra: test
 Requires-Dist: plone.app.robotframework; extra == "test"
 Requires-Dist: plone.app.testing[robot]; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: robotsuite; extra == "test"
+Requires-Dist: lxml; extra == "test"
 
 plone.app.event
 ===============
 
 ``plone.app.event`` is the calendaring framework for Plone. 
 
 It provides 
@@ -154,14 +155,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Fix calculation of eventaccessor urls @1letter (#387)
+
+
 5.1.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Require setuptools 68.2 or higher for building the package.
@@ -1031,15 +1041,15 @@
 - Remove ``data_postprocessing`` logic, which was handling ``open_end`` and
   ``whole_day`` events and was manipulating the object on form submission.
   Instead, just adapt start/end dates on indexing and when accessing them via
   ``IEventAccessor``.
   [thet]
 
 - Remove the ``plone.app.event.EventTypes`` vocabulary, which relied on
-  temporaily creating types. It's used for importing ical files. It should be
+  temporarily creating types. It's used for importing ical files. It should be
   possible to figure out, which types might suitable for creating events from
   ical VEVENT entries.
   [thet]
 
 - No need to return DateTime objects for the indexer.
   Products.DateRecurringIndex works with Python datetime objects.
   [thet]
@@ -1318,15 +1328,15 @@
 
 - Allow query parameters for timezone vocabularies for filtering. Create the
   "Timezones" vocabulary from SimpleTerm objects with a value and title set
   for better support with plone.app.widgets AjaxSelectWidget.
   [thet]
 
 - Remove "ploneintegration" from setuptools extra section and GenericSetup
-  profile. PLEASE UPDATE YOUR INSTALLTIONS, to use Archetypes or Dexterity
+  profile. PLEASE UPDATE YOUR INSTALLATIONS, to use Archetypes or Dexterity
   instead and to use plone.app.portlets 2.5a1! This change makes it easier for
   Plone to integrate plone.app.event.
   [thet]
 
 
 1.0.5 (2014-02-11)
 ------------------
```

### Comparing `plone.app.event-5.1.1/plone.app.event.egg-info/SOURCES.txt` & `plone.app.event-5.1.2/plone.app.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.1/plone.app.event.egg-info/requires.txt` & `plone.app.event-5.1.2/plone.app.event.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,7 +34,8 @@
 Zope
 
 [test]
 plone.app.robotframework
 plone.app.testing[robot]
 plone.testing
 robotsuite
+lxml
```

### Comparing `plone.app.event-5.1.1/pyproject.toml` & `plone.app.event-5.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 [build-system]
-requires = ["setuptools>=68.2", "wheel"]
+requires = ["setuptools>=68.2"]
 
 [tool.towncrier]
 directory = "news/"
 filename = "CHANGES.rst"
 title_format = "{version} ({project_date})"
 underlines = ["-", ""]
 
@@ -36,20 +36,44 @@
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "tests"
 name = "Tests"
 showcontent = true
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  towncrier_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.isort]
 profile = "plone"
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  isort_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.black]
 target-version = ["py38"]
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  black_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.codespell]
 ignore-words-list = "discreet,"
 skip = "*.po,"
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  codespell_ignores = "foo,bar"
@@ -101,15 +125,14 @@
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
-#  """
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
     ".meta.toml",
     ".pre-commit-config.yaml",
```

### Comparing `plone.app.event-5.1.1/setup.py` & `plone.app.event-5.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.1.1"
+version = "5.1.2"
 
 
 long_description = "\n\n".join(
     [
         Path("README.rst").read_text(),
         (Path(".") / "docs" / "installation.rst").read_text(),
         Path("CHANGES.rst").read_text(),
@@ -81,10 +81,11 @@
     ],
     extras_require={
         "test": [
             "plone.app.robotframework",
             "plone.app.testing [robot]",
             "plone.testing",
             "robotsuite",
+            "lxml",
         ],
     },
 )
```

