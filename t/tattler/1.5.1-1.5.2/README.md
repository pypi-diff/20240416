# Comparing `tmp/tattler-1.5.1.tar.gz` & `tmp/tattler-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tattler-1.5.1.tar", last modified: Mon Mar  4 15:27:21 2024, max compression
+gzip compressed data, was "tattler-1.5.2.tar", last modified: Tue Apr 16 14:34:38 2024, max compression
```

## Comparing `tattler-1.5.1.tar` & `tattler-1.5.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.494758 tattler-1.5.1/
--rw-r--r--   0 michele    (501) staff       (20)     1473 2024-02-18 09:43:08.000000 tattler-1.5.1/LICENSE.txt
--rw-r--r--   0 michele    (501) staff       (20)     7791 2024-03-04 15:27:21.494541 tattler-1.5.1/PKG-INFO
--rw-r--r--   0 michele    (501) staff       (20)     6929 2024-03-04 15:24:45.000000 tattler-1.5.1/README.rst
--rw-r--r--   0 michele    (501) staff       (20)     1308 2024-03-04 15:27:06.000000 tattler-1.5.1/pyproject.toml
--rw-r--r--   0 michele    (501) staff       (20)       38 2024-03-04 15:27:21.494805 tattler-1.5.1/setup.cfg
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.474256 tattler-1.5.1/src/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.475151 tattler-1.5.1/src/tattler/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.474352 tattler-1.5.1/src/tattler/client/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.479079 tattler-1.5.1/src/tattler/client/tattler_py/
--rw-r--r--   0 michele    (501) staff       (20)     2352 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/__init__.py
--rw-r--r--   0 michele    (501) staff       (20)     2139 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/client/tattler_py/replay_dead_letters.py
--rw-r--r--   0 michele    (501) staff       (20)      526 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/client/tattler_py/serialization.py
--rw-r--r--   0 michele    (501) staff       (20)     5691 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/tattler_client.py
--rw-r--r--   0 michele    (501) staff       (20)     3149 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/client/tattler_py/tattler_client_http.py
--rw-r--r--   0 michele    (501) staff       (20)      753 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/tattler_client_utils.py
--rw-r--r--   0 michele    (501) staff       (20)     3093 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/client/tattler_py/tattler_cmd.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.480238 tattler-1.5.1/src/tattler/client/tattler_py/tests/
--rw-r--r--   0 michele    (501) staff       (20)     5762 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler.py
--rw-r--r--   0 michele    (501) staff       (20)     1244 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_client_utils.py
--rw-r--r--   0 michele    (501) staff       (20)     4644 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_cmd.py
--rw-r--r--   0 michele    (501) staff       (20)    11550 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_http.py
--rw-r--r--   0 michele    (501) staff       (20)     2661 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_module.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.483008 tattler-1.5.1/src/tattler/server/
--rw-r--r--   0 michele    (501) staff       (20)    18207 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/pluginloader.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.484729 tattler-1.5.1/src/tattler/server/plugins/
--rw-r--r--   0 michele    (501) staff       (20)      920 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/server/plugins/passthrough_addressbook_tattler_plugin.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.485016 tattler-1.5.1/src/tattler/server/plugins/tests/
--rw-r--r--   0 michele    (501) staff       (20)     2368 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/server/plugins/tests/test_passthrough_addressbook.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.486580 tattler-1.5.1/src/tattler/server/sendable/
--rw-r--r--   0 michele    (501) staff       (20)     3610 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/__init__.py
--rw-r--r--   0 michele    (501) staff       (20)     1359 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/blacklist.py
--rw-r--r--   0 michele    (501) staff       (20)     3682 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/bulksms.py
--rw-r--r--   0 michele    (501) staff       (20)     2352 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/template_processor.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.488217 tattler-1.5.1/src/tattler/server/sendable/tests/
--rw-r--r--   0 michele    (501) staff       (20)     5210 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_bulksms.py
--rw-r--r--   0 michele    (501) staff       (20)     2458 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_module.py
--rw-r--r--   0 michele    (501) staff       (20)    20435 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_sendable.py
--rw-r--r--   0 michele    (501) staff       (20)     1582 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_template_processor.py
--rw-r--r--   0 michele    (501) staff       (20)    13312 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_vector_email.py
--rw-r--r--   0 michele    (501) staff       (20)     6472 2024-02-20 13:42:44.000000 tattler-1.5.1/src/tattler/server/sendable/tests/test_vector_sms.py
--rw-r--r--   0 michele    (501) staff       (20)     8849 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/sendable/vector_email.py
--rw-r--r--   0 michele    (501) staff       (20)    12621 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/sendable/vector_sendable.py
--rw-r--r--   0 michele    (501) staff       (20)     4177 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/sendable/vector_sms.py
--rw-r--r--   0 michele    (501) staff       (20)    12359 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/tattler_utils.py
--rw-r--r--   0 michele    (501) staff       (20)     8099 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tattlersrv_http.py
--rw-r--r--   0 michele    (501) staff       (20)     5088 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/templatemgr.py
--rw-r--r--   0 michele    (501) staff       (20)     2939 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/templateprocessor_jinja.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.490443 tattler-1.5.1/src/tattler/server/tests/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.475079 tattler-1.5.1/src/tattler/server/tests/fixtures/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.492130 tattler-1.5.1/src/tattler/server/tests/fixtures/plugin_loading_order/
--rw-r--r--   0 michele    (501) staff       (20)      205 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugin_loading_order/a_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)      205 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugin_loading_order/b_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)      207 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugin_loading_order/c_tattler_plugin.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.492414 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins/
--rw-r--r--   0 michele    (501) staff       (20)      192 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins/test1_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)      192 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins/test2_tattler_plugin.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.492700 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_integration/
--rw-r--r--   0 michele    (501) staff       (20)      208 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_integration/addbar_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)      208 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_integration/addfoo_tattler_plugin.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.493005 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_sanity_check/
--rw-r--r--   0 michele    (501) staff       (20)      206 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_sanity_check/good_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)      220 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/fixtures/plugins_sanity_check/warn_tattler_plugin.py
--rw-r--r--   0 michele    (501) staff       (20)    14273 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/test_pluginloader.py
--rw-r--r--   0 michele    (501) staff       (20)      466 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/test_tattler_templates.py
--rw-r--r--   0 michele    (501) staff       (20)    24534 2024-03-04 15:24:45.000000 tattler-1.5.1/src/tattler/server/tests/test_tattler_utils.py
--rw-r--r--   0 michele    (501) staff       (20)    19070 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/test_tattlersrv_http.py
--rw-r--r--   0 michele    (501) staff       (20)     4984 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/test_templatemgr.py
--rw-r--r--   0 michele    (501) staff       (20)     2494 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/test_templateprocessor_jinja.py
--rw-r--r--   0 michele    (501) staff       (20)      242 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/testutils.py
--rw-r--r--   0 michele    (501) staff       (20)     4122 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/server/tests/testutils_templates.py
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.475198 tattler-1.5.1/src/tattler/templates/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.475250 tattler-1.5.1/src/tattler/templates/demoscope/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.475298 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.494047 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/
--rw-r--r--   0 michele    (501) staff       (20)    26536 2024-02-20 16:41:46.000000 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/body_html
--rw-r--r--   0 michele    (501) staff       (20)     3120 2024-02-20 16:41:46.000000 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/body_plain
--rw-r--r--   0 michele    (501) staff       (20)        1 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/priority
--rw-r--r--   0 michele    (501) staff       (20)       32 2024-02-18 09:43:08.000000 tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/subject
-drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-03-04 15:27:21.494266 tattler-1.5.1/src/tattler.egg-info/
--rw-r--r--   0 michele    (501) staff       (20)     7791 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/PKG-INFO
--rw-r--r--   0 michele    (501) staff       (20)     3107 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/SOURCES.txt
--rw-r--r--   0 michele    (501) staff       (20)        1 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/dependency_links.txt
--rw-r--r--   0 michele    (501) staff       (20)      131 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/entry_points.txt
--rw-r--r--   0 michele    (501) staff       (20)       44 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/requires.txt
--rw-r--r--   0 michele    (501) staff       (20)        8 2024-03-04 15:27:21.000000 tattler-1.5.1/src/tattler.egg-info/top_level.txt
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.216151 tattler-1.5.2/
+-rw-r--r--   0 michele    (501) staff       (20)     1473 2024-02-18 09:43:08.000000 tattler-1.5.2/LICENSE.txt
+-rw-r--r--   0 michele    (501) staff       (20)     7814 2024-04-16 14:34:38.215939 tattler-1.5.2/PKG-INFO
+-rw-r--r--   0 michele    (501) staff       (20)     6929 2024-03-04 15:24:45.000000 tattler-1.5.2/README.rst
+-rw-r--r--   0 michele    (501) staff       (20)     1335 2024-04-16 14:19:52.000000 tattler-1.5.2/pyproject.toml
+-rw-r--r--   0 michele    (501) staff       (20)       38 2024-04-16 14:34:38.216190 tattler-1.5.2/setup.cfg
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.198166 tattler-1.5.2/src/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.199186 tattler-1.5.2/src/tattler/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.198264 tattler-1.5.2/src/tattler/client/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.202997 tattler-1.5.2/src/tattler/client/tattler_py/
+-rw-r--r--   0 michele    (501) staff       (20)     2352 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/__init__.py
+-rw-r--r--   0 michele    (501) staff       (20)     2139 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/client/tattler_py/replay_dead_letters.py
+-rw-r--r--   0 michele    (501) staff       (20)      526 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/client/tattler_py/serialization.py
+-rw-r--r--   0 michele    (501) staff       (20)     5691 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/tattler_client.py
+-rw-r--r--   0 michele    (501) staff       (20)     3149 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/client/tattler_py/tattler_client_http.py
+-rw-r--r--   0 michele    (501) staff       (20)      753 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/tattler_client_utils.py
+-rw-r--r--   0 michele    (501) staff       (20)     3577 2024-04-16 06:30:50.000000 tattler-1.5.2/src/tattler/client/tattler_py/tattler_cmd.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.204283 tattler-1.5.2/src/tattler/client/tattler_py/tests/
+-rw-r--r--   0 michele    (501) staff       (20)     5762 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler.py
+-rw-r--r--   0 michele    (501) staff       (20)     1244 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_client_utils.py
+-rw-r--r--   0 michele    (501) staff       (20)     8867 2024-04-16 06:30:50.000000 tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_cmd.py
+-rw-r--r--   0 michele    (501) staff       (20)    11550 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_http.py
+-rw-r--r--   0 michele    (501) staff       (20)     2661 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_module.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.205817 tattler-1.5.2/src/tattler/server/
+-rw-r--r--   0 michele    (501) staff       (20)    18207 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/pluginloader.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.206121 tattler-1.5.2/src/tattler/server/plugins/
+-rw-r--r--   0 michele    (501) staff       (20)      920 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/server/plugins/passthrough_addressbook_tattler_plugin.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.206377 tattler-1.5.2/src/tattler/server/plugins/tests/
+-rw-r--r--   0 michele    (501) staff       (20)     2368 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/server/plugins/tests/test_passthrough_addressbook.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.208090 tattler-1.5.2/src/tattler/server/sendable/
+-rw-r--r--   0 michele    (501) staff       (20)     3610 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/__init__.py
+-rw-r--r--   0 michele    (501) staff       (20)     1359 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/blacklist.py
+-rw-r--r--   0 michele    (501) staff       (20)     3682 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/bulksms.py
+-rw-r--r--   0 michele    (501) staff       (20)     2352 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/template_processor.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.209626 tattler-1.5.2/src/tattler/server/sendable/tests/
+-rw-r--r--   0 michele    (501) staff       (20)     5210 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_bulksms.py
+-rw-r--r--   0 michele    (501) staff       (20)     2458 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_module.py
+-rw-r--r--   0 michele    (501) staff       (20)    20435 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_sendable.py
+-rw-r--r--   0 michele    (501) staff       (20)     1582 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_template_processor.py
+-rw-r--r--   0 michele    (501) staff       (20)    17928 2024-04-16 06:35:10.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_vector_email.py
+-rw-r--r--   0 michele    (501) staff       (20)     6472 2024-02-20 13:42:44.000000 tattler-1.5.2/src/tattler/server/sendable/tests/test_vector_sms.py
+-rw-r--r--   0 michele    (501) staff       (20)    10282 2024-04-16 06:34:50.000000 tattler-1.5.2/src/tattler/server/sendable/vector_email.py
+-rw-r--r--   0 michele    (501) staff       (20)    12621 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/server/sendable/vector_sendable.py
+-rw-r--r--   0 michele    (501) staff       (20)     4177 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/server/sendable/vector_sms.py
+-rw-r--r--   0 michele    (501) staff       (20)    12359 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/server/tattler_utils.py
+-rw-r--r--   0 michele    (501) staff       (20)     8099 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tattlersrv_http.py
+-rw-r--r--   0 michele    (501) staff       (20)     5088 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/templatemgr.py
+-rw-r--r--   0 michele    (501) staff       (20)     2939 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/templateprocessor_jinja.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.212003 tattler-1.5.2/src/tattler/server/tests/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.199018 tattler-1.5.2/src/tattler/server/tests/fixtures/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.213465 tattler-1.5.2/src/tattler/server/tests/fixtures/plugin_loading_order/
+-rw-r--r--   0 michele    (501) staff       (20)      205 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugin_loading_order/a_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)      205 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugin_loading_order/b_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)      207 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugin_loading_order/c_tattler_plugin.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.213767 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins/
+-rw-r--r--   0 michele    (501) staff       (20)      192 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins/test1_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)      192 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins/test2_tattler_plugin.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.214062 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_integration/
+-rw-r--r--   0 michele    (501) staff       (20)      208 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_integration/addbar_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)      208 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_integration/addfoo_tattler_plugin.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.214369 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_sanity_check/
+-rw-r--r--   0 michele    (501) staff       (20)      206 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_sanity_check/good_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)      220 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/fixtures/plugins_sanity_check/warn_tattler_plugin.py
+-rw-r--r--   0 michele    (501) staff       (20)    14273 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/test_pluginloader.py
+-rw-r--r--   0 michele    (501) staff       (20)      466 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/test_tattler_templates.py
+-rw-r--r--   0 michele    (501) staff       (20)    24534 2024-03-04 15:24:45.000000 tattler-1.5.2/src/tattler/server/tests/test_tattler_utils.py
+-rw-r--r--   0 michele    (501) staff       (20)    19070 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/test_tattlersrv_http.py
+-rw-r--r--   0 michele    (501) staff       (20)     4984 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/test_templatemgr.py
+-rw-r--r--   0 michele    (501) staff       (20)     2494 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/test_templateprocessor_jinja.py
+-rw-r--r--   0 michele    (501) staff       (20)      242 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/testutils.py
+-rw-r--r--   0 michele    (501) staff       (20)     4122 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/server/tests/testutils_templates.py
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.199261 tattler-1.5.2/src/tattler/templates/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.199318 tattler-1.5.2/src/tattler/templates/demoscope/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.199372 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.215510 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/
+-rw-r--r--   0 michele    (501) staff       (20)    26536 2024-02-20 16:41:46.000000 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/body_html
+-rw-r--r--   0 michele    (501) staff       (20)     3120 2024-02-20 16:41:46.000000 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/body_plain
+-rw-r--r--   0 michele    (501) staff       (20)        1 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/priority
+-rw-r--r--   0 michele    (501) staff       (20)       32 2024-02-18 09:43:08.000000 tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/subject
+drwxr-xr-x   0 michele    (501) staff       (20)        0 2024-04-16 14:34:38.215697 tattler-1.5.2/src/tattler.egg-info/
+-rw-r--r--   0 michele    (501) staff       (20)     7814 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/PKG-INFO
+-rw-r--r--   0 michele    (501) staff       (20)     3107 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/SOURCES.txt
+-rw-r--r--   0 michele    (501) staff       (20)        1 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/dependency_links.txt
+-rw-r--r--   0 michele    (501) staff       (20)      131 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/entry_points.txt
+-rw-r--r--   0 michele    (501) staff       (20)       44 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/requires.txt
+-rw-r--r--   0 michele    (501) staff       (20)        8 2024-04-16 14:34:38.000000 tattler-1.5.2/src/tattler.egg-info/top_level.txt
```

### Comparing `tattler-1.5.1/LICENSE.txt` & `tattler-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/PKG-INFO` & `tattler-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tattler
-Version: 1.5.1
+Version: 1.5.2
 Summary: A client-server notification system for HTML emails, sms and more.
 Author-email: Michele Mazzucchi <support@tattler.dev>
 Project-URL: Home, https://tattler.dev
 Project-URL: Documentation, https://docs.tattler.dev/
 Project-URL: Repository, https://github.com/tattler-community/tattler-community
 Project-URL: Issues, https://github.com/tattler-community/tattler-community/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Communications
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: humanize>=4.7.0
 Requires-Dist: envdir>=1.0.1
 
 .. |badge_pipeline| image:: https://gitlab.com/tattler/tattler-community/badges/main/pipeline.svg
