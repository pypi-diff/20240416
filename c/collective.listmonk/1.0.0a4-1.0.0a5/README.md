# Comparing `tmp/collective.listmonk-1.0.0a4.tar.gz` & `tmp/collective.listmonk-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.listmonk-1.0.0a4.tar", last modified: Tue Apr  9 22:06:13 2024, max compression
+gzip compressed data, was "collective.listmonk-1.0.0a5.tar", last modified: Tue Apr 16 04:46:31 2024, max compression
```

## Comparing `collective.listmonk-1.0.0a4.tar` & `collective.listmonk-1.0.0a5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.019106 collective.listmonk-1.0.0a4/
--rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)      783 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/CONTRIBUTORS.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/LICENSE.md
--rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     6781 2024-04-09 22:06:13.018797 collective.listmonk-1.0.0a4/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/constraints.txt
--rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docker-compose.yml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.008615 collective.listmonk-1.0.0a4/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docs/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docs/dlr.svg
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.008962 collective.listmonk-1.0.0a4/news/
--rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/news/.changelog_template.jinja
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/news/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-09 22:06:13.019152 collective.listmonk-1.0.0a4/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.004640 collective.listmonk-1.0.0a4/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.009118 collective.listmonk-1.0.0a4/src/collective/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.011607 collective.listmonk-1.0.0a4/src/collective/listmonk/
--rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.011911 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.012547 collective.listmonk-1.0.0a4/src/collective/listmonk/content/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2742 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/content/newsletter.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.012969 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/dependencies.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/interfaces.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1445 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/listmonk.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013507 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3074 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/collective.listmonk.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005232 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013701 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     3171 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005384 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013893 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     2581 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
--rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/update.py
--rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/permissions.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005712 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.014623 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/rolemap.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.014832 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/Newsletter.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.015041 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.015907 collective.listmonk-1.0.0a4/src/collective/listmonk/services/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1254 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     6397 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/subscriptions.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016088 collective.listmonk-1.0.0a4/src/collective/listmonk/setuphandlers/
--rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/setuphandlers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3185 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016423 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.018051 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     6781 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     2449 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016751 collective.listmonk-1.0.0a4/tests/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017258 collective.listmonk-1.0.0a4/tests/api/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4657 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/test_mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5182 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/test_subscriptions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3116 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017616 collective.listmonk-1.0.0a4/tests/setup/
--rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/test_setup_install.py
--rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017792 collective.listmonk-1.0.0a4/tests/setup/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/upgrades/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.788432 collective.listmonk-1.0.0a5/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)      942 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/CONTRIBUTORS.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/LICENSE.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     6940 2024-04-16 04:46:31.788133 collective.listmonk-1.0.0a5/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/constraints.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/docker-compose.yml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.779146 collective.listmonk-1.0.0a5/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/docs/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/docs/dlr.svg
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.779476 collective.listmonk-1.0.0a5/news/
+-rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/news/.changelog_template.jinja
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/news/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-16 04:46:31.788480 collective.listmonk-1.0.0a5/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.775176 collective.listmonk-1.0.0a5/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.779628 collective.listmonk-1.0.0a5/src/collective/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.781952 collective.listmonk-1.0.0a5/src/collective/listmonk/
+-rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.782211 collective.listmonk-1.0.0a5/src/collective/listmonk/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.782482 collective.listmonk-1.0.0a5/src/collective/listmonk/content/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/content/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2742 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/content/newsletter.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.782746 collective.listmonk-1.0.0a5/src/collective/listmonk/controlpanel/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/controlpanel/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/controlpanel/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/interfaces.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1445 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/listmonk.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.783176 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3074 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/collective.listmonk.pot
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.775763 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.783323 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3171 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.775919 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/en/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.783471 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/en/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2581 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/locales/update.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/permissions.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.776244 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.784285 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/rolemap.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.784458 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/types/Newsletter.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.784643 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/profiles.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.785414 collective.listmonk-1.0.0a5/src/collective/listmonk/services/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/services/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/services/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1261 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/services/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/services/mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     6397 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/services/subscriptions.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.785576 collective.listmonk-1.0.0a5/src/collective/listmonk/setuphandlers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/setuphandlers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3185 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.785873 collective.listmonk-1.0.0a5/src/collective/listmonk/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/upgrades/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective/listmonk/upgrades/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.787427 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     6940 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     2449 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.786189 collective.listmonk-1.0.0a5/tests/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.786641 collective.listmonk-1.0.0a5/tests/api/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/api/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4657 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/api/test_mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5182 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/api/test_subscriptions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3116 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.786990 collective.listmonk-1.0.0a5/tests/setup/
+-rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/setup/test_setup_install.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-16 04:46:31.787176 collective.listmonk-1.0.0a5/tests/setup/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-16 04:46:31.000000 collective.listmonk-1.0.0a5/tests/setup/upgrades/conftest.py
```

### Comparing `collective.listmonk-1.0.0a4/.editorconfig` & `collective.listmonk-1.0.0a5/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/LICENSE.GPL` & `collective.listmonk-1.0.0a5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/LICENSE.md` & `collective.listmonk-1.0.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/PKG-INFO` & `collective.listmonk-1.0.0a5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a5 (2024-04-15)
+
+
+### Bug fixes:
+
+- Make @mailings GET service available on any content where the user has Send Newsletter permission. @davisagli #13
+
 ## 1.0.0a4 (2024-04-09)
 
 
 ### New features:
 
 - Send an email confirmation of a new subscription. @davisagli #12
