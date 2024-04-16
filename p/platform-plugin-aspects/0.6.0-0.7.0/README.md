# Comparing `tmp/platform-plugin-aspects-0.6.0.tar.gz` & `tmp/platform_plugin_aspects-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-plugin-aspects-0.6.0.tar", last modified: Tue Apr  9 16:29:01 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.7.0.tar", last modified: Tue Apr 16 16:07:41 2024, max compression
```

## Comparing `platform-plugin-aspects-0.6.0.tar` & `platform_plugin_aspects-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.116888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.116888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.231516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.235516 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:41.000000 platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 16:07:41.239516 platform_plugin_aspects-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-16 16:07:37.000000 platform_plugin_aspects-0.7.0/setup.py
```

### Comparing `platform-plugin-aspects-0.6.0/CHANGELOG.rst` & `platform_plugin_aspects-0.7.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.0 - 2024-04-12
+******************
+
+Added
+=====
+
+* Add endpoint for fetchGuestToken
+
 0.6.0 - 2024-04-08
 ******************
 
 Added
 =====
 
 * Allow to embed translated Superset Dashboards.
```

### Comparing `platform-plugin-aspects-0.6.0/LICENSE` & `platform_plugin_aspects-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """
 platform_plugin_aspects Django application initialization.
 """
 
 from django.apps import AppConfig
