# Comparing `tmp/design.plone.iocittadino-1.0.0b8.tar.gz` & `tmp/design.plone.iocittadino-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.iocittadino-1.0.0b8.tar", last modified: Tue Mar  5 13:34:43 2024, max compression
+gzip compressed data, was "design.plone.iocittadino-1.0.0b9.tar", last modified: Tue Mar 12 13:25:28 2024, max compression
```

## Comparing `design.plone.iocittadino-1.0.0b8.tar` & `design.plone.iocittadino-1.0.0b9.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.352168 design.plone.iocittadino-1.0.0b8/
--rw-r--r--   0 lucabel    (501) staff       (20)     2195 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/.gitlab-ci.yml
--rw-r--r--   0 lucabel    (501) staff       (20)     5073 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)     1338 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      121 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    27191 2024-03-05 13:34:43.351794 design.plone.iocittadino-1.0.0b8/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    20478 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)     2623 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/TODO.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.220409 design.plone.iocittadino-1.0.0b8/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7971 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       95 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      363 2024-03-05 13:34:43.353213 design.plone.iocittadino-1.0.0b8/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2420 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.189654 design.plone.iocittadino-1.0.0b8/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.221023 design.plone.iocittadino-1.0.0b8/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.227343 design.plone.iocittadino-1.0.0b8/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.231391 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/
--rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.233131 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1191 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2732 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/mailfromfield.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.234857 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      332 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.238583 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/
--rw-r--r--   0 lucabel    (501) staff       (20)    10198 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      351 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    14501 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/message.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.239678 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/mixins/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/mixins/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      418 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/mixins/current_user.py
--rw-r--r--   0 lucabel    (501) staff       (20)    20129 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      118 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/types.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4787 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/user.py
--rw-r--r--   0 lucabel    (501) staff       (20)      365 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/indexers.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.241361 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      742 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1671 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/constrains.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.243019 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      717 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.245391 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1584 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     7252 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/download.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4085 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/download_traversers.py
--rw-r--r--   0 lucabel    (501) staff       (20)      784 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/mail.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.246005 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/static/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/static/.gitkeep
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.194624 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/templates/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.246508 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/templates/mail/
--rw-r--r--   0 lucabel    (501) staff       (20)    10319 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/templates/mail/mail.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1959 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.247635 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      278 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/content/modello_pratica.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.248869 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/
--rw-r--r--   0 lucabel    (501) staff       (20)     2999 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      201 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.251219 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1620 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/blob_storage.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.254448 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/
--rw-r--r--   0 lucabel    (501) staff       (20)      559 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      646 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1321 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/message_catalog.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1808 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/pratica_catalog.py
--rw-r--r--   0 lucabel    (501) staff       (20)      281 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/user_catalog.py
--rw-r--r--   0 lucabel    (501) staff       (20)      475 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    12702 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/store.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.255092 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/demo/
--rw-r--r--   0 lucabel    (501) staff       (20)   145225 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/demo/demo_contents.json
--rw-r--r--   0 lucabel    (501) staff       (20)      290 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/dependencies.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.257120 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      518 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.258242 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      153 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.259930 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1775 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1146 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.262205 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2433 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/message.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11612 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1355 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/modellopratica.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.262807 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/exceptions/
--rw-r--r--   0 lucabel    (501) staff       (20)      197 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/exceptions/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.267532 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)     1055 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/layer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4061 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/modello_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/pdf.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4275 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/store.py
--rw-r--r--   0 lucabel    (501) staff       (20)      235 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/traversing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.271530 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.199461 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/__pycache__/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.272147 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     9376 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/design.plone.iocittadino.po
--rw-r--r--   0 lucabel    (501) staff       (20)     9503 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/design.plone.iocittadino.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.200070 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.272817 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     9376 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/en/LC_MESSAGES/design.plone.iocittadino.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.200682 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.273459 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    11381 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/it/LC_MESSAGES/design.plone.iocittadino.po
--rw-r--r--   0 lucabel    (501) staff       (20)     1595 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      509 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/update.sh
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.276504 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/
--rw-r--r--   0 lucabel    (501) staff       (20)     4300 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/assegno_maternita.json
--rw-r--r--   0 lucabel    (501) staff       (20)     9224 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/contrassegno_parcheggio_disabili.json
--rw-r--r--   0 lucabel    (501) staff       (20)     2495 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/empty.json
--rw-r--r--   0 lucabel    (501) staff       (20)     6869 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/suolo_pubblico.json
--rw-r--r--   0 lucabel    (501) staff       (20)     3579 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/test_spid.json
--rw-r--r--   0 lucabel    (501) staff       (20)     1086 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.203601 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.282691 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      197 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      629 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      198 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.283795 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)      142 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/registry/main.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      258 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1322 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.285617 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     2837 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/types/ModelloPratica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      295 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/types/Servizio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      317 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.286356 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/demo_contents/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/demo_contents/.gitkeep
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.288879 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      134 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      348 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      269 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/uninstall/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.290239 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      190 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.293936 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      597 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4911 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/message.py
--rw-r--r--   0 lucabel    (501) staff       (20)      992 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/mixin.py
--rw-r--r--   0 lucabel    (501) staff       (20)      798 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/modello_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7742 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/pratiche.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.295011 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      260 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.298528 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      927 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1248 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1608 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3224 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1948 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/update.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.300229 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message_workflow/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      400 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message_workflow/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1244 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message_workflow/workflow.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.301909 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/operatori_pratica/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/operatori_pratica/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      393 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/operatori_pratica/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1181 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/operatori_pratica/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.305392 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1475 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1335 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1762 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6051 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2866 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/update.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.307430 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica_workflow/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      400 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica_workflow/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2074 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica_workflow/workflow.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1939 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/setuphandlers.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.309710 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/
--rw-r--r--   0 lucabel    (501) staff       (20)     1990 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      578 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.312814 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/
--rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      225 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2409 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/fields.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.316675 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     1127 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_checkbox.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      692 2024-03-05 13:34:41.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_html.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      859 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_radiogroup.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_text.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3630 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/pratica.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.318532 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/
--rw-r--r--   0 lucabel    (501) staff       (20)      775 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/fonts.css
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/main.css
--rw-r--r--   0 lucabel    (501) staff       (20)     1848 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/pratica.css
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.319151 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)      927 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/templates/pratica_pdf.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     2074 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.345148 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)       81 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3661 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/disabled_test_view_pratica_report.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13264 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/dummy.pdf
--rw-r--r--   0 lucabel    (501) staff       (20)     4391 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/restapi_mixin.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3469 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_ct_modello_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3726 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_download_report.py
--rw-r--r--   0 lucabel    (501) staff       (20)      650 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_group.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6186 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_event_creation_notify.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3639 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_extender.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9548 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2283 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4117 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2452 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_patch.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7170 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_transition.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1505 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_operatori_pratica_restapi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2368 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_assigned_notify.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1990 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_created_notify_editor.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_transition_notify.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3749 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_extender.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4810 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11226 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3404 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3081 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6206 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_patch.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4619 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8763 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_transition.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5027 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2496 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5639 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5790 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_lisitng.py
--rw-r--r--   0 lucabel    (501) staff       (20)      873 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_patch.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2869 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_workflow.py
--rw-r--r--   0 lucabel    (501) staff       (20)      692 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_modello_pratica_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4110 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3459 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10877 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6346 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_listing.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3855 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_patch.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2624 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_workflow.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3561 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_user_store.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.346811 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      853 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      701 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/upgrades.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.348486 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      251 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1164 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/vocabularies/vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-05 13:34:43.349241 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    27191 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    11904 2024-03-05 13:34:43.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      129 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      301 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-03-05 13:34:42.000000 design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.652637 design.plone.iocittadino-1.0.0b9/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2195 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/.gitlab-ci.yml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5404 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)     1338 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      121 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    27016 2024-03-12 13:25:28.652790 design.plone.iocittadino-1.0.0b9/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    20594 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)     2623 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/TODO.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.594925 design.plone.iocittadino-1.0.0b9/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7971 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       95 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      363 2024-03-12 13:25:28.653375 design.plone.iocittadino-1.0.0b9/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2420 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.583048 design.plone.iocittadino-1.0.0b9/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.595196 design.plone.iocittadino-1.0.0b9/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.597865 design.plone.iocittadino-1.0.0b9/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.599561 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/
+-rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.600321 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1191 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2732 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/mailfromfield.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.601122 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      332 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.602815 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/
+-rw-r--r--   0 lucabel    (501) staff       (20)    10198 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      351 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    14501 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/message.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.603294 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/mixins/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/mixins/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      418 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/mixins/current_user.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    20129 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      118 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/types.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4921 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/user.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      365 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/indexers.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.604009 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      742 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1671 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/constrains.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.604683 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      717 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.605627 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1584 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     7252 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/download.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4085 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/download_traversers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      784 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/mail.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.605920 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/static/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/static/.gitkeep
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.584851 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/templates/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.606122 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/templates/mail/
+-rw-r--r--   0 lucabel    (501) staff       (20)    10319 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/templates/mail/mail.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     1959 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.606544 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      278 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/content/modello_pratica.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.607161 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2999 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      201 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.608081 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1620 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/blob_storage.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.609399 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/
+-rw-r--r--   0 lucabel    (501) staff       (20)      559 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      646 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1321 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/message_catalog.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1808 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/pratica_catalog.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      281 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/user_catalog.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      475 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    12702 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/store.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.609633 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/demo/
+-rw-r--r--   0 lucabel    (501) staff       (20)   145225 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/demo/demo_contents.json
+-rw-r--r--   0 lucabel    (501) staff       (20)      290 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/dependencies.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.610428 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      518 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.611003 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      153 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.611661 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1775 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1146 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.612667 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2433 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/message.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11612 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1355 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/modellopratica.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.613028 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/exceptions/
+-rw-r--r--   0 lucabel    (501) staff       (20)      197 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/exceptions/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.615395 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1122 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/layer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4061 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/modello_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/pdf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4487 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/store.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      235 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/traversing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.618546 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.586936 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/__pycache__/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.618776 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     9376 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/design.plone.iocittadino.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     9503 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/design.plone.iocittadino.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.587198 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.619595 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     9376 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/en/LC_MESSAGES/design.plone.iocittadino.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.587461 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.619930 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    11381 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/it/LC_MESSAGES/design.plone.iocittadino.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1595 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      509 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/update.sh
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.621178 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/
+-rw-r--r--   0 lucabel    (501) staff       (20)     4300 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/assegno_maternita.json
+-rw-r--r--   0 lucabel    (501) staff       (20)     9224 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/contrassegno_parcheggio_disabili.json
+-rw-r--r--   0 lucabel    (501) staff       (20)     2495 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/empty.json
+-rw-r--r--   0 lucabel    (501) staff       (20)     6869 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/suolo_pubblico.json
+-rw-r--r--   0 lucabel    (501) staff       (20)     3579 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/test_spid.json
+-rw-r--r--   0 lucabel    (501) staff       (20)     1086 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.588471 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.623382 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      197 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      629 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      198 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.623828 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)      142 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/registry/main.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      258 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1322 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.624292 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2837 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/types/ModelloPratica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      295 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/types/Servizio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      317 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.624520 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/demo_contents/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/demo_contents/.gitkeep
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.625313 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      134 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      348 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      269 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/uninstall/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.625782 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      190 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.627519 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      597 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5190 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/message.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      992 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/mixin.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      798 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/modello_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7742 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/pratiche.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.628005 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      260 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.629760 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      927 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1248 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1608 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3224 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1948 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/update.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.630406 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message_workflow/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message_workflow/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      400 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message_workflow/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1244 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message_workflow/workflow.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.631056 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/operatori_pratica/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/operatori_pratica/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      393 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/operatori_pratica/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1181 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/operatori_pratica/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.633168 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1475 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1335 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1762 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6051 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2866 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/update.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.634262 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica_workflow/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica_workflow/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      400 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica_workflow/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2074 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica_workflow/workflow.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1939 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/setuphandlers.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.635010 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1990 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      578 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.635740 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/
+-rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      225 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2409 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/fields.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.636799 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1127 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_checkbox.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)      692 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_html.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)      859 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_radiogroup.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_text.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3630 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/pratica.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.637895 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/
+-rw-r--r--   0 lucabel    (501) staff       (20)      775 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/fonts.css
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/main.css
+-rw-r--r--   0 lucabel    (501) staff       (20)     1848 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/pratica.css
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.638181 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)      927 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/templates/pratica_pdf.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     2074 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.650871 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)       81 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3661 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/disabled_test_view_pratica_report.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13264 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/dummy.pdf
+-rw-r--r--   0 lucabel    (501) staff       (20)     4391 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/restapi_mixin.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3469 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_ct_modello_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3726 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_download_report.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      650 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_group.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6186 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_event_creation_notify.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4726 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_extender.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9548 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2283 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4117 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2452 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_patch.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7170 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_transition.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1505 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_operatori_pratica_restapi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2368 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_assigned_notify.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1990 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_created_notify_editor.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_transition_notify.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3749 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_extender.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4810 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11226 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3404 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3081 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6206 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_patch.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4619 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8763 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_transition.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5027 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2496 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5639 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5790 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_lisitng.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      873 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_patch.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2869 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_workflow.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      692 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_modello_pratica_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4110 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3459 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10877 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6346 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_listing.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3855 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_patch.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2624 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_workflow.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3561 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_user_store.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.651683 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      853 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      701 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/upgrades.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.652424 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      251 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1164 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/vocabularies/vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-12 13:25:28.597587 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    27016 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    11904 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      129 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      301 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-03-12 13:25:28.000000 design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/top_level.txt
```

### Comparing `design.plone.iocittadino-1.0.0b8/.gitlab-ci.yml` & `design.plone.iocittadino-1.0.0b9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/CHANGES.rst` & `design.plone.iocittadino-1.0.0b9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 Changelog
 =========
 
