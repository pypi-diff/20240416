# Comparing `tmp/tendril_interests-0.5.8.tar.gz` & `tmp/tendril_interests-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_interests-0.5.8.tar", last modified: Mon Apr 15 15:58:43 2024, max compression
+gzip compressed data, was "tendril_interests-0.6.0.tar", last modified: Tue Apr 16 18:43:30 2024, max compression
```

## Comparing `tendril_interests-0.5.8.tar` & `tendril_interests-0.6.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.319001 tendril_interests-0.5.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5721 2024-04-15 15:58:43.319001 tendril_interests-0.5.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.287001 tendril_interests-0.5.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_interests-0.5.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-15 15:58:43.319001 tendril_interests-0.5.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3582 2024-04-09 19:31:13.000000 tendril_interests-0.5.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.283002 tendril_interests-0.5.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.5.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.5.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.291001 tendril_interests-0.5.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.5.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.295002 tendril_interests-0.5.8/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21600 2024-04-05 09:10:59.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1498 2024-04-15 15:41:13.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.295002 tendril_interests-0.5.8/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril_interests-0.5.8/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.295002 tendril_interests-0.5.8/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril_interests-0.5.8/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril_interests-0.5.8/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.295002 tendril_interests-0.5.8/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril_interests-0.5.8/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril_interests-0.5.8/src/tendril/authz/roles/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril_interests-0.5.8/src/tendril/authz/roles/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.299002 tendril_interests-0.5.8/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril_interests-0.5.8/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril_interests-0.5.8/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.299002 tendril_interests-0.5.8/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.5.8/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.299002 tendril_interests-0.5.8/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.5.8/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril_interests-0.5.8/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril_interests-0.5.8/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril_interests-0.5.8/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril_interests-0.5.8/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril_interests-0.5.8/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.299002 tendril_interests-0.5.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril_interests-0.5.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.299002 tendril_interests-0.5.8/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_interests-0.5.8/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.303001 tendril_interests-0.5.8/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_interests-0.5.8/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      361 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/core/topology/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.303001 tendril_interests-0.5.8/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.5.8/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.303001 tendril_interests-0.5.8/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril_interests-0.5.8/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril_interests-0.5.8/src/tendril/db/controllers/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril_interests-0.5.8/src/tendril/db/controllers/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.303001 tendril_interests-0.5.8/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril_interests-0.5.8/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril_interests-0.5.8/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.303001 tendril_interests-0.5.8/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril_interests-0.5.8/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril_interests-0.5.8/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril_interests-0.5.8/src/tendril/db/models/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril_interests-0.5.8/src/tendril/db/models/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.307001 tendril_interests-0.5.8/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril_interests-0.5.8/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril_interests-0.5.8/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8346 2024-04-10 20:05:40.000000 tendril_interests-0.5.8/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.307001 tendril_interests-0.5.8/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-04-05 09:10:45.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/export.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3044 2024-04-15 11:57:14.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-04-05 09:09:51.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/localizers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20183 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril_interests-0.5.8/src/tendril/interests/mixins/policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.307001 tendril_interests-0.5.8/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril_interests-0.5.8/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.307001 tendril_interests-0.5.8/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril_interests-0.5.8/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5996 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.311001 tendril_interests-0.5.8/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril_interests-0.5.8/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril_interests-0.5.8/src/tendril/libraries/mixins/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2024-04-09 21:11:30.000000 tendril_interests-0.5.8/src/tendril/libraries/mixins/interests_graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril_interests-0.5.8/src/tendril/libraries/mixins/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril_interests-0.5.8/src/tendril/libraries/mixins/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.311001 tendril_interests-0.5.8/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril_interests-0.5.8/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril_interests-0.5.8/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.311001 tendril_interests-0.5.8/src/tendril/policies/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril_interests-0.5.8/src/tendril/policies/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril_interests-0.5.8/src/tendril/policies/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril_interests-0.5.8/src/tendril/policies/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.315001 tendril_interests-0.5.8/src/tendril_interests.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5721 2024-04-15 15:58:43.000000 tendril_interests-0.5.8/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3368 2024-04-15 15:58:43.000000 tendril_interests-0.5.8/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-15 15:58:43.000000 tendril_interests-0.5.8/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      729 2024-04-15 15:58:43.000000 tendril_interests-0.5.8/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-15 15:58:43.000000 tendril_interests-0.5.8/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 15:58:43.311001 tendril_interests-0.5.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril_interests-0.5.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.595836 tendril_interests-0.6.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-16 18:43:30.595836 tendril_interests-0.6.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_interests-0.6.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:43:30.599836 tendril_interests-0.6.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3589 2024-04-16 18:42:17.000000 tendril_interests-0.6.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.555837 tendril_interests-0.6.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21600 2024-04-05 09:10:59.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1498 2024-04-15 15:41:13.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril_interests-0.6.0/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril_interests-0.6.0/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril_interests-0.6.0/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril_interests-0.6.0/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril_interests-0.6.0/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril_interests-0.6.0/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril_interests-0.6.0/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril_interests-0.6.0/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_interests-0.6.0/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_interests-0.6.0/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      363 2024-04-16 18:10:38.000000 tendril_interests-0.6.0/src/tendril/core/topology/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.0/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril_interests-0.6.0/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril_interests-0.6.0/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril_interests-0.6.0/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril_interests-0.6.0/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril_interests-0.6.0/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril_interests-0.6.0/src/tendril/db/models/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril_interests-0.6.0/src/tendril/db/models/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril_interests-0.6.0/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril_interests-0.6.0/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8346 2024-04-10 20:05:40.000000 tendril_interests-0.6.0/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-04-05 09:10:45.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/export.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3044 2024-04-15 11:57:14.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-04-05 09:09:51.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/localizers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20185 2024-04-16 18:31:53.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril_interests-0.6.0/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5996 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.583837 tendril_interests-0.6.0/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2024-04-09 21:11:30.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.583837 tendril_interests-0.6.0/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril_interests-0.6.0/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/src/tendril/policies/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril_interests-0.6.0/src/tendril/policies/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril_interests-0.6.0/src/tendril/policies/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril_interests-0.6.0/src/tendril/policies/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/src/tendril_interests.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3368 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      736 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tox.ini
```

### Comparing `tendril_interests-0.5.8/.gitignore` & `tendril_interests-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/.readthedocs.yml` & `tendril_interests-0.6.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/.travis.yml` & `tendril_interests-0.6.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/LICENSE` & `tendril_interests-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/PKG-INFO` & `tendril_interests-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.5.8
+Version: 0.6.0
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
@@ -32,15 +32,15 @@
 Requires-Dist: pytz
 Requires-Dist: polars
 Requires-Dist: makefun
 Requires-Dist: asgiref
 Requires-Dist: inflection
 Requires-Dist: deepdiff[optimize]
 Requires-Dist: tendril-utils-types
