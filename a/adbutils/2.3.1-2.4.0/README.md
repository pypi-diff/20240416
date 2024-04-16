# Comparing `tmp/adbutils-2.3.1.tar.gz` & `tmp/adbutils-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.3.1.tar", last modified: Mon Apr  8 04:31:59 2024, max compression
+gzip compressed data, was "adbutils-2.4.0.tar", last modified: Tue Apr 16 08:04:54 2024, max compression
```

## Comparing `adbutils-2.3.1.tar` & `adbutils-2.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 04:31:53.000000 adbutils-2.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 04:31:53.000000 adbutils-2.3.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 04:31:59.000000 adbutils-2.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 04:31:59.000000 adbutils-2.3.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 04:31:53.000000 adbutils-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 04:31:59.859289 adbutils-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-08 04:31:53.000000 adbutils-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.851289 adbutils-2.3.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-08 04:31:53.000000 adbutils-2.3.1/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-08 04:31:53.000000 adbutils-2.3.1/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 04:31:53.000000 adbutils-2.3.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 04:31:53.000000 adbutils-2.3.1/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 04:31:53.000000 adbutils-2.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 04:31:53.000000 adbutils-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 04:31:59.859289 adbutils-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 04:31:53.000000 adbutils-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/test_adb_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 08:04:47.000000 adbutils-2.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.342109 adbutils-2.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 08:04:47.000000 adbutils-2.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.342109 adbutils-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-16 08:04:47.000000 adbutils-2.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 08:04:47.000000 adbutils-2.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 08:04:47.000000 adbutils-2.4.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 08:04:54.000000 adbutils-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 08:04:54.000000 adbutils-2.4.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 08:04:47.000000 adbutils-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-16 08:04:54.346109 adbutils-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-16 08:04:47.000000 adbutils-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-16 08:04:47.000000 adbutils-2.4.0/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 08:04:54.000000 adbutils-2.4.0/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.342109 adbutils-2.4.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-16 08:04:47.000000 adbutils-2.4.0/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-16 08:04:47.000000 adbutils-2.4.0/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:04:47.000000 adbutils-2.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 08:04:47.000000 adbutils-2.4.0/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 08:04:47.000000 adbutils-2.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 08:04:47.000000 adbutils-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-16 08:04:54.346109 adbutils-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 08:04:47.000000 adbutils-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 08:04:47.000000 adbutils-2.4.0/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:54.346109 adbutils-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-16 08:04:47.000000 adbutils-2.4.0/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:04:47.000000 adbutils-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-16 08:04:47.000000 adbutils-2.4.0/tests/test_adb_server.py
```

### Comparing `adbutils-2.3.1/.coveragerc` & `adbutils-2.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/.github/workflows/main.yml` & `adbutils-2.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/.github/workflows/publish-to-pypi.yml` & `adbutils-2.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/.travis.yml` & `adbutils-2.4.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/LICENSE` & `adbutils-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/PKG-INFO` & `adbutils-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.3.1
+Version: 2.4.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.3.1/README.md` & `adbutils-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/__init__.py` & `adbutils-2.4.0/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/__main__.py` & `adbutils-2.4.0/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/_adb.py` & `adbutils-2.4.0/adbutils/_adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 from adbutils._utils import adb_path
 from adbutils.errors import AdbConnectionError, AdbError, AdbTimeout
 
 from adbutils._proto import *
 from adbutils._version import __version__
 
-_OKAY = "OKAY"
-_FAIL = "FAIL"
+_OKAY = b"OKAY"
+_FAIL = b"FAIL"
 
 
 def _check_server(host: str, port: int) -> bool:
     """ Returns if server is running """
     s = socket.socket()
     try:
         s.settimeout(.1)
@@ -89,14 +89,18 @@
         return self.conn.send(data)
 
     def read(self, n: int) -> bytes:
         try:
             return self._read_fully(n)
         except socket.timeout:
             raise AdbTimeout("adb read timeout")