+1.0.0b9 (2024-03-12)
+--------------------
+
+- Aggiunto modo per aggiungere campi al messaggio e al suo summary serializer
+  registrando delle utility per interfacce predefinite
+  [lucabel]
+- Aggiunto campi precompilabili (idCard, expirationDate, countyOfBirth, 
+  placeOfBirthName, placeOfBirth, placeOfBirthIstatCode)
+  [lucabel]
+
+
+
 1.0.0b8 (2024-03-05)
 --------------------
-- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b7 (unreleased)
 --------------------
 
 - Fix the PDF Report + new survey field type added to pdf generation: radiogroup
   [folix-01]
 - Fix: #49945 l'areaopeartore va in errore se il modello pratica è stato cancellato
   (Aggiunto workaround per non mandare in errore, serve però che i dati siano in qualche modo
   recuperabili anche se il modello è stato eliminato)
   [mamico]
-- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b6 (2023-10-25)
 --------------------
 
 - Allow users to retrieve their own messages also if ModelloPratica is private.
```

### Comparing `design.plone.iocittadino-1.0.0b8/DEVELOP.rst` & `design.plone.iocittadino-1.0.0b9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/LICENSE.GPL` & `design.plone.iocittadino-1.0.0b9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/LICENSE.rst` & `design.plone.iocittadino-1.0.0b9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/PKG-INFO` & `design.plone.iocittadino-1.0.0b9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.iocittadino
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: An add-on for Plone
 Home-page: https://gitlab.com/redturtle/io-comune/design.plone.iocittadino
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,31 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: design.plone.policy
-Requires-Dist: souper.plone
-Requires-Dist: weasyprint>=58.1
-Requires-Dist: collective.z3cform.datagridfield>=3.0.0
-Requires-Dist: collective.exportimport
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
-Requires-Dist: freezegun; extra == "test"
-Requires-Dist: redturtle.prenotazioni; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://gitlab.com/redturtle/io-comune/design.plone.iocittadino/badges/master/coverage.svg
 
