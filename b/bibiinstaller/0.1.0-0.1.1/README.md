# Comparing `tmp/bibiinstaller-0.1.0.tar.gz` & `tmp/bibiinstaller-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiinstaller-0.1.0.tar", last modified: Mon Apr 15 03:23:03 2024, max compression
+gzip compressed data, was "bibiinstaller-0.1.1.tar", last modified: Tue Apr 16 15:10:57 2024, max compression
```

## Comparing `bibiinstaller-0.1.0.tar` & `bibiinstaller-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.267013 bibiinstaller-0.1.0/
--rw-rw-rw-   0        0        0     1251 2024-04-13 13:51:35.000000 bibiinstaller-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      305 2024-04-13 10:21:15.000000 bibiinstaller-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3365 2024-04-15 03:23:03.265951 bibiinstaller-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2517 2024-04-15 03:15:54.000000 bibiinstaller-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.186840 bibiinstaller-0.1.0/docs/
--rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiinstaller-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiinstaller-0.1.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.191129 bibiinstaller-0.1.0/docs/source/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.193373 bibiinstaller-0.1.0/docs/source/_static/
--rw-rw-rw-   0        0        0    35080 2024-04-13 10:50:31.000000 bibiinstaller-0.1.0/docs/source/_static/bibiinstaller.png
--rw-rw-rw-   0        0        0     6986 2024-04-13 10:52:53.000000 bibiinstaller-0.1.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiinstaller-0.1.0/docs/source/install.rst
--rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiinstaller-0.1.0/docs/source/quickstart.rst
--rw-rw-rw-   0        0        0     1026 2024-04-15 03:21:08.000000 bibiinstaller-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 03:23:03.267013 bibiinstaller-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-04-15 03:19:25.000000 bibiinstaller-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.171613 bibiinstaller-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.197853 bibiinstaller-0.1.0/src/bibiinstaller/
--rw-rw-rw-   0        0        0      106 2024-04-13 11:27:59.000000 bibiinstaller-0.1.0/src/bibiinstaller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.172597 bibiinstaller-0.1.0/src/bibiinstaller/assets/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.211967 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/
--rw-rw-rw-   0        0        0      450 2024-03-21 05:16:41.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.214222 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/exes/
--rwxrwxrwx   0        0        0    62464 2024-04-13 03:52:45.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe
--rw-rw-rw-   0        0        0       69 2024-04-13 03:59:40.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/exes/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.227354 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/icon_configs/
--rwxrwxrwx   0        0        0  6142464 2023-11-19 10:07:11.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe
--rw-rw-rw-   0        0        0      467 2024-04-14 15:33:16.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini
--rw-rw-rw-   0        0        0      217 2024-04-13 11:12:54.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/icon_configs/commands.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.228518 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/micromamba/
--rwxrwxrwx   0        0        0  9011200 2024-04-10 22:44:34.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.242788 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/mirrors/
--rw-rw-rw-   0        0        0      810 2024-04-12 10:39:24.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/mirrors/.condarc
--rw-rw-rw-   0        0        0      123 2024-04-12 10:38:00.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/mirrors/.mambarc
--rw-rw-rw-   0        0        0      503 2024-04-12 10:39:44.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/mirrors/pip.ini
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.243910 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.177045 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/Plugins/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.247274 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/
--rw-rw-rw-   0        0        0     3072 2024-03-06 07:19:53.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll
--rw-rw-rw-   0        0        0  1640084 2024-04-13 11:06:42.000000 bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip
--rw-rw-rw-   0        0        0      642 2024-04-13 14:50:20.000000 bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_configs.py
--rw-rw-rw-   0        0        0    39811 2024-04-15 01:26:26.000000 bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_windows.py
--rw-rw-rw-   0        0        0     3243 2024-04-14 13:26:49.000000 bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_windows.yaml
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.251724 bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/
--rw-rw-rw-   0        0        0    14917 2024-04-04 09:53:45.000000 bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/application.nsi
--rw-rw-rw-   0        0        0    14990 2024-04-04 09:53:13.000000 bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/bibiinstaller.nsi
--rw-rw-rw-   0        0        0    14917 2024-03-06 07:19:53.000000 bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/spyder.nsi
--rw-rw-rw-   0        0        0     1479 2024-04-04 15:14:40.000000 bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/test_nsi_templates.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.260528 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/
--rw-rw-rw-   0        0        0      219 2024-04-05 12:09:46.000000 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/add_packages.txt
--rw-rw-rw-   0        0        0      121 2024-04-04 14:14:53.000000 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/editable_packages.txt
--rw-rw-rw-   0        0        0      143 2024-04-04 14:13:18.000000 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/extra_packages.txt
--rw-rw-rw-   0        0        0      216 2024-04-08 09:43:12.000000 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/skip_packages.txt
--rw-rw-rw-   0        0        0      188 2024-04-04 14:13:52.000000 bibiinstaller-0.1.0/src/bibiinstaller/package_configs/unwanted_packages.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.263766 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/
--rw-rw-rw-   0        0        0     3365 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 03:23:03.000000 bibiinstaller-0.1.0/src/bibiinstaller.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 03:23:03.262768 bibiinstaller-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-02 14:37:56.000000 bibiinstaller-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      914 2024-04-13 13:28:05.000000 bibiinstaller-0.1.0/tests/learn_env_path.py
--rw-rw-rw-   0        0        0     1731 2024-04-13 13:28:32.000000 bibiinstaller-0.1.0/tests/learn_pypi_yarg.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.789991 bibiinstaller-0.1.1/
+-rw-rw-rw-   0        0        0     1251 2024-04-13 13:51:35.000000 bibiinstaller-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      305 2024-04-13 10:21:15.000000 bibiinstaller-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3306 2024-04-16 15:10:57.788992 bibiinstaller-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2517 2024-04-15 03:15:54.000000 bibiinstaller-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.669258 bibiinstaller-0.1.1/docs/
+-rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiinstaller-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiinstaller-0.1.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.673258 bibiinstaller-0.1.1/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.674260 bibiinstaller-0.1.1/docs/source/_static/
+-rw-rw-rw-   0        0        0    35080 2024-04-13 10:50:31.000000 bibiinstaller-0.1.1/docs/source/_static/bibiinstaller.png
+-rw-rw-rw-   0        0        0     6986 2024-04-13 10:52:53.000000 bibiinstaller-0.1.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiinstaller-0.1.1/docs/source/install.rst
+-rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiinstaller-0.1.1/docs/source/quickstart.rst
+-rw-rw-rw-   0        0        0     1028 2024-04-16 15:07:38.000000 bibiinstaller-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:10:57.790991 bibiinstaller-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1055 2024-04-16 15:07:47.000000 bibiinstaller-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.354261 bibiinstaller-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.681261 bibiinstaller-0.1.1/src/bibiinstaller/
+-rw-rw-rw-   0        0        0      106 2024-04-16 15:08:02.000000 bibiinstaller-0.1.1/src/bibiinstaller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.355259 bibiinstaller-0.1.1/src/bibiinstaller/assets/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.722261 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/
+-rw-rw-rw-   0        0        0      450 2024-03-21 05:16:41.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.725261 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/exes/
+-rwxrwxrwx   0        0        0    62464 2024-04-13 03:52:45.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe
+-rw-rw-rw-   0        0        0       69 2024-04-13 03:59:40.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/exes/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.738993 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/icon_configs/
+-rwxrwxrwx   0        0        0  6142464 2023-11-19 10:07:11.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe
+-rw-rw-rw-   0        0        0      551 2024-04-16 14:56:40.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini
+-rw-rw-rw-   0        0        0      217 2024-04-13 11:12:54.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/icon_configs/commands.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.740993 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/micromamba/
+-rwxrwxrwx   0        0        0  9011200 2024-04-10 22:44:34.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.756993 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/mirrors/
+-rw-rw-rw-   0        0        0      810 2024-04-12 10:39:24.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/mirrors/.condarc
+-rw-rw-rw-   0        0        0      123 2024-04-12 10:38:00.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/mirrors/.mambarc
+-rw-rw-rw-   0        0        0      503 2024-04-12 10:39:44.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/mirrors/pip.ini
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.758991 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.359263 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/Plugins/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.763989 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/
+-rw-rw-rw-   0        0        0     3072 2024-03-06 07:19:53.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll
+-rw-rw-rw-   0        0        0  1640084 2024-04-13 11:06:42.000000 bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip
+-rw-rw-rw-   0        0        0      642 2024-04-13 14:50:20.000000 bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_configs.py
+-rw-rw-rw-   0        0        0    40651 2024-04-16 14:54:47.000000 bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_windows.py
+-rw-rw-rw-   0        0        0     3244 2024-04-16 14:56:38.000000 bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_windows.yaml
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.770993 bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/
+-rw-rw-rw-   0        0        0    14917 2024-04-04 09:53:45.000000 bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/application.nsi
+-rw-rw-rw-   0        0        0    14990 2024-04-04 09:53:13.000000 bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/bibiinstaller.nsi
+-rw-rw-rw-   0        0        0    14917 2024-03-06 07:19:53.000000 bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/spyder.nsi
+-rw-rw-rw-   0        0        0     1479 2024-04-04 15:14:40.000000 bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/test_nsi_templates.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.779994 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/
+-rw-rw-rw-   0        0        0      219 2024-04-05 12:09:46.000000 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/add_packages.txt
+-rw-rw-rw-   0        0        0      121 2024-04-04 14:14:53.000000 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/editable_packages.txt
+-rw-rw-rw-   0        0        0      143 2024-04-04 14:13:18.000000 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/extra_packages.txt
+-rw-rw-rw-   0        0        0      216 2024-04-08 09:43:12.000000 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/skip_packages.txt
+-rw-rw-rw-   0        0        0      188 2024-04-04 14:13:52.000000 bibiinstaller-0.1.1/src/bibiinstaller/package_configs/unwanted_packages.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.786992 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/
+-rw-rw-rw-   0        0        0     3306 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 15:10:57.000000 bibiinstaller-0.1.1/src/bibiinstaller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:10:57.784995 bibiinstaller-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-02 14:37:56.000000 bibiinstaller-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      914 2024-04-13 13:28:05.000000 bibiinstaller-0.1.1/tests/learn_env_path.py
+-rw-rw-rw-   0        0        0     1731 2024-04-13 13:28:32.000000 bibiinstaller-0.1.1/tests/learn_pypi_yarg.py
```

### Comparing `bibiinstaller-0.1.0/LICENSE.txt` & `bibiinstaller-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/PKG-INFO` & `bibiinstaller-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: bibiinstaller
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bibi Installer using pynsist for Windows
 Home-page: https://github.com/bibiparrot/bibiinstaller
 Author: Chunqi Shi
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiinstaller
 Project-URL: Issues, https://github.com/bibiparrot/bibiinstaller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: yarg>=0.1.9
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: bibiflags>=0.1.5
 Requires-Dist: packaging>=24.0
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: pillow>=10.3.0
-Requires-Dist: pyarmor>=8.5.2
 
 BibiInstaller
 ===
 
 
 
 ## Getting Started