+    
+    def read_uint32(self) -> int:
+        data = self.read(4)
+        return int.from_bytes(data, "little")
 
     def _read_fully(self, n: int) -> bytes:
         t = n
         buffer = b''
         while t > 0:
             chunk = self.conn.recv(t)
             if not chunk:
@@ -134,15 +138,15 @@
             chunk = self.read(4096)
             if not chunk:
                 break
             content += chunk
         return content.decode(encoding, errors='replace') if encoding else content
 
     def check_okay(self):
-        data = self.read_string(4)
+        data = self.read(4)
         if data == _FAIL:
             raise AdbError(self.read_string_block())
         elif data == _OKAY:
             return
         raise AdbError("Unknown data: %r" % data)
```

### Comparing `adbutils-2.3.1/adbutils/_deprecated.py` & `adbutils-2.4.0/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/_device.py` & `adbutils-2.4.0/adbutils/_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 import socket
 import subprocess
 import threading
 import typing
 from typing import Optional, Union
 
+from PIL import Image
 
 from adbutils._deprecated import DeprecatedExtension
 from adbutils.install import InstallExtension
 from adbutils.screenrecord import ScreenrecordExtension
 from adbutils.screenshot import ScreenshotExtesion
 
 from adbutils._adb import AdbConnection, BaseClient
@@ -289,14 +290,59 @@
         c.check_okay()
         content = c.read_string_block()
         for line in content.splitlines():
             parts = line.split()
             if len(parts) != 3:
                 continue
             yield ReverseItem(*parts[1:])
+    
+    def framebuffer(self) -> Image.Image:
+        """Capture device screen and return PIL.Image object
+
+        Raises:
+            NotImplementedError
+        """
+        # Ref: https://android.googlesource.com/platform/system/core/+/android-cts-7.0_r18/adb/framebuffer_service.cpp
+        # Ref: https://github.com/DeviceFarmer/adbkit/blob/c16081384ca34addbdab318bda3c76434b7538af/src/adb/command/host-transport/framebuffer.ts
+        c = self.open_transport()
+        c.send_command("framebuffer:")
+        c.check_okay()
+        
+        version = c.read_uint32()
+        if version == 16:
+            raise NotImplementedError("Unsupported version 16")
+        bpp = c.read_uint32() # bits per pixel
+        if bpp != 24 and bpp != 32:
+            raise NotImplementedError("Unsupported bpp(bits per pixel)", bpp)
+        size = c.read_uint32()
+        if size == 1:
+            # FIXME: what is this?
+            size = c.read_uint32()
+        width = c.read_uint32()
+        height = c.read_uint32()
+        red_offset = c.read_uint32()
+        red_length = c.read_uint32() # always 8
+        blue_offset = c.read_uint32()
+        blue_length = c.read_uint32() # always 8
+        green_offset = c.read_uint32()
+        green_length = c.read_uint32() # always 8
+        alpha_offset = c.read_uint32()
+        alpha_length = c.read_uint32()
+
+        color_format = 'RGB'
+        if blue_offset == 0:
+            color_format = 'BGR'
+        if bpp == 32 or alpha_length:
+            color_format += 'A'
+
+        if color_format != 'RGBA' and color_format != 'RGB':
+            raise NotImplementedError("Unsupported color format")
+        buffer = c.read(size)
+        image = Image.frombytes(color_format, (width, height), buffer)
+        return image
 
     def push(self, local: str, remote: str) -> str:
         return self.adb_output("push", local, remote)
 
     def create_connection(
         self, network: Network, address: Union[int, str]
     ) -> socket.socket:
@@ -456,7 +502,8 @@
     """provide custom functions for some complex operations"""
 
     def __init__(
         self, client: BaseClient, serial: str = None, transport_id: int = None
     ):
         BaseDevice.__init__(self, client, serial, transport_id)
         ScreenrecordExtension.__init__(self)