@@ -544,15 +530,17 @@
                 "new_field_a": "A_value",
                 "new_field_b": "B_value",
                 "new_field_c": "C_value",
             }
 
 La stessa identica cosa è possibile per i messaggi, registrando utility fatte
 alla stessa identica maniera per le interfacce IMessageStoreFieldsExtender e
-IMessageStoreSerializerExtender
+IMessageStoreSerializerExtender; c'è inoltre un'interfaccia
+IMessageStoreSerializerSummaryExtender utile per estendere il serializer dell
+summary.
 
 
 Traduzioni
 ==========
 
 Questo prodotto è stato tradotto in:
 
@@ -613,30 +601,42 @@
 
 - RedTurtle, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+1.0.0b9 (2024-03-12)
+--------------------
+
+- Aggiunto modo per aggiungere campi al messaggio e al suo summary serializer
+  registrando delle utility per interfacce predefinite
+  [lucabel]
+- Aggiunto campi precompilabili (idCard, expirationDate, countyOfBirth, 
+  placeOfBirthName, placeOfBirth, placeOfBirthIstatCode)
+  [lucabel]
+
+
+
 1.0.0b8 (2024-03-05)
 --------------------
-- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b7 (unreleased)
 --------------------
 
 - Fix the PDF Report + new survey field type added to pdf generation: radiogroup
   [folix-01]
 - Fix: #49945 l'areaopeartore va in errore se il modello pratica è stato cancellato
   (Aggiunto workaround per non mandare in errore, serve però che i dati siano in qualche modo
   recuperabili anche se il modello è stato eliminato)
   [mamico]
-- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b6 (2023-10-25)
 --------------------
 
 - Allow users to retrieve their own messages also if ModelloPratica is private.
```

### Comparing `design.plone.iocittadino-1.0.0b8/README.rst` & `design.plone.iocittadino-1.0.0b9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,17 @@
                 "new_field_a": "A_value",
                 "new_field_b": "B_value",
                 "new_field_c": "C_value",
             }
 
 La stessa identica cosa è possibile per i messaggi, registrando utility fatte
 alla stessa identica maniera per le interfacce IMessageStoreFieldsExtender e
-IMessageStoreSerializerExtender
+IMessageStoreSerializerExtender; c'è inoltre un'interfaccia
+IMessageStoreSerializerSummaryExtender utile per estendere il serializer dell
+summary.
 
 
 Traduzioni
 ==========
 
 Questo prodotto è stato tradotto in:
```

### Comparing `design.plone.iocittadino-1.0.0b8/TODO.txt` & `design.plone.iocittadino-1.0.0b9/TODO.txt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/docs/conf.py` & `design.plone.iocittadino-1.0.0b9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/setup.py` & `design.plone.iocittadino-1.0.0b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.iocittadino",
-    version="1.0.0b8",
+    version="1.0.0b9",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/actions/mailfromfield.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/actions/mailfromfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/__init__.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/message.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/message.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/adapters/content_store/user.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/adapters/content_store/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,30 @@
     # TODO: usare il registry
     # we can have saved the field timestamp to manage the
     # privacy requirements
     # the name convetion should have the following format: "<key>.timestamp" = "2023-08-21T10:34:51.252947"
     user_properties = [
         "id",
         "fullname",
-        "fullname",
         "nome",
         "cognome",
         "fiscalNumber",
         "mobile",
         "gender",
         "dateOfBirth",
         "placeOfBirth",
         "address",
         "digitalAddress",
         "email",
+        "placeOfBirth",
+        "placeOfBirthIstatCode",
+        "placeOfBirthName",
+        "countyOfBirth",
+        "idCard",
+        "expirationDate",
     ]
 
     def __init__(self, context, user, request):
         self.context = context
         self.user = user
         self.request = request
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/behaviors/constrains.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/behaviors/constrains.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/download.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/download.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/download/download_traversers.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/download/download_traversers.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/mail.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/mail.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/browser/templates/mail/mail.pt` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/browser/templates/mail/mail.pt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/__init__.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/blob_storage.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/blob_storage.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/__init__.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/message_catalog.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/message_catalog.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/catalog/pratica_catalog.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/catalog/pratica_catalog.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/data_store/soup/store.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/data_store/soup/store.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/demo/demo_contents.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/demo/demo_contents.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/events.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/events.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/events/interfaces.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/events/interfaces.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/message.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/message.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/content_store/handlers/pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/content_store/handlers/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/events/modellopratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/events/modellopratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/__init__.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 from .store import ISerializeMessageToJsonSummary  # noqa
 from .store import ISerializePraticaToJson  # noqa
 from .store import ISerializePraticaToJsonSummary  # noqa
 from .store import ISerializePraticheToJson  # noqa
 from .store import IUserStore  # noqa
 from .store import IMessageStoreFieldsExtender  # noqa
 from .store import IMessageStoreSerializerExtender  # noqa
+from .store import IMessageStoreSerializerSumamaryExtender  # noqa
 from .traversing import IBlobTraverse  # noqa
 from .traversing import IMessageTraverse  # noqa
 from .traversing import IPraticaTraverse  # noqa
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/modello_pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/modello_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/interfaces/store.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/interfaces/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,21 @@
 class IMessageStoreSerializerExtender(Interface):
     """
     Interface for Message Store serializer; we can use it to mark utilities that
     provides metadata to extend the default serializer
     """
 
 
+class IMessageStoreSerializerSumamaryExtender(Interface):
+    """
+    Interface for Message Store serializer; we can use it to mark utilities that
+    provides metadata to extend the default serializer
+    """
+
+
 class IMessageContentStore(Interface):
     """
     Interface for Store adapters. Each adapter should implement these methods
     """
 
     def __init__(context, request):
         """
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/README.rst` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/design.plone.iocittadino.po` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/__pycache__/LC_MESSAGES/design.plone.iocittadino.po`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/design.plone.iocittadino.pot` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/design.plone.iocittadino.pot`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/en/LC_MESSAGES/design.plone.iocittadino.po` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/en/LC_MESSAGES/design.plone.iocittadino.po`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/it/LC_MESSAGES/design.plone.iocittadino.po` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/it/LC_MESSAGES/design.plone.iocittadino.po`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/locales/update.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/assegno_maternita.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/assegno_maternita.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/contrassegno_parcheggio_disabili.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/contrassegno_parcheggio_disabili.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/empty.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/empty.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/suolo_pubblico.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/suolo_pubblico.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/models/test_spid.json` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/models/test_spid.json`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/permissions.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/controlpanel.xml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/rolemap.xml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/profiles/default/types/ModelloPratica.xml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/profiles/default/types/ModelloPratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/message.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from zope.component import getAllUtilitiesRegisteredFor
 from design.plone.iocittadino.interfaces import IPraticaContentStore
 from design.plone.iocittadino.interfaces import ISerializeMessagesToJson
 from design.plone.iocittadino.interfaces import ISerializeMessageToJson
 from design.plone.iocittadino.interfaces import ISerializeMessageToJsonSummary
 from design.plone.iocittadino.interfaces import ISerializePraticaToJsonSummary
 from design.plone.iocittadino.interfaces.store import IMessageStoreSerializerExtender