-from edx_django_utils.plugins import PluginSettings, PluginSignals
+from edx_django_utils.plugins import PluginSettings, PluginSignals, PluginURLs
 
 
 class PlatformPluginAspectsConfig(AppConfig):
     """
     Configuration for the aspects Django application.
     """
 
     name = "platform_plugin_aspects"
 
     plugin_app = {
+        PluginURLs.CONFIG: {
+            "lms.djangoapp": {
+                PluginURLs.NAMESPACE: "",
+                PluginURLs.REGEX: r"^aspects/",
+                PluginURLs.RELATIVE_PATH: "urls",
+            },
+        },
         PluginSettings.CONFIG: {
             "lms.djangoapp": {
                 "production": {PluginSettings.RELATIVE_PATH: "settings.production"},
                 "common": {PluginSettings.RELATIVE_PATH: "settings.common"},
             },
             "cms.djangoapp": {
                 "production": {PluginSettings.RELATIVE_PATH: "settings.production"},
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/extensions/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 from web_fragments.fragment import Fragment
 
 from platform_plugin_aspects.utils import _, generate_superset_context, get_model
 
 TEMPLATE_ABSOLUTE_PATH = "/instructor_dashboard/"
 BLOCK_CATEGORY = "aspects"
 
-ASPECTS_SECURITY_FILTERS_FORMAT = [
-    "org = '{course.org}'",
-    "course_name = '{course.display_name}'",
-    "course_run = '{course.id.run}'",
-]
-
 
 class AddSupersetTab(PipelineStep):
     """
     Add superset tab to instructor dashboard.
     """
 
     def run_filter(
@@ -32,45 +26,42 @@
         """Execute filter that modifies the instructor dashboard context.
         Args:
             context (dict): the context for the instructor dashboard.
             _ (str): instructor dashboard template name.
         """
         course = context["course"]
         dashboards = settings.ASPECTS_INSTRUCTOR_DASHBOARDS
-        extra_filters_format = settings.SUPERSET_EXTRA_FILTERS_FORMAT
-
-        filters = ASPECTS_SECURITY_FILTERS_FORMAT + extra_filters_format
 
         user = get_current_user()
 
         user_language = (
             get_model("user_preference").get_value(user, "pref-lang") or "en_US"
         )
         formatted_language = user_language.replace("-", "_")
         if formatted_language not in settings.SUPERSET_DASHBOARD_LOCALES:
             formatted_language = "en_US"
 
+        context["course_id"] = course.id
         context = generate_superset_context(
             context,
-            user,
             dashboards=dashboards,
-            filters=filters,
             language=formatted_language,
         )
 
         template = Template(self.resource_string("static/html/superset.html"))
         html = template.render(Context(context))
         frag = Fragment(html)
         frag.add_css(self.resource_string("static/css/superset.css"))
         frag.add_javascript(self.resource_string("static/js/embed_dashboard.js"))
         section_data = {
             "fragment": frag,
             "section_key": BLOCK_CATEGORY,
             "section_display_name": _("Analytics"),
-            "course_id": str(course.id),
+            "course_id": str(context.get("course_id")),
+            "superset_guest_token_url": str(context.get("superset_guest_token_url")),
             "superset_url": str(context.get("superset_url")),
             "template_path_prefix": TEMPLATE_ABSOLUTE_PATH,
         }
         context["sections"].append(section_data)
         return {
             "context": context,
         }
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     from platform_plugin_aspects.tasks import (  # pylint: disable=import-outside-toplevel
         dump_course_to_clickhouse,
     )
 
     dump_course_to_clickhouse.delay(str(course_key))
 
 
-@receiver(post_save, sender=get_model("user_profile"))
 def on_user_profile_updated(  # pylint: disable=unused-argument  # pragma: no cover
     sender, instance, **kwargs
 ):
     """
     Receives post save signal and queues the dump job.
     """
     # import here, because signal is registered at startup, but items in tasks are not yet able to be loaded
@@ -49,15 +48,21 @@
     dump_data_to_clickhouse.delay(
         sink_module=sink.__module__,
         sink_name=sink.__class__.__name__,
         object_id=str(instance.id),
     )
 
 
-@receiver(post_save, sender=get_model("external_id"))
+# Connect the UserProfile.post_save signal handler only if we have a model to attach to.
+# (prevents celery errors during tests)
+_user_profile = get_model("user_profile")
+if _user_profile:
+    post_save.connect(on_user_profile_updated, sender=_user_profile)  # pragma: no cover
+
+
 def on_externalid_saved(  # pylint: disable=unused-argument  # pragma: no cover
     sender, instance, **kwargs
 ):
     """
     Receives post save signal and queues the dump job.
     """
     # import here, because signal is registered at startup, but items in tasks are not yet able to be loaded
@@ -69,14 +74,21 @@
     dump_data_to_clickhouse.delay(
         sink_module=sink.__module__,
         sink_name=sink.__class__.__name__,
         object_id=str(instance.id),
     )
 
 
+# Connect the ExternalId.post_save signal handler only if we have a model to attach to.
+# (prevents celery errors during tests)
+_external_id = get_model("external_id")
+if _external_id:
+    post_save.connect(on_externalid_saved, sender=_external_id)  # pragma: no cover
+
+
 @receiver(USER_RETIRE_LMS_MISC)
 def on_user_retirement(  # pylint: disable=unused-argument  # pragma: no cover
     sender, user, **kwargs
 ):
     """
     Receives a user retirement signal and queues the retire_user job.
     """
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/html/superset.html`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <h2>{{display_name}}</h2>
 
     {% if exception %}
     <p>{% trans 'Superset is not configured properly. Please contact your system administrator.'%}</p>
     <p>{{exception}}</p>
     {% elif not superset_dashboards %}
     <p>Dashboard UUID is not set. Please set the dashboard UUID in the Studio.</p>
-    {% elif superset_url and superset_token %} {% if xblock_id %}
+    {% elif superset_url and superset_guest_token_url %} {% if xblock_id %}
     <div class="superset-embedded-container" id="superset-embedded-container-{{xblock_id}}"></div>
     {% else %}
     <div class="aspects-tabs">
         {% for dashboard in superset_dashboards %}
         <div class="aspects-tab">
             {% if forloop.counter == 1 %}
             <input type="radio" id="tab-{{forloop.counter}}" name="tab-group-1" checked="checked" />
@@ -27,11 +27,11 @@
         {% endfor %}
     </div>
     {% endif %}
 
     <script type="text/javascript">
         window.superset_dashboards = {{superset_dashboards | safe }};
         window.superset_url = "{{superset_url}}";
-        window.superset_token = "{{superset_token}}";
+        window.superset_guest_token_url = "{{superset_guest_token_url}}";
     </script>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
 ********** {{{{ddiissppllaayy__nnaammee}}}} **********
 {% if exception %}
 {% trans 'Superset is not configured properly. Please contact your system
 administrator.'%}
 {{exception}}
 {% elif not superset_dashboards %}
 Dashboard UUID is not set. Please set the dashboard UUID in the Studio.
-{% elif superset_url and superset_token %} {% if xblock_id %}
+{% elif superset_url and superset_guest_token_url %} {% if xblock_id %}
 {% else %}
 {% for dashboard in superset_dashboards %}
 {% if forloop.counter == 1 %} #{% else %} o{% endif %} {{dashboard.name}}
 {% endfor %}
 {% endif %}
 {% endif %}
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/static/js/superset.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 /* Javascript for SupersetXBlock. */
 function SupersetXBlock(runtime, element, context) {
     const dashboard_uuid = context.dashboard_uuid;
     const superset_url = context.superset_url;
-    const superset_token = context.superset_token;
+    const superset_guest_token_url = runtime.handlerUrl(element, 'get_superset_guest_token');
     const xblock_id = context.xblock_id
 
     function initSuperset(supersetEmbeddedSdk) {
-        embedDashboard(dashboard_uuid, superset_url, superset_token, xblock_id);
+        embedDashboard(dashboard_uuid, superset_url, superset_guest_token_url, xblock_id);
     }
 
     if (typeof require === "function") {
         require(["supersetEmbeddedSdk"], function(supersetEmbeddedSdk) {
             window.supersetEmbeddedSdk = supersetEmbeddedSdk;
             initSuperset();
         });
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 
 from __future__ import annotations
 
 import logging
 import os
 import uuid
 from importlib import import_module
+from urllib.parse import urljoin
 
 from django.conf import settings
+from django.core.exceptions import ImproperlyConfigured
+from django.urls import reverse
+from requests.exceptions import HTTPError
 from supersetapiclient.client import SupersetClient
 from xblock.reference.user_service import XBlockUser
 
 logger = logging.getLogger(__name__)
 
 if settings.DEBUG:  # pragma: no cover
     os.environ["OAUTHLIB_INSECURE_TRANSPORT"] = "1"
@@ -22,122 +26,131 @@
 def _(text):
     """
     Define a dummy `gettext` replacement to make string extraction tools scrape strings marked for translation.
     """
     return text
 
 
-def generate_superset_context(  # pylint: disable=dangerous-default-value
+def generate_superset_context(
     context,
-    user,
     dashboards,
-    filters=[],
     language=None,
-):
+) -> dict:
     """
     Update context with superset token and dashboard id.
 
     Args:
-        context (dict): the context for the instructor dashboard. It must include a course object
+        context (dict): the context for the instructor dashboard. It must include a course_id.
         user (XBlockUser or User): the current user.
         superset_config (dict): superset config.
         dashboards (list): list of superset dashboard uuid.
         filters (list): list of filters to apply to the dashboard.
         language (str): the language code of the end user.
     """
-    course = context["course"]
+    course_id = context["course_id"]
     superset_config = settings.SUPERSET_CONFIG
 
     if language:
         for dashboard in dashboards:
-            if not dashboard["allow_translations"]:
+            if not dashboard.get("allow_translations"):
                 continue
             dashboard["slug"] = f"{dashboard['slug']}-{language}"
             dashboard["uuid"] = str(get_uuid5(dashboard["uuid"], language))
 
-    superset_token, dashboards = _generate_guest_token(
-        user=user,
-        course=course,
-        superset_config=superset_config,
-        dashboards=dashboards,
-        filters=filters,
+    superset_url = _fix_service_url(superset_config.get("service_url"))
+
+    # Use an absolute LMS URL here, just in case we're being rendered in an MFE.
+    guest_token_url = urljoin(
+        settings.LMS_ROOT_URL,
+        reverse(
+            "platform_plugin_aspects:superset_guest_token",
+            kwargs={"course_id": course_id},
+        ),
     )
 
-    if superset_token:
-        superset_url = _fix_service_url(superset_config.get("service_url"))
-        context.update(
-            {
-                "superset_token": superset_token,
-                "superset_dashboards": dashboards,
-                "superset_url": superset_url,
-            }
-        )
-    else:
-        context.update(
-            {
-                "exception": str(dashboards),
-            }
-        )
+    context.update(
+        {
+            "superset_dashboards": dashboards,
+            "superset_url": superset_url,
+            "superset_guest_token_url": guest_token_url,
+        }
+    )
 
     return context
 
 
-def _generate_guest_token(user, course, superset_config, dashboards, filters):
+def generate_guest_token(user, course, dashboards, filters) -> str:
     """
-    Generate a Superset guest token for the user.
+    Generate and return a Superset guest token for the user.
+
+    Raise ImproperlyConfigured if the Superset API client request fails for any reason.
 
     Args:
         user: User object.
-        course: Course object.
+        course: Course object, used to populate `filters` template strings.
+        dashboards: list of dashboard UUIDs to grant access to.
+        filters: list of string filters to apply.
 
     Returns:
         tuple: Superset guest token and dashboard id.
         or None, exception if Superset is missconfigured or cannot generate guest token.
     """
+    superset_config = settings.SUPERSET_CONFIG
     superset_internal_host = _fix_service_url(
         superset_config.get("internal_service_url")
         or superset_config.get("service_url")
     )
     superset_username = superset_config.get("username")
     superset_password = superset_config.get("password")
 
-    try:
-        client = SupersetClient(
-            host=superset_internal_host,
-            username=superset_username,
-            password=superset_password,
-        )
-    except Exception as exc:  # pylint: disable=broad-except
-        logger.error(exc)
-        return None, exc
-
     formatted_filters = [filter.format(course=course, user=user) for filter in filters]
 
     data = {
         "user": _superset_user_data(user),
         "resources": [
             {"type": "dashboard", "id": dashboard["uuid"]} for dashboard in dashboards
         ],
         "rls": [{"clause": filter} for filter in formatted_filters],
     }
 
     try:
-        logger.info(f"Requesting guest token from Superset, {data}")
+        client = SupersetClient(
+            host=superset_internal_host,
+            username=superset_username,
+            password=superset_password,
+        )
         response = client.session.post(
             url=f"{superset_internal_host}api/v1/security/guest_token/",
             json=data,
             headers={"Content-Type": "application/json"},
         )
         response.raise_for_status()
-        token = response.json()["token"]
+        token = response.json().get("token")
+        return token
+
+    except HTTPError as err:
+        # Superset server errors sometimes come with messages, so log the response.
+        logger.error(
+            f"{err.response.status_code} {err.response.json()} for url: {err.response.url}, data: {data}"
+        )
+        raise ImproperlyConfigured(
+            _(
+                "Unable to fetch Superset guest token, "
+                "Superset server error {server_response}"
+            ).format(server_response=err.response.json())
+        ) from err
 
-        return token, dashboards
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception as exc:
         logger.error(exc)
-        return None, exc
+        raise ImproperlyConfigured(
+            _(
+                "Unable to fetch Superset guest token, "
+                "mostly likely due to invalid settings.SUPERSET_CONFIG"
+            )
+        ) from exc
 
 
 def _fix_service_url(url: str) -> str:
     """
     Append a trailing slash to the given url, if missing.
 
     SupersetClient requires a trailing slash for service URLs.
```

### Comparing `platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.7.0/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 README.rst
 setup.cfg
 setup.py
 platform_plugin_aspects/__init__.py
 platform_plugin_aspects/apps.py
 platform_plugin_aspects/signals.py
 platform_plugin_aspects/tasks.py
+platform_plugin_aspects/urls.py
 platform_plugin_aspects/utils.py
+platform_plugin_aspects/views.py
 platform_plugin_aspects/waffle.py
 platform_plugin_aspects/xblock.py
 platform_plugin_aspects.egg-info/PKG-INFO
 platform_plugin_aspects.egg-info/SOURCES.txt
 platform_plugin_aspects.egg-info/dependency_links.txt
 platform_plugin_aspects.egg-info/entry_points.txt
 platform_plugin_aspects.egg-info/not-zip-safe
```

### Comparing `platform-plugin-aspects-0.6.0/requirements/constraints.txt` & `platform_plugin_aspects-0.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.6.0/setup.py` & `platform_plugin_aspects-0.7.0/setup.py`

 * *Files identical despite different names*