```

### Comparing `tattler-1.5.1/README.rst` & `tattler-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/pyproject.toml` & `tattler-1.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tattler"
-version = "1.5.1"
+version = "1.5.2"
 authors = [{name = "Michele Mazzucchi", email = "support@tattler.dev"}]
 # have license information implicitly loaded from LICENSE* file
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3 :: Only",
     "Operating System :: POSIX",
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Topic :: Communications",
     ]
 description = "A client-server notification system for HTML emails, sms and more."
 readme = "README.rst"
+requires-python = ">= 3.9"
 dependencies = [
     "Jinja2 >= 3.1.2",
     "humanize >= 4.7.0",
     "envdir >= 1.0.1",
 ]
 
 [project.scripts]
```

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/__init__.py` & `tattler-1.5.2/src/tattler/client/tattler_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/replay_dead_letters.py` & `tattler-1.5.2/src/tattler/client/tattler_py/replay_dead_letters.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/serialization.py` & `tattler-1.5.2/src/tattler/client/tattler_py/serialization.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tattler_client.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tattler_client.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tattler_client_http.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tattler_client_http.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tattler_client_utils.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tattler_client_utils.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tattler_cmd.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tattler_cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Command-line interface to tattler client"""
 
 import re
 import argparse
 import logging
 import os
 import sys
+import json
 from typing import Tuple
 
 from tattler.client.tattler_py import send_notification
 
 log = logging.getLogger(__name__)
 log.setLevel(os.getenv('LOG_LEVEL', 'info').upper())
 
@@ -42,19 +43,25 @@
     parser.add_argument('scope', help='name of scope holding event', type=alnum_argument)
     parser.add_argument('event_name', help='name of event to notify', type=alnum_argument)
     parser.add_argument('context', nargs='*', default={}, type=contextvar, help='Optional key=value variables to add to context. Repeat to set multiple variables. Default: no context.')
     parser.add_argument('-v', '--vectors', type=(lambda x: x.split(',')), help="Optional comma-separated list of vectors to restrict the notification to. Default: deliver to all event-defined vectors.")
     parser.add_argument('-s', '--server', type=server_endpoint_spec, default="127.0.0.1:11503", help="Optional address:port of tattler server to request notification to. Default: 127.0.0.1:11503.")
     parser.add_argument('-m', '--mode', choices={'debug', 'staging', 'production'}, default="debug", help="Optional mode for sending the notification (debug, staging, production). Default: debug.")
     parser.add_argument('-p', '--priority', type=int, choices={1, 2, 3, 4, 5}, help="Optional priority for the notification. Default: None.")
+    parser.add_argument('-j', '--json-context', type=argparse.FileType('r', encoding='utf-8'), help='Optional path to a JSON file holding context data. Any command-line context vars gets merged on top of it.')
     return parser.parse_args(args=args)
 
 def main():
     """Main function run on command line call."""
     args = parse_cmdline(sys.argv[1:])
+    if args.json_context:
+        jctx = json.load(args.json_context)
+        if not isinstance(jctx, dict):
+            raise ValueError(f"Context file must be a dictionary (JSON object), not {type(jctx)}")
+        args.context = {**jctx, **dict(args.context)}
     success, details = send_notification(args.scope, args.event_name, args.recipient, dict(args.context), vectors=args.vectors, mode=args.mode, priority=args.priority, srv_addr=args.server[0], srv_port=args.server[1])
     if success:
         log.info("Notification succeeded. Details: %s", details)
     else:
         log.error("Notification failed. Details: %s", details)
         sys.exit(1)
```

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_client_utils.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_client_utils.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_cmd.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_cmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """Tests for command-line interface to tattler client"""
 
 import unittest
 from unittest import mock
 import sys