-Requires-Dist: tendril-connector-rabbitmq
+Requires-Dist: tendril-connector-rabbitmq>=0.2.0
 Requires-Dist: tendril-connector-influxdb
 Requires-Dist: tendril-connector-grafana
 Requires-Dist: tendril-apiserver-core
 Requires-Dist: wheel
 Provides-Extra: docs
 Requires-Dist: setuptools_scm; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `tendril_interests-0.5.8/README.rst` & `tendril_interests-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/Makefile` & `tendril_interests-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/_static/custom.css` & `tendril_interests-0.6.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/_static/favicon.ico` & `tendril_interests-0.6.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/_static/logo.png` & `tendril_interests-0.6.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/_static/logo_packed.png` & `tendril_interests-0.6.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/_templates/about.html` & `tendril_interests-0.6.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/conf.py` & `tendril_interests-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/index.rst` & `tendril_interests-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/docs/installation.rst` & `tendril_interests-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/setup.py` & `tendril_interests-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     'pytz',
     'polars',
     'makefun',
     'asgiref',
     'inflection',
     'deepdiff[optimize]',
     'tendril-utils-types',
-    'tendril-connector-rabbitmq',
+    'tendril-connector-rabbitmq>=0.2.0',
     'tendril-connector-influxdb',
     'tendril-connector-grafana',
     'tendril-apiserver-core',  # Need this because of HTTPCodedException import which are otherwise unused. Cleanup instead.
 ]
 
 install_requires = core_dependencies + ['wheel']
```

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/routers/interests.py` & `tendril_interests-0.6.0/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/base.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/interests.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_approvals.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_graphs.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_graphs.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_monitors.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_monitors.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/apiserver/templates/interests_policies.py` & `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/authz/approvals/interests.py` & `tendril_interests-0.6.0/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/authz/approvals/manager.py` & `tendril_interests-0.6.0/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/authz/roles/interests.py` & `tendril_interests-0.6.0/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/authz/roles/interests_approvals.py` & `tendril_interests-0.6.0/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/common/interests/approvals.py` & `tendril_interests-0.6.0/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/common/interests/exceptions.py` & `tendril_interests-0.6.0/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/common/interests/memberships.py` & `tendril_interests-0.6.0/src/tendril/common/interests/memberships.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/config/__init__.py` & `tendril_interests-0.6.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/config/interests.py` & `tendril_interests-0.6.0/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/controllers/interests.py` & `tendril_interests-0.6.0/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/controllers/interests_approvals.py` & `tendril_interests-0.6.0/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/controllers/interests_policies.py` & `tendril_interests-0.6.0/src/tendril/db/controllers/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/models/interests.py` & `tendril_interests-0.6.0/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/models/interests_approvals.py` & `tendril_interests-0.6.0/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/db/models/interests_policies.py` & `tendril_interests-0.6.0/src/tendril/db/models/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/base.py` & `tendril_interests-0.6.0/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/manager.py` & `tendril_interests-0.6.0/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/approvals.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/export.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/export.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/graphs.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/graphs.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/localizers.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/localizers.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/monitors.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/monitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 tags[spec.multiple_discriminators[0]] = parts[0]
             if len(parts) > 1:
                 raise ValueError(f"Don't know how to construct an influxdb "
                                  f"string from parts {parts}")
 
         return measurement, tags
 
