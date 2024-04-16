# Comparing `tmp/matchcode-toolkit-4.0.0.tar.gz` & `tmp/matchcode-toolkit-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchcode-toolkit-4.0.0.tar", last modified: Sat Mar 16 02:25:41 2024, max compression
+gzip compressed data, was "matchcode-toolkit-4.1.0.tar", last modified: Tue Apr 16 19:53:44 2024, max compression
```

## Comparing `matchcode-toolkit-4.0.0.tar` & `matchcode-toolkit-4.1.0.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/
--rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/.gitattributes
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.076289 matchcode-toolkit-4.0.0/.github/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.080289 matchcode-toolkit-4.0.0/.github/workflows/
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/.github/workflows/docs-ci.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/.github/workflows/pypi-release.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      755 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/.gitignore
--rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/.readthedocs.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/AUTHORS.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1413 2024-03-16 02:24:50.000000 matchcode-toolkit-4.0.0/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/NOTICE
--rw-r--r--   0 jono      (1000) jono      (1000)     4161 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2535 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/apache-2.0.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/azure-pipelines.yml
--rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/configure
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.080289 matchcode-toolkit-4.0.0/docs/
--rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/make.bat
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.084288 matchcode-toolkit-4.0.0/docs/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/scripts/doc8_style_check.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/scripts/sphinx_build_link_check.sh
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.084288 matchcode-toolkit-4.0.0/docs/source/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.084288 matchcode-toolkit-4.0.0/docs/source/_static/
--rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/source/_static/theme_overrides.css
--rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/source/conf.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.084288 matchcode-toolkit-4.0.0/docs/source/contribute/
--rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/source/contribute/contrib_doc.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/source/index.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/docs/source/skeleton-usage.rst
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.076289 matchcode-toolkit-4.0.0/etc/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.084288 matchcode-toolkit-4.0.0/etc/ci/
--rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/azure-container-deb.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/azure-container-rpm.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1240 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/azure-posix.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/azure-win.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/install_sudo.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/macports-ci
--rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/macports-ci.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/ci/mit.LICENSE
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.088288 matchcode-toolkit-4.0.0/etc/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/check_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/fetch_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/gen_pypi_simple.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/gen_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/gen_requirements_dev.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_dejacode.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/pyproject.toml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/requirements-dev.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     1492 2024-03-16 02:25:41.096288 matchcode-toolkit-4.0.0/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode-toolkit-4.0.0/setup.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.076289 matchcode-toolkit-4.0.0/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.088288 matchcode-toolkit-4.0.0/src/matchcode_toolkit/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     5142 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1691 2024-03-16 02:24:50.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit/plugin_fingerprint.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/
--rw-r--r--   0 jono      (1000) jono      (1000)     4161 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2319 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      200 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-15 00:37:28.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-03-16 02:25:40.000000 matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)     6064 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/tests/test_fingerprinting.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.080289 matchcode-toolkit-4.0.0/tests/testfiles/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-03-16 02:25:41.092288 matchcode-toolkit-4.0.0/tests/testfiles/fingerprinting/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
--rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode-toolkit-4.0.0/tests/testfiles/fingerprinting/test.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/
+-rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.gitattributes
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/.github/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/.github/workflows/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.github/workflows/docs-ci.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.github/workflows/pypi-release.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      755 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.gitignore
+-rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/.readthedocs.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/AUTHORS.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1588 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/NOTICE
+-rw-r--r--   0 jono      (1000) jono      (1000)     4012 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2386 2024-04-16 19:50:16.000000 matchcode-toolkit-4.1.0/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/apache-2.0.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/azure-pipelines.yml
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/configure
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/make.bat
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/scripts/doc8_style_check.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/scripts/sphinx_build_link_check.sh
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/_static/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/_static/theme_overrides.css
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/conf.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.285125 matchcode-toolkit-4.1.0/docs/source/contribute/
+-rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/contribute/contrib_doc.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/index.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/docs/source/skeleton-usage.rst
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/etc/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.289125 matchcode-toolkit-4.1.0/etc/ci/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-container-deb.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-container-rpm.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1240 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-posix.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/azure-win.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/install_sudo.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/macports-ci
+-rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/macports-ci.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/ci/mit.LICENSE
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/etc/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/check_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/fetch_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/gen_requirements_dev.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_dejacode.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/pyproject.toml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/requirements-dev.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1492 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode-toolkit-4.1.0/setup.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/src/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/src/matchcode_toolkit/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     7504 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-04-16 18:36:22.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1767 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit/plugin_fingerprint.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/
+-rw-r--r--   0 jono      (1000) jono      (1000)     4012 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2451 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      200 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-15 00:37:28.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-04-16 19:53:44.000000 matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.293125 matchcode-toolkit-4.1.0/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     7473 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/test_fingerprinting.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.281125 matchcode-toolkit-4.1.0/tests/testfiles/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-04-16 19:53:44.297125 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55466 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55546 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate-mod2.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55519 2024-04-16 19:44:23.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/inflate.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/test.json
```

### Comparing `matchcode-toolkit-4.0.0/.github/workflows/docs-ci.yml` & `matchcode-toolkit-4.1.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/.github/workflows/pypi-release.yml` & `matchcode-toolkit-4.1.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/.gitignore` & `matchcode-toolkit-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/.readthedocs.yml` & `matchcode-toolkit-4.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/CHANGELOG.rst` & `matchcode-toolkit-4.1.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+v4.1.0
+------
+
+*2024-04-15* -- Add new functions to compute fingerprints on text resources for approximate file matching (https://github.com/nexB/matchcode-toolkit/issues/5)
+
 v4.0.0
 ------
 
 *2024-03-15* -- Rename ``FingerprintPackage`` pipeline to ``FingerprintCodebase``
 
 v3.1.0
 ------
```

### Comparing `matchcode-toolkit-4.0.0/CODE_OF_CONDUCT.rst` & `matchcode-toolkit-4.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/Makefile` & `matchcode-toolkit-4.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/NOTICE` & `matchcode-toolkit-4.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/PKG-INFO` & `matchcode-toolkit-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 4.0.0
+Version: 4.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,16 +68,15 @@
   # Activate the virtual environment you want to install MatchCode-toolkit into,
   # change directories to the ``matchcode-toolkit`` directory
   pip install --editable .
 
 or built into a wheel and then installed:
 ::
 
-  pip install flot
-  flot --wheel --sdist # The built wheel will be in the dist/ directory
+  python setup.py build bdist_wheel
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
@@ -85,17 +84,16 @@
 ``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
 Resources and computes those values for directories.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
-MatchCode toolkit provides the ``scan_and_fingerprint_package`` pipeline for
-ScanCode.io. This is the same as the ``scan_single_package`` pipeline, but has the
-added step of computing fingerprints for directories.
+MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
+``fingerprint_codebase`` pipelines for ScanCode.io.
 
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
```

### Comparing `matchcode-toolkit-4.0.0/README.rst` & `matchcode-toolkit-4.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,15 @@
   # Activate the virtual environment you want to install MatchCode-toolkit into,
   # change directories to the ``matchcode-toolkit`` directory
   pip install --editable .
 
 or built into a wheel and then installed:
 ::
 
-  pip install flot
-  flot --wheel --sdist # The built wheel will be in the dist/ directory
+  python setup.py build bdist_wheel
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
@@ -42,17 +41,16 @@
 ``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
 Resources and computes those values for directories.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
-MatchCode toolkit provides the ``scan_and_fingerprint_package`` pipeline for
-ScanCode.io. This is the same as the ``scan_single_package`` pipeline, but has the
-added step of computing fingerprints for directories.
+MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
+``fingerprint_codebase`` pipelines for ScanCode.io.
 
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
```

### Comparing `matchcode-toolkit-4.0.0/apache-2.0.LICENSE` & `matchcode-toolkit-4.1.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/azure-pipelines.yml` & `matchcode-toolkit-4.1.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/configure` & `matchcode-toolkit-4.1.0/configure`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/docs/Makefile` & `matchcode-toolkit-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/docs/make.bat` & `matchcode-toolkit-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/docs/source/conf.py` & `matchcode-toolkit-4.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/docs/source/contribute/contrib_doc.rst` & `matchcode-toolkit-4.1.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/docs/source/skeleton-usage.rst` & `matchcode-toolkit-4.1.0/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/azure-container-deb.yml` & `matchcode-toolkit-4.1.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/azure-container-rpm.yml` & `matchcode-toolkit-4.1.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/azure-posix.yml` & `matchcode-toolkit-4.1.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/azure-win.yml` & `matchcode-toolkit-4.1.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/macports-ci` & `matchcode-toolkit-4.1.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/macports-ci.ABOUT` & `matchcode-toolkit-4.1.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/ci/mit.LICENSE` & `matchcode-toolkit-4.1.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/README.rst` & `matchcode-toolkit-4.1.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/check_thirdparty.py` & `matchcode-toolkit-4.1.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/fetch_thirdparty.py` & `matchcode-toolkit-4.1.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/gen_pypi_simple.py` & `matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `matchcode-toolkit-4.1.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/gen_requirements.py` & `matchcode-toolkit-4.1.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/gen_requirements_dev.py` & `matchcode-toolkit-4.1.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/test_utils_pypi_supported_tags.py` & `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `matchcode-toolkit-4.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_dejacode.py` & `matchcode-toolkit-4.1.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_pip_compatibility_tags.py` & `matchcode-toolkit-4.1.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_pypi_supported_tags.py` & `matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `matchcode-toolkit-4.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_requirements.py` & `matchcode-toolkit-4.1.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_thirdparty.py` & `matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/etc/scripts/utils_thirdparty.py.ABOUT` & `matchcode-toolkit-4.1.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/pyproject.toml` & `matchcode-toolkit-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/requirements-dev.txt` & `matchcode-toolkit-4.1.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/setup.cfg` & `matchcode-toolkit-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit/halohash.py` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit/halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,10 +34,11 @@
 
     @classmethod
     def steps(cls):
         return (cls.fingerprint_codebase,)
 
     def fingerprint_codebase(self):
         """
-        Compute directory fingerprints for matching purposes
+        Compute directory and resource fingerprints for matching purposes
         """
         matchcode.fingerprint_codebase_directories(self.project)
+        matchcode.fingerprint_codebase_resources(self.project)
```

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit/plugin_fingerprint.py` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit/plugin_fingerprint.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/PKG-INFO` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 4.0.0
+Version: 4.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,16 +68,15 @@
   # Activate the virtual environment you want to install MatchCode-toolkit into,
   # change directories to the ``matchcode-toolkit`` directory
   pip install --editable .
 
 or built into a wheel and then installed:
 ::
 
-  pip install flot
-  flot --wheel --sdist # The built wheel will be in the dist/ directory
+  python setup.py build bdist_wheel
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
@@ -85,17 +84,16 @@
 ``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
 Resources and computes those values for directories.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
-MatchCode toolkit provides the ``scan_and_fingerprint_package`` pipeline for
-ScanCode.io. This is the same as the ``scan_single_package`` pipeline, but has the
-added step of computing fingerprints for directories.
+MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
+``fingerprint_codebase`` pipelines for ScanCode.io.
 
 
 License
 -------
 
 SPDX-License-Identifier: Apache-2.0
```

### Comparing `matchcode-toolkit-4.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt` & `matchcode-toolkit-4.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -68,8 +68,11 @@
 src/matchcode_toolkit.egg-info/requires.txt
 src/matchcode_toolkit.egg-info/top_level.txt
 src/matchcode_toolkit/pipelines/__init__.py
 src/matchcode_toolkit/pipelines/fingerprint_codebase.py
 src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
 tests/test_fingerprinting.py
 tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+tests/testfiles/fingerprinting/inflate-mod.c
+tests/testfiles/fingerprinting/inflate-mod2.c
+tests/testfiles/fingerprinting/inflate.c
 tests/testfiles/fingerprinting/test.json
```

### Comparing `matchcode-toolkit-4.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json` & `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-4.0.0/tests/testfiles/fingerprinting/test.json` & `matchcode-toolkit-4.1.0/tests/testfiles/fingerprinting/test.json`

 * *Files identical despite different names*