```

### Comparing `bibiinstaller-0.1.0/README.md` & `bibiinstaller-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/docs/Makefile` & `bibiinstaller-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/docs/source/_static/bibiinstaller.png` & `bibiinstaller-0.1.1/docs/source/_static/bibiinstaller.png`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/docs/source/conf.py` & `bibiinstaller-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/docs/source/quickstart.rst` & `bibiinstaller-0.1.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/pyproject.toml` & `bibiinstaller-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "bibiinstaller"
-version = "0.1.0"
+version = "0.1.1"
 description = "Bibi Installer using pynsist for Windows"
 authors = [
     {name = "Chunqi SHI", email = "chunqishi@gmail.com"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "yarg>=0.1.9",
+#    "yarg>=0.1.9",
     "loguru>=0.7.2",
     "bibiflags>=0.1.5",
     "packaging>=24.0",
     "tomli>=2.0.1",
     "pillow>=10.3.0",
-    "pyarmor>=8.5.2",
+#    "pyarmor>=8.5.2",
 ]
 
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `bibiinstaller-0.1.0/setup.py` & `bibiinstaller-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 https://docs.python.org/3.11/distutils/setupscript.html
 https://pythonforthelab.com/blog/how-create-setup-file-your-project/
 https://setuptools.pypa.io/en/latest/userguide/entry_point.html
 '''
 
 setup(
     name='bibiinstaller',
-    version='0.1.0',
+    version='0.1.1',
     url='https://github.com/bibiparrot/bibiinstaller',
     license='GPL v3',
     author='Chunqi Shi',
     author_email='chunqishi@gmail.com',
     description='Bibi Installer using pynsist for Windows',
     package_dir={'': 'src'},
     packages=find_packages(
         where='src',  # '.' by default
         include=['*'],  # ['*'] by default
         exclude=[],  # empty by default
     ),
     install_requires=[
-        "yarg>=0.1.9",
+#        "yarg>=0.1.9",
         "loguru>=0.7.2",
         "bibiflags>=0.1.5",
         "packaging>=24.0",
         "tomli>=2.0.1",
         "pillow>=10.3.0",
     ],
     entry_points={
```

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/mirrors/.condarc` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/mirrors/.condarc`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip` & `bibiinstaller-0.1.1/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_configs.py` & `bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_configs.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_windows.py` & `bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,30 +133,31 @@
         **{
             key: (data[key] if val.default == val.empty else data.get(key, val.default))
             for key, val in inspect.signature(cls).parameters.items()
         }
     )
 
 
-def subprocess_run(args):
+def subprocess_run(args, exit=True):
     """
     Wrapper-function around subprocess.run.
 
     When the sub-process exits with a non-zero return code,
     prints out a message and exits with the same code.
     """
     logger.info(f'$ {" ".join([str(x) for x in args])}')
     cp = subprocess.run(args, capture_output=True, text=True)
     logger.info(cp.stdout)
     try:
         cp.check_returncode()
     except subprocess.CalledProcessError as exc:
         logger.warning(exc)
         logger.debug(cp.stderr)
-        sys.exit(cp.returncode)
+        if exit:
+            sys.exit(cp.returncode)
 
 
 def create_python_env(target_directory, python_version: str, environment_name: str = None):
     micromamba_path = ASSETS_HOME / 'Windows' / 'micromamba'
     logger.debug(f"micromamba_path = [{micromamba_path}]")
     micromamba_exes = list(micromamba_path.glob('*.exe'))
     if len(micromamba_exes) < 1:
@@ -335,15 +336,15 @@
     pip_download_dir = (Path(work_dir) / f"pip_download_only_binaries").resolve()
     logger.info(f'make pip download dir: [{pip_download_dir}]')
     pip_download_dir.mkdir(parents=True, exist_ok=True)
 
     logger.debug(f'requirements_wheel_pypi = {requirements_wheel_pypi}')
     for requirement in requirements_wheel_pypi:
         subprocess_run([python, "-m", "pip", "download", "--only-binary", ":all:", "--dest",
-                        pip_download_dir, requirement])
+                        pip_download_dir, requirement], exit=False)
 
     whl_files = pip_download_dir.glob("*.whl")
 
     canonicalize_wheels = []
     for whl_file in whl_files:
         # logger.debug(f'whl_file = {whl_file}')
         name, version = canonicalize_wheel_filename(whl_file)
@@ -490,14 +491,15 @@
     # fill extra_wheel_sources, local_wheels
     # SEE: https://pynsist.readthedocs.io/en/latest/
 
     '''
     files = []
     wanted_rqmts_freeze, rqmts_wheel, rqmts_editable = separate_wheels_and_packages(python, unwanted_packages)
     skip_pypi_wheels = [package_name] + skip_pypi_packages