+from design.plone.iocittadino.interfaces.store import (
+    IMessageStoreSerializerSumamaryExtender,
+)
 
 from .mixin import PortalUrlMixIn
 
 
 class MessageAttachmentsMixIn(PortalUrlMixIn):
     message = None
 
@@ -112,14 +115,18 @@
             "item_id": self.message.intid,
             "title": self.message.attrs.get("title"),
             "userid": self.message.attrs.get("userid"),
             "state": self.message.attrs.get("state"),
             "date": datetimelike_to_iso(self.message.attrs.get("date")),
             "message": self.message.attrs.get("message"),
         }
+        for utility in getAllUtilitiesRegisteredFor(
+            IMessageStoreSerializerSumamaryExtender
+        ):
+            result.update(utility.get_fields(self.message))
         return result
 
 
 @interface.implementer(ISerializeMessagesToJson)
 @component.adapter(list, interface.Interface)
 class MessageListSerializer:
     def __init__(self, messages, request):
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/mixin.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/mixin.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/modello_pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/modello_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/serializers/pratiche.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/serializers/pratiche.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message/update.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/message_workflow/workflow.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/message_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/operatori_pratica/get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/operatori_pratica/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica/update.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/restapi/services/pratica_workflow/workflow.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/restapi/services/pratica_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/setuphandlers.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/__init__.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/fields.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_checkbox.pt` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_checkbox.pt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_html.pt` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_html.pt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_radiogroup.pt` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/fields/templates/survey_radiogroup.pt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/fonts.css` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/fonts.css`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/static/pratica.css` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/static/pratica.css`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/survey_pdf/templates/pratica_pdf.pt` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/survey_pdf/templates/pratica_pdf.pt`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/testing.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/disabled_test_view_pratica_report.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/disabled_test_view_pratica_report.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/dummy.pdf` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/dummy.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/restapi_mixin.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/restapi_mixin.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_ct_modello_pratica.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_ct_modello_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_download_report.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_download_report.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_group.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_event_creation_notify.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_event_creation_notify.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_extender.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_extender.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,112 +1,113 @@
 # -*- coding: utf-8 -*-
 # import datetime
-import base64
+import unittest
 
-import transaction
-from pkg_resources import resource_string
+# import freezegun
+from plone import api
+from plone.app.testing import TEST_USER_ID
+from plone.app.testing import setRoles
+from Products.CMFPlone.tests.utils import MockMailHost
+from Products.MailHost.interfaces import IMailHost
 
 # from z3c.relationfield import RelationValue
 from zope import interface
 from zope.component import getMultiAdapter
 from zope.component import getSiteManager
 
-from design.plone.iocittadino.interfaces import IMessageContentStore
-from design.plone.iocittadino.interfaces import IMessageStoreFieldsExtender
-from design.plone.iocittadino.interfaces import IMessageStoreSerializerExtender
 from design.plone.iocittadino.interfaces import IPraticaContentStore