+from pathlib import Path
 
 from tattler.client.tattler_py.tattler_cmd import main
 
 class CmdLineTest(unittest.TestCase):
     """Tests for command line interface of tattler client"""
 
+    def setUp(self) -> None:
+        self.mypath = Path(__file__).parent
+        self.jsonctx = {
+            typename: str(self.mypath / 'fixtures' / f'jsonctx_{typename}.json')
+                        for typename in ['malformatted', 'invalid', 'valid', 'empty']
+        }
+        return super().setUp()
+    
     def test_main_rejects_unknown_arguments(self):
         """Main rejects unknown positional arguments"""
         with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
             with self.assertRaises(SystemExit) as err:
                 msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo']
                 main()
 
@@ -45,36 +54,89 @@
                 msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', '=context with empty name']
                 main()
     
     def test_short_params_passed_through(self):
         """Cmdline short params are passed through to send_notification"""
         with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
             with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
-                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2']
+                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', self.jsonctx['empty']]
                 msnot.return_value = True, 'asd'
                 main()
                 msnot.assert_called_once()
                 msnot.assert_called_with('myscope', 'myevent', '1', {'foo': 'bar', 'x': 'var'}, vectors=['email', 'sms'], mode='staging', priority=2, srv_addr='3.4.5.6', srv_port=321)
 
     def test_long_params_passed_through(self):
         """Cmdline short params are passed through to send_notification"""
         with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
             with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