```

### Comparing `collective.listmonk-1.0.0a4/README.md` & `collective.listmonk-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/docker-compose.yml` & `collective.listmonk-1.0.0a5/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/docs/dlr.svg` & `collective.listmonk-1.0.0a5/docs/dlr.svg`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/pyproject.toml` & `collective.listmonk-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/setup.py` & `collective.listmonk-1.0.0a5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {Path("CONTRIBUTORS.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="collective.listmonk",
-    version="1.0.0a4",
+    version="1.0.0a5",
     description="A Listmonk newsletter integration for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/content/newsletter.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/content/newsletter.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/listmonk.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/listmonk.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/collective.listmonk.pot` & `collective.listmonk-1.0.0a5/src/collective/listmonk/locales/collective.listmonk.pot`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a5/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a5/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/update.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/rolemap.xml` & `collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/Newsletter.xml` & `collective.listmonk-1.0.0a5/src/collective/listmonk/profiles/default/types/Newsletter.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles.zcml` & `collective.listmonk-1.0.0a5/src/collective/listmonk/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/services/base.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/services/base.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/services/configure.zcml` & `collective.listmonk-1.0.0a5/src/collective/listmonk/services/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       permission="collective.listmonk.newsletter.send"
       name="@mailings"
       />
 
   <plone:service
       method="GET"
       factory=".mailings.ListMailings"
-      for="Products.CMFCore.interfaces.ISiteRoot"
+      for="plone.dexterity.interfaces.IDexterityContent"
       permission="collective.listmonk.newsletter.send"
       name="@mailings"
       />
 
   <utility
       factory=".mailings.MailingCatalogFactory"
       name="collective.listmonk.mailings"
```

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/services/mailings.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/services/mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/services/subscriptions.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective/listmonk/testing.py` & `collective.listmonk-1.0.0a5/src/collective/listmonk/testing.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/PKG-INFO` & `collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a5 (2024-04-15)
+
+
+### Bug fixes:
+
+- Make @mailings GET service available on any content where the user has Send Newsletter permission. @davisagli #13
+
 ## 1.0.0a4 (2024-04-09)
 
 
 ### New features:
 
 - Send an email confirmation of a new subscription. @davisagli #12
```

### Comparing `collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/SOURCES.txt` & `collective.listmonk-1.0.0a5/src/collective.listmonk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/api/test_mailings.py` & `collective.listmonk-1.0.0a5/tests/api/test_mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/api/test_subscriptions.py` & `collective.listmonk-1.0.0a5/tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/conftest.py` & `collective.listmonk-1.0.0a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/setup/test_setup_install.py` & `collective.listmonk-1.0.0a5/tests/setup/test_setup_install.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/setup/test_setup_uninstall.py` & `collective.listmonk-1.0.0a5/tests/setup/test_setup_uninstall.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a4/tests/setup/upgrades/conftest.py` & `collective.listmonk-1.0.0a5/tests/setup/upgrades/conftest.py`

 * *Files identical despite different names*