-from design.plone.iocittadino.tests.restapi_mixin import Mixin
+from design.plone.iocittadino.interfaces import IPraticaStoreFieldsExtender
+from design.plone.iocittadino.interfaces import IPraticaStoreSerializerExtender
+from design.plone.iocittadino.interfaces import ISerializePraticaToJson
+from design.plone.iocittadino.testing import DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
 
-PDF_B64 = base64.b64encode(
-    resource_string("design.plone.iocittadino.tests", "dummy.pdf")
-)
+# from zope.component import getUtility
+# from zope.intid.interfaces import IIntIds
 
 
-@interface.implementer(IMessageStoreFieldsExtender)
+@interface.implementer(IPraticaStoreFieldsExtender)
 class FieldExtender(object):
     @property
     def fields(self):
         return {
             "new_field_a": {"required": False},
             "new_field_b": {"required": False},
             "new_field_c": {"required": False},
         }
 
 
-@interface.implementer(IMessageStoreSerializerExtender)
-class ExtendsMessageSerializer(object):
+@interface.implementer(IPraticaStoreSerializerExtender)
+class ExtendsPraticaSerializer(object):
     def get_fields(self, pratica):
         return {
             "new_field_a": "A_value",
             "new_field_b": "B_value",
             "new_field_c": "C_value",
         }
 
 
-class TestPraticaExtender(Mixin):
-    # layer = DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
+class TestPraticaExtender(unittest.TestCase):
+    layer = DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
 
     def setUp(self):
-        super().setUp()
+        self.app = self.layer["app"]
         self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+        self.portal._original_MailHost = self.portal.MailHost
+        self.portal.MailHost = mailhost = MockMailHost("MailHost")
+        api.portal.set_registry_record(
+            "plone.email_from_address", "noreply@holokinesislibros.com"
+        )
         sm = getSiteManager(context=self.portal)
-        self.pratica_id = self.pratica_storage.add(
-            {
-                "form_id": self.modello_pratica.UID(),
-                "data": "a value",
-            }
-        ).intid
 
-        self.message_initial_state = "pending"
-        self.message_text = "Testing message"
-        self.message_id = self.message_storage.add(
-            {
-                "pratica_id": self.pratica_id,
-                "message": self.message_text,
-                "attachments": [
-                    {
-                        "name": "dummy.txt",
-                        "data": "data:plain/text;base64,ZHVtbXkgdGV4dCBmaWxl",
-                    },
-                    {
-                        "name": "dummy.pdf",
-                        "data": f"data:application/pdf;base64,${PDF_B64}",
-                    },
-                ],
-            }
-        ).intid
+        sm.unregisterUtility(provided=IMailHost)
+        sm.registerUtility(mailhost, provided=IMailHost)
+
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+
+        # create contents
+        self.servizio = api.content.create(
+            type="Servizio",
+            id="example-service",
+            title="Example Service",
+            container=self.portal,
+        )
+
+        self.modello_pratica = api.content.create(
+            type="ModelloPratica",
+            id="example-modello",
+            title="Example Modello",
+            container=self.servizio,
+        )
 
         # register utility for file extension
         sm.registerUtility(
-            FieldExtender(), name="field_extender", provided=IMessageStoreFieldsExtender
+            FieldExtender(), name="field_extender", provided=IPraticaStoreFieldsExtender
         )
         sm.registerUtility(
-            ExtendsMessageSerializer(),
+            ExtendsPraticaSerializer(),
             name="serializer_extender",
-            provided=IMessageStoreSerializerExtender,
+            provided=IPraticaStoreSerializerExtender,
         )
-        transaction.commit()
 
     @property
-    def pratica_storage(self):
+    def tool(self):
         return getMultiAdapter((self.portal, self.request), IPraticaContentStore)
 
-    @property
-    def message_storage(self):
-        return getMultiAdapter((self.portal, self.request), IMessageContentStore)
-
     def test_extended_fields(self):
-        fields = self.message_storage.fields
+        fields = self.tool.fields
         self.assertIn("new_field_a", fields)
         self.assertIn("new_field_b", fields)
         self.assertIn("new_field_c", fields)
 
-    def test_get_return_serialized_data(self):
-        resp = self.api_session_manager.get(
-            f"{self.portal_url}/@message/{self.message_id}",
-        )
-        self.assertEqual(resp.status_code, 200)
-
-        res = resp.json()
-        self.assertEqual(res["new_field_a"], "A_value")
-        self.assertEqual(res["new_field_b"], "B_value")
-        self.assertEqual(res["new_field_c"], "C_value")
+    def test_extended_serializer(self):
+        pratica = self.tool.add(
+            {
+                "form_id": self.modello_pratica.UID(),
+                "data": "some data",
+                "state": "ongoing",
+            }
+        )
+        result = getMultiAdapter((pratica, self.request), ISerializePraticaToJson)()
+        self.assertIn("new_field_a", result)
+        self.assertIn("new_field_b", result)
+        self.assertIn("new_field_c", result)
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_patch.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_patch.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_message_store_transition.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_store_transition.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_operatori_pratica_restapi.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_operatori_pratica_restapi.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_assigned_notify.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_assigned_notify.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_created_notify_editor.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_created_notify_editor.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_event_transition_notify.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_event_transition_notify.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_extender.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_message_extender.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,140 @@
 # -*- coding: utf-8 -*-
 # import datetime