-                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '--vectors', 'email,sms', '--server', '3.4.5.6:321', '--mode', 'staging', '--priority', '2']
+                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '--vectors', 'email,sms', '--server', '3.4.5.6:321', '--mode', 'staging', '--priority', '2', '--json-context', self.jsonctx['empty']]
                 msnot.return_value = True, 'asd'
                 main()
                 msnot.assert_called_once()
                 msnot.assert_called_with('myscope', 'myevent', '1', {'foo': 'bar', 'x': 'var'}, vectors=['email', 'sms'], mode='staging', priority=2, srv_addr='3.4.5.6', srv_port=321)
     
+    def test_json_context_missing_file(self):
+        """If a JSON context file is provided that does not exist, run fails"""
+        with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
+            with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
+                args = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', 'not_existing_path']
+                msys.argv = args
+                msnot.return_value = True, 'asd'
+                with self.assertRaises(SystemExit):
+                    main()
+
+    def test_json_context_unacceptable_content(self):
+        """If a JSON context file is provided that includes parsable content with invalid format, run fails"""
+        with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
+            with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
+                args = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', self.jsonctx['invalid']]
+                msys.argv = args
+                msnot.return_value = True, 'asd'
+                with self.assertRaises(ValueError):
+                    main()
+
+    def test_json_context_malformatted_content(self):
+        """If a JSON context file is provided that includes unparsable content, run fails"""
+        with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
+            with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
+                args = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', self.jsonctx['malformatted']]
+                msys.argv = args
+                msnot.return_value = True, 'asd'
+                with self.assertRaises(ValueError):
+                    main()
+
+    def test_json_context_pure(self):
+        """If a JSON context file is provided, it is acquired"""
+        with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
+            with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
+                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', self.jsonctx['valid']]
+                msnot.return_value = True, 'asd'
+                main()
+                msnot.assert_called_once()
+                msnot.assert_called_with('myscope', 'myevent', '1', {'foo': 'bar', 'x': 'var', 'jsonvar1': [1, 2, 3], 'jsonvar2': {"object": {}}, 'overrideme': 1}, vectors=['email', 'sms'], mode='staging', priority=2, srv_addr='3.4.5.6', srv_port=321)
+
+    def test_json_context_merged_cmdline(self):
+        """If both a JSON context file is provided and command-line context, the latter is merged onto the former"""
+        with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
+            with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
+                msys.argv = ['tattler_notify', '1', 'myscope', 'myevent', 'foo=bar', 'x=var', 'overrideme=x', '-v', 'email,sms', '-s', '3.4.5.6:321', '-m', 'staging', '-p', '2', '-j', self.jsonctx['valid']]
+                msnot.return_value = True, 'asd'
+                main()
+                msnot.assert_called_once()
+                msnot.assert_called_with('myscope', 'myevent', '1', {'foo': 'bar', 'x': 'var', 'jsonvar1': [1, 2, 3], 'jsonvar2': {"object": {}}, 'overrideme': 'x'}, vectors=['email', 'sms'], mode='staging', priority=2, srv_addr='3.4.5.6', srv_port=321)
+
     def test_nonzero_exit_code_if_delivery_fails(self):
         """Cmd exists non-zero if notification request fails to send"""
         with mock.patch('tattler.client.tattler_py.tattler_cmd.sys') as msys:
             with mock.patch('tattler.client.tattler_py.tattler_cmd.send_notification') as msnot:
                 msys.argv = ['tattler_notify', '1', 'myscope', 'myevent']
                 msys.exit.side_effect = sys.exit
                 # msnot.return_value = True, 'asd'
                 # main()
                 # msnot.reset_mock()
                 msnot.return_value = False, 'asd'
                 with self.assertRaises(SystemExit) as err:
                     main()