-    @with_mq_client
+    @with_mq_client()
     async def monitor_publish(self, spec: MonitorSpec, value,
                               name=None, timestamp=None,
                               additional_localizers=None,
                               mq=None):
         if not timestamp:
             timestamp = time.clock_gettime_ns(time.CLOCK_REALTIME)
         elif isinstance(timestamp, datetime):
```

### Comparing `tendril_interests-0.5.8/src/tendril/interests/mixins/policies.py` & `tendril_interests-0.6.0/src/tendril/interests/mixins/policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/libraries/interests/base.py` & `tendril_interests-0.6.0/src/tendril/libraries/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/libraries/interests/manager.py` & `tendril_interests-0.6.0/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/monitors/spec.py` & `tendril_interests-0.6.0/src/tendril/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/policies/base.py` & `tendril_interests-0.6.0/src/tendril/policies/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril/policies/manager.py` & `tendril_interests-0.6.0/src/tendril/policies/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril_interests.egg-info/PKG-INFO` & `tendril_interests-0.6.0/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.5.8
+Version: 0.6.0
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
@@ -32,15 +32,15 @@
 Requires-Dist: pytz
 Requires-Dist: polars
 Requires-Dist: makefun
 Requires-Dist: asgiref
 Requires-Dist: inflection
 Requires-Dist: deepdiff[optimize]
 Requires-Dist: tendril-utils-types
-Requires-Dist: tendril-connector-rabbitmq
+Requires-Dist: tendril-connector-rabbitmq>=0.2.0
 Requires-Dist: tendril-connector-influxdb
 Requires-Dist: tendril-connector-grafana
 Requires-Dist: tendril-apiserver-core
 Requires-Dist: wheel
 Provides-Extra: docs
 Requires-Dist: setuptools_scm; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `tendril_interests-0.5.8/src/tendril_interests.egg-info/SOURCES.txt` & `tendril_interests-0.6.0/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/src/tendril_interests.egg-info/requires.txt` & `tendril_interests-0.6.0/src/tendril_interests.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pytz
 polars
 makefun
 asgiref
 inflection
 deepdiff[optimize]
 tendril-utils-types
-tendril-connector-rabbitmq
+tendril-connector-rabbitmq>=0.2.0
 tendril-connector-influxdb
 tendril-connector-grafana
 tendril-apiserver-core
 wheel
 
 [build]
 setuptools_scm
```

### Comparing `tendril_interests-0.5.8/tests/coveralls.py` & `tendril_interests-0.6.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.5.8/tox.ini` & `tendril_interests-0.6.0/tox.ini`

 * *Files identical despite different names*