-import unittest
+import base64
 
-# import freezegun
-from plone import api
-from plone.app.testing import TEST_USER_ID
-from plone.app.testing import setRoles
-from Products.CMFPlone.tests.utils import MockMailHost
-from Products.MailHost.interfaces import IMailHost
+import transaction
+from pkg_resources import resource_string
 
 # from z3c.relationfield import RelationValue
 from zope import interface
 from zope.component import getMultiAdapter
 from zope.component import getSiteManager
 
+from design.plone.iocittadino.interfaces import IMessageContentStore
+from design.plone.iocittadino.interfaces import IMessageStoreFieldsExtender
+from design.plone.iocittadino.interfaces import IMessageStoreSerializerExtender
+from design.plone.iocittadino.interfaces import IMessageStoreSerializerSumamaryExtender
 from design.plone.iocittadino.interfaces import IPraticaContentStore
-from design.plone.iocittadino.interfaces import IPraticaStoreFieldsExtender
-from design.plone.iocittadino.interfaces import IPraticaStoreSerializerExtender
-from design.plone.iocittadino.interfaces import ISerializePraticaToJson
-from design.plone.iocittadino.testing import DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
+from design.plone.iocittadino.tests.restapi_mixin import Mixin
 
-# from zope.component import getUtility
-# from zope.intid.interfaces import IIntIds
+PDF_B64 = base64.b64encode(
+    resource_string("design.plone.iocittadino.tests", "dummy.pdf")
+)
 
 
-@interface.implementer(IPraticaStoreFieldsExtender)
+@interface.implementer(IMessageStoreFieldsExtender)
 class FieldExtender(object):
     @property
     def fields(self):
         return {
             "new_field_a": {"required": False},
             "new_field_b": {"required": False},
             "new_field_c": {"required": False},
         }
 
 
-@interface.implementer(IPraticaStoreSerializerExtender)
-class ExtendsPraticaSerializer(object):
+@interface.implementer(IMessageStoreSerializerExtender)
+class ExtendsMessageSerializer(object):
     def get_fields(self, pratica):
         return {
             "new_field_a": "A_value",
             "new_field_b": "B_value",
             "new_field_c": "C_value",
         }
 
 
-class TestPraticaExtender(unittest.TestCase):
-    layer = DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
+@interface.implementer(IMessageStoreSerializerSumamaryExtender)
+class ExtendsMessageSerializerSummary(object):
+    def get_fields(self, pratica):
+        return {
+            "new_field_summary_a": "A_value",
+            "new_field_summary_b": "B_value",
+            "new_field_summary_c": "C_value",
+        }
+
+
+class TestPraticaExtender(Mixin):
+    # layer = DESIGN_PLONE_IOCITTADINO_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.app = self.layer["app"]
+        super().setUp()
         self.portal = self.layer["portal"]
-        self.request = self.layer["request"]
-        self.portal._original_MailHost = self.portal.MailHost
-        self.portal.MailHost = mailhost = MockMailHost("MailHost")
-        api.portal.set_registry_record(
-            "plone.email_from_address", "noreply@holokinesislibros.com"
-        )
         sm = getSiteManager(context=self.portal)
+        self.pratica_id = self.pratica_storage.add(
+            {
+                "form_id": self.modello_pratica.UID(),
+                "data": "a value",
+            }
+        ).intid
 
-        sm.unregisterUtility(provided=IMailHost)
-        sm.registerUtility(mailhost, provided=IMailHost)
-
-        setRoles(self.portal, TEST_USER_ID, ["Manager"])
-
-        # create contents
-        self.servizio = api.content.create(
-            type="Servizio",
-            id="example-service",
-            title="Example Service",
-            container=self.portal,
-        )
-
-        self.modello_pratica = api.content.create(
-            type="ModelloPratica",
-            id="example-modello",
-            title="Example Modello",
-            container=self.servizio,
-        )
+        self.message_initial_state = "pending"
+        self.message_text = "Testing message"
+        self.message_id = self.message_storage.add(
+            {
+                "pratica_id": self.pratica_id,
+                "message": self.message_text,
+                "attachments": [
+                    {
+                        "name": "dummy.txt",
+                        "data": "data:plain/text;base64,ZHVtbXkgdGV4dCBmaWxl",
+                    },
+                    {
+                        "name": "dummy.pdf",
+                        "data": f"data:application/pdf;base64,${PDF_B64}",
+                    },
+                ],
+            }
+        ).intid
 
         # register utility for file extension
         sm.registerUtility(
-            FieldExtender(), name="field_extender", provided=IPraticaStoreFieldsExtender
+            FieldExtender(), name="field_extender", provided=IMessageStoreFieldsExtender
         )
         sm.registerUtility(
-            ExtendsPraticaSerializer(),
+            ExtendsMessageSerializer(),
             name="serializer_extender",
-            provided=IPraticaStoreSerializerExtender,
+            provided=IMessageStoreSerializerExtender,
+        )
+        sm.registerUtility(
+            ExtendsMessageSerializerSummary(),
+            name="serializer_summary_extender",
+            provided=IMessageStoreSerializerSumamaryExtender,
         )
+        transaction.commit()
 
     @property
-    def tool(self):
+    def pratica_storage(self):
         return getMultiAdapter((self.portal, self.request), IPraticaContentStore)
 