-                self.assertEqual(err.exception.code, 1)
+                self.assertEqual(err.exception.code, 1)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_http.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_http.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/client/tattler_py/tests/test_tattler_module.py` & `tattler-1.5.2/src/tattler/client/tattler_py/tests/test_tattler_module.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/pluginloader.py` & `tattler-1.5.2/src/tattler/server/pluginloader.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/plugins/passthrough_addressbook_tattler_plugin.py` & `tattler-1.5.2/src/tattler/server/plugins/passthrough_addressbook_tattler_plugin.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/plugins/tests/test_passthrough_addressbook.py` & `tattler-1.5.2/src/tattler/server/plugins/tests/test_passthrough_addressbook.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/__init__.py` & `tattler-1.5.2/src/tattler/server/sendable/__init__.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/blacklist.py` & `tattler-1.5.2/src/tattler/server/sendable/blacklist.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/bulksms.py` & `tattler-1.5.2/src/tattler/server/sendable/bulksms.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/template_processor.py` & `tattler-1.5.2/src/tattler/server/sendable/template_processor.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_bulksms.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_bulksms.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_module.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_sendable.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_sendable.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_template_processor.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_template_processor.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_vector_email.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_vector_email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+"""Tests for email vector sendable"""
+
 import unittest
 from unittest import mock
 import os
 import re