+    logger.info(f'is_wheel_first={is_wheel_first}')
     if not is_wheel_first:
         wheels_pypi_download = []
         packages = []
         extra_wheel_sources = []
 
         '''"import sysconfig; print(sysconfig.get_path('purelib'))"'''
         site_packages_dir = work_dir / 'packaging-venv' / 'Lib' / 'site-packages'
@@ -869,15 +871,15 @@
 def get_absolute_path(root, file):
     if file is not None:
         return (Path(root) / file).resolve()
 
 
 def url_exist(url):
     try:
-        response = requests.head(url)
+        response = requests.head(url, timeout=5)
         return response.status_code == 200
     except requests.exceptions.RequestException as e:
         return False
 
 
 def find_python_embed_amd64_versions(python_version):
     pattern = r'(\d+)\.(\d+)\.(\d+)'
@@ -939,14 +941,30 @@
     # for pynsist to locate makensis [shutil.which("makensis")]
     # logger.debug(os.environ["PATH"])
     os.environ["PATH"] += os.pathsep + str(work_nsis_dir)
     # logger.debug(os.environ["PATH"])
     return work_nsis_dir
 
 
+def strtobool(val):
+    """Convert a string representation of truth to true (1) or false (0).
+
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+    """
+    val = val.lower()
+    if val in ('y', 'yes', 't', 'true', 'on', '1'):
+        return True
+    elif val in ('n', 'no', 'f', 'false', 'off', '0'):
+        return False
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
+
+
 def main():
     import argparse
     parser = argparse.ArgumentParser(
         prog='bibiinstaller',
         description='python installer package named bibi.')
     parser.add_argument('configs.py')
     flags = BibiFlags(app_name='bibiinstaller_windows',
@@ -968,27 +986,32 @@
     bitness = flags.parameters.get('bitness') or configs.BITNESS
     entrypoint = flags.parameters.get('entrypoint') or configs.ENTRYPOINT
     package = flags.parameters.get('package') or configs.PACKAGE_NAME
 
     pynsist_version = flags.parameters.get('pynsist_version')
     suffix = flags.parameters.get('suffix')
     pypi_server = flags.parameters.get('pypi_server')
-    is_wheel_first = flags.parameters.get('is_wheel_first')
+    is_wheel_first = strtobool(flags.parameters.get('is_wheel_first', False))
 
     icon_path = get_absolute_path(project_root,
                                   flags.parameters.get('icon_path') or configs.ICON_PATH)
+    if not Path(icon_path).exists():
+        sys.exit(f"NOT Exist icon_path = [{icon_path}]")
 
     if not str(icon_path).lower().endswith('ico'):
         icon_path_convert = str(icon_path) + '.ico'
         png_to_icon(icon_path, icon_path_convert)
         icon_path = Path(icon_path_convert).resolve()
 
     license_path = get_absolute_path(project_root,
                                      flags.parameters.get('license_txt_path') or configs.LICENSE_TXT_PATH)
 
+    if not Path(license_path).exists():
+        sys.exit(f"NOT Exist license_path = [{license_path}]")
+
     extra_requirements_txt_path = get_absolute_path(
         project_root,
         flags.parameters.get('extra_requirements_txt_path') or configs.EXTRA_REQUIREMENTS_TXT_PATH
     )
     extra_packages_txt_path = get_absolute_path(
         project_root,
         flags.parameters.get('extra_packages_txt_path'))
```

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/bibiinstaller_windows.yaml` & `bibiinstaller-0.1.1/src/bibiinstaller/bibiinstaller_windows.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   - default: 2.8
     dest: pynsist_version
     help: pynsist version of the installer
     option_strings:
       - --pynsist_version
     type: str
 
-  - default: true
+  - default: false
     dest: is_wheel_first
     help: pynsist using wheel online instead of local installed packages.
     option_strings:
       - --is_wheel_first
     type: bool
 
   - dest: pypi_server
```

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/application.nsi` & `bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/application.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/bibiinstaller.nsi` & `bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/bibiinstaller.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/spyder.nsi` & `bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/spyder.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller/nsi_templates/test_nsi_templates.py` & `bibiinstaller-0.1.1/src/bibiinstaller/nsi_templates/test_nsi_templates.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller.egg-info/PKG-INFO` & `bibiinstaller-0.1.1/src/bibiinstaller.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: bibiinstaller
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bibi Installer using pynsist for Windows
 Home-page: https://github.com/bibiparrot/bibiinstaller
 Author: Chunqi Shi
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiinstaller
 Project-URL: Issues, https://github.com/bibiparrot/bibiinstaller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: yarg>=0.1.9
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: bibiflags>=0.1.5
 Requires-Dist: packaging>=24.0
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: pillow>=10.3.0
-Requires-Dist: pyarmor>=8.5.2
 
 BibiInstaller
 ===
 
 
 
 ## Getting Started
```

### Comparing `bibiinstaller-0.1.0/src/bibiinstaller.egg-info/SOURCES.txt` & `bibiinstaller-0.1.1/src/bibiinstaller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/tests/learn_env_path.py` & `bibiinstaller-0.1.1/tests/learn_env_path.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.0/tests/learn_pypi_yarg.py` & `bibiinstaller-0.1.1/tests/learn_pypi_yarg.py`

 * *Files identical despite different names*