+    @property
+    def message_storage(self):
+        return getMultiAdapter((self.portal, self.request), IMessageContentStore)
+
     def test_extended_fields(self):
-        fields = self.tool.fields
+        fields = self.message_storage.fields
         self.assertIn("new_field_a", fields)
         self.assertIn("new_field_b", fields)
         self.assertIn("new_field_c", fields)
 
-    def test_extended_serializer(self):
-        pratica = self.tool.add(
-            {
-                "form_id": self.modello_pratica.UID(),
-                "data": "some data",
-                "state": "ongoing",
-            }
-        )
-        result = getMultiAdapter((pratica, self.request), ISerializePraticaToJson)()
-        self.assertIn("new_field_a", result)
-        self.assertIn("new_field_b", result)
-        self.assertIn("new_field_c", result)
+    def test_get_return_serialized_data(self):
+        resp = self.api_session_manager.get(
+            f"{self.portal_url}/@message/{self.message_id}",
+        )
+        self.assertEqual(resp.status_code, 200)
+
+        res = resp.json()
+        self.assertEqual(res["new_field_a"], "A_value")
+        self.assertEqual(res["new_field_b"], "B_value")
+        self.assertEqual(res["new_field_c"], "C_value")
+
+    def test_get_return_serialized_data_message_summary(self):
+        resp = self.api_session_manager.get(
+            f"{self.portal_url}/@pratiche",
+        )
+        self.assertEqual(resp.status_code, 200)
+
+        res = resp.json()
+        message = res["items"][0]["messages"][0]
+        self.assertEqual(message["new_field_summary_a"], "A_value")
+        self.assertEqual(message["new_field_summary_b"], "B_value")
+        self.assertEqual(message["new_field_summary_c"], "C_value")
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_serializer.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_patch.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_patch.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_search.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_pratica_store_transition.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_pratica_store_transition.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_lisitng.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_lisitng.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_patch.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_patch.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_message_workflow.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_message_workflow.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_modello_pratica_serializer.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_modello_pratica_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_add.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_add.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_delete.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_delete.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_get.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_get.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_listing.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_listing.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_patch.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_patch.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_restapi_pratica_workflow.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_restapi_pratica_workflow.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/tests/test_user_store.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/tests/test_user_store.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/configure.zcml` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/upgrades/upgrades.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design/plone/iocittadino/vocabularies/vocabularies.py` & `design.plone.iocittadino-1.0.0b9/src/design/plone/iocittadino/vocabularies/vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/PKG-INFO` & `design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.iocittadino
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: An add-on for Plone
 Home-page: https://gitlab.com/redturtle/io-comune/design.plone.iocittadino
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,31 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: design.plone.policy
-Requires-Dist: souper.plone
-Requires-Dist: weasyprint>=58.1
-Requires-Dist: collective.z3cform.datagridfield>=3.0.0
-Requires-Dist: collective.exportimport
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
-Requires-Dist: freezegun; extra == "test"
-Requires-Dist: redturtle.prenotazioni; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://gitlab.com/redturtle/io-comune/design.plone.iocittadino/badges/master/coverage.svg
 
@@ -544,15 +530,17 @@
                 "new_field_a": "A_value",
                 "new_field_b": "B_value",
                 "new_field_c": "C_value",
             }
 
 La stessa identica cosa è possibile per i messaggi, registrando utility fatte
 alla stessa identica maniera per le interfacce IMessageStoreFieldsExtender e
-IMessageStoreSerializerExtender
+IMessageStoreSerializerExtender; c'è inoltre un'interfaccia
+IMessageStoreSerializerSummaryExtender utile per estendere il serializer dell
+summary.
 
 
 Traduzioni
 ==========
 
 Questo prodotto è stato tradotto in:
 
@@ -613,30 +601,42 @@
 
 - RedTurtle, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+1.0.0b9 (2024-03-12)
+--------------------
+
+- Aggiunto modo per aggiungere campi al messaggio e al suo summary serializer
+  registrando delle utility per interfacce predefinite
+  [lucabel]
+- Aggiunto campi precompilabili (idCard, expirationDate, countyOfBirth, 
+  placeOfBirthName, placeOfBirth, placeOfBirthIstatCode)
+  [lucabel]
+
+
+
 1.0.0b8 (2024-03-05)
 --------------------
-- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi al messaggio e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b7 (unreleased)
 --------------------
 
 - Fix the PDF Report + new survey field type added to pdf generation: radiogroup
   [folix-01]
 - Fix: #49945 l'areaopeartore va in errore se il modello pratica è stato cancellato
   (Aggiunto workaround per non mandare in errore, serve però che i dati siano in qualche modo
   recuperabili anche se il modello è stato eliminato)
   [mamico]
-- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando 
+- Aggiunto modo per aggiungere campi alla pratica e al suo serializer registrando
   delle utility per interfacce predefinite
   [lucabel]
 
 1.0.0b6 (2023-10-25)
 --------------------
 
 - Allow users to retrieve their own messages also if ModelloPratica is private.
```

### Comparing `design.plone.iocittadino-1.0.0b8/src/design.plone.iocittadino.egg-info/SOURCES.txt` & `design.plone.iocittadino-1.0.0b9/src/design.plone.iocittadino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