+import random
 
 from pathlib import Path
 
 from tattler.server.sendable.vector_email import EmailSendable, get_smtp_server
 
 data_recipients = {
     'email': ['support@test123.com'],
@@ -103,14 +106,15 @@
                 e.send(context={'one': '1'}, priority='invalid_value')
 
     def test_email_plain(self):
         """Plain email contains no HTML declaration"""
         e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
         self.assertNotIn('HTML', e.content(context={}))
         self.assertNotIn('html', e.content(context={}))
+        self.assertIn('Message-ID:', e.content(context={}))
 
     def test_email_html(self):
         """HTML email contains text/html part"""
         e = EmailSendable('event_with_email_and_sms', data_recipients['email'], template_base=tbase_standard_path)
         self.assertIn('''Content-Type: text/html; charset=''', e.content(context={'one': '#1234#'}))
 
     def test_html_and_plain_place_html_last(self):
@@ -120,33 +124,100 @@
             e.send(context={'one': 'asd'})
             msmtp.assert_called()
             msmtp.return_value.sendmail.assert_called_once()
             msgtext = msmtp.return_value.sendmail.call_args.args[2]
             regex_html_after_plain = re.compile('^Content-Type: text/plain; .*Content-Type: text/html;', re.MULTILINE | re.DOTALL)
             self.assertIsNotNone(regex_html_after_plain.search(msgtext))
 
+    def test_message_id_uses_sender_domain(self):
+        """Message-Id uses domain of sender"""
+        with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
+            mgetenv.side_effect = lambda k,v=None: { 'TATTLER_EMAIL_SENDER': 'foo@aksjdfhksadf.com' }.get(k, os.getenv(k, v))
+            e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
+            self.assertIn('Message-ID:', e.content(context={}))
+            msgidline = [line for line in e.content(context={}).splitlines() if line.startswith('Message-ID:')][0]
+            msgid = msgidline.split(' ', 1)[1]
+            self.assertEqual(msgid[0], '<')
+            self.assertEqual(msgid[-1], '>')
+            self.assertIn('@', msgid)
+            domain = msgid.split('@', 1)[1]
+            self.assertEqual(domain, 'aksjdfhksadf.com>')
+
     def test_email_send_triggers_delivery(self):
         """send() calls smtp().sendmail()"""
         with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
             e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
             e.send()
             msmtp.assert_called()
             msmtp.return_value.sendmail.assert_called_once()
             self.assertIn('Plain text', msmtp.return_value.sendmail.call_args.args[2])
             self.assertIn('Subject: Subject', msmtp.return_value.sendmail.call_args.args[2])
             msmtp.return_value.starttls.assert_not_called()
     
+    def test_email_delivery_tls_connection_if_tls_port(self):
+        """If TATTLER_SMTP_ADDRESS includes a well-known port of SMTP TLS service, connect with SMTP_SSL"""
+        tls_ports = [465, 587]
+        non_tls_ports = [25, 2525]
+        addresses = ['12.34.56.78', '[a::b]', 'foo.bar.com']
+        with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
+            with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP_SSL') as msmtps:
+                e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
+                with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
+                    for addr in addresses:
+                        for port in tls_ports+non_tls_ports:
+                            mgetenv.side_effect = lambda k,v=None: { 'TATTLER_SMTP_ADDRESS': f"{addr}:{port}" }.get(k, os.getenv(k, v))
+                            e.send()
+                            if port in tls_ports:
+                                msmtp.assert_not_called()
+                                msmtps.assert_called_once()
+                                self.assertIn('timeout', msmtps.call_args.kwargs)
+                                self.assertIsNotNone(msmtps.call_args.kwargs['timeout'])
+                            else:
+                                msmtps.assert_not_called()
+                                msmtp.assert_called_once()
+                                self.assertIn('timeout', msmtp.call_args.kwargs)
+                                self.assertIsNotNone(msmtp.call_args.kwargs['timeout'])
+                            msmtp.reset_mock()
+                            msmtps.reset_mock()
+
+    def test_email_delivery_timeout(self):
+        """Setting TATTLER_SMTP_TIMEOUT envvar controls timeout param to SMTP connection"""
+        with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
+            e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
+            with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
+                # use random number to avoid inadvertently matching default value
+                rndval = random.randint(1, 100)
+                mgetenv.side_effect = lambda k,v=None: { 'TATTLER_SMTP_TIMEOUT': rndval }.get(k, os.getenv(k, v))
+                e.send()
+                msmtp.assert_called_once()
+                self.assertIn('timeout', msmtp.call_args.kwargs)
+                self.assertEqual(msmtp.call_args.kwargs['timeout'], rndval)
+
+    def test_email_delivery_rejects_invalid_timeout(self):
+        """Invalid timeouts are replaced with default"""
+        with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
+            e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
+            with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
+                # use random number to avoid inadvertently matching default value
+                for tval in ['-1', '', 'asd']:
+                    mgetenv.side_effect = lambda k,v=None: { 'TATTLER_SMTP_TIMEOUT': tval }.get(k, os.getenv(k, v))
+                    e.send()
+                    msmtp.assert_called_once()
+                    self.assertIn('timeout', msmtp.call_args.kwargs)
+                    self.assertEqual(msmtp.call_args.kwargs['timeout'], 30)
+                    msmtp.reset_mock()
+
     def test_email_delivery_tls(self):
         """When TATTLER_SMTP_TLS envvar is given, smtp().starttls() is called upon send()"""
         with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
             e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
             with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
                 mgetenv.side_effect = lambda k,v=None: { 'TATTLER_SMTP_TLS': 'yes' }.get(k, os.getenv(k, v))
                 e.send()
-                msmtp().starttls.assert_called()
+                msmtp.return_value.starttls.assert_called()
 
     def test_email_delivery_smtpauth(self):
         """When TATTLER_SMTP_AUTH envvar is given, smtp().login() is called with the credentials it indicates."""
         with mock.patch('tattler.server.sendable.vector_email.smtplib.SMTP') as msmtp:
             e = EmailSendable('event_with_email_plain', data_recipients['email'], template_base=tbase_standard_path)
             with mock.patch('tattler.server.sendable.vector_email.vector_sendable.getenv') as mgetenv:
                 mgetenv.side_effect = lambda k,v=None: { 'TATTLER_SMTP_AUTH': 'username:password' }.get(k, os.getenv(k, v))
@@ -210,8 +281,8 @@
             EmailSendable.validate_configuration()
             mgetenv.side_effect = lambda x, y=None: {'TATTLER_SMTP_ADDRESS': 'a 1.2.3.4'}.get(x, os.getenv(x, y))
             with self.assertRaises(ValueError, msg="validate_configuration() does not raise upon invalid setting 'TATTLER_SMTP_ADDRESS'"):
                 EmailSendable.validate_configuration()
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()             # pragma: no cover
```

### Comparing `tattler-1.5.1/src/tattler/server/sendable/tests/test_vector_sms.py` & `tattler-1.5.2/src/tattler/server/sendable/tests/test_vector_sms.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/vector_email.py` & `tattler-1.5.2/src/tattler/server/sendable/vector_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import smtplib
 
 from tattler.server.sendable import vector_sendable
 
 # SMTP X-Priority header
 _valid_priorities = [1, 2, 3, 4, 5]
 _default_priority = 3
+_smtp_timeout_s = 30
 
 logging.basicConfig(level=os.getenv('LOG_LEVEL', 'info').upper())
 log = logging.getLogger(__name__)
 
 email_re = re.compile(r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)")
 
 ip4_re = re.compile(r'^(?P<srv>(\d+\.){3}\d+)')
@@ -112,14 +113,17 @@
             msg = MIMENonMultipart('text', 'plain')
 
         # fill out header
         msg['From'] = self.sender()
         msg['To'] = ", ".join(self.recipients)
         msg['Date'] = formatdate()
         msg['Subject'] = self.subject(context)
+        # gmail requires a Message-ID to be present. E.g. <A5A1B9EB-DBD6-4DE4-902D-F32E2D7D6B86@email.com>
+        sender_domain = self.sender().split('@')[1].lower()
+        msg['Message-ID'] = f'<{self.nid}@{sender_domain}>'
 
         self._add_msg_parts(msg, context)
 
         # add priority information, if required
         msg = self._add_priority_info(msg)
 
         return msg
@@ -183,21 +187,37 @@
 
     def do_send(self, recipients: Iterable[str], context: Mapping[str, Any], priority: Optional[int]=None) -> None:
         assert isinstance(context, dict), f"context must be a dictionary in do_send(); not {type(context)}"
         if priority is not None:
             self.set_priority(priority)
         msg = self.content(context)
         smtp_server, smtp_server_port = get_smtp_server(vector_sendable.getenv("TATTLER_SMTP_ADDRESS", '127.0.0.1'))
+        tls_connect = smtp_server_port in (465, 587)
         try:
-            server = smtplib.SMTP(smtp_server, smtp_server_port)
+            smtp_conn_timeout = int(vector_sendable.getenv("TATTLER_SMTP_TIMEOUT", _smtp_timeout_s))
+            if smtp_conn_timeout <= 0:
+                raise ValueError
+        except ValueError:
+            smtp_conn_timeout = int(_smtp_timeout_s)
+            log.warning("Invalid value given for TATTLER_SMTP_TIMEOUT='%s'. Set to number of seconds as a positive integer (e.g. 1, 5, 99). Falling back to default %s", vector_sendable.getenv("TATTLER_SMTP_TIMEOUT"), smtp_conn_timeout)
+        try:
+            log.info("Attempting email delivery of '%s' via SMTP%s %s:%s (timeout=%ss)...", self.event(), '_TLS' if tls_connect else '', smtp_server, smtp_server_port, smtp_conn_timeout)
+            if tls_connect:
+                server = smtplib.SMTP_SSL(smtp_server, smtp_server_port, timeout=smtp_conn_timeout)
+            else:
+                server = smtplib.SMTP(smtp_server, smtp_server_port, timeout=smtp_conn_timeout)
         except ConnectionRefusedError:
             log.error("Failed to connect to SMTP server (%s:%s) to deliver email. Giving up.", smtp_server, smtp_server_port)
             raise
         smtp_tls = vector_sendable.getenv("TATTLER_SMTP_TLS", None)
         if smtp_tls:
+            log.debug("Changing SMTP connection to TLS (STARTTLS).")
             server.starttls()
         smtp_auth = vector_sendable.getenv("TATTLER_SMTP_AUTH", None)
         if smtp_auth:
+            log.debug("Attempting SMTP auth ...")
             u, p = smtp_auth.split(':', 1)
             server.login(u, p)
+        log.debug("Delivering SMTP content ...")
         server.sendmail(self.sender(), recipients, msg)
         server.quit()
+        log.info("SMTP delivery to %s:%s completed successfully.", smtp_server, smtp_server_port)
```

### Comparing `tattler-1.5.1/src/tattler/server/sendable/vector_sendable.py` & `tattler-1.5.2/src/tattler/server/sendable/vector_sendable.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/sendable/vector_sms.py` & `tattler-1.5.2/src/tattler/server/sendable/vector_sms.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tattler_utils.py` & `tattler-1.5.2/src/tattler/server/tattler_utils.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tattlersrv_http.py` & `tattler-1.5.2/src/tattler/server/tattlersrv_http.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/templatemgr.py` & `tattler-1.5.2/src/tattler/server/templatemgr.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/templateprocessor_jinja.py` & `tattler-1.5.2/src/tattler/server/templateprocessor_jinja.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/test_pluginloader.py` & `tattler-1.5.2/src/tattler/server/tests/test_pluginloader.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/test_tattler_utils.py` & `tattler-1.5.2/src/tattler/server/tests/test_tattler_utils.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/test_tattlersrv_http.py` & `tattler-1.5.2/src/tattler/server/tests/test_tattlersrv_http.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/test_templatemgr.py` & `tattler-1.5.2/src/tattler/server/tests/test_templatemgr.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/test_templateprocessor_jinja.py` & `tattler-1.5.2/src/tattler/server/tests/test_templateprocessor_jinja.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/server/tests/testutils_templates.py` & `tattler-1.5.2/src/tattler/server/tests/testutils_templates.py`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/body_html` & `tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/body_html`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler/templates/demoscope/demoevent/email/body_plain` & `tattler-1.5.2/src/tattler/templates/demoscope/demoevent/email/body_plain`

 * *Files identical despite different names*

### Comparing `tattler-1.5.1/src/tattler.egg-info/PKG-INFO` & `tattler-1.5.2/src/tattler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tattler
-Version: 1.5.1
+Version: 1.5.2
 Summary: A client-server notification system for HTML emails, sms and more.
 Author-email: Michele Mazzucchi <support@tattler.dev>
 Project-URL: Home, https://tattler.dev
 Project-URL: Documentation, https://docs.tattler.dev/
 Project-URL: Repository, https://github.com/tattler-community/tattler-community
 Project-URL: Issues, https://github.com/tattler-community/tattler-community/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Communications
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: humanize>=4.7.0
 Requires-Dist: envdir>=1.0.1
 
 .. |badge_pipeline| image:: https://gitlab.com/tattler/tattler-community/badges/main/pipeline.svg
```

### Comparing `tattler-1.5.1/src/tattler.egg-info/SOURCES.txt` & `tattler-1.5.2/src/tattler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