+        ScreenshotExtesion.__init__(self)
```

### Comparing `adbutils-2.3.1/adbutils/_proto.py` & `adbutils-2.4.0/adbutils/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/_utils.py` & `adbutils-2.4.0/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/errors.py` & `adbutils-2.4.0/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/install.py` & `adbutils-2.4.0/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/pidcat.py` & `adbutils-2.4.0/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/screenrecord.py` & `adbutils-2.4.0/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils/shell.py` & `adbutils-2.4.0/adbutils/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 
 import abc
 import datetime
 import json
 import re
+import time
 from typing import List, Optional, Union
 from adbutils._proto import WindowSize, AppInfo, RunningAppInfo
 from adbutils.errors import AdbError, AdbInstallError
 from adbutils._utils import escape_special_characters
 from retry import retry
 
 from adbutils.sync import Sync
@@ -42,19 +43,33 @@
     def getprop(self, prop: str) -> str:
         return self.shell(["getprop", prop]).strip()
 
     def keyevent(self, key_code: Union[int, str]):
         """adb shell input keyevent KEY_CODE"""
         self.shell(["input", "keyevent", str(key_code)])
 
-    def volume_up(self):
-        self.shell("input keyevent VOLUME_UP")
-
-    def volume_down(self):
-        self.shell("input keyevent VOLUME_DOWN")
+    def volume_up(self, times: int = 1):
+        """
+        Increase the volume by times step
+        :param times: times to increase volume，default is 1(Wake up volume bar).
+        :return:
+        """
+        for _ in range(times):
+            self.shell("input keyevent VOLUME_UP")
+            time.sleep(0.5)
+
+    def volume_down(self, times: int = 1):
+        """
+        Decrease the volume by times step
+        :param times: times to decrease volume，default is 1(Wake up volume bar).
+        :return:
+        """
+        for _ in range(times):
+            self.shell("input keyevent VOLUME_DOWN")
+            time.sleep(0.5)
 
     def volume_mute(self):
         self.shell("input keyevent VOLUME_MUTE")
 
     def reboot(self):
         self.shell("reboot")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adbutils-2.3.1/adbutils/sync.py` & `adbutils-2.4.0/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/adbutils.egg-info/PKG-INFO` & `adbutils-2.4.0/adbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.3.1
+Version: 2.4.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.3.1/adbutils.egg-info/SOURCES.txt` & `adbutils-2.4.0/adbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/assets/images/pidcat.png` & `adbutils-2.4.0/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/build_wheel.py` & `adbutils-2.4.0/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/examples/reset-offline.py` & `adbutils-2.4.0/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/setup.cfg` & `adbutils-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/test_real_device/conftest.py` & `adbutils-2.4.0/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/test_real_device/test_adb.py` & `adbutils-2.4.0/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/test_real_device/test_deprecated.py` & `adbutils-2.4.0/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/test_real_device/test_device.py` & `adbutils-2.4.0/test_real_device/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     # adb connect device devpath is "unknown"
     # assert device.get_devpath().startswith("usb:")
 
 
 def test_keyevent(device: AdbDevice):
     # make sure no error raised
     device.keyevent(4)
-    device.volume_up()
-    device.volume_down()
+    device.volume_up(2)
+    device.volume_down(3)
     device.volume_mute()
 
 
 def test_switch_screen(device: AdbDevice):
     device.switch_screen(False)
     device.switch_screen(True)
 
@@ -160,15 +160,20 @@
         data += chunk
     assert b"Hello Android" == data
 
 
 def test_screenshot(device: AdbDevice):
     im = device.screenshot()
     assert im.mode == "RGB"
-    
+
+
+def test_framebuffer(device: AdbDevice):
+    im = device.framebuffer()
+    assert im.size
+
 
 def test_app_info(device: AdbDevice):
     pinfo = device.app_current()
     app_info = device.app_info(pinfo.package)
     assert app_info.package_name is not None
```

### Comparing `adbutils-2.3.1/test_real_device/test_forward_reverse.py` & `adbutils-2.4.0/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/test_real_device/test_utils.py` & `adbutils-2.4.0/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/tests/adb_server.py` & `adbutils-2.4.0/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.1/tests/conftest.py` & `adbutils-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

